# One-Shot Recognition of Manufacturing Defects in Steel Surfaces

This repository contains the codes for the paper:  
**Deshpande, A. M., Minai, A. A., & Kumar, M. (2020). One-Shot Recognition of Manufacturing Defects in Steel Surfaces.** [[arxiv](https://arxiv.org/abs/2005.05815)] [[paper](https://doi.org/10.1016/j.promfg.2020.05.146)] [[website](https://adipandas.github.io/one-shot-steel-surfaces/)] [[code](https://github.com/adipandas/one-shot-steel-surfaces)]

<img src="assets/one_shot_steel_defect_demo.svg">

### Abstract

<p align=" justify">
Quality control is an essential process in manufacturing to make the product defect-free as well as to meet customer needs. The automation of this process is important to maintain high quality along with the high manufacturing throughput. With recent developments in deep learning and computer vision technologies, it has become possible to detect various features from the images with near-human accuracy. However, many of these approaches are data intensive. Training and deployment of such a system on manufacturing floors may become expensive and time-consuming. The need for large amounts of training data is one of the limitations of the applicability of these approaches in real-world manufacturing systems. In this work, we propose the application of a Siamese convolutional neural network to do one-shot recognition for such a task. Our results demonstrate how one-shot learning can be used in quality control of steel by identification of defects on the steel surface. This method can significantly reduce the requirements of training data and can also be run in real-time.
</p>

### Network Architecture

<img src="assets/siamese_network.svg" width="800px">

### Training Loss curve
<div>
<img src="assets/final_train_loss.svg" width="800px" height="500px"/>
</div>

### Requirements
```
numpy
scipy
matplotlib
torch
torchvision
scikit-learn
imutils
opencv-python
Pillow
jupyterlab
```

##### Do the following in given order to install all the packages

Create a python virtual environment, preferrablely using [Anaconda](https://www.anaconda.com/products/individual/get-started).  
Download anaconda and install from [here](https://www.anaconda.com/products/individual/get-started).  
To create the virtual environment, open terminal (anaconda prompt) and execute:
```
conda create -n steel_p36 python=3.6
```

Activate python environment in your terminal:
```
conda activate steel_p36
```

Run the following commands in your terminal to install all the dependencies.
```
pip install numpy scipy matplotlib
pip install jupyterlab
pip install Pillow
pip install opencv-contrib-python
pip install -U scikit-learn
pip install torch torchvision
```

## Dataset
You can get the dataset from the following website:

* NEU Steel Surface defect dataset [1]: [website](http://faculty.neu.edu.cn/yunhyan/NEU_surface_defect_database.html)

Sometimes, I have noticed that the server of this website is down and it cannot be reached.

In that case you can download the dataset from the following link directly:
* NEU surface defect database: [Google Drive](https://drive.google.com/open?id=0B5OUtBsSxu1Bdjh4dk1SeGYtNFU)

## Citation

If you use the code provided in this repository, please cite this work as follows:
```
@article{deshpande20201064,
title={{One-Shot Recognition of Manufacturing Defects in Steel Surfaces}},
journal= {Procedia Manufacturing},
volume= {48},
pages= {1064 - 1071},
year= {2020},
note= {48th SME North American Manufacturing Research Conference, NAMRC 48},
issn= {2351-9789},
doi= {https://doi.org/10.1016/j.promfg.2020.05.146},
url= {http://www.sciencedirect.com/science/article/pii/S2351978920315985},
author= {Aditya M. Deshpande and Ali A. Minai and Manish Kumar},
keywords= {Computer Vision, Deep Learning, Metallic Surface, Convolutional Neural Network, Defect Detection, One-shot recognition, Industrial Internet of Things, Cyber-physical systems, Siamese neural network, Few-shot learning},
}
```

### References and credits
* Song, K., & Yan, Y. (2013). A noise robust method based on completed local binary patterns for hot-rolled steel strip surface defects. Applied Surface Science, 285, 858-864.
