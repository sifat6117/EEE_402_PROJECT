# EEE_402_PROJECT
Here all necessary files of our project "A Deep Learning Framework for Simultaneous Brain Tumor Segmentation and Classification from MRI Images" are stated.

A short brief on our Project:

>Project Title:  A Deep Learning Framework for Simultaneous
                 Brain Tumor Segmentation and Classification from
                 MRI Images
>
> A TensorFlow-based, multi-task convolutional neural network that simultaneously segments brain tumors and classifies their type (meningioma, glioma, pituitary) from contrast-enhanced T1-weighted MRI scans. Features a shared encoder, Convolutional Block Attention Module (CBAM), dual decoder/classifier heads, end-to-end preprocessing (MATLAB→JPEG/PNG, resize, normalize, channel-expand) and on-the-fly Albumentations augmentations.
> 
> Methodology:
>
>
> <img width="849" height="539" alt="image" src="https://github.com/user-attachments/assets/b0fe079b-d7be-4580-9da1-87ec0eab8041" />


Data Preprocessing:


![photo_2025-08-04_21-21-33](https://github.com/user-attachments/assets/2deb2ae3-2985-4199-aa72-6d959b84e5de)

Model Architecture:

<img width="895" height="886" alt="image" src="https://github.com/user-attachments/assets/72924bc8-5be6-45b5-9239-6398439ed73b" />


> Key results:
>
> * "97 %" classification accuracy (vs. 96.49 % ResNet50, 95.94 % InceptionV3)
> * "0.7930" validation Dice score (vs. 0.7629 U-Net), "0.7046" test Dice score
>
> Classification Result:
> 
> <img width="1451" height="817" alt="image" src="https://github.com/user-attachments/assets/e78c5de9-ba96-4ba8-9049-46d14ea15e9f" />

Confusion Matrix:

<img width="1161" height="886" alt="image" src="https://github.com/user-attachments/assets/a5e5c49d-3946-4c31-9a3e-99ea17d2ab4b" />


Segmentation Result:

<img width="889" height="914" alt="image" src="https://github.com/user-attachments/assets/d883b3db-9b4a-4112-acc4-5b6b76b9e959" />


> Contents
>
> * `data/` MATLAB→image conversion and train/test split scripts
> * `models/` architecture definitions (encoder, CBAM, decoder & classifier heads)
> * `train.py` / `evaluate.py` training loops with multi-task loss (cross-entropy + BCE+Dice)
> * `notebooks/` visualization of metrics (loss curves, confusion matrix, IoU, Hausdorff)
> * `README.md` installation, usage instructions, and detailed architecture diagram
>   
> Group 5 (G1), EEE 402 AI & ML Laboratory, BUET
>
> Group Members(according to IDs):
>
> Md. Woahidur Rahman           ID: 2006102
>
> Shahriar Rashid Khan Sifat    ID: 2006117
>
> Tanvir Arafat Fahim           ID: 2006118
