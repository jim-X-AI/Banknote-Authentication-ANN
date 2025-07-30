# Banknote Authentication using ANN

This project implements an Artificial Neural Network (ANN) to classify banknotes as genuine or forged based on features extracted from wavelet transforms.

## Dataset
The dataset contains the following features:
- **Variance (VWTI)**  
- **Skewness (SWTI)**  
- **Kurtosis (CWTI)**  
- **Entropy (EI)**  
- **Class (0: Genuine, 1: Forged)**  

Source: [UCI Banknote Dataset](https://archive.ics.uci.edu/ml/datasets/banknote+authentication)

## Model Architecture
- **Input Layer:** 4 neurons (one per feature)  
- **Hidden Layers:**  
  - Dense (16 neurons, `elu` activation)  
  - Dense (32 neurons, `relu` activation)  
  - Dense (32 neurons, `relu` activation)  
- **Output Layer:** 1 neuron (`sigmoid` activation for binary classification)  

## Training
- **Optimizer:** SGD (Stochastic Gradient Descent)  
- **Loss Function:** Binary Cross-Entropy  
- **Metrics:** Accuracy, Precision, Recall, F1-Score  
- **Epochs:** 42  
- **Validation Split:** 20%  

## Results
- **Accuracy:** 100% (on both training and test sets)  
- **Precision, Recall, F1-Score:** 1.0  

## Usage
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/Banknote-Authentication-ANN.git
2. Install dependencies:
  ```bash
  pip install numpy pandas tensorflow scikit-learn
3. Run the notebook:
  ```bash
  jupyter notebook Banknote_Authentication_ANN.ipynb

## Future Improvements

