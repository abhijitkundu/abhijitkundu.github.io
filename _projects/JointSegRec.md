---
layout: distill_project
title: Semantic 3D Reconstruction
description: Joint Semantic Segmentation and 3D Reconstruction from Monocular Video
img: assets/img/JointSegRec/JointSegRec_teaser.png
importance: 6
category: research
date: 2014-09-06

authors:
  - name: Abhijit Kundu
    url: "https://abhijitkundu.info"
    affiliations:
      name: Georgia Tech
  - name: Yin Li
    url: "https://www.biostat.wisc.edu/~yli/"
    affiliations:
      name: Georgia Tech
  - name: Frank Dellaert
    url: "https://dellaert.github.io/"
    affiliations:
      name: Georgia Tech
  - name: Fuxin Li
    url: "https://web.engr.oregonstate.edu/~lif/"
    affiliations:
      name: Georgia Tech
  - name: James M. Rehg
    url: "https://rehg.org"
    affiliations:
      name: Georgia Tech

citation_key: KunduECCV2014JointSegRec
---

<p>
    <a href="../../assets/pdf/HybridSFM-ECCV2014.pdf" class="btn btn-primary z-depth-1">Paper <i class="fas fa-file-pdf"></i></a>
    <a href="../../assets/pdf/HybridSFM-ECCV2014-supp.pdf" class="btn btn-primary z-depth-1">Supp <i class="fas fa-file-pdf"></i></a>
    <a href="https://www.youtube.com/watch?v=0zHMMQPswgY" class="btn btn-primary z-depth-1">Video <i class="fab fa-youtube"></i></a>
</p>


## Abstract

We present an approach for joint inference of 3D scene structure and semantic labeling for monocular video. Starting with monocular image stream, our framework produces a 3D volumetric semantic + occupancy map, which is much more useful than a series of 2D semantic label images or a sparse point cloud produced by traditional semantic segmentation and Structure from Motion(SfM) pipelines respectively. We derive a Conditional Random Field (CRF) model defined in the 3D space, that jointly infers the semantic category and occupancy for each voxel. Such a joint inference in the 3D CRF paves the way for more informed priors and constraints, which is otherwise not possible if solved separately in their traditional frameworks. We make use of class specific semantic cues that constrain the 3D structure in areas, where multiview constraints are weak. Our model comprises of higher order factors, which helps when the depth is unobservable.We also make use of class specific semantic cues to reduce either the degree of such higher order factors, or to approximately model them with unaries if possible. We demonstrate improved 3D structure and temporally consistent semantic segmentation for difficult, large scale, forward moving monocular image sequences.


## Videos

<div class="embed-responsive embed-responsive-16by9">
    <iframe width="560" height="330" src="https://www.youtube.com/embed/0zHMMQPswgY" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
</div>
