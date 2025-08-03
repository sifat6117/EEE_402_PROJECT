# EEE_402_PROJECT
Here all necessary files of our project "A Deep Learning Framework for Simultaneous Brain Tumor Segmentation and Classification from MRI Images" are stated.

A short brief on our Project:

>Project Title:  A Deep Learning Framework for Simultaneous
                 Brain Tumor Segmentation and Classification from
                 MRI Images
>
> A TensorFlow-based, multi-task convolutional neural network that simultaneously segments brain tumors and classifies their type (meningioma, glioma, pituitary) from contrast-enhanced T1-weighted MRI scans. Features a shared encoder, Convolutional Block Attention Module (CBAM), dual decoder/classifier heads, end-to-end preprocessing (MATLAB→JPEG/PNG, resize, normalize, channel-expand) and on-the-fly Albumentations augmentations.
>
> Key results:
>
> * "97 %" classification accuracy (vs. 96.49 % ResNet50, 95.94 % InceptionV3)
> * "0.7930" validation Dice score (vs. 0.7629 U-Net), "0.7046" test Dice score
>
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
