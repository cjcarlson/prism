##`prism`
A package to access and visualize data from the [Oregon State PRISM project](http://www.prism.oregonstate.edu/).  Data is all in the form of gridded rasters for the continental US at 3 different scales: daily, monthly and 30 year normals.  Please see their webpage for a full description of the data products, or [see their overview](http://www.prism.oregonstate.edu/documents/PRISM_datasets_aug2013.pdf).

### Quickstart
Currently the package is only available on github and installable with `devtools`

```r
library(devtools)
install_github(repo = "prism", username = "ropensci")
library(prism)
```

### Downloading data

Data is available in 3 different forms as mentioned above.  Each one has it's own function to download data. While each data type has slightly different temporal parameters, the type options are always the same.  Keep in mind these are modeled parameters, not measured.  Please see the [full description](http://www.prism.oregonstate.edu/documents/Daly2008_PhysiographicMapping_IntJnlClim.pdf) for how they are calculated.

| Parameter name| Descrption           |
|:---------------:|:-------------:|
| *tmean*      | Mean temperature | 
| *tmax*      | Maximum temperature      | 
| *tmin* | Minimum temperature      |
| *ppt*  | Total precipitation (Rain and snow)|


