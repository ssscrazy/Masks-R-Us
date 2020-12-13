# Masks-R-Us

## Goal:
The goal of this project is determine, from real-time video footage, whether or not an individual human is wearing a mask. We trained a machine learning algorithm using the data sets linked below in order to accomplish this. More information can be found in our report: "Final Report.pdf"

## Code:
The code was developed entirely in Python. We developed two primary Python programs.
The first of these is called "Augmented_train_net.ipynb" This program was used to train the machine learning model we used to classify between masked and unmasked people. We used a pretrained Pytorch ResNet-50 model and then applied transfer learning to retrain the model to differentiate between masked and unmasked people. This is meant to run with Google Colab or in a Jupyter notebook. More information can be found in our report. 

The second of these is called "video_masked_or_not.py" This program takes the model generated by the first program. It looks at a webcam on your computer and samples individual frames. Then, it runs each of these frames through our classifier to detect whether or not you are wearing a mask properly. On lines 99/100 of this program, you can find a tuneable constant parameter. This parameter can be used to adjust for different camera quality and lighting conditions. This program can be run like any standard Python program from the terminal or command prompt. You must have the OpenCV and PyTorch libraries installed.

## Data Sets:
We used the following data sets to train our machine learning algorithm:
http://mmlab.ie.cuhk.edu.hk/projects/CelebA.html - People without masks
https://github.com/cabani/MaskedFace-Net - People wearing masks properly and people wearing masks improperly

## Google Drive Link
Here is a read-only link to the Google Drive we used for this project: 
https://drive.google.com/drive/folders/1YeNshscfAkP8w8arQuJiCTdGuDcSgJcV?usp=sharing

In the drive, you can find photos from our data set, and the various training programs we wrote. 
