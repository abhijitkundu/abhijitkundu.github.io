---
layout: distill_project
title: Semantic Video Segmentation
description: Feature Space Optimization for Semantic Video Segmentation
img: assets/img/fso/fso_teaser_low.webp
importance: 4
category: research
date: 2016-06-26

authors:
  - name: Abhijit Kundu
    url: "https://abhijitkundu.info"
    affiliations:
      name: Georgia Tech
  - name: Vibhav Vineet
    url: "http://vibhavvineet.info/"
    affiliations:
      name: Intel Labs
  - name: Vladlen Koltun
    url: "https://vladlen.info/"
    affiliations:
      name: Intel Labs

citation_key: KunduCVPR2016VideoFSO
---

<p>
    <a href="../../assets/pdf/VideoFSO_CVPR16.pdf" class="btn btn-primary z-depth-1">Paper <i class="fas fa-file-pdf"></i></a>
    <a href="../../assets/pdf/VideoFSO_CVPR16_slides.pdf" class="btn btn-primary z-depth-1">Slides <i class="fas fa-file-powerpoint"></i></a>
    <a href="../../assets/pdf/VideoFSO_CVPR16_poster.pdf" class="btn btn-primary z-depth-1">Poster <i class="fas fa-file-pdf"></i></a>
    <a href="https://bitbucket.org/infinitei/videoparsing" class="btn btn-primary z-depth-1">Code <i class="fab fa-bitbucket"></i></a>
    <a href="https://www.youtube.com/watch?v=KPaY5DitFxw" class="btn btn-primary z-depth-1">Talk <i class="fab fa-youtube"></i></a>
</p>


## Abstract

We present an approach to long-range spatio-temporal regularization in semantic video segmentation. Temporal regularization in video is challenging because both the camera and the scene may be in motion. Thus Euclidean distance in the space-time volume is not a good proxy for correspondence. We optimize the mapping of pixels to a Euclidean feature space so as to minimize distances between corresponding points. Structured prediction is performed by a dense CRF that operates on the optimized features. Experimental results demonstrate that the presented approach increases the accuracy and temporal consistency of semantic video segmentation.


## Videos

### Results on Cityscapes dataset
<div class="embed-responsive embed-responsive-16by9">
    <iframe class="embed-responsive-item" src="https://www.youtube.com/embed/Nok6Xludc_Q"></iframe>
</div>

### Comparison on Camvid dataset
<div class="embed-responsive embed-responsive-16by9">
    <iframe class="embed-responsive-item" src="https://www.youtube.com/embed/k9EgyFpiH8g"></iframe>
</div>

