![Pipeline status](https://gitlab.peulen.xyz/tpeulen/k2dist/badges/master/pipeline.svg?style=flat-square)

# k2dist

``k2dist`` is a tool to compute orientation factor (kappa2) distributions.

![k2dist GUI][1]


## Building and installation
``k2dist`` can be installed from the source code in a python environment that
resolves all necessary dependencies. Alternatively, ``k2dist`` can be installed 
via conda.

### Source
To install ``k2dist`` from the source clone the git repository and run the
setup script.

```commandline
git clone https://gitlab.peulen.xyz/tpeulen/k2dist
cd k2dist
python setup.py install
```
After installing ``k2dist`` you can open the GUI from the commandline.

```commandline
k2dist
```

### Conda
``k2dist`` depends on common python packages that can be installed from conda-forge. 
The easiest installation path is using conda/mamba 

```bash
mamba install k2dist -c tpeulen
```

To avoid potential conflicts ``k2dist`` can be installed in a separate environment. 

```bash
conda env create -n k2dist
conda activate k2dist
mamba install k2dist -c tpeulen
```

`k2dist` can be started from the command line as follows:

```commandline
k2dist
```


[1]: doc/gui.png "k2dist GUI"
