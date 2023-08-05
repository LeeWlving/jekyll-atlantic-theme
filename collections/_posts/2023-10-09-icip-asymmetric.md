---
layout: post
title: "Asymmetric Scalable Cross-modal Hashing"
date: 2023-07-08T10:26:40+10:00
authors: ["Wenyun Li"]
categories: ["RemoteSensing", "Hash", "InformationRetrieval"]
tags: ["InformationRetrieval"]
description: icip 2023 paper.
thumbnail: "https://pic.imgdb.cn/item/64ce32f71ddac507ccac955c.png"
image: "https://pic.imgdb.cn/item/64ce33661ddac507ccae2f0a.png"
---

Cross-modal hashing is a practical approach to solving the problem of large-scale multimedia retrieval. However, there are still specific issues that the current methods cannot solve, such as how to construct binary codes rather than relax them to continuity effectively and how to prevent  $n \times n$ problem.  This paper proposes a novel Asymmetric Scalable Cross-Modal Hashing (ASCMH) to address these issues. It learns a common latent space from the kernelized features of different modalities. It then transforms the similarity matrix optimization to a distance-distance difference minimization problem with the help of semantic labels and common latent space. Additionally, we use an orthogonal constraint of label information to construct hash codes necessary for search accuracy. Extensive experiments on three benchmark datasets show that our ASCMH outperforms the SOTA cross-modal hashing methods.

## Framework

Overall framework of our methods are shown:

[![p95mrTO.jpg](https://pic.imgdb.cn/item/64ce33c21ddac507ccaf7faf.jpg)](https://pic.imgdb.cn/item/64ce33c21ddac507ccaf7faf.jpg)

> The proposed Locality Preserving Multiview Graph Hashing (LPMGH) framework.

In this paper, we have presented ASCMH, a novel approach for large-scale multimedia retrieval.
ASCMH addresses the challenges of constructing binary codes effectively by learning a common latent space from the kernelized features of different modalities. This approach ensures that the binary codes capture the underlying relationships between multimedia data accurately. By transforming the similarity matrix optimization into a distance-distance difference minimization problem, ASCMH effectively prevents the n × n problem and reduces the computational complexity associated with large-scale datasets. 
One key aspect of ASCMH is the utilization of semantic labels. These labels provide valuable information about the semantic affinity between different data instances. By incorporating an orthogonal constraint of label information, ASCMH constructs hash codes that not only preserve the semantic information but also enhance search accuracy. This combination of semantic labels and common latent space enables ASCMH to generate more discriminative binary codes, leading to improved retrieval performance. 
The experimental evaluation of ASCMH on three benchmark datasets showcases its superiority over state-of-the-art cross-modal hashing methods. The results demonstrate that ASCMH consistently outperforms the baselines in terms of mean average precision (mAP) and top-N precision. The mAP values for different code lengths indicate that ASCMH achieves accurate and efficient retrieval across various scenarios. These findings validate the effectiveness of ASCMH in capturing the semantic relationships between multimedia data and generating discriminative binary codes. 
In conclusion, ASCMH presents a novel approach to address the challenges in large-scale multimedia retrieval. By learning a common latent space and leveraging semantic labels, ASCMH effectively constructs binary codes and optimizes similarity matrices to enhance search accuracy. The experimental results demonstrate the superiority of ASCMH over existing methods, highlighting its potential for practical applications in the field of multimedia retrieval. Further research and exploration of ASCMH can lead to advancements in cross-modal hashing techniques and contribute to the development of more efficient and accurate retrieval systems.


The paper is available at [link](https://figshare.com/s/daab78f7eeb893b25465).

<!-- The Video of our oral presentation is:
<iframe
    width="640"
    height="480"
    src="https://www.youtube.com/watch?v=IP_A_Tor4v8"
    frameborder="0"
    allow="autoplay; encrypted-media"
    allowfullscreen
>
</iframe> -->
