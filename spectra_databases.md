# Metabolomics spectra databases

A very good overview on databases (including links) can be found at the Metabolomics Society Homepage: [Link](http://metabolomicssociety.org/resources/metabolomics-databases)

Another collection of links to databases can be found at the Fiehn lab homepage: [Link](http://fiehnlab.ucdavis.edu/projects/fiehnlib). The provided information is much less sorted and partially deprecated.

## GC-MS database table (incomplete) 

Name | Link | Licence | estimated quality | file format(s) | comments
---|---|---|---|---|---
Golm DB | http://gmd.mpimp-golm.mpg.de/ | free | *+* | `.msl`, `.msp (Golm style)` | last update online in 2011, german project (DFG, MaxPlanck)
Fiehn DB | | non-free (?), several MS vendors have/had licences | *-* | `.msp (Fiehn style)` | seems to be deprecated
MassBank of Northern America (MoNA) | http://mona.fiehnlab.ucdavis.edu/downloads | free | *++* | `JSON` (with metadata);  `.msp (MoNA style)` (w/o metadata) | `.msp (MoNA style)` should be compatible with `NIST MS Search`
MassBank | http://www.massbank.jp/en/about.html | free | | | provides also software and API
NIST | | commercial | | NIST format, can be exported as `.msp (NIST style)` | 
Human Metabolome Database (HMDB) | http://www.hmdb.ca/ | free | *+++* | `XML` | provides also structures and protein DBs

## Spectra file format converter

We need a converter to be able to automatically compare and combine the different databases. 

- **Inputs:** All `*.msp` formats, HMDB-XML, MoNA-JSON
- **Outputs:** to be discussed. Potentially useful outputs: MoNA `*.msp`, MoNA-JSON (?), HMDB-XML

  - I think we should refrain of defining and using a newly defined format. I see some drawbacks in each of the ones existing, but IMHO it really does not make sense to increase the confusion about the right format.
  
- **Examples** of all formats can be found here: [./Beispiele_SpektrenFormate.zip]
  - Every example uses the same two metabolites, only `nist_msSearch_output.msp` uses two different ones

## More information on single DBs

**MoNA:** MassBank of Northern America (MoNA) collects spectra from many other free databases (e.g. HMDB, RTX Fiehnlib, LipidBlast) and combines them into one huge library. You can restrict the spectra either based on the method (e.g. GC-MS) or based on the source (e.g. HMDB). 

**HMDB:** Human Metabolome Database (HMDB) is a freely available electronic database containing detailed information about small molecule metabolites found in the human body. Sorted by human body fluids (e.g. serum, saliva). Contains many metadata.

**Golm:** The 2011 version includes most commercially available metabolites. The group is still integrating new ones, but does not upload them online. Current versions are available directly from the Kopka lab. "Ich würde denken dass unserer öffentlicher Teil ziemlich komplementär zu Fiehnlib und dem GC-MS Anteil der Massbank sind." (Zitat Leiter Golm DB)

**MassBank:** A collection of free databases from different labs allover the world.