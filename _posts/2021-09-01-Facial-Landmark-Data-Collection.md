---
layout: page
title: "Facial Landmark Data Collection"
subtitle: "An Optimization to Train Facial Emotion Detection Learning Models"
date:   2021-09-01 21:21:21 +0530
categories: ["Image and Video Processing"]
---

Created with Roshan Prabhakar, Leevi Symister, and Kaiser Williams under the supervision of Professor Tsachy Wiessman and Doctor Shubham Chandak.

# Abstract
In-person theater performances have become difficult due to COVID-19, hence video conferencing softwares like Zoom have become increasingly popular to deliver live virtual performances. Such performances require a deliverance of audience feedback information to performers so that they can adapt their performance. However, typical audience feedback is not viable in a virtual setting. Intuition suggests that extracting feedback from an audience preoccupied with a performance by requiring a redirection of their attention to the feedback will result in inadequate representations of an audience’s emotional state. More authentic feedback can be gained by analyzing real time emotions of the audience through the use of a live webcam by extracting facial expressions.

Existing facial emotional recognition softwares map a face mesh to a subject and derive emotional states through the use of CNNs and a Facial Action Coding System (the current standard for determining emotions from a facial state). These models are trained on a variety of images from publicly available datasets as well as images scraped from the web. This project aims to develop software that performs more tangible data collection as it relates to the audience-performer feedback loop: specifically the collection of emotional expressions and corresponding reactionary expressions (clapping, booing, etc.). This project aims to determine whether there exists a relationship between face mesh data collected across frames and reactionary motions during said frames which may not be easily observable through the webcam, by building a database of such data entries which may be used to train a machine learning model. Should a relationship be found, such a model could be deployed within virtual performance frameworks to enable live collection of audience feedback information. Our code is available [here](https://github.com/roshanprabhakar/af-datacollection).

# Paper
[Publication](https://theinformaticists.com/2021/08/21/facial-landmark-data-collection-to-train-facial-emotion-detection-learning-models/) and [Presentation](https://youtu.be/vy755xJtyiw)