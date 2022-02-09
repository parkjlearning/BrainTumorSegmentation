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
<br> We build CNN-based models for pixel-by-pixel segmentation of brain tumor subregions [0: Not tumor, 1: Necrotic/Core, 2: Edema, 3: Enhancing core]. Two models with <a href=”https://arxiv.org/abs/1505.04597/”> U-Net </a> and FC-DenseNet architectures were trained and their performance was evaluated. 

## Models


## Additional info. 



<!-- MARKDOWN LINKS & IMAGES -->
[license-shield]: https://img.shields.io/github/license/othneildrew/Best-README-Template.svg?style=for-the-badge
[license-url]: https://github.com/parkjlearning/covid19_forecasting/blob/main/LICENSE.txt
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
[linkedin-url]: https://linkedin.com/in/juncholpark
