---
title: "Image Comparator"
date: 2025-07-12 16:25:10 +0800
categories: [Image alignment]
tags: [Image Comparision, Alignment, Multi-modal, Image alignment, homography, transformation, python, homographynet]
---

# Image Comparator for RGB and Thermal (IR) images

### Check the image comparator I have built using RGB and Thermal images: 
[Demo](https://amartyacsb.github.io/ImageComparator)

### Live Demo: RGB ∥ Thermal Comparator

<div style="position:relative; padding-bottom:56.25%; height:0; overflow:hidden; margin-bottom:1rem;">
  <iframe
    src="https://amartyacsb.github.io/ImageComparator/"
    style="position:absolute; top:0; left:0; width:100%; height:100%; border:0;"
    allowfullscreen
  ></iframe>
</div>
<iframe src="…/ImageComparator/" width="100%" height="600" frameborder="0"></iframe>


#### Introduction
###### Image comparator for the image alignment of 2 domains for images captured by different sensors of a drone gimbal 

#### Description
###### No Photoshop or online image alignment tool was used. The 2 images were captured by Drone Gimbal as part of my work when flying drones at commercial properties. You can see there are thermal anomalies of Air Leakage on the infrared image which isn't visible on the RGB image which our normal cameras click. We want to first align these images taken by different sensors of the gimbal camera. I have used DeepHomography Net and classical computer vision algorithms to align them. More details to follow!

#### Check my Github repo as I build more functionalities over the next few weeks: 
[Github Link for project](https://github.com/AmartyaCSB/ImageComparator)
