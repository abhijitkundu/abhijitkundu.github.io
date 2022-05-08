---
layout: distill_project
title: Panoptic Neural Fields
description: A Semantic Object-Aware Neural Scene Representation
img: assets/img/pnf/kitti360_nvs50_train02.webp
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
---

## Abstract

We present Panoptic Neural Fields (PNF), an object-aware neural scene representation that decomposes a scene into a set of objects (things) and background (stuff).  Each object is represented by an oriented 3D bounding box and a multi-layer perceptron (MLP) that takes position, direction, and time and outputs density and radiance.  The background stuff is represented by a similar MLP that additionally outputs semantic labels. Each object MLPs are instance-specific and thus can be smaller and faster than previous object-aware approaches, while still leveraging category-specific priors incorporated via meta-learned initialization. Our model builds a panoptic radiance field representation of any scene from just color images. We use off-the-shelf algorithms to predict camera poses, object tracks, and 2D image semantic segmentations. Then we jointly optimize the MLP weights and bounding box parameters using analysis-by-synthesis with self-supervision from color images and pseudo-supervision from predicted semantic segmentations. During experiments with real-world dynamic scenes, we find that our model can be used effectively for several tasks like novel view synthesis, 2D panoptic segmentation, 3D scene editing, and multiview depth prediction.