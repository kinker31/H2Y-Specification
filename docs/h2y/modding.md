## Planned Method
For H2Y, see about implementing HHX.

For H2Y+, use EXDEFS instead.

### H2Y's HHE Extensions (HHX)
Technically, HHE *does* allow for modding the level tiles, main menu options, and most other assets that normally have graphic patches associated with them, but currently it requires using a DOS program that only fully functions on an older version of Heretic. This, to put it lightly, is *not* ideal.

HereticHackED Extended (HHX) aims to solve this. HHX can follow what BEX does, but with the following changes/additions:
* String mnemonics should include almost any relevant user-facing text string that vanilla HHE can modify
* Account for whatever extra hardcoded shenanigans Heretic engages in
* Disable the graphical text startup Heretic normally uses if desired 
 * (This could be done with a simple boolean value, or through the usage of the LOADXH2Y lump)
* Allow up to nine maps to be defined for the sixth episode
  * As a default, E6M3 leads to E6M9.

### Planned String Mnemonics
All text is treated as capitals by default.
|Mnemonic Name|Default Value|
|-|-|
|T_NGAME|New Game|

More detail to come as I see fit.
