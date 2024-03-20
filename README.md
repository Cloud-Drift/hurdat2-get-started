[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/Cloud-Drift/hurdat2-get-started/HEAD)

# hurdat2-get-started (experimental: [branch](https://github.com/kevinsantana11/clouddrift/tree/hurdat2-adapter))
This repository contains a notebooks to get you started with the [HURDAT2 dataset](https://www.aoml.noaa.gov/hrd/hurdat/Data_Storm.html) using python and the [*xarray* library](https://docs.xarray.dev/en/stable/). 


## Using examples
This guide is for running (experimental) labelled examples. It assumes you are performing actions within an isolated environment created via `venv`, `conda` or `micromamba`.
It also should be noted that in the examples the remote and branch should be replaced with those identified by the branch link.


0. Create a folder named `experimental-<some-identifier>` (e.g. - experimental-hurdat2-adapter), `cd` into it.
1. Check out the remote branch locally (e.g.)
```bash
git clone https://github.com/kevinsantana11/clouddrift # pull down the remote
cd clouddrift
git checkout hurdat2-adapter # checkout the branch
```

2. Install the build dependencies
```bash
pip install build twine docutils
```

3. Build the **experimental package**! (this will create a `.whl` file in the `./dist/` folder)
```bash 
python -m build
```

4. go back up to the base dir we initially created `cd ..`

5. Check out the experimental repository (e.g)
```bash
git clone git@github.com:kevinsantana11/hurdat2-get-started.git
```

6. Install dependencies
```bash
conda install -f environment.yaml
```

7. Install the **experimental package** (e.g.)
```bash
python -m pip install ../clouddrift/dist/clouddrift-0.32.0-py3-none-any.whl # note 0.32.0 can be replaced with any version
```

8. You can now run the experimental notebook


- `hurdat2_get_started.ipynb` demonstrates loading the dataset, selecting a subset of the trajectories and then plot them using `cartopy`

This notebook should be readily executable in a binder environment which can be launched by clicking the "launch binder" badge above :point_up:. Alternatively, you can run the notebook in a python environment containing the python libraries listed in the file `environment.yml`.

Feel free to contribute to this repo or raise an issue!
