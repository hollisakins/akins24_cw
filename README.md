# COSMOS-Web LRDs
Repository for data and figures from Akins et al. (2024) paper on LRDs in COSMOS-Web

`seds/*_sed.pdf`: This directory includes SED plots (as in Figures 4, 5, and 6 in the paper) for all 429 objects in the sample. Note that for objects with F1800W coverage, we omit the ACS/F814W cutouts, and PRIMER-NIRCam cutouts are not shown, but the photometry is used. 

`COSMOS-Web_LRDs_May2024.dat`: This is an extended and machine-readable form of Table 1 in the paper, including coordinates, photometry (in all available bands), and derived physical properties (from QSO and galaxy fits) for all 429 objects in the sample. The file is in the `ecsv` format, and can be read into python using `astropy`: 
```
from astropy.table import Table
t = Table.read('COSMOS-Web_LRDs_May2024.dat', format='ascii.ecsv')
```

`COSMOS-Web_LRDs_bol_LF.dat`: This file provides the tabulated values for the LRD bolometric luminosity function from Figure 9. In the paper we provide the bolometric LF in 0.5 dex bins, here we additionally include the LF marginalized over the bin size, as described in the text. 


`COSMOS-Web_LRDs_SMF.dat`: This file provides the tabulated values for the LRD contribution to the stellar mass function from Figure 12. Format is identical to `COSMOS-Web_LRDs_bol_LF.dat`.  




Happy to provide additional data, please reach out [over email](mailto:hollis.akins@gmail.com). 
If you use these data or intend to study these objects further, please cite the COSMOS-Web LRD population paper
```
Akins, H. B., Casey, C. M., ???, et al. 2024,
arXiv: 24XX.XXXX, doi: XXXXXX
```
