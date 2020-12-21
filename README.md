# ensoNN

This repository is for testing ENSO Neural Network codes following [Toms et al. 2020, JAMES](https://agupubs.onlinelibrary.wiley.com/doi/full/10.1029/2019MS002002)

It uses [iNNvestigate](https://github.com/albermax/innvestigate)

## Setup steps

Setup your conda environment:

```conda env create -f environment.yml```

Activate your conda environment:

```conda activate ensonn```

Setup the environment to appear in Jupyter:

```python -m ipykernel install --user --name ensonn --display-name "Python (ensonn)"```

Launch Jupyter and select this environment before running the example notebooks.

## Codes

Tomsetal_reproduce.ipynb is my attempt to reproduce Figures 6b, 7a, 7b from the Toms et al. 2020 paper.  

Currently, it is very close, but I have some issues that I am not sure about.  In particular, there are some slight differences in the patterns outside of the ENSO region, which I assume are due to:

1. My version of the NN is not 100% accurate in 100 epochs as they report.  They use an initial learning rate of 0.01 which is reduced by a factor of 0.5 after 50 epochs. I am not sure how to reduce the learning rate.

2. Some differences in the number of El Nino events.  Toms et al reports 337 total El Nino samples including both training and testing data.  I have 410.  I have not yet determined why the number is different.
