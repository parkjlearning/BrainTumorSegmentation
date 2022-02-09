<!-- PROJECT SHIELDS -->
[![MIT License][license-shield]][license-url]
[![LinkedIn][linkedin-shield]][linkedin-url]


# Brain tumor segmentation with U-Net and FC-DenseNets
Semantic image segmentation predicts class labels for each pixel in the image. In medicine, semantic segmentation is widely used for medical image diagnostics, where machines can augment analysis performed by radiologists with efficiency and scalability. One active area of research is brain tumor segmentation, where deep neural networks are trained to predict where each pixel falls into tumorous tissue classes that were labeled by neuroradiologists. In this work, we used a data set comprising clinically-acquired pre-operative multimodal MRI scans of glioblastoma and lower grade glioma, common types of brain tumors. This data set was preprocessed and labeled by neuroradiologists for BraTS 2020 competiton. We trained two state-of-the-art deep neural network models for image segmentation, U-net and FC-DeepNets and evaluated their performance.

## Motivation
<div align="center">
<a href="https://github.com/parkjlearning/BrainTumorSegmentation/blob/master/Final_Report_Brain_tumor_segmentation_on_multimodal_MRI_scans_with_deep_learning.pdf">
<img src="https://github.com/parkjlearning/BrainTumorSegmentation/blob/master/snapshots/Fig4_BraTS_annotations_structures.jpeg" style="width:900px;height:400px;"></a>
<div align="left">
<br> We build CNN-based models for pixel-by-pixel segmentation of brain tumor subregions [0: Not tumor, 1: Necrotic/Core, 2: Edema, 3: Enhancing core]. Two models with 
<a href="https://arxiv.org/pdf/1505.04597.pdf">U-Net</a> and <a href="https://arxiv.org/pdf/1611.09326.pdf">FC-DenseNets</a> architectures were trained and their performance was evaluated using various metrics (see below). The MRI data are collected/preprocessed by the BraTS community for 2020 <a href="https://www.med.upenn.edu/cbica/brats2020/data.html">BraTS</a> challenge.  

## Models
<div align="center">
<a href="https://github.com/parkjlearning/BrainTumorSegmentation/blob/master/Final_Report_Brain_tumor_segmentation_on_multimodal_MRI_scans_with_deep_learning.pdf">
<img src="https://github.com/parkjlearning/BrainTumorSegmentation/blob/master/snapshots/Fig8_U-Net_architecture.png" style="width:850px;height:700px;"></a>
<div align="left">
U-Net comprises symmetrical downsampling, upsampling paths, and skip connections between them (Ronneberger et al., 2015).
<div align="center">
<a href="https://github.com/parkjlearning/BrainTumorSegmentation/blob/master/Final_Report_Brain_tumor_segmentation_on_multimodal_MRI_scans_with_deep_learning.pdf">
<img src="https://github.com/parkjlearning/BrainTumorSegmentation/blob/master/snapshots/Fig12_FC-DenseNets_architecture.png" style="width:750px;height:700px;"></a>
<div align="left">
Fully-convolutional DenseNets also comprises downsampling (contracting) and upsampling (expanding) paths as well as the skip connections from the downsampling to the upsampling path. The downsampling path incorporated three dense blocks, in which all feature outputs are iteratively concatenated in a feedforward fashion to facilitate the feature reuse. 
  
## Model evaluation 
<div align="center">
<a href="https://github.com/parkjlearning/BrainTumorSegmentation/blob/master/Final_Report_Brain_tumor_segmentation_on_multimodal_MRI_scans_with_deep_learning.pdf">
<img src="https://github.com/parkjlearning/BrainTumorSegmentation/blob/master/snapshots/Fig10_goundtruth_prediction.png" style="width:950px;height:700px;"></a>
<div align="left">
To assess model performance, we used the held out test set and visualized model predictions and ground truths in tandem for each class and observed that they largely overlapped.   
  
  



## Additional info. 



<!-- MARKDOWN LINKS & IMAGES -->
[license-shield]: https://img.shields.io/github/license/othneildrew/Best-README-Template.svg?style=for-the-badge
[license-url]: https://github.com/parkjlearning/covid19_forecasting/blob/main/LICENSE.txt
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
[linkedin-url]: https://linkedin.com/in/juncholpark
