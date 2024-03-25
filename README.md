[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/Cloud-Drift/hurdat2-get-started/HEAD)

# hurdat2-get-started (experimental)
This repository contains a notebooks to get you started with the [HURDAT2 dataset](https://www.aoml.noaa.gov/hrd/hurdat/Data_Storm.html) using python and the [*xarray* library](https://docs.xarray.dev/en/stable/). 


## Using experimental examples
Make sure you install the dependencies for the notebook and clouddrift:
```bash
conda env create -n hurdat2-get-started -f environment.yaml
conda env update -n hurdat2-get-started --file dependencies/clouddrift/environment.yaml
```

Utilize the `hurdat2-get-started` environment for the notebooks