# ensoNN

This repository is for testing ENSO Neural Network codes following different papers:

1.  tomeetal2020:  following [Toms et al. 2020, JAMES](https://agupubs.onlinelibrary.wiley.com/doi/full/10.1029/2019MS002002)

It uses [iNNvestigate](https://github.com/albermax/innvestigate)

2. hametal2019: following [Ham et al. 2019, Nature](https://rdcu.be/cdnSI)


## Setup steps

Setup your conda environment:

```conda env create -f environment.yml```

Activate your conda environment:

```conda activate ensonn```

Setup the environment to appear in Jupyter:

```python -m ipykernel install --user --name ensonn --display-name "Python (ensonn)"```

Launch Jupyter and select this environment before running the example notebooks.

## Codes

In `tomsetal2020`:

Tomsetal_reproduce.ipynb is my attempt to reproduce Figures 6b, 7a, 7b from the Toms et al. 2020 paper.

predict_ENSO.ipynb takes the NN from Toms et al. and applies it to predicting ENSO at a specified lead time.

In `hametal2019`:


