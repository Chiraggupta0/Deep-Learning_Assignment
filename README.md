# 📊 Text Sentiment Classification using Deep Learning (RNN, LSTM, GRU)
📌 Overview

This project implements deep learning models for sentiment analysis on text data using:

Recurrent Neural Network (RNN)
Long Short-Term Memory (LSTM)
Gated Recurrent Unit (GRU)

The goal is to classify movie reviews as positive or negative and compare model performance.

🎯 Objective
Understand sequence modeling in deep learning
Implement RNN, LSTM, and GRU architectures
Compare their performance on text data
Analyze improvements of LSTM & GRU over traditional RNN
📂 Dataset
Dataset Used: IMDB Movie Review Dataset
Total Samples: 50,000
Training Data: 25,000
Testing Data: 25,000
Type: Binary Classification (Positive / Negative)

✔ Balanced dataset
✔ Available via TensorFlow/Keras

🧹 Data Preprocessing

Steps applied before training:

🔹 Text Cleaning
Lowercasing
Removing punctuation
Removing stopwords
Removing special characters
🔹 Tokenization

Example:

"I love this movie" → [45, 23, 87, 102]
🔹 Padding
Fixed sequence length: 200
Ensures uniform input size for models
🧠 Model Architectures
🔸 1. RNN Model
Embedding Layer (128 units)
Simple RNN (64 units)
Dense Layer (Sigmoid activation)
🔸 2. LSTM Model
Embedding Layer (128 units)
LSTM Layer (64 units)
Dense Layer (Sigmoid activation)

✔ Handles long-term dependencies using gates:

Forget Gate
Input Gate
Output Gate
🔸 3. GRU Model
Embedding Layer (128 units)
GRU Layer (64 units)
Dense Layer (Sigmoid activation)

✔ Uses:

Update Gate
Reset Gate

✔ Faster and simpler than LSTM

⚙️ Training Configuration
Epochs: 3
Batch Size: 64
Optimizer: Adam
Loss Function: Binary Crossentropy
Validation Split: 20%
📈 Results & Insights
RNN struggles with long-term dependencies
LSTM performs better due to memory cells
GRU achieves similar performance with fewer parameters
LSTM & GRU outperform basic RNN in sentiment classification
🛠️ Tech Stack
Python
TensorFlow / Keras
NumPy
Matplotlib


🚀 How to Run
# Clone repository
git clone https://github.com/your-username/your-repo-name.git

# Navigate to project
cd your-repo-name

# Install dependencies
pip install -r requirements.txt

# Run notebook/script
jupyter notebook
📌 Future Improvements
Use pretrained embeddings (GloVe, Word2Vec)
Hyperparameter tuning
Add attention mechanism
Deploy model using Flask/Streamlit
👨‍🎓 Author

Chirag Gupta
MCA (AI & ML)
