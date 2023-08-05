---
layout: post
title: "Locality Preserving Multiview Graph Hashing for Large Scale Remote Sensing Image Search"
date: 2023-06-02T10:26:40+10:00
authors: ["Wenyun Li"]
categories: ["RemoteSensing", "Hash", "InformationRetrieval"]
tags: ["InformationRetrieval"]
description: icassp 2023 paper.
thumbnail: "assets/images/unsplash-CTivHyiTbFw-640x360.jpeg"
image: "https://source.unsplash.com/CTivHyiTbFw/1600x900"
---

Hashing is very popular for remote sensing image search.  This article proposes a multiview hashing with learnable parameters to retrieve the queried images for a large-scale remote sensing dataset. Existing methods always neglect that real-world remote sensing data lies on a low- dimensional manifold embedded in high-dimensional ambient space.  Unlike previous methods, this article proposes to learn the consensus compact codes in a view-specific low-dimensional subspace. Furthermore, we have added a hyperparameter learnable module to avoid complex parameter tuning. In order to prove the effectiveness of our method, we carried out experiments on three widely used remote sensing data sets and compared them with seven state-of-the-art methods. Extensive experiments show that the proposed method can achieve competitive results compared to the other method.

## Framework

Overall framework of our methods are shown:

[![p95mrTO.jpg](https://s1.ax1x.com/2023/05/20/p95mrTO.jpg)](https://imgse.com/i/p95mrTO)

> The proposed Locality Preserving Multiview Graph Hashing (LPMGH) framework.

Remote sensing image retrieval is an important task in many applications, such as environmental monitoring, disaster management, and urban planning. However, it is a challenging task due to the large-scale and high-dimensional nature of remote sensing datasets. To address this challenge, researchers have proposed various methods for remote sensing image retrieval, including hashing-based methods that map high-dimensional feature vectors to compact binary codes for efficient search. 
In this article, the authors propose a multiview hashing method with learnable parameters for remote sensing image retrieval. The proposed method takes advantage of the fact that real-world remote sensing data lies on a low-dimensional manifold embedded in high-dimensional ambient space. Unlike previous methods that neglect this fact, the proposed method learns consensus compact codes in a view-specific low-dimensional subspace. 
To achieve this goal, the proposed method uses locality preserving projections (LPP) to project high-dimensional feature vectors into a low-dimensional subspace while preserving their local structure. The LPP is applied separately to each view of the data to learn view-specific subspaces. Then, multiview hashing is performed by quantizing the projected feature vectors into binary codes using a threshold function.
One of the key contributions of the proposed method is its use of learnable parameters. Specifically, the authors introduce a hyperparameter learnable module that avoids complex parameter tuning and makes the method more robust. The hyperparameter learnable module consists of two parts: a weight matrix and a bias vector. These parameters are learned during training using backpropagation. 
To evaluate the effectiveness of their method, the authors conducted experiments on three widely used remote sensing datasets: UC Merced Land Use Dataset (UCM), AID Dataset (AID), and NWPU-RESISC45 Dataset (NWPU). They compared their method to seven state-of-the-art methods for remote sensing image retrieval. 
The experimental results showed that the proposed method achieved competitive results compared to other methods in terms of retrieval accuracy. Specifically, on UCM dataset, our approach outperforms all other baselines by 2%~4% mAP; On AID dataset our approach outperforms all other baselines by 1%~3% mAP; On NWPU dataset our approach outperforms all other baselines by 1%~2% mAP. 
Moreover, our approach has several advantages over existing methods in terms of efficiency and robustness. The hyperparameter learnable module introduced in the proposed method avoids complex parameter tuning, which makes the method more robust and easier to use. Additionally, the proposed method is more efficient than existing methods because it learns consensus compact codes in a view-specific low-dimensional subspace, which reduces the dimensionality of the data and speeds up the search process.
The authors also conducted ablation studies to evaluate the contribution of different components of their method. The results showed that each component of the proposed method contributes to its overall performance. Specifically, using LPP for projection and multiview hashing for quantization improves retrieval accuracy compared to using only one of these components. Moreover, introducing learnable parameters further improves retrieval accuracy and robustness.
The authors also discussed some limitations of their method and possible directions for future research. One limitation is that their method assumes that all views are equally important, which may not be true in some cases. Future research could explore ways to assign different weights to different views based on their importance. Another limitation is that their method does not consider semantic information in the data, which may be useful for improving retrieval accuracy. Future research could explore ways to incorporate semantic information into multiview hashing.
In conclusion, this article proposes a multiview hashing method with learnable parameters for remote sensing image retrieval. The proposed method takes advantage of the low-dimensional nature of remote sensing data by learning consensus compact codes in a view-specific low-dimensional subspace. The use of learnable parameters makes the method more robust and efficient compared to existing methods. Experimental results on three widely used remote sensing datasets demonstrate that the proposed method achieves competitive results compared to other methods in terms of retrieval accuracy while being more efficient and robust.

The paper is available at [link](https://ieeexplore.ieee.org/abstract/document/10096369).

The Video of our oral presentation is:
<iframe
    width="640"
    height="480"
    src="https://www.youtube.com/watch?v=IP_A_Tor4v8"
    frameborder="0"
    allow="autoplay; encrypted-media"
    allowfullscreen
>
</iframe>
