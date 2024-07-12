---
layout: distill_project
title: Virtual Multi-view Fusion
description: Virtual Multi-view Fusion for 3D Semantic Segmentation
img: assets/img/multiview_segmentation/scene0708_00_combined.webp
og_image: assets/img/multiview_segmentation/virtualMVFusion_thumbnail.gif
importance: 5
category: research
date: 2020-08-23

authors:
  - name: Abhijit Kundu
    url: "https://abhijitkundu.info"
    affiliations:
      name: Google Research
  - name: Xiaoqi Yin
    url: "https://scholar.google.com/citations?user=2eADYP8AAAAJ&hl=en"
    affiliations:
      name: Google Research
  - name: Alireza Fathi
    url: "https://www.alirezafathi.org/"
    affiliations:
      name: Google Research
  - name: David Ross
    url: "https://research.google/people/author23969/"
    affiliations:
      name: Google Research
  - name: Brian Brewington
    url: "https://scholar.google.com/citations?user=wQTWcRgAAAAJ&hl=en"
    affiliations:
      name: Google Research
  - name: Thomas Funkhouser
    url: "https://www.cs.princeton.edu/~funk/"
    affiliations:
      name: Google Research
  - name: Caroline Pantofaru
    url: "https://scholar.google.com/citations?user=vKAKE1gAAAAJ&hl=en"
    affiliations:
      name: Google Research

citation_key: KunduECCV2020VirtualMVFusion
---

<!-- Import the component -->
<script type="module" src="https://unpkg.com/@google/model-viewer/dist/model-viewer.min.js"></script>

<p>
    <a href="https://arxiv.org/pdf/2007.13138.pdf" class="btn btn-primary z-depth-1">Paper <i class="fas fa-file-pdf"></i></a>
    <a href="https://youtu.be/f_LYCKvzo_I" class="btn btn-primary z-depth-1">Short Video <i class="fab fa-youtube"></i></a>
    <a href="https://youtu.be/dJILFsB2CpA" class="btn btn-primary z-depth-1">Long Video <i class="fab fa-youtube"></i></a>
</p>

## Abstract

<div class="row">
  <div class="col-lg-6 text-center">
    <h4>Input mesh</h4>
      <video width="384" playsinline="" autoplay="" loop="" preload="" muted="">
        <source src="../../assets/videos/multiview_segmentation/scene0708_00_input.mp4" type="video/mp4">
      </video>
  </div>
  <div class="col-lg-6 text-center">
    <h4>Output labeled mesh</h4>
      <video width="384" playsinline="" autoplay="" loop="" preload="" muted="">
        <source src="../../assets/videos/multiview_segmentation/scene0708_00_ours.mp4" type="video/mp4">
      </video>
  </div>
</div>

Semantic segmentation of 3D meshes is an important problem for 3D scene understanding. In this paper we revisit the classic multiview representation of 3D meshes and study several techniques that make them effective for 3D semantic segmentation of meshes. Given a 3D mesh reconstructed from RGBD sensors, our method effectively chooses different virtual views of the 3D mesh and renders multiple 2D channels for training an effective 2D semantic segmentation model. Features from multiple per view predictions are finally fused on 3D mesh vertices to predict mesh semantic segmentation labels. Using the large scale indoor 3D semantic segmentation benchmark of ScanNet, we show that our virtual views enable more effective training of 2D semantic segmentation networks than previous multiview approaches. When the 2D per pixel predictions are aggregated on 3D surfaces, our virtual multiview fusion method is able to achieve significantly better 3D semantic segmentation results compared to all prior multiview approaches and recent 3D convolution approaches.


## Method

<div class="embed-responsive embed-responsive-16by9">
    <iframe class="embed-responsive-item" src="https://www.youtube.com/embed/dJILFsB2CpA" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
</div>


## Results

### Interactive meshes segmented by our method

<div class="row">
  <div class="col-lg-6">
    <model-viewer src="../../assets/glb/multiview_segmentation/scene0761_00.glb" style="width: 100%; height: 320px;" alt="scene0761_00.glb"
      auto-rotate camera-controls>
    </model-viewer>
  </div>
  <div class="col-lg-6">
    <model-viewer src="../../assets/glb/multiview_segmentation/scene0776_00.glb" style="width: 100%; height: 320px;" alt="scene0776_00.glb"
      auto-rotate camera-controls>
    </model-viewer>
  </div>
  <div class="col-lg-6">
    <model-viewer src="../../assets/glb/multiview_segmentation/scene0709_00.glb" style="width: 100%; height: 320px;" alt="scene0709_00.glb"
      auto-rotate camera-controls>
    </model-viewer>
  </div>
  <div class="col-lg-6">
    <model-viewer src="../../assets/glb/multiview_segmentation/scene0708_00.glb" style="width: 100%; height: 320px;" alt="scene0708_00.glb"
      auto-rotate camera-controls>
    </model-viewer>
  </div>
</div>

<div class="row">
  <img width="100%" src="../../assets/img/multiview_segmentation/nyu20_legend.jpg" alt="NYU 20 category legend">
</div>


### More results on Scannet dataset

<div class="row">
  <div class="col-lg-6">
    <video width="100%" playsinline="" autoplay="" loop="" preload="" muted="">
      <source src="../../assets/videos/multiview_segmentation/scene0221_00_ours.mp4" type="video/mp4">
    </video>
  </div>
  <div class="col-lg-6">
    <video width="100%" playsinline="" autoplay="" loop="" preload="" muted="">
      <source src="../../assets/videos/multiview_segmentation/scene0733_00_ours.mp4" type="video/mp4">
    </video>
  </div>
  <div class="col-lg-6">
    <video width="100%" playsinline="" autoplay="" loop="" preload="" muted="">
      <source src="../../assets/videos/multiview_segmentation/scene0435_01_ours.mp4" type="video/mp4">
    </video>
  </div>
  <div class="col-lg-6">
    <video width="100%" playsinline="" autoplay="" loop="" preload="" muted="">
      <source src="../../assets/videos/multiview_segmentation/scene0708_00_ours.mp4" type="video/mp4">
    </video>
  </div>
  <div class="col-lg-6">
    <video width="100%" playsinline="" autoplay="" loop="" preload="" muted="">
      <source src="../../assets/videos/multiview_segmentation/scene0645_00_ours.mp4" type="video/mp4">
    </video>
  </div>
  <div class="col-lg-6">
    <video width="100%" playsinline="" autoplay="" loop="" preload="" muted="">
      <source src="../../assets/videos/multiview_segmentation/scene0721_00_ours.mp4" type="video/mp4">
    </video>
  </div>
</div>

<div class="row">
  <img width="100%" src="../../assets/img/multiview_segmentation/nyu20_legend.jpg" alt="NYU 20 category legend">
</div>
