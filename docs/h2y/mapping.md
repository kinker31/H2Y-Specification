## Non-Generalzied Linedefs
Linedef layout should be identical to Doom 2/Boom's layout, save for the following changes:

* Linedef specials that modify floor/ceiling scrolling should *not* be implemented
* Translucent linedefs should rely on the default tranmap lump.
* Heretic line special functionality should remain as-is (on suggestion from Gaz)
* Friction modifier linedefs should be able to work with untagged sectors set to Special 15
* 178/198: S1/SR Activate Script (use linedef tag to denote script number)
* 224/225: W1/WR Activate Script (use linedef tag to denote script number)
* 250-253: [S1|SR|W1|WR] Always Activate Script (use linedef tag to denote script number)
* 254: Scroll Wall exactly with Floor/Ceiling
* 255: Scroll Wall Opposite to Floor/Ceiling
* MBF's 271 and 272 should also be included
* Point Pushers/Pullers could work as-is without the need of a special linedef to do so.
* Boom's extra linedef bitflags can remain as-is.

## Generalized Linedefs
Boom's generalized linedef specification can remain as-is, save for the following changes:
* <ins>Locked Door Bits:</ins>
  * Lock bits instead individually control what key the player needs to open the door/activate the switch
  * 0 for this field requires any of the three keys, and all 3 bits require all three keys
  * Skull/Keycard bit instead controls if the keys get consumed in the process
   * (Any-key doors will ignore the key-consume bit instead)
   * (Alternatively, the key consume bit takes the topmost key from the inventory (Yellow, then Green, then Blue)

## Sectors
Heretic's sector special layout can remain as is, with the following additions:

* 11: %5 lava damage, scroll west 28, and blink 0.5 per second
* 52 - 55: Scroll [E|N|S|W] 50 (Very Fast)
* 56 - 59: Wind [E|N|S|W] 50 (Very Fast)
* <ins>Generalized Sector Bits:</ins>
  * Bit 6: Damage 4% Normal
  * Bit 7: Damage 5% Lava
    * (Bit 6 + 7) = 8% Lava Fast
  * Bit 8: Secret
  * Bit 9: Ceiling Flat Scrolls with Floor (If a wind sector, instead slowly oscillates wind strength)
  * Bit 10: Enable Friction
