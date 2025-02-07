# MNIST Digit Classification with PyTorch  
A convolutional neural network (CNN) implementation using PyTorch to classify handwritten digits from the MNIST dataset.

## Key Features  

### **Dataset**  
- Uses the **MNIST dataset**:  
  - 60,000 training images + 10,000 test images.  
  - 28x28 grayscale images of handwritten digits (0-9).  

### **Model Architecture**  
- **CNN structure**:  
  - **Convolutional Layers**:  
    - `Conv1`: 1 input channel → 16 output channels, kernel=5, ReLU activation, max pooling (kernel=2).  
    - `Conv2`: 16 input channels → 32 output channels, kernel=5, ReLU activation, max pooling (kernel=2).  
  - **Fully Connected Layer**:  
    - Output layer with 10 classes (digits 0-9).  

### **Training**  
- **Optimizer**: Adam (`lr=1e-3`).  
- **Loss Function**: Cross-Entropy Loss.  
- **Epochs**: 10.  
- **Batch Size**: 100.  
- Automatically saves trained weights to `mnist_cnn.pt`.  

### **Evaluation**  
- Achieves **~98-99% test accuracy** on MNIST test data.  

### **Visualization**  
- Displays a **5x5 grid of sample training images** with labels.  
- Compares model predictions vs. ground truth labels for test data (e.g., `Predict: [7 2 1 0 4...]` vs `Actual: [7 2 1 0 4...]`).  
