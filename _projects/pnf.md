---
layout: distill_project
title: Panoptic Neural Fields
description: A Semantic Object-Aware Neural Scene Representation
img: assets/img/pnf/kitti360_nvs50_train02.webp
og_image: assets/img/pnf/pnf_applications.gif
importance: 1
category: research
date: 2022-05-8

authors:
  - name: Abhijit Kundu
    url: "https://abhijitkundu.info"
    affiliations:
      name: Google Research
  - name: Kyle Genova
    url: "https://www.kylegenova.com/"
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
  - name: Caroline Pantofaru
    url: "https://scholar.google.com/citations?user=vKAKE1gAAAAJ&hl=en"
    affiliations:
      name: Google Research
  - name: Leonidas J. Guibas
    url: "https://geometry.stanford.edu/member/guibas/"
    affiliations:
      name: Google Research
  - name: Andrea Tagliasacchi
    url: "https://taiya.github.io/"
    affiliations:
      name: Google Research
  - name: Frank Dellaert
    url: "https://dellaert.github.io/"
    affiliations:
      name: Google Research
  - name: Thomas Funkhouser
    url: "https://www.cs.princeton.edu/~funk/"
    affiliations:
      name: Google Research

citation_key: KunduCVPR2022PNF
bibliography: pnf.bib


toc:
  - name: Video
  - name: Abstract
  - name: Applications
  - name: Results

_styles: >
  .video_with_border{
    border:1px solid gray;
  }

---

<p>
    <a href="https://arxiv.org/pdf/2205.04334.pdf" class="btn btn-primary z-depth-1">Paper <i class="fas fa-file-pdf"></i></a>
    <a href="../../assets/pdf/PNF_CVPR22_Poster.pdf" class="btn btn-primary z-depth-1">Poster <i class="fas fa-file-pdf"></i></a>
    <a href="https://youtu.be/3aXHxuQ-xBM" class="btn btn-primary z-depth-1">Talk <i class="fab fa-youtube"></i></a>
</p>

## Video

<div class="embed-responsive embed-responsive-16by9">
    <iframe class="embed-responsive-item" src="https://www.youtube.com/embed/3aXHxuQ-xBM" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
</div>


## Abstract

We present Panoptic Neural Fields (PNF), an object-aware neural scene representation that decomposes a scene into a set of objects (things) and background (stuff).  Each object is represented by an oriented 3D bounding box and a multi-layer perceptron (MLP) that takes position, direction, and time and outputs density and radiance.  The background stuff is represented by a similar MLP that additionally outputs semantic labels. Each object MLPs are instance-specific and thus can be smaller and faster than previous object-aware approaches, while still leveraging category-specific priors incorporated via meta-learned initialization. Our model builds a panoptic radiance field representation of any scene from just color images. We use off-the-shelf algorithms to predict camera poses, object tracks, and 2D image semantic segmentations. Then we jointly optimize the MLP weights and bounding box parameters using analysis-by-synthesis with self-supervision from color images and pseudo-supervision from predicted semantic segmentations. During experiments with real-world dynamic scenes, we find that our model can be used effectively for several tasks like novel view synthesis, 2D panoptic segmentation, 3D scene editing, and multiview depth prediction.

## Applications

Panoptic Neural Fields can be used for several applications shown below.

<div class="row">
  <video width="100%" playsinline="" autoplay="" loop="" preload="" muted="">
    <source src="../../assets/videos/pnf/pnf_applications.mp4" type="video/mp4">
  </video>
</div>

## Results

We evaluate or method on KITTI<d-cite key="Geiger2012CVPR"></d-cite> and KITTI-360<d-cite key="Kitti360"></d-cite> datasets. Results are shown below. For all results we use the same semantic <d-footnote>Semantic colormap: <img class="img-fluid" src="../../assets/img/pnf/semantic_colormap.jpg" alt="Semantic colormap"></d-footnote>.
and depth <d-footnote>Depth colormap: <img class="img-fluid" src="../../assets/img/pnf/depth_colormap.jpg" alt="Depth colormap"></d-footnote> colormaps.


### Results on (dynamic) KITTI scenes

<div class="row mt-3">
  <video class="video_with_border" width="100%" playsinline="" autoplay="" loop="" preload="" muted="">
    <source src="../../assets/videos/pnf/pnf_kitti_0009.mp4" type="video/mp4">
  </video>
</div>
<div class="row mt-3">
  <video class="video_with_border" width="100%" playsinline="" autoplay="" loop="" preload="" muted="">
    <source src="../../assets/videos/pnf/pnf_kitti_0011.mp4" type="video/mp4">
  </video>
</div>
<div class="row mt-3">
  <video class="video_with_border" width="100%" playsinline="" autoplay="" loop="" preload="" muted="">
    <source src="../../assets/videos/pnf/pnf_kitti_0018.mp4" type="video/mp4">
  </video>
</div>



### Novel view synthesis results on KITTI-360

<div class="row d-flex justify-content-center text-center">
  <div class="col">
    Rendered <b>semantic</b> segmentation
  </div>
  <div class="col">
    Rendered <b>depth</b> maps
  </div>
</div>
<div class="row mt-0">
  <video width="100%" playsinline="" autoplay="" loop="" preload="" muted="">
    <source src="../../assets/videos/pnf/kitti360_nvs50_train02_hstacked.mp4" type="video/mp4">
  </video>
</div>
<div class="row mt-2">
  <video width="100%" playsinline="" autoplay="" loop="" preload="" muted="">
    <source src="../../assets/videos/pnf/kitti360_nvs50_train03_hstacked.mp4" type="video/mp4">
  </video>
</div>

### Scene editing

Since our proposed panoptic neural field scene representation is object aware, it allows seamless manipulation and editing of different objects present in the scene by simply changing object pose or MLP parameters. We show some examples of scene editing below.

<div class="row d-flex justify-content-center text-center">
  <div class="col">
    Rendered <b>without</b> scene editing
  </div>
  <div class="col">
    Rendered <b>with</b> scene editing
  </div>
</div>
<div class="row mt-0">
  <video width="100%" playsinline="" autoplay="" loop="" preload="" muted="">
    <source src="../../assets/videos/pnf/scene_editing_kitti_2011_09_26_drive_0035.mp4" type="video/mp4">
  </video>
</div>
<div class="row mt-2">
  <video width="100%" playsinline="" autoplay="" loop="" preload="" muted="">
    <source src="../../assets/videos/pnf/dancing1_kitti_2011_09_26_drive_0018.mp4" type="video/mp4">
  </video>
</div>
<div class="row mt-2">
  <video width="100%" playsinline="" autoplay="" loop="" preload="" muted="">
    <source src="../../assets/videos/pnf/cloning03_kitti_2011_09_26_drive_0018.mp4" type="video/mp4">
  </video>
</div>
