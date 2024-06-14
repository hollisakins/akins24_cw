# COSMOS-Web LRDs
Repository for data and figures from Akins et al. (2024) paper on LRDs in COSMOS-Web

`seds/*_sed.pdf`: This directory includes SED plots (as in Figures 4, and 5 in the paper) for all 434 objects in the sample. Note that for objects with F1800W coverage, we omit the ACS/F814W cutouts, and PRIMER-NIRCam cutouts are not shown, but the photometry is used. 

<img src="https://github.com/hollisakins/akins24_cw/assets/38053732/18da3dd9-bf87-432b-8c02-68fd3404f8f1" width=50% height=50%>


`COSMOS-Web_LRDs_Jun2024.dat`: This is an extended and machine-readable form of Table 1 in the paper, including coordinates, photometry (in all available bands), and derived physical properties (from QSO and galaxy fits) for all 434 objects in the sample. The file is in the `ecsv` format, and can be read into python using `astropy`: 
```
from astropy.table import Table
t = Table.read('COSMOS-Web_LRDs_Jun2024.dat', format='ascii.ecsv')
```

`COSMOS-Web_LRDs_bol_LF.dat`: This file provides the tabulated values for the LRD bolometric luminosity function from Figure 8. In the paper we provide the bolometric LF in 0.5 dex bins, here we additionally include the LF marginalized over the bin size, as described in the text. 


`COSMOS-Web_LRDs_SMF.dat`: This file provides the tabulated values for the LRD contribution to the stellar mass function from Figure 11. Format is identical to `COSMOS-Web_LRDs_bol_LF.dat`.  



`COSMOS-Web_LRDs_stacked_SED.dat`: This file provides the median-stacked "maximal" SED model presented in Figure 13, from the X-ray to the radio. Wavelengths are in microns, and we provide flux density in µJy and monochromatic luminosity in solar luminosities. 


Happy to provide additional data, please reach out [over email](mailto:hollis.akins@gmail.com). 
If you use these data or intend to study these objects further, please cite the COSMOS-Web LRD paper:
```
Akins, H. B., Casey, C. M., Lambrides, E. et al. 2024,
arXiv: 24XX.XXXX, doi: XXXXXX
```
