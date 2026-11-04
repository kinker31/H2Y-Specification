## H2Y+ Additions
Read H2Y's mapping proposal first.

### Linedef Additions

* 273 - 276: [G1|GR] Script [Activate|Always Actiavte]
* 1024 - 1027: W1/WR Change Music Looping (1026+ resets music)
* 1028 - 1031: W1/WR Change Music Once (1026+ resets music)
* 1032: Custom Sector COLORMAP
* 277/278: W1/S1 Autosave (if enabled)

(yes, I *did* steal some of this from ID24; Most of it's because I'd rather not fnagle with Music Changer things ever again.)

### Sector Additions

* Bit 11: Alternate Damage Mode (MBF21 functionality, mostly instakills, check for bits 6 and 7 instead)
* Bit 12: Kill grounded monsters (+Bit 11: Kill ALL monsters)
* Bit 13: Silence Sector Movement
* Bit 14: Silence Sector Actors
