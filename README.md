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
