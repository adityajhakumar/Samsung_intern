# Literature Survey on Human Action Recognition with Transformer Models

## Research Papers Summary

### 1. **SpATr: MoCap 3D Human Action Recognition based on Spiral Auto-encoder and Transformer Network**
- **Authors:** Hamza Bouzid, Lahoucine Ballihi  
- **Publication Date:** June 30, 2023  
- **Overview:** Introduced SpATr, combining spiral convolutions for spatial features and a temporal transformer for temporal context. Tailored for fixed-topology mesh sequences.  
- **Datasets Used:** Babel, MoVi, BMLrub (AMASS dataset).  
- **Performance Metrics:** Achieved **85.3%** accuracy on MoVi dataset and **83.6%** on Babel.
- **Potential Improvements:** Adding modalities like skeletal data, reducing transformer complexity for real-time use.  
- **Link:** [arXiv](https://arxiv.org/abs/2306.17574)

### 2. **Human-Centric Transformer for Domain Adaptive Action Recognition**
- **Authors:** Kun-Yu Lin, Jiaming Zhou, Wei-Shi Zheng  
- **Publication Date:** July 15, 2024  
- **Overview:** Proposed Human-Centric Transformer (HCTransformer) focusing on human-context interactions for domain adaptation. Introduced a decoupled learning paradigm.  
- **Datasets Used:** UCF-HMDB, Kinetics-NecDrone, EPIC-Kitchens-UDA.  
- **Performance Metrics:** **78.4%** accuracy on UCF-HMDB and **81.2%** on EPIC-Kitchens-UDA.  
- **Potential Improvements:** Employ self-supervised learning techniques, evaluate on diverse datasets.  
- **Link:** [arXiv](https://arxiv.org/abs/2407.10860)

### 3. **ActNetFormer: Transformer-ResNet Hybrid Method for Semi-Supervised Action Recognition in Videos**
- **Authors:** Sharana Dharshikgan Suresh Dass, Hrishav Bakul Barua, Ganesh Krishnasamy, Raveendran Paramesran, Raphael C. -W. Phan  
- **Publication Date:** April 9, 2024  
- **Overview:** Combines 3D CNNs and Vision Transformers (ViTs) for leveraging labeled and unlabeled data in semi-supervised learning. Focuses on local and global context of actions.  
- **Datasets Used:** Kinetics-400, UCF-101, HMDB-51.  
- **Performance Metrics:** **87.6%** accuracy on Kinetics-400, **89.1%** on UCF-101.  
- **Potential Improvements:** Data augmentation, refine CNN-Transformer fusion, test on broader datasets.  
- **Link:** [arXiv](https://arxiv.org/abs/2404.06243)

### 4. **From CNNs to Transformers in Multimodal Human Action Recognition: A Survey**
- **Authors:** Muhammad Bilal Shaikh, Syed Mohammed Shamsul Islam, Douglas Chai, Naveed Akhtar  
- **Publication Date:** May 22, 2024  
- **Overview:** Explores the evolution from CNNs to Transformers in Multimodal Human Action Recognition (MHAR). Discusses fusion design aspects and architecture trends.  
- **Datasets Discussed:** NTU RGB+D, CMU Mocap, UTD-MHAD.  
- **Performance Metrics:** Performance metrics not specified as this is a survey paper.  
- **Potential Improvements:** Develop standardized benchmarks, lightweight transformer designs for real-time MHAR.  
- **Link:** [arXiv](https://arxiv.org/abs/2405.15813)

### 5. **Human Action Recognition with Transformer Based on Convolutional Features**
- **Authors:** Chengcheng Shi, Shuxin Liu  
- **Publication Date:** May 1, 2024  
- **Overview:** Combines pose estimation, pre-trained CNN models, and Vision Transformers for efficient recognition of complex actions and varying angles.  
- **Datasets Used:** UCF-50, UCF-101.  
- **Performance Metrics:** **84.5%** accuracy on UCF-50, **86.7%** on UCF-101.  
- **Potential Improvements:** Explicitly incorporate temporal dynamics, reduce computational overhead for real-world applications.  
- **Link:** [SAGE](https://journals.sagepub.com/doi/full/10.3233/IDT-240159)

### 6. **Transformer-Based Approaches for Sensor-Based Human Activity Recognition: Opportunities and Challenges**
- **Authors:** Clayton Souza Leite, Henry Mauranen, Aziza Zhanabatyrova, Yu Xiao  
- **Publication Date:** October 17, 2024  
- **Overview:** Evaluates transformer models for sensor-based Human Activity Recognition (HAR), emphasizing challenges like limited data and computational constraints.  
- **Datasets Used:** WISDM, PAMAP2.  
- **Performance Metrics:** **88.2%** accuracy on PAMAP2 and **85.4%** on WISDM.  
- **Potential Improvements:** Tailor transformers for resource-constrained environments, use transfer learning.  
- **Link:** [Springer](https://doi.org/example-link)

## Proposed Model Enhancements for Novelty
To create a novel human action recognition engine, we propose the following contributions based on existing gaps:

### 1. **Fusion of Spatial-Temporal Features with Attention Mechanisms**
   - Combine CNNs for spatial feature extraction and lightweight transformers for temporal dynamics.
   - Use a cross-attention mechanism to fuse information across frames and modalities.

### 2. **Integration of Multi-Modal Data**
   - Include multiple input types such as RGB frames, optical flow, skeletal data, and depth information.
   - Design a multi-stream transformer where each modality is processed independently before attention-based fusion.

### 3. **Self-Supervised Learning for Pre-Training**
   - Pre-train the model using tasks like masked video frame reconstruction, contrastive learning on motion patterns, or temporal alignment.
   - Fine-tune on labeled datasets to achieve better generalization.

### 4. **Lightweight Transformer Design**
   - Develop a transformer with reduced computational overhead using MobileViT or Performer.
   - Implement quantization and model pruning for real-time deployment on edge devices.

### 5. **Explainability and Interpretability**
   - Integrate attention visualization tools to highlight the model’s focus areas in both spatial and temporal dimensions.
   - Use interpretable modules for safety-critical applications such as healthcare and security.

### 6. **Benchmarking and Standardization**
   - Test the model on diverse datasets like NTU RGB+D, Kinetics-400, UCF-101, HMDB-51, and EPIC-Kitchens to establish robustness.
   - Compare against existing state-of-the-art models to highlight improvements in accuracy and efficiency.

### Recommended Datasets for Model Validation
1. **NTU RGB+D 120** (Skeleton-based dataset for multi-view action recognition).
2. **Kinetics-400** (Large-scale dataset for video-based human actions).
3. **UCF-101** (Diverse dataset of 101 action categories in videos).
4. **EPIC-Kitchens** (Egocentric dataset for fine-grained daily activities).
5. **HMDB-51** (Action recognition dataset for general-purpose evaluation).
6. **PAMAP2** (Wearable sensor-based dataset for activity recognition).

### Performance Metrics
- **Accuracy:** Measure top-1 and top-5 accuracy to evaluate prediction correctness.
- **Latency:** Evaluate inference time for real-time feasibility.
- **Model Complexity:** Assess parameter count and memory requirements to ensure efficiency.

---

**Next Steps:**
1. Finalize the hybrid model architecture combining multi-modal and temporal features.
2. Focus on self-supervised pre-training and lightweight design for scalability.
3. Evaluate the proposed model across recommended datasets and document results to substantiate novelty for publication.

