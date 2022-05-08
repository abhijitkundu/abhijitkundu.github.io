---
layout: distill_project
title: Multibody Visual SLAM
description: Realtime Multibody Visual SLAM with a Smoothly Moving Monocular Camera
img: assets/img/mvslam/multibodyVSLAM_thumbnail.jpg
importance: 6
category: research
date: 2011-11-06

authors:
  - name: Abhijit Kundu
    url: "https://abhijitkundu.info"
    affiliations:
      name: IIIT Hyderabad
  - name: K. Madhava Krishna
    url: "https://robotics.iiit.ac.in/PrincipalInvestigators.html"
    affiliations:
      name: IIIT Hyderabad
  - name: C. V. Jawahar
    url: "https://faculty.iiit.ac.in/~jawahar/"
    affiliations:
      name: IIIT Hyderabad

citation_key: KunduICCV2011
---

<p>
    <a href="../../assets/pdf/abhijit_etal_iccv2011.pdf" class="btn btn-primary z-depth-1">Paper <i class="fas fa-file-pdf"></i></a>
    <a href="../../assets/pdf/abhijit_etal_iccv2011_supp.pdf" class="btn btn-primary z-depth-1">Supp <i class="fas fa-file-pdf"></i></a>
</p>


## Abstract

This paper presents a realtime, incremental multibody visual SLAM system that allows choosing between full 3D reconstruction or simply tracking of the moving objects. Motion reconstruction of dynamic points or objects from a monocular camera is considered very hard due to well known problems of observability. We attempt to solve the problem with a Bearing only Tracking (BOT) and by integrating multiple cues to avoid observability issues. The BOT is accomplished through a particle filter, and by integrating multiple cues from the reconstruction pipeline. With the help of these cues, many real world scenarios which are considered unobservable with a monocular camera is solved to reasonable accuracy. This enables building of a unified dynamic 3D map of scenes involving multiple moving objects. Tracking and reconstruction is preceded by motion segmentation and detection which makes use of efficient geometric constraints to avoid difficult degenerate motions, where objects move in the epipolar plane. Results reported on multiple challenging real world image sequences verify the efficacy of the proposed framework.


## Videos

<div class="embed-responsive embed-responsive-16by9">
    <iframe width="560" height="315" src="https://www.youtube.com/embed/LKjTtKmkyXo" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
</div>