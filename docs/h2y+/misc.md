## Misc. H2Y+ Specification Stuffs
Cross port ACS should be implemented here, ideally to both standards if ACS is deemed in-scope for base H2Y.

* Rely on UMAPINFO 3.0+, much like what MBF21 does for episode/map flow, and finale screens.
  * Fall back on default H2Y behavior when a UMAPINFO lump isn't found
* TINTTABx: Allows for different transparency handling for some entities, perhaps defined in HHX+
* HHX&####: General purpose HHX sprite number [&], sprite frame [####].
* LOOPSND&: General purpose looping sound number [&].
* AMBIENT&: General purpose random ambient noise number [&]
