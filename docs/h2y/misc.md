## Unsorted Specification Stuff
If Cross-port ACS is deemed out of scope for H2Y, bring its relevant functionality over to H2Y+ instead.

* E1-E6PAL/ E1-E6END: Allows for any episode to use E2's custom palette/endscreen functionality
  * ExENDVy: Episode X endscreen, scroll upwards, slide y
  * ExENDhy: Episode X endscreen, vertical rightwards, slide y
  * FINAL1/2 can be used as normal instead if desired
* LOADXH2Y: Alternative LOADING ANSI lump, doesn't display loading text at all
* ENDH2YTX: ALternative ENDTEXT ANSI lump, bit 0 functions as background intensity instead of blink
* MAPEx: Allows for custom map lumps past the first three episodes

Boom's ANIMATED and SWITCHES lump should work as they do in Boom, but need to have Heretic's (very few) pre-defined animated textures and switches at the start of the list.
COLORMAPs should also be supported too, since Boom supports them.
