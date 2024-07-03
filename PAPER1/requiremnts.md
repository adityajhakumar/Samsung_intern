
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
1. **Framework**:
   - TensorFlow, specifically TensorFlow Lite, for benchmarking and measuring inference performance

2. **Operating System**:
   - Suitable for running TensorFlow and supporting the required hardware (typically Android or iOS for mobile devices)

### Environmental Setup:
- The study conducted experiments using TensorFlow’s benchmark tools to measure inference time, memory footprint, and model size over 1000 inferences using 4 threads.

These requirements ensure that the models can perform real-time activity classification efficiently on mobile devices.
