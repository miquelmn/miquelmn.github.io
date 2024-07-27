---
title: "Assessing fidelity in XAI post-hoc techniques: A comparative study with ground truth explanations datasets"
excerpt: "An objective fidelity comparison of 16 XAI methods."
header:
  image: /assets/img/04_txuxi/0.png
  teaser: /assets/img/04_txuxi/0.png
sidebar:
  - title: "Responsibilities"
    image: /assets/img/04_txuxi/0.png
    image_alt: "logo"
    text: "Software, Visualization, Formal analysis , Writing - Original Draft"
---

The evaluation of the fidelity of eXplainable Artificial Intelligence (XAI) methods to their underlying models is a challenging task, primarily due to the absence of a ground truth for explanations. However, assessing fidelity is a necessary step for ensuring a correct XAI methodology. In this study, we conduct a fair and objective comparison of the current state-of-the-art XAI methods by introducing three novel image datasets with reliable ground truth for explanations. The primary objective of this comparison is to identify methods with low fidelity and eliminate them from further research, thereby promoting the development of more trustworthy and effective XAI techniques. Our results demonstrate that XAI methods based on the direct gradient calculation and the backpropagation of output information to input yield higher accuracy and reliability compared to methods relying on perturbation based or Class Activation Maps (CAM). However, these methods tend to generate more noisy saliency maps. These findings have significant implications for the advancement of XAI methods, enabling the elimination of erroneous explanations and fostering the development of more robust and reliable XAI.

[Link to the article](https://www.sciencedirect.com/science/article/pii/S0004370224001152)