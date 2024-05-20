# Automatic Video Captioning 

## Overview

The video captioning task for machine learning models entails the generation of textual descriptions for a given video. 
Some simpler models have been executed as experiments, with and without adversarial examples, to better understand the pros and cons of existing video captioning models.

Here, notebooks to run the CNN-LSTM and evaluation metrics are included. The LLaVA model was tested directly through its published UI. 

For more information on my research and findings, read [my paper](https://github.com/pranavas11/Automatic-Video-Captioning/blob/main/Automatic%20Video%20Captioning.pdf) and [project presentation](https://github.com/pranavas11/Automatic-Video-Captioning/blob/main/AVC%20Presentation.pdf).

## Notebooks

### Notebook 1: Metrics.ipynb

Description:
- Metrics jupyter notebook shows calculations of metrics for BLEU, ROUGE-L, and METEOR scores for all of the experiments (CNN, CNN-Adversarial, LLaVA, LLaVA-Adversarial).
- Data folder is referenced

### Notebook 2: Keras_MSVD.ipynb

Description:
- This Jupyter Notebook contains the code for running a pre-trained CNN-LSTM model for video captioning.
- KerasModel folder is referenced

## Data

- The `data` folder contains relevant resulting captions used in the notebooks. We based our data on the MSVD testing dataset. There is the base training data, results from training the CNN-LSTM ("greedy") and LLaVA models with and without adversarial examples. 
- The `KerasModel` folder contains all relevant information for running the CNN-LSTM included in the notebooks. This folder includes the videos for the testing dataset, a set of already extracted features for said videos, and another copy of both using adversarial data.


## Usage

- Can run jupyter notebooks with data provided
- `Keras_MSVD.ipynb` was designed to be used in Google Colab, but contains information on adjusting the notebook to run locally. This notebook references the `KerasModel` folder. To use the notebook as is, place this folder in extracted form at the highest level of your Google Drive directory. Afterwards, just follow the instructions in the notebook to generate your captions!


## References

Code referenced/adapted in the creation of these notebooks can be found at:
- [LLaVA Model](https://github.com/haotian-liu/LLaVA)
- [CNN-LSTM Model](https://github.com/Shreyz-max/Video-Captioning)
- [Caption Evaluation](https://github.com/vsubhashini/caption-eval)
