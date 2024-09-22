# [TPAMI'24] Mine yOur owN Anatomy: Revisiting Medical Image Segmentation with Extremely Limited Labels

[![arXiv](https://img.shields.io/badge/arXiv-2209.13476-b31b1b.svg)](https://arxiv.org/abs/2209.13476)

This is the PyTorch implemention of our TPAMI 2024 paper "**Mine yOur owN Anatomy: Revisiting Medical Image Segmentation with Extremely Limited Labels**" by [Chenyu You](http://chenyuyou.me/), [Weicheng Dai](https://weichengdai1.github.io/), [Fenglin Liu](https://eng.ox.ac.uk/people/fenglin-liu/), [Yifei Min](https://scholar.google.com/citations?user=pFWnzL0AAAAJ&hl=en/), [Nicha C. Dvornek](https://scholar.google.com/citations?user=HrzdtUUAAAAJ&hl=en/), [Xiaoxiao Li](https://scholar.google.com/citations?user=sdENOQ4AAAAJ&hl=en/), [David A. Clifton](https://eng.ox.ac.uk/people/david-clifton/), [Lawrence Staib](https://medicine.yale.edu/profile/lawrence-staib/), and [James S. Duncan](https://medicine.yale.edu/profile/james-duncan/). 

## Abstract
> Recent studies on contrastive learning have achieved remarkable performance solely by leveraging few labels in the context of medical image segmentation. Existing methods mainly focus on instance discrimination and invariant mapping. However, they face three common pitfalls: (1) tailness: medical image data usually follows an implicit long-tail class distribution. Blindly leveraging all pixels in training hence can lead to the data imbalance issues, and cause deteriorated performance; (2) consistency: it remains unclear whether a segmentation model has learned meaningful and yet consistent anatomical features due to the intra-class variations between different anatomical features; and (3) diversity: the intra-slice correlations within the entire dataset have received significantly less attention. This motivates us to seek a principled approach for strategically making use of the dataset itself to discover similar yet distinct samples from different anatomical views. In this paper, we introduce a novel semi-supervised 2D medical image segmentation framework termed Mine yOur owN Anatomy (MONA), and make three contributions. First, prior work argues that every pixel equally matters to the model training; we observe empirically that this alone is unlikely to define meaningful anatomical features, mainly due to lacking the supervision signal. We show two simple solutions towards learning invariances - through the use of stronger data augmentations and nearest neighbors. Second, we construct a set of objectives that encourage the model to be capable of decomposing medical images into a collection of anatomical features in an unsupervised manner. Lastly, we both empirically and theoretically, demonstrate the efficacy of our MONA on three benchmark datasets with different labeled settings, achieving new state-of-the-art under different labeled semi-supervised settings.


## Citation

If you find this project useful, please consider citing:

```bibtex
@article{you2024mine,
  title={Mine your own anatomy: Revisiting medical image segmentation with extremely limited labels},
  author={You, Chenyu and Dai, Weicheng and Liu, Fenglin and Min, Yifei and Dvornek, Nicha C and Li, Xiaoxiao and Clifton, David A and Staib, Lawrence and Duncan, James S},
  journal={IEEE Transactions on Pattern Analysis and Machine Intelligence},
  year={2024},
  publisher={IEEE}
}
```
