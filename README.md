# A Survey on Facial Expression Recognition of Static and Dynamic Emotions

This is the official repository for our [paper](https://arxiv.org/pdf/2408.15777) entitled *“A Survey on Facial Expression Recognition of Static and Dynamic Emotions”*.

## Taxonomy Overview

![images/taxonomy_overview.png](images/taxonomy_overview.png)

Taxonomy of FER of static and dynamic emotions. We present a hierarchical taxonomy that categorizes existing FER models by input type, task challenges, and network structures within a systematic framework, aiming to provide a comprehensive overview of the current FER research landscape. First, we have introduced datasets, metrics, and workflow (including literature and codes) into a public GitHub repository. Then, image-based SFER and video- based DFER overcome different task challenges using various learning strategies and model designs. Following, we analyzed recent advances of FER on benchmark datasets. Finally, we discussed and concluded some important issues and potential trends in FER, highlighting directions for future developments.

## Comparisons with SOTA FER-related reviews

![images/comparisons.png](images/comparisons.png)

## Datasets

![images/Datasets.jpg](images/Datasets.jpg)

Image-based static facial frames (Above) and video-based dynamic facial sequences (Below) of seven basic emotions in the lab and wild. Samples are from (a) JAFFE, (b) CK+, (c) SFEW, (d) ExpW, (e) RAF-DB, (f) AffectNet, (g) EmotioNet, (h) CK+, (i) Oulu-CASIA, (j) DFEW, (k) FERV39k, and (l) MAFW.

## Workflow of Generic Facial Expression Recognition

![images/Workflow.jpg](images/Workflow.jpg)

The workflow and main components of generic facial expression recognition.

## Image-based Static FER

Image-based static facial expression recognition (SFER) involves extracting features from a single image, which captures complex spatial information that related to facial expressions, such as landmarks, and their geometric structures and relationships. In the following, we will first introduce the general architecture of SFER, and then elaborate specific design of SFER methods from the challenge-solving perspectives, including disturbance-invariant SFER, 3D SFER, uncertainty-aware SFER, compound SFER, cross-domain SFER, limited-supervised SFER, and cross-modal SFER.

### General SFER

![images/gernearl_based_SFER_00.jpg](images/gernearl_based_SFER_00.jpg)

The architecture of general SFER. Figure is reproduced based on (a) CNN-based model, (b) GCN-based model, and (c) Transformer-based model.

### Disturbance-invariant SFER

![images/Disturbance_invariant_SFER_00.jpg](images/Disturbance_invariant_SFER_00.jpg)

The architecture of disturbance-invariant SFER. Figure is reproduced based on (a) Attention-based model (AMP-Net) and (b) Decomposition-based model.

### 3D SFER

![images/3D_SFER_00.jpg](images/3D_SFER_00.jpg)

The architecture of 3D SFER. Figure is reproduced based on (a) GAN-based learning (GAN-Int) and (b) Multi-view learning (MV-CNN).

### Uncertainty-aware SFER

![images/Uncertainy_aware_SFER_00.jpg](images/Uncertainy_aware_SFER_00.jpg)

The architecture of uncertainty-aware SFER. Figure is reproduced based on (a) the label uncertainty learning (LA-Net) and (b) data uncertainty learning (LNSU-Net).

### Compound SFER

Compound emotions refer to complex emotional states formed by the combination of at least two basic emotions, which are not independent, discrete categories but exist within a continuous emotional spectrum composed of multiple dimensions. Compared with discrete "basic" emotions or a few dimensions, compound emotions provide a more accurate representation of the diversity and continuity of human complex emotions.

### Cross-domain SFER

![images/crossdomain_sfer.png](images/crossdomain_sfer.png)

The architecture of cross-domain SFER. Figure is reproduced based on (a) the transfer learning-based model (CSRL) and (b) the adaption learning-based model (AGRA).

### Weak-supervised SFER

![images/Weak-supervised.jpg](images/Weak-supervised.jpg)

The architecture of weak-supervised SFER. Figure is reproduced based on the Ada-CM.

### Cross-modal SFER

![images/Cross-modal.png](images/Cross-modal.png)

The architecture of cross-modal SFER. Figure is reproduced based on the CEprompt.

## Video-based Dynamic Facial Expression Recognition

The video-based DFER involves analyzing facial expressions that change over time, necessitating a framework that effectively integrates spatial and temporal information. The core objective of DFER is to extract and learn the features of expression changes from video sequences or image sequences. Due to the complexity and diversity of input video or image sequences, DFER faces various task challenges. Based on different solution approaches, these challenges can be categorized into seven basic types: general DFER, sampling-based DFER, expression intensity-aware DFER, multi-modal DFER, static to dynamic FER, self-supervised DFER, and cross-modal DFER.

### General DFER

![images/generaldfer.png](images/generaldfer.png)

The architecture of general DFER. Figure is reproduced based on (a) CNN-RNN based model (SAANet) and (b) the transformer-based model (EST).

### Sampling-based DFER

![images/fig9-Sampling-based_dfer_00.jpg](images/fig9-Sampling-based_dfer_00.jpg)

The architecture of sampling-based DFER. Figure is reproduced based on explainable sampling (Freq-HD).

### Expression Intensity-aware DFER

Facial expressions are inherently dynamic, with intensity either gradually shifting from neutral to peak and back or abruptly transitioning from peak to neutral, making the accurate capture of these fluctuations essential for understanding expression dynamics.

### Static to Dynamic FER

The static to dynamic FER utilized the high-performance SFER knowledge to explore appearance features and dynamic dependencies.

### Multi-modal DFER

![images/multi_modal_fusion_dfer.png](images/multi_modal_fusion_dfer.png)

The architecture of multi-modal DFER. Figure is reproduced based on the fusion-based model (T-MEP).

### Self-supervised DFER

![images/Self_supervised_DFER_00.jpg](images/Self_supervised_DFER_00.jpg)

The architecture of self-supervised DFER. This is reproduced based on the MAE-DFER.

### Visual-Language DFER

![images/DFER_CLIP.png](images/DFER_CLIP.png)

The architecture of vision-language DFER. Figure is reproduced based on DFER-CLIP.

## Citation

If you find our work useful, please cite our paper:

```latex

@article{wang_survey_2024,
		title = {A Survey on Facial Expression Recognition of Static and Dynamic Emotions},
		author = {Wang, Yan and Yan, Shaoqi and Liu, Yang and Song, Wei and Liu, Jing and Chang, Yang and Mai, Xinji and Hu, Xiping and Zhang, Wenqiang and Gan, Zhongxue},
	  journal = {arXiv preprint arXiv:2408.15777},
	  year = {2024}
}

```
