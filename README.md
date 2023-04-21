# Reproducibility of Multi-Objective Reinforcement Learning Recommendation: Interplay between Effectiveness and Beyond-Accuracy Perspectives
This repository refers to source codes and datasets of the reproducibility study _Reproducibility of Multi-Objective Reinforcement Learning Recommendation:
Interplay between Effectiveness and Beyond-Accuracy Perspectives_ submitted to The 17th ACM Recommender Systems Conference (RecSys 2023).

Due to the size limits of GitHub, we load the files at this [link](https://drive.google.com/file/d/1L40DnK4N9_iR0tXtGLWpXW6QfGcoUZVI/view?usp=share_link). This link contains two folders:

 1. SMORL: it contains the source codes and datasets to reproduce the results in Section 4;
 2. my_sir_elliot: it contains the source codes and datasets to reproduce the results in Section 5.
 
Please, make sure to have a Python `3.8.0` or later version installed on your device.

We advice to treat these folders as two separate projects. For each project, you may create the virtual environment with the requirements files we included as follows:

```
$ python3 -m venv venv
$ source venv/bin/activate
$ pip install --upgrade pip
$ pip install -r requirements.txt
```
 To run the models in the SMORL project, you should install a version of ```pytorch``` compatible with the CUDA version of your device.
 
 ## SMORL Project
 
 In the SMORL Project, you find two folders:
 
 1. _div4rec_ contains datasets and files needed to run the models and the results gathered in Section 4;
 2. _src_ contains the source codes to run the models.
 
 To run a model, you may run the following commands:
 

```
$ cd src
$ python -u {modelname}.py
```
where {modelname} is one of the following: ```Caser```, ```CaserSMORL```, ```GRU```, ```GRUSMORL```, ```NexItNet```, ```NextItNetSMORL```, ```SASRec```, ```SASRecSMORL```.

In these files, you should change the datasets name in the ```Args``` class. Please, you should use ```rc15``` for the RC 15 dataset, while ```retail_rocket``` for the Retailrocket dataset. You will find the results in the corresponding folder within the _div4rec_ directory.
