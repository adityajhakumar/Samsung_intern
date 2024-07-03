
### Hardware Requirements:
1. **Sensors**:
   - Accelerometer
   - Gyroscope
   - Magnetometer (optional, for additional accuracy)

2. **Computational Resources**:
   - On-device CPU (used for model inference)
   - Potential utilization of on-device GPU for parallel operations to reduce computation load and inference time

3. **Memory and Storage**:
   - Memory footprint and model size vary depending on the model architecture:
     - CNN: 51.05 MB of RAM, 25.80 MB storage
     - CNN-LSTM: 6.45 MB of RAM, 2.25 MB storage
     - ViT: 32.07 MB of RAM, 15.22 MB storage
     - HART: 12.74 MB of RAM, 5.91 MB storage
     - HARTOneMSA: 8.89 MB of RAM, 5.21 MB storage



### Software Requirements:
1. **Frameworks and Libraries**:
   - **TensorFlow**: The experiments utilized TensorFlow, specifically TensorFlow Lite, for benchmarking and performance measurement. TensorFlow Lite is crucial for deploying machine learning models on mobile devices due to its optimized performance and reduced model size.
   - **PyTorch**: PyTorch was also used for implementing and training the models. The flexibility and dynamic computation graph of PyTorch are advantageous for research and development.

2. **Development Tools**:
   - **TensorFlow Benchmark Tools**: These tools were used to measure inference time, memory footprint, and model size. The experiments involved running 1000 inferences using 4 threads to gather performance metrics.

3. **Operating System**:
   - The models and experiments were designed to be compatible with mobile operating systems that support TensorFlow Lite. Typically, this would include Android and iOS platforms.

4. **Model Architectures**:
   - Various model architectures were implemented and tested, including:
     - **ViT (Vision Transformer)**: Known for its performance in computer vision tasks.
     - **HART (Human Activity Recognition Transformer)**: Specifically designed for activity recognition.
     - **MobileHART**: An optimized version of HART for mobile devices.
     - **CNN (Convolutional Neural Network)**: Commonly used in image and activity recognition tasks.
     - **CNN-LSTM (Long Short-Term Memory)**: Combines CNN for feature extraction and LSTM for sequence modeling.

5. **Benchmark Datasets**:
   - The paper utilized multiple publicly available datasets to evaluate model performance, including:
     - RealWorld
     - HHAR (Huawei Activity Recognition)
     - MotionSense
     - SHL (Sussex-Huawei Locomotion)

### Additional Details:
- The software stack is designed to ensure that models can perform real-time activity classification efficiently on mobile devices. 
- The focus on TensorFlow Lite indicates a need for optimization and efficient deployment in resource-constrained environments like mobile devices.
- The choice of PyTorch for initial model development suggests that the authors valued the ease of experimentation and rapid prototyping that PyTorch offers.


### Environmental Setup:
- The study conducted experiments using TensorFlow’s benchmark tools to measure inference time, memory footprint, and model size over 1000 inferences using 4 threads.

These requirements ensure that the models can perform real-time activity classification efficiently on mobile devices.
