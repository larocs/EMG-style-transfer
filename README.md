# What is EMG-style-transfer?
EMG-style-transfer is a set of ML models used for doing timeseries style transfer based on EMG signals.
You can transfer the EMG patterns from one reference signal to another signal using classical style transfer techniques.
Alternatively, you can use the "fast-style-transfer" method to train a model that learns how to transfer a specific EMG pattern to any input signal.

## Table of Contents
  * [Installation](#installation)
  * [Usage](#usage)
  * [Results](#results)
  * [Datasets](#datasets)
  * [Paper](#paper)

# Installation
We strongly recommend the usage of Anaconda for managing python environments. 
This set-up was tested under Windows #10.
```
$ conda create --name emg_style_transfer python=3.6
$ conda activate emg_style_transfer
$ git clone https://github.com/larocs/EMG-style-transfer
$ cd EMG-style-transfer/
$ pip install -r requirements.txt
$ jupyter notebook
	
```
	
# Usage
You can use the Jupyter Notebook "EMG_style_transfer" to do a step-by-step running of the model. 
Alternatively, you can use "EMG_fast_neural_style_transfer" to train a transformer network that can fastly transfer the learned style to any given input.

You can change the way to load dataset and train inside the notebook.

You can change the configurations for the prediction model on configuration.json file or directly on the jupyter notebook.

You can change the pre-loaded discriminator model used for feature extraction (taken from the project https://github.com/larocs/EMG-GAN) by any other model that you want.

You can also change the selected feature layers according to your needs.


# Datasets
This work used a private EMG dataset from Parkinson's Disease patients for the style signals and an EMG open-source dataset called NinaPro for the content signals.
NinaPro is an open-source dataset that can be downloaded on: http://ninapro.hevs.ch/

# Paper
Zanini, R. A.; Colombini, E. L. "Parkinson’s Disease EMG Data Augmentation and Simulation with DCGANs and Style Transfer". Sensors 2020, 20, 2605, doi: 10.3390/s20092605.

```
@article{DBLP:journals/sensors/ZaniniC20,
  author    = {Rafael Anicet Zanini and
               Esther Luna Colombini},
  title     = {Parkinson's Disease {EMG} Data Augmentation and Simulation with DCGANs
               and Style Transfer},
  journal   = {Sensors},
  volume    = {20},
  number    = {9},
  pages     = {2605},
  year      = {2020},
  url       = {https://doi.org/10.3390/s20092605},
  doi       = {10.3390/s20092605},
  timestamp = {Sat, 30 May 2020 19:58:33 +0200},
  biburl    = {https://dblp.org/rec/journals/sensors/ZaniniC20.bib},
  bibsource = {dblp computer science bibliography, https://dblp.org}
}
```
&nbsp;


# Interested in contributing to EMG-prediction?
Thanks for the interest and please read the [Contributing](https://github.com/larocs/EMG-style-transfer/blob/master/CONTRIBUTING.md) recommendations.

# Authors
Esther Luna Colombini & Rafael Anicet Zanini