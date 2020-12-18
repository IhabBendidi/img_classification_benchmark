# Image classification benchmark
A performance benchmark of recent image classification models in deep learning

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/IhabBendidi/img_classification_benchmark/blob/main/CNN_benchmark.ipynb)
[![GitHub license](https://img.shields.io/github/license/Naereen/StrapDown.js.svg)](https://github.com/IhabBendidi/img_classification_benchmarkblob/master/LICENSE)

Image classification is considered a resolved task in academia. A lot of model architectures have appeared on the subject, achieving very high performance, starting from Alexnet, to some very accurate recent models. These models have also proven the possibility of using their weights on new tasks, which got called on Transfer Learning. This work is a comparative benchmark between the recent image classification models, using models trained from scratch built on known architectures, as well as finetuning and applying transfer learning on other pretrained models, while freezing different layers for comparative purposes.

### Dataset 

The dataset used is CIFAR-10, which is a dataset that consists of 60000 32x32 colour images in 10 classes, with 6000 images per class. There are 50000 training images and 10000 test images. We import the dataset from Pytorch datasets.

The dataset is divided into five training batches and one test batch, each with 10000 images. The test batch contains exactly 1000 randomly-selected images from each class. The training batches contain the remaining images in random order, but some training batches may contain more images from one class than another. Between them, the training batches contain exactly 5000 images from each class.

More details about the dataset can be found [here](https://www.cs.toronto.edu/~kriz/cifar.html)


### Installation  

- **Google Colaboratory**

The notebook associated to this work can be opened on Google Collaboratory without any installation using the `Open In Colab` badge above. There would be no need to import any file into the Colaboratory, the code for that is included in the Notebook.

- **Local Installation**

If the notebook is accessed locally, you need to have Pytorch installed, while having GPU on your device, as well as Cuda enabled. More instructions about that can be found [here](https://pytorch.org/get-started/locally/).

Afterward, clone this repository, and with a working Python 3 installation (Except for Python 3.9), on a terminal accessing the root of the repository, run the following command :

```
pip3 install -r requirements.txt
```

To run the notebook, you would need Jupyter Notebook installed, following the instructions [here](https://jupyter.org/install). You can then run on terminal :

```
jupyter notebook
```

You can then access this notebook under Jupyter.

### Notebook outline

**I - Data Preparation and Helper Functions**
1. *Data Preparation*
2. *Train/Test Helper Functions*

**II - Pretrained Model : Resnet**
1. *Finetune all layers*
2. *Finetune the two last layers*
3. *Finetune only the last layer*

**III - Existing Architecture : SqueezeNet**
1. *Pretrained Model : Finetuning classification layer*
2. *Training the model from scratch*

**IV - CNN model from scratch**


