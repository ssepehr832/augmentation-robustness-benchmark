# Impact of Data Augmentation on Model Robustness and Confidence in Image Classification

## Abstract
Modern vision models often perform well on clean test images but can degrade sharply under real-world image conditions such as blur, noise, and illumination changes. In this project, we will investigate whether stronger data augmentation strategies during training improve robustness to such corruptions, and whether robustness gains come at the cost of clean accuracy or prediction confidence.

We will train an image classification model on the Tiny ImageNet-64 dataset using multiple augmentation pipelines:
1. A standard baseline (random crop/flip)
2. Stronger augmentation approaches such as RandAugment / AutoAugment-style policies and AugMix

After training, we will evaluate each model on clean Tiny ImageNet-64 as well as systematically corrupted versions of the test images (e.g. Gaussian blur, additive noise, brightness/contrast shifts) generated with a controlled corruption suite (e.g. via Albumentations).

We will report:
- Clean accuracy  
- Corruption robustness across corruption types and severity levels  
- Changes in confidence or calibration (e.g. reliability curves or calibration error)

The outcome will quantify which augmentation strategies best improve robustness and characterize the trade-offs between clean performance and robustness in practical vision settings.

## Team
- Clayton McCormack  
- Faizullah Yousufi  
- Sepehr Seghatoleslami  
- Jose Renzo Delos Santos  