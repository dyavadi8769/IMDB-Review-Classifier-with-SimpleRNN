# IMDB Review Classifier with SimpleRNN

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![TensorFlow](https://img.shields.io/badge/TensorFlow-2.15-orange)
![Streamlit](https://img.shields.io/badge/Streamlit-Web%20App-green)

## Project Overview
A deep learning project that classifies IMDB movie reviews as positive or negative using a Simple Recurrent Neural Network (RNN) with an interactive web interface.

## Features
- **End-to-End Pipeline**:
  - Text preprocessing & tokenization
  - Sequence padding to fixed length (500 words)
  - Model training with early stopping
- **Interactive Demo**:
  - Real-time sentiment prediction
  - Confidence score visualization
- **Model Architecture**:
  - Embedding layer (128 dimensions)
  - SimpleRNN layer (128 units)
  - Dense output layer with sigmoid activation


## 🚀 How It Works

1. **Data Preparation**:
**Loads IMDB dataset (25,000 reviews)
   - Converts words to integer sequences
   - Pads/truncates sequences to 500 words

2. **Model Architecture**:
   ```python
   model = Sequential([
       Embedding(10000, 128, input_length=500),
       SimpleRNN(128, activation='relu'),
       Dense(1, activation='sigmoid')
   ])

3. **Training**:
   - Binary cross-entropy loss
   - Adam optimizer
   - Early stopping (patience=5)

4. **Inference**:
   - Preprocesses user input text
   - Makes real-time predictions
   - Displays sentiment (Positive/Negative) with confidence score



## Commands to Setup Project on Local Machine

1. **Clone the repository:**
   ```bash
   git clone https://github.com/dyavadi8769/IMDB-Review-Classifier-with-SimpleRNN.git
   cd IMDB-Review-Classifier-with-SimpleRNN
2.  **Create a virtual environment and activate it:**
    ```bash
    conda create -p env python==3.10 -y
    conda activate env/ 
3.  **Install the Required Dependecies:**
    ```bash
    pip install -r requirements.txt
4. **Run the app.py to Classify IMDB Reviews :**
    ```bash
    python app.py
# Author:

```bash
Author: Sai Kiran Reddy Dyavadi
Role  : Data Scientist
Email : dyavadi324@gmail.com
```
