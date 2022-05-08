---
layout: distill_project
title: 3D-RCNN
description: Instance-level 3D Object Reconstruction via Render-and-Compare
img: assets/img/3drcnn/3drcnn_teaser.jpg
importance: 2
category: research
date: 2018-06-18

authors:
  - name: Abhijit Kundu
    url: "https://abhijitkundu.info"
    affiliations:
      name: Georgia Tech
  - name: Yin Li
    url: "https://www.biostat.wisc.edu/~yli/"
    affiliations:
      name: Georgia Tech
  - name: James M. Rehg
    url: "https://rehg.org"
    affiliations:
      name: Georgia Tech

citation_key: 3DRCNN_CVPR2018

bibliography: 3D-RCNN.bib
---

<p>
    <a href="../../assets/pdf/3DRCNN_CVPR18.pdf" class="btn btn-primary z-depth-1">Paper <i class="fas fa-file-pdf"></i></a>
    <a href="../../assets/pdf/3DRCNN_CVPR18_slides.pdf" class="btn btn-primary z-depth-1">Slides <i class="fas fa-file-powerpoint"></i></a>
    <a href="../../assets/pdf/3DRCNN_CVPR18_poster.pdf" class="btn btn-primary z-depth-1">Poster <i class="fas fa-file-pdf"></i></a>
    <a href="https://colab.research.google.com/drive/13sMw-nUw1tmZzuLvMduRr71bcJRy72Ly" class="btn btn-primary z-depth-1">Code <i class="fab fa-github"></i></a>
    <a href="https://youtu.be/Jl1NeziAHFY?t=6m57s" class="btn btn-primary z-depth-1">Talk <i class="fab fa-youtube"></i></a>
</p>


## Abstract

We present a fast inverse-graphics framework for instance-level 3D scene understanding. We train a deep convolutional network that learns to map image regions to the full 3D shape and pose of all object instances in the image. Our method produces a compact 3D representation of the scene, which can be readily used for applications like autonomous driving. Many traditional 2D vision outputs, like instance segmentations and depth-maps, can be obtained by simply rendering our output 3D scene model. We exploit class-specific shape priors by learning a low dimensional shape-space from collections of CAD models. We present novel representations of shape and pose, that strive towards better 3D equivariance and generalization. In order to exploit rich supervisory signals in the form of 2D annotations like segmentation, we propose a differentiable Render-and-Compare loss that allows 3D shape and pose to be learned with 2D supervision. We evaluate our method on the challenging real-world datasets of Pascal3D+ and KITTI, where we achieve state-of-the-art results.

## Method

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/3drcnn/pipeline.jpeg" title="pipeline image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Overview of the method.
</div>

## Results

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/3drcnn/kitti_qualiatative.jpeg" title="kitti qualiatative" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Reconstruction results on KITTI<d-cite key="Geiger2012CVPR"></d-cite> dataset.
</div>

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/3drcnn/surreal_qualitative.jpeg" title="surreal qualitative" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Reconstruction results on SURREAL<d-cite key="varol2017surreal"></d-cite>  dataset.
</div>


## Downloads

<p>
    <a href="https://drive.google.com/uc?id=1Im74Wbj807iOLlWQpkTHIlislvCHsSVZ">
        <i class="fab fa-google-drive"></i> Learned TSDF-PCA shape models.
    </a>
</p>


<p>
    <a href="https://colab.research.google.com/drive/13sMw-nUw1tmZzuLvMduRr71bcJRy72Ly">
        <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/> Colab demo of learned shape models.
    </a>
</p>
