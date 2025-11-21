**AI-Based Recyclable Waste Classification**



![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)




**Overview**



This project applies deep learning techniques to classify recyclable waste into six categories using a fine-tuned ResNet-50 model. Four different training configurations were compared to study how learning rate, training duration, and dataset composition influence model performance.



*All experiments were conducted in Google Colab Pro using an A100 GPU.*



The six waste categories included are:



* cardboard
* glass
* metal
* paper
* plastic
* trash



**Dataset Access**



Two datasets were used for training and evaluation:



1. Original Dataset



https://drive.google.com/drive/folders/16Zs7avXr6p8Ajk075gQX9DVsBb5Gn4ZU?usp=drive\_link



2\.     New Dataset



https://drive.google.com/drive/folders/1MEKyRiCEgJOVCKbC8uvHpifTdALyqJhQ?usp=drive\_link



Both datasets follow a directory structure compatible with PyTorch’s ImageFolder.



**Trained Models (Weights)**



Due to GitHub size limits, the trained .pth model files are stored in Google Drive.



Download Trained Models



https://drive.google.com/drive/folders/14K4bVQZQY4DbDxflgj5u0Vf8utFghxqL?usp=drive\_link



**This folder contains:**



Model 1 (Baseline)



Model 2 (Higher LR)



Model 3 (Reduced Epochs)



Model 4 (New Dataset)





**Model Configurations**



Model	Learning Rate	Epochs	Dataset	Purpose

Model 1	0.00001	50	Original	Baseline configuration

Model 2	0.0001	50	Original	Test effect of higher learning rate

Model 3	0.00001	10	Original	Test effect of reduced training

Model 4	0.00001	50	New Dataset	Test impact of dataset diversity

Features



Fine-tuned ResNet-50 architecture



Multiple experimental setups



Validation accuracy and loss curves



Confusion matrices



Precision, recall, and F1-score comparisons



ROC curves



FPR vs FNR analysis



Comprehensive model comparison



**Project Structure**



project-folder/

│── CS316\_AI\_Based\_Recyclable\_Waste\_Classification.ipynb

│── requirements.txt

│── README.md

│── LICENSE

│── (Not included on GitHub) models/  → Models available via Google Drive



**How to Run**



Install dependencies:



pip install -r requirements.txt





2\.  Open the notebook:



CS316\_AI\_Based\_Recyclable\_Waste\_Classification.ipynb





3\.  Run all cells to:



Load dataset



Train models



Generate evaluation plots



Compare model performance



Requirements

torch

torchvision

numpy

matplotlib

pillow

scikit-learn

opencv-python



**Acknowledgments**



This project was completed as part of **Prince Sultan University**,

College of Computer and Information Systems,

CS316: Introduction to AI and Data Science.



We would like to express our gratitude to Dr. Sawsan AlHalawani for her supervision, guidance, and continuous support throughout the course and the development of this project.



**License**



**This project is licensed under the MIT License.**



**You are free to use, modify, and distribute this code, as long as credit is given:**



**Copyright (c) 2025 Deem Alhaqbani, Norah Bin Salamah, Lina Bin Muammar**



**Full license text is available in the LICENSE file.**




