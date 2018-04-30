# Low dose CT image denoising using a generative adversarial network with wasserstein distance and perceptual loss

This repository contains the code for CNN/WGAN-MSE/VGG network introduced in the following paper

[Low dose CT image denoising using a generative adversarial network with wasserstein distance and perceptual loss](https://ieeexplore.ieee.org/abstract/document/8340157/)

## Installation
Make sure you have [Python](https://www.python.org/) installed, then install [TensorFlow](https://www.tensorflow.org/install/) on your system.

## Usage

### Prepare the training data

In order to start the training process, please prepare your ``training data`` in the following form:

* ``data``: N x W x H
* ``label``: N x W x H 

Here N, W, and H are number, depth, width, and height of the input data, respectively. Then ``data`` and ``label`` are stored in a ``hdf5`` file.

### Pre-trained VGG model

Please also download the pre-trained VGG model from [here](https://mega.nz/1a61c789-50d3-42f8-92af-09f89e3a152e).

### Training network
```
python train_cnn.py
python train_wgan.py
``` 


## Contact

yangq4 at rpi dot edu

Any discussions, suggestions and questions are welcome!





## Citation
```
@article{ldct_wgan_perceptual_loss,
author={Q. Yang and P. Yan and Y. Zhang and H. Yu and Y. Shi and X. Mou and M. K. Kalra and Y. Zhang and L. Sun and G. Wang},
journal={IEEE Transactions on Medical Imaging},
title={Low Dose CT Image Denoising Using a Generative Adversarial Network with Wasserstein Distance and Perceptual Loss},
year={2018},
volume={},
number={},
pages={1-1},
doi={10.1109/TMI.2018.2827462},
ISSN={0278-0062},
month={},
}
```

## Requirements

