# Metabolomics spectra databases

A very good overview on databases (including links) can be found at the Metabolomics Society Homepage: [Link](http://metabolomicssociety.org/resources/metabolomics-databases)

Another collection of links to databases can be found at the Fiehn lab homepage: [Link](http://fiehnlab.ucdavis.edu/projects/fiehnlib). The provided information is much less sorted and partially deprecated.

## GC-MS database table (incomplete) 

Name | Link | Provider | Licence | \# of spectra | estimated quality | file format(s) | comments
---|---|---|---|---|---|---|---
Golm DB | http://gmd.mpimp-golm.mpg.de/ | | free | | | `.msl`, `.msp (Golm style)` | last update online in 2011, german project (DFG, MaxPlanck)
Fiehn DB | | | non-free (?), several MS vendors have/had licences | | | `.msp (Fiehn style)` | seems to be deprecated
MassBank of Northern America (MoNA) | http://mona.fiehnlab.ucdavis.edu/downloads | Fiehn lab | free | | | `JSON` (internal MoNA format);  `.msp (MoNA style)` | `.msp (MoNA style)` should be compatible with `NIST MS Search`
MassBank | http://www.massbank.jp/en/about.html | | free | | |  | provides also software and API
NIST | | | commercial | | | NIST format, can be exported as `.msp (NIST style)` | 
Human Metabolome Database (HMDB) | | | free | | | `XML` | 

### More information on single DBs

**Golm:** The 2011 version includes most commercially available metabolites. The group is still integrating new ones, but does not upload them online. Current versions are available directly from the Kopka lab.

**MoNA:** MoNA seems more like a collection of other free databases (e.g. HMDB), all provided as `.msp`.

**MassBank:** Like MoNA, a collection of free databases from different labs allover the world.