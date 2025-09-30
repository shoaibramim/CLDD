# Cotton Leaf Disease Detection (CLDD)

This repository contains the implementation and experiments conducted for the study **"Cotton Leaf Disease Detection and Classification Using Fine-tuned ResNet50 Architecture"**.  
Several state-of-the-art deep learning architectures (ResNet50, MobileNetV3, and Xception) were fine-tuned and evaluated under different experimental settings.  
Additionally, the best-performing model was compared against an existing study [Gurjot et al.](http://dx.doi.org/10.1002/fsn3.70658).

---

## Repository Structure

### 1. `CLDD_MobileNetV3.ipynb`
- Contains experiments using **MobileNetV3** under different hyperparameter settings.
- Includes experiments run for **30 epochs** and **60 epochs**.
- Evaluates performance variations with different training configurations.

### 2. `CLDD_ResNet50.ipynb`
- Implements experiments with **ResNet50** across multiple hyperparameter settings.
- Since ResNet50 achieved the **best results**, this notebook also includes:
  - Comparative analysis with the baseline model.
  - Visualization of evaluation metrics.

### 3. `CLDD_Xception.ipynb`
- Contains experiments conducted with **Xception** model.
- Evaluates performance under different parameter configurations.

### 4. `Comparison_With_Gurjot_et_al.ipynb`
- Implements the proposed **fine-tuned ResNet50 architecture** on the dataset used in [*Gurjot et al.*](http://dx.doi.org/10.1002/fsn3.70658)'s paper.
- Two experiments are included:
  1. **Direct usage of provided train/test folders** (original ratio not strictly 80:20).  
  2. **Re-splitting of train folder into 80:20 ratio** to maintain consistency with the dataset splitting approach used in this study.

---

## Dataset
- The experiments are conducted on the dataset introduced in the paper  
  [**"A Comprehensive Cotton Leaf Disease Dataset for Enhanced Detection and Classification"**](https://www.sciencedirect.com/science/article/pii/S235234092400876X).  
- The dataset was collected specifically for cotton leaf disease detection tasks.

---

## Models Evaluated
- **ResNet50** (best-performing, with fine-tuning, augmentation, and class imbalance handling)
- **MobileNetV3**
- **Xception**

---

## Results (Highlights)
- **ResNet50** achieved the best performance with Dual Augmentation strategy and class imbalance handling:
  - Accuracy: **97.89%**
  - Precision: **0.9762**
  - Recall: **0.9769**
  - F1-score: **0.9766**

---

## Acknowledgement
This work is part of my undergraduate thesis, conducted under the department of Computer Science and Engineering, University of Chittagong.


