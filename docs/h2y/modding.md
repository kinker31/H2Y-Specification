## H2Y's HHE Extensions (HHX)
Technically, HHE *does* allow for modding the level tiles, main menu options, and most other assets that normally have graphic patches associated with them, but currently it requires using a DOS program that only fully functions on an older version of Heretic. This, to put it lightly, is *not* ideal.

**MAJOR TODO:** Could all this be completely replaced with EXDEFS? Or, at least on H2Y+?

HereticHackED Extended (HHX) aims to solve this. HHX can follow what BEX does, but with the following changes/additions:
* String mnemonics should include almost any relevant user-facing text string that vanilla HHE can modify
* Account for whatever extra hardcoded shenanigans Heretic engages in
* Disable the graphical text startup Heretic normally uses if desired
* Allow up to nine maps to be defined for all six episodes
  * (Maybe also allow secret maps to exit to any other map? Depends on if H2Y should support UMAPINFO or not.)

More detail to come as I see fit.
