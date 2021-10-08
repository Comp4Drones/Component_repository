---
title: UDANET - AI drone system modules
componentId: WP3-36_2
---

# WP3-36_2 - AI drone system modules

|||
|-|-|
|ID|WP3-36_2|
|Contributor|UDANET|
|Levels|Functional|
|Require|Dataset|
|Provide|Designed and implemented algorithm|
|Input|Plant images|
|Output|Disease classification|
|C4D building block|Data analytics|
|TRL|4-5|

## Detailed Description

An artificial intelligent method to classify leaf diseases will be designed and implemented. The methods inputs are images from cameras, and the output is the plant health status classification. Artificial intelligence algorithms with different characteristics will be designed and implemented with the aim of taking into account the computational cost of each, as well as the over-fitting problem and the dataset that is not always adequate, and the diagnostic performance is drastically decreased when used on test datasets from new environments (i.e. generalization problem).

A large amount of data increases the performance of machine learning algorithms and avoids over-fitting problems. Creating a large amount of data in the agricultural sector for the design of models for the diagnosis and detection of plant diseases is an open and challenging task that takes a lot of time and resources. One way to increase the dataset will be to use data augmentation techniques. It increases the diversity of training data for machine learning algorithms without collecting new data.

## Contribution and Improvements

The improving objective of this component is to develop and test the algorithms, increase the reference dataset using basic image manipulation and deep learning based image augmentation techniques such as image flipping, cropping, rotation, colour transformation, PCA colour augmentation, noise injection, Generative Adversarial Networks (GANs) and Neural Style Transfer (NST) techniques. Performance of the data augmentation techniques was studied using state of the art transfer learning techniques both in terms of accuracy and computational cost.

## Design and Implementation

It is developed through the Tensorflow and Python framework.
