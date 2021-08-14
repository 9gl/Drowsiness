# Laptop Test:

To test the code on a computer, the first step will be to have a python environments manager, such as Python Anaconda.

https://www.anaconda.com/distribution/

## Environment Creation:

### Pytorch

First we will create a suitable enviroment for pytorch.

    conda create --name pytorch

To activate the enviroment run the following command:

    activate pytorch

In the case of Anaconda the PyTorch page has a small widget that allows you to customize the PyTorch installation code according to the operating system and the python environment manager, in my case the configuration is as follows.

https://pytorch.org/

<img src="https://i.ibb.co/6RMJp5F/image.png" width="800">

    conda install pytorch torchvision cudatoolkit=10.2 -c pytorch
    
### Dependencies
    
The other packages we need are the following:

    pip install opencv-python matplotlib tqdm python-vlc Pillow
    
Anyway we attach the file requirements.txt where all packages come in our environment.

### Jupyter Notebook

Inside the **Drowsiness**, **Emotion detection** and **YoloV3** folders, you will find a file "Notebook.ipynb" which contains the code to run the programs in jupyter notebook, however I attach in each folder a file called "notebook.py" with the code in format **. py **.

    conda install -c conda-forge notebook

Command to start jupyter notebook

    jupyter notebook
