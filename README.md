# k2dist

``k2dist`` is an tool to compute orientation factor (kappa2) distributions.

![k2dist GUI][1]


## Building and installation
``k2dist`` can be installed from the source code in an python environment that
resolves all necessary dependencies. Alternatively, ``k2dist`` can be installed 
via conda.

### Source
To install ``k2dist`` from the source code clone the git repository and run the
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
``k2dist`` depends on common python packages such as ``numpy``. Additionally, ``k2dist`` depends on 
``scikit-fluorescence``. Thus, to install ``k2dist`` make sure that conda channels that provide packages for the necessary
dependencies are listed in the ``.condarc`` file 

```yaml
channels:
  - salilab
  - tpeulen
  - tpeulen/label/nightly
  - conda-forge
  - defaults
```

To avoid potential conflicts ``k2dist`` can be installed in a separate environment. 

```commandline
conda create -n test
conda install k2dist
```


[1]: doc/gui.png "k2dist GUI"
