# COSMOS-Web LRDs
Repository for data and figures from Akins et al. (2024) paper on LRDs in COSMOS-Web


`COSMOS-Web_LRDs_May2024.dat`: this is an extended and machine-readable form of Table 1 in the paper, including coordinates, photometry (in all available bands), and derived physical properties (from QSO and galaxy fits) for all 429 objects in the sample. The file is in the `ecsv` format, and can be read into python using `astropy`: 
```
from astropy.table import Table
t = Table.read('COSMOS-Web_LRDs_May2024.dat', format='ascii.ecsv')
```

`COSMOS-Web_LRDs_bol_LF.dat`: 


`COSMOS-Web_LRDs_SMF.dat`: 



Happy to provide additional data, please reach out [over email](mailto:hollis.akins@gmail.com). 
If you use these data or intend to study these objects further, please cite the COSMOS-Web LRD population paper
```
Akins, H. B., Casey, C. M., ???, et al. 2024,
arXiv: 24XX.XXXX, doi: XXXXXX
```
