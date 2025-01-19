# Literature Survey on Human Action Recognition with Transformer Models

## Research Papers Summary

| **Paper Title**                                                                 | **Authors**                              | **Year** | **Datasets Used**                  | **Performance Metrics**                              | **Potential Improvements**                                                                 |
|--------------------------------------------------------------------------------|-----------------------------------------|----------|------------------------------------|-----------------------------------------------------|-------------------------------------------------------------------------------------------|
| SpATr: MoCap 3D Human Action Recognition based on Spiral Auto-encoder and Transformer Network | Hamza Bouzid, Lahoucine Ballihi         | 2023     | Babel, MoVi, BMLrub                | 85.3% (MoVi), 83.6% (Babel)                         | Add skeletal data, optimize transformer complexity for real-time applications             |
| Human-Centric Transformer for Domain Adaptive Action Recognition               | Kun-Yu Lin, Jiaming Zhou, Wei-Shi Zheng | 2024     | UCF-HMDB, Kinetics-NecDrone, EPIC-Kitchens-UDA | 78.4% (UCF-HMDB), 81.2% (EPIC-Kitchens-UDA)         | Incorporate self-supervised learning, test on more diverse datasets                       |
| ActNetFormer: Transformer-ResNet Hybrid Method for Semi-Supervised Action Recognition in Videos | Sharana Dharshikgan Suresh Dass et al.  | 2024     | Kinetics-400, UCF-101, HMDB-51     | 87.6% (Kinetics-400), 89.1% (UCF-101)               | Refine CNN-Transformer integration, apply advanced data augmentation                     |
| From CNNs to Transformers in Multimodal Human Action Recognition: A Survey     | Muhammad Bilal Shaikh et al.            | 2024     | NTU RGB+D, CMU Mocap, UTD-MHAD     | Metrics not provided                                | Develop standardized benchmarks, create lightweight designs for real-time applications   |
| Human Action Recognition with Transformer Based on Convolutional Features      | Chengcheng Shi, Shuxin Liu              | 2024     | UCF-50, UCF-101                    | 84.5% (UCF-50), 86.7% (UCF-101)                     | Incorporate explicit temporal dynamics, optimize for real-world use                      |
| Transformer-Based Approaches for Sensor-Based Human Activity Recognition       | Clayton Souza Leite et al.              | 2024     | WISDM, PAMAP2                      | 88.2% (PAMAP2), 85.4% (WISDM)                       | Adapt transformers for constrained environments, apply transfer learning                 |

## Proposed Model Enhancements for Novelty

1. **Fusion of Spatial-Temporal Features with Attention Mechanisms**: Combine CNNs for spatial features and lightweight transformers for temporal dynamics with cross-attention fusion.

2. **Integration of Multi-Modal Data**: Leverage modalities such as RGB, optical flow, skeletal data, and depth with a multi-stream transformer model.

3. **Self-Supervised Pre-Training**: Use masked video frame prediction, contrastive motion learning, or temporal alignment for pre-training.

4. **Lightweight Design**: Develop transformers optimized for low-latency inference using MobileViT or Performer, and apply quantization/pruning.

5. **Explainability**: Integrate attention visualization tools and interpretable modules for critical applications.

6. **Robust Benchmarking**: Test across diverse datasets like NTU RGB+D, Kinetics-400, UCF-101, and HMDB-51 to establish performance.

### Recommended Datasets for Validation
1. **NTU RGB+D 120**: Multi-view skeleton-based action recognition.
2. **Kinetics-400**: Large-scale video-based dataset.
3. **UCF-101**: 101 categories of diverse actions.
4. **EPIC-Kitchens**: Egocentric dataset for daily activities.
5. **HMDB-51**: General-purpose action dataset.
6. **PAMAP2**: Sensor-based activity recognition.

### Performance Metrics
- **Accuracy:** Top-1 and Top-5 accuracy.
- **Latency:** Evaluate inference time.
- **Model Complexity:** Parameter count and memory efficiency.

---

**Next Steps:**
1. Design the hybrid architecture incorporating the above improvements.
2. Validate on recommended datasets and compare results.
3. Document methodology and findings to establish novelty for publication.

