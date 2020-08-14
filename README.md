# Miami DS Meet-Up August 19th, 2020
## Overview

In this session, we will dive into "Building Advanced Image Classifiers with PyTorch".  We will build an image classifier that will be able to detect 5 different types of flowers using an actual vision dataset from Kaggle:

https://www.kaggle.com/alxmamaev/flowers-recognition 

The dataset contains 4242 images across 5 difference classes.   For those of you that want to follow along with Colab, there is a slightly smaller flower dataset you will load.

## Session Agenda
1.  Review deep learning basics
2.  Understand CNN components and why they work
3.  Code a simple CNN model from scratch
4.  Build a state of the art classifier using a pre-trained network

## Setting Up Your Environment
You have 3 options to follow along.  If you have a GPU on your laptop/desktop, you can load the libraries and dataset locally and run the notebook locally.   Otherwise, you can choose to run the notebook (free) in Google Colab.  Note, it is not required that you run the notebook to attend the session but it will help you understand the content.

### Option 1 - Setup your own laptop/PC with GPU for this workbook

If you have a GPU and want to work on your own laptop/PC:

1.  Download the dataset from Kaggle (https://www.kaggle.com/alxmamaev/flowers-recognition) and unzip the dataset on your local drive
2.  Download Anaconda  (https://www.anaconda.com/distribution/)
3.  Create a virtual environment using Anaconda on your local machine by following these commands:

```
conda create --name MiamiData2020 python=3.8
conda activate MiamiData2020
conda install pytorch torchvision cudatoolkit=10.2 -c pytorch
conda install matplotlib jupyter
conda install -c intel scikit-learn
pip install efficientnet_pytorch
pip install torchsummary
python -m ipykernel install --user --name MiamiData2020 --display-name "MiamiData2020"
git clone https://github.com/jacobffjensen/MiamiDS2020June
jupyter notebook
```

4. Skip Option 2 below and deactivate the first code cell of the notebook by selecting it and typing "R" (intended for Colab only)
5. Specify the directory of your dataset in the 2nd cell below.

### Option 2 - Follow along in a Google Colab workbook

If you want to work in Google Colab, into Colab and pull the notebook file from GitHub:
1.  Go to colab.research.google.com
2.  Click **GitHub** and paste the address **https://github.com/jacobffjensen/MiamiDS2020August**
3.  Click **Search Icon**
4.  Click on **MiamiDSMeetupAugust2020.ipynb**, notebook should now open
5.  Set the notebook settings to **Python** and **GPU** (**Edit -> Notebook Settings**) 

Then, we will load the dataset into Colab by executing the first cell (click the cell, then click **crtl+enter**).

### Option 3 - Just follow along during the presentation
Running the notebook is not required to get something out of the session :)