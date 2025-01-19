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

To ensure the proposed model aligns with the goal of being a lightweight transformer, we can refine the **Proposed Model Enhancements** section and add specific considerations for lightweight design:

---

### Proposed Model Enhancements for Lightweight Design

1. **Simplified Attention Mechanisms**  
   - Replace standard attention with efficient variants like Linformer, Performer, or Nyströmformer to reduce computational complexity and memory usage.

2. **Feature Compression Techniques**  
   - Employ dimensionality reduction methods (e.g., PCA or Autoencoders) for spatial and temporal features before feeding them into the transformer layers.

3. **Integration of Multi-Modal Data in Lightweight Streams**  
   - Use separate lightweight encoders for each data modality (e.g., RGB, optical flow, skeleton data), with a shared transformer decoder to aggregate information efficiently.

4. **Efficient Model Architectures**  
   - Explore architectures like MobileViT or EfficientFormer, which are designed for low-resource environments while maintaining performance.

5. **Self-Supervised Learning with Minimal Overhead**  
   - Leverage pre-training tasks like masked video prediction with reduced feature dimensions to minimize training cost.

6. **Quantization and Model Compression**  
   - Apply techniques like post-training quantization, pruning, and knowledge distillation to ensure the model is deployable on edge devices.

---

### Key Datasets with Lightweight Considerations
1. **NTU RGB+D 120**  
   - Apply data sampling techniques to limit the data fed to the model while maintaining temporal context.
2. **Kinetics-400 (Reduced Frames)**  
   - Process reduced frame sequences to lower computational load.
3. **PAMAP2 (Sensor Data)**  
   - Ideal for low-latency models designed for real-time recognition.

---

