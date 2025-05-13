---
title: "A comprehensive study on fidelity metrics for XAI"
excerpt: "A novel meta-evaluation process to verify fidelity measures."
header:
  image: /assets/img/05_fidelity/1.jpg
  teaser: /assets/img/05_fidelity/1.jpg
sidebar:
  - title: "Responsibilities"
    image: /assets/img/05_fidelity/1.jpg
    image_alt: "logo"
    text: "Software, Visualization, Formal analysis , Writing - Original Draft"
---

The use of eXplainable Artificial Intelligence (XAI) systems has introduced a set of challenges that need resolution. Herein, we focus on how to correctly select an XAI method, an open questions within the field. The inherent difficulty of this task is due to the lack of a ground truth. Several authors have proposed metrics to approximate the fidelity of different XAI methods. These metrics lack verification and have concerning disagreements. In this study, we proposed a novel methodology to verify fidelity metrics, using transparent models. These models allowed us to obtain explanations with perfect fidelity. Our proposal constitutes the first objective benchmark for these metrics, facilitating a comparison of existing proposals, and surpassing existing methods. We applied our benchmark to assess the existing fidelity metrics in two different experiments, each using public datasets comprising 52,000 images. The images from these datasets had a size a 128 by 128 pixels and were synthetic data that simplified the training process. We identified that two fidelity metrics, Faithfulness Estimate and Faithfulness Correlation, obtained the expected perfect results for linear models, showing their ability to approximate fidelity for this kind of methods. However, when present with non-linear models, as the ones most used in the state-of-the-art,all metric values, indicated a lack of fidelity, with the best one showing a 30% deviation from the expected values for perfect explanation. Our experimentation led us to conclude that the current fidelity metrics are not reliable enough to be used in real scenarios. From this finding, we deemed it necessary to development new metrics, to avoid the detected problems, and we recommend the usage of our proposal as a benchmark within the scientific community to address these limitations.
[Link to the article](https://www.sciencedirect.com/science/article/pii/S0306457324002590)