# 🎭 Shakespeare Text Generation using RNN

Generate Shakespeare-style text by training a character-level Recurrent Neural Network (RNN) on Shakespeare’s writings. The model learns sequential patterns to create coherent and stylistically similar text passages.

The repository includes a full workflow notebook and a trained model for easy experimentation.

---

## 📁 Project Folder Structure

📦 Shakespeare-Text-Generation-RNN
- │
- ├── Rnn_Project2_Text_Generation_Shakespeare.ipynb # Notebook containing full workflow:
- │ # data preprocessing, training, evaluation, text generation
- │
- ├── lstm_shakespeare_model.pth # Trained LSTM model saved after training
- │
- └── README.md # Project documentation


---

## 📝 Problem Statement

Build a deep learning model to generate Shakespeare-style text using a character-level RNN.  
The model learns from sequences of characters to predict the next character, enabling it to produce novel text passages that mimic Shakespeare’s writing style.

---

## 📚 Dataset Details

**Source:** Tiny Shakespeare dataset  
**Format:** Plain text (~1MB)

**Characteristics:**
- Character-level data (letters, punctuation, spaces)
- Rich literary style and diverse vocabulary

---

## 🛠️ Model & Approach

- Character-level RNN trained to predict the next character from previous sequences  
- **Architectures compared:** SimpleRNN, LSTM, GRU  
- **Loss Function:** Cross-Entropy Loss  
- **Training:** Multiple epochs with sequence-based input-target pairs  
- **Text Generation:** Sampling techniques with temperature scaling  
- **Evaluation:** Train/validation loss + qualitative inspection of generated text  

---

## 🎯 Key Highlights

- Generated text mimics Shakespeare’s style and rhythm  
- Demonstrated the RNN’s ability to learn long-range dependencies  
- Strong foundation for sequence modeling in NLP  
- Shows the creative potential of deep learning models  

---

## 🔎 Model Performance

| Model      | Train Loss | Validation Loss |
|------------|------------|-----------------|
| SimpleRNN  | 1.2820     | 1.2842          |
| LSTM       | 0.9914     | 0.9977          |
| GRU        | 1.1040     | 1.1320          |

**Observations:**
- **LSTM** achieves the best train/validation loss → best for character-level generation  
- **GRU** performs better than SimpleRNN but worse than LSTM  
- SimpleRNN struggles with long-term dependencies  

---

## 📌 Conclusion & Insights

- Character-level LSTM effectively captures long-term dependencies in Shakespearean text  
- Generated text showcases Shakespeare-like vocabulary and rhythm  
- Provides a strong base for advanced NLP projects such as Transformers  

---

## 🚀 Potential Improvements

### 📊 Model & Architecture
- Shift to word-level modeling  
- Try deeper or stacked GRUs  
- Explore Transformer-based architectures  
- Add embedding layers for dense character representations  

### 🔧 Hyperparameter Optimization
- Tune sequence length, hidden units, layers  
- Adjust batch size, learning rate  
- Extend epochs and use LR schedulers  

### 🎨 Sampling & Generation
- Add **Top-K**, **Top-P (Nucleus) Sampling**  
- Improve coherence with temperature tuning  

---

## ⚠️ Limitations

- High computational cost  
- Long text coherence still challenging  
- Memory usage grows with sequence length  
- Style limited to training corpus  

---

## ✅ Key Takeaway

This project demonstrates the core principles of sequence modeling and natural language generation using LSTMs:

- Prepares text for next-character prediction  
- Builds and trains memory-capable LSTM networks  
- Implements temperature-based sampling for creative text generation  

The LSTM model establishes the foundation for future improvements using word-level models, attention mechanisms, and Transformers.

---
