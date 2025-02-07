# MNIST Digit Classification with Scikit-Learn  
A machine learning project comparing traditional classifiers (e.g., SGD, Random Forest, SVM, KNN) to classify handwritten digits from the MNIST dataset.

## Key Features  

### **Dataset**  
- **MNIST dataset**:  
  - 70,000 grayscale images (60,000 training + 10,000 test) of digits 0-9.  
  - 28x28 pixel resolution.  

### **Models & Techniques**  
- **Binary Classification** (5 vs. non-5):  
  - SGDClassifier (Linear Model)  
  - RandomForestClassifier  
  - Precision-Recall/ROC curve analysis  
- **Multiclass Classification**:  
  - SVM (Support Vector Machine)  
  - One-vs-Rest strategy  
  - K-Nearest Neighbors (KNN)  
- **Error Analysis**:  
  - Confusion matrix visualization  
  - Error normalization by row/column  
- **Hyperparameter Tuning**:  
  - GridSearchCV for optimizing KNN (`n_neighbors` and `weights`)  

### **Training & Evaluation**  
- Achieves **97% test accuracy** with tuned KNN.  
- Key metrics for binary classification:  
  - Precision: ~90% (at 80% recall)  
  - ROC AUC: 0.96 (Random Forest)  
- Multiclass evaluation:  
  - SGDClassifier baseline: ~85% accuracy (improves to ~89% with scaling).  

### **Visualization**  
- Displays 10x10 grid of sample MNIST digits.  
- Precision-Recall/ROC curves for binary classifier comparison.  
- Confusion matrices for error analysis (raw counts and normalized).  
