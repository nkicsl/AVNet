# AVNet
AVNet: A retinal artery/vein classification network with category-attention weighted fusion

Please read our [paper]() for more details.

## Introduction

**Background and Objective**: Automatic artery/vein (A/V) classification in retinal image is of great importance in detecting vascular abnormalities, which may provide biomarkers for early diagnosis of many systemic diseases. It is intuitive to apply popular deep semantic segmentation network for A/V classification. However, the model is required to provide powerful representation ability since vessel is much more complex than general objects. Moreover, deep network may lead to inconsistent classification results for the same vessel due to the lack of structured optimization objective.

**Methods:** In this paper, we propose a novel segmentation network named AVNet, which effectively enhances the classification ability of the model by integrating category-attention weighted fusion (CWF) module, significantly improving the pixel-level A/V classification results.
Then, a graph based vascular structure reconstruction (VSR) algorithm is employed to reduce the segment-wise inconsistency, verifying the effect of the graph model on noisy vessel segmentation results.

**Results**: The proposed method has been verified on three datasets, DRIVE, LES-AV and WIDE. AVNet achieves pixel-level accuracies of 90.62%, 90.34%, and 93.16%, respectively, and VSR has further improved the performance by 0.19%, 1.85% and 0.64%. AVNet+VSR achieves the state-of-the-art results on these three datasets.

**Conclusion**: The proposed method achieves competitive performance in A/V classification task.

## Usage
+ A Caffe implementation of class balanced cross-entropy loss function can be found at https://github.com/alexgkendall/caffe-segnet
+ Fine-tuned from pretrained GoogLeNet.
