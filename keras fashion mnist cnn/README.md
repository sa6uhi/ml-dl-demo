# Fashion MNIST Classification with Keras  
A deep learning project using Keras/TensorFlow to classify fashion items from the Fashion MNIST dataset, achieving **88% test accuracy**.

## Key Features  

### **Dataset**  
- **Fashion MNIST**:  
  - 70,000 grayscale images (60,000 training + 10,000 test).  
  - 10 classes: T-shirt/top, Trouser, Pullover, Dress, Coat, Sandal, Shirt, Sneaker, Bag, Ankle Boot.  
  - 28x28 pixel resolution.  

### **Models**  
1. **Simple Neural Network**:  
   - `Flatten` → `Dense(128, ReLU)` → `Dense(10, Softmax)`  
   - **Accuracy**: ~88% on test data.  

2. **Convolutional Neural Network (CNN)**:  
   - Architecture:  
     ```python
     Conv2D(32, kernel=(3,3), ReLU) → MaxPooling2D  
     Conv2D(32, kernel=(3,3), ReLU) → MaxPooling2D  
     Flatten → Dense(128, ReLU) → Dense(10, Softmax)  
     ```  
   - Trained for 5 epochs.  
   - Comparable accuracy to the simple NN (~88%).  

### **Training**  
- **Optimizer**: Adam.  
- **Loss**: Sparse Categorical Crossentropy.  
- **Preprocessing**:  
  - Pixel values normalized to [0, 1].  
  - Reshaped to `(28, 28, 1)` for CNN.  

### **Visualization**  
- Displays sample images with labels.  
- Prediction confidence plots (correct predictions in skyblue, misclassifications in lightcoral).
