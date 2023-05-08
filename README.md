# GnnLtsm-trafficPrediction

<h4>Highschool research project on using GNNs to perform predictions on the positions of traffic
 </h4>

---

## Motivation

- Create a prototype that gives credence to the idea of using GNNs to perform scene prediction in a driving scenerio
- Help new learners to learn AI in Pytorch.
- Learn AI. 

---

## Dataset

[Dataset](https://www.kaggle.com/datasets/robikscube/driving-video-with-object-tracking) of 1000 video files of vechicle driving footage and multi-object tracking labels. Includes:

- Unique ID's for each object
- Classification for type of object. Bus, Car, Pedestrian, Motorbike
- Position of box coordinates relative to camera

---

## Results

- The GNN-based and LTSM based programs are implimented in Pytorch
- Compare the accuracy of GNN and LTSM
- GNN still requires more work/research as of 5/7/2023
- Structure of GNN program
 - Graph each frame of a video as a node graph
  - Ground truth will have positions of box cordinates encoded into nodes and the distance between each object as a relationship
 - Train a GNN to perform predictions on what each relationship would look like
  - Given a node graph, it should guess what the relationship will b
 - Give an LTSM sets of these graphs of tx - ty-1 to predict the box cordinates of each node in ty
 
- Structure of pure LTSM program
 - Get a sequence of a single object which is done by using the unique ID given in the data set
 - Train to guess the next step of the single object
 - Perform this accross multiple objects in a video

---

## Document

The notebook is divided into the following sections

- Import libraries
  - numpy, panda, torch, torchvision, sklearn, matplotlib, Image, etc
- Utility functions for saving and loading models
- Show the project folder structure
  - Pytorch provides a default folder structure for easy loading training and testing images

## Contact

ericxu1728@gmail.com