# 🤖 GPT-Style Text Generator

> An educational implementation of a **Decoder-Only Transformer Language Model** built using **TensorFlow/Keras** to demonstrate autoregressive text generation, next-token prediction, and the fundamental architecture behind GPT-style language models.

![Python](https://img.shields.io/badge/Python-3.x-blue)
![TensorFlow](https://img.shields.io/badge/TensorFlow-Deep%20Learning-orange)
![Keras](https://img.shields.io/badge/Keras-Neural%20Networks-red)
![NLP](https://img.shields.io/badge/NLP-Transformer-success)
![License](https://img.shields.io/badge/License-MIT-green)

---

# 📖 Overview

GPT-Style Text Generator is a deep learning project that implements the core concepts of **decoder-only transformer architectures** used in modern autoregressive language models.

Rather than serving as a production-scale GPT implementation, this project focuses on understanding and building the complete text generation pipeline from the ground up.

The implementation demonstrates:

- Text preprocessing
- Vocabulary construction
- Tokenization
- Sequence generation
- Token & positional embeddings
- Masked self-attention
- Decoder-only transformer blocks
- Next-token prediction
- Autoregressive text generation

The project is designed as an educational exploration of transformer-based language modeling while emphasizing clean implementation and modular neural network components.

---

# ❓ Problem Statement

Large Language Models such as GPT generate coherent text by predicting one token at a time using decoder-only transformer architectures.

Understanding how these models work internally can be challenging because most production implementations are highly optimized and abstracted.

This project simplifies the architecture into an educational implementation that demonstrates how transformer-based language models perform next-token prediction and autoregressive text generation.

---

# 🎯 Objectives

- Understand decoder-only transformer architectures
- Implement autoregressive next-token prediction
- Explore token and positional embeddings
- Demonstrate masked self-attention
- Build a complete text generation workflow
- Apply TensorFlow/Keras for NLP model development

---

# ✨ Features

- Educational decoder-only Transformer implementation
- Custom Token + Positional Embedding layer
- Masked Multi-Head Self-Attention
- Feed Forward Network
- Next-token prediction
- Autoregressive text generation
- Dataset preprocessing pipeline
- Vocabulary creation
- Sequence padding
- Interactive prediction examples
- TensorFlow/Keras implementation

---

# 🏗 High-Level Architecture

```text
Text Dataset
      │
      ▼
Tokenization
      │
      ▼
Vocabulary Creation
      │
      ▼
Input / Target Sequence Generation
      │
      ▼
Token Embedding
      │
      ▼
Positional Embedding
      │
      ▼
Decoder-Only Transformer Block
      │
      ▼
Dense + Softmax
      │
      ▼
Next Token Prediction
      │
      ▼
Autoregressive Text Generation
```

---

# 🔄 Training Pipeline

```text
Dataset

↓

Text Preprocessing

↓

Tokenization

↓

Padding

↓

Input / Target Preparation

↓

Token Embedding

↓

Positional Embedding

↓

Decoder-only Transformer

↓

Softmax Prediction

↓

Categorical Cross Entropy Loss

↓

Backpropagation

↓

Trained Language Model
```

---

# ⚡ Inference Pipeline

```text
Input Prompt

↓

Tokenization

↓

Embedding

↓

Transformer Decoder

↓

Softmax

↓

Predict Next Token

↓

Append Prediction

↓

Repeat

↓

Generated Text
```

---

# 📊 Data Flow

The project follows an autoregressive language modeling workflow:

1. Create a small educational text corpus.
2. Convert words into numerical tokens.
3. Pad sequences to fixed length.
4. Prepare input-target pairs for next-token prediction.
5. Train the transformer using teacher forcing.
6. Predict one token at a time during inference.
7. Append predicted tokens to generate complete text.

---

# 🧠 Model Architecture

The implemented model consists of:

- Token Embedding Layer
- Positional Embedding Layer
- Decoder-Only Transformer Block ×2
- Feed Forward Network
- Residual Connections
- Layer Normalization
- Dense Output Layer
- Softmax Activation

### Model Summary

| Component | Value |
|-----------|------:|
| Embedding Dimension | 32 |
| Transformer Blocks | 2 |
| Vocabulary Size | 1000 |
| Total Parameters | 90,664 |
| Training Epochs | 300 |

---

# 📁 Project Structure

```text
gpt-style-text-generator/

│── src/
│   └── gpt_style_text_generator.py

│── outputs/
│   ├── training_output.png
│   └── generated_text_examples.png

│── requirements.txt
│── README.md
```

---

# 🛠 Technologies Used

### Programming

- Python

### Deep Learning

- TensorFlow
- Keras

### Scientific Computing

- NumPy

### Concepts

- Natural Language Processing (NLP)
- Transformer Architecture
- Autoregressive Language Modeling
- Neural Networks
- Deep Learning

---

# 💡 Engineering Concepts Demonstrated

- Modular neural network components
- Custom Keras layers
- Decoder-only Transformer implementation
- Data preprocessing pipeline
- Training workflow
- Inference workflow
- Autoregressive decoding
- Educational visualization of transformer concepts

---

# 🧠 Machine Learning Concepts Demonstrated

- Vocabulary generation
- Tokenization
- Sequence padding
- Teacher forcing
- Token embeddings
- Positional embeddings
- Masked self-attention
- Decoder-only transformers
- Feed Forward Networks
- Cross-entropy optimization
- Gradient-based training
- Next-token prediction
- Language modeling

---

# 📈 Results

The model was trained on a small educational dataset demonstrating transformer-based language modeling.

### Training Summary

| Metric | Value |
|---------|------:|
| Epochs | 300 |
| Final Training Accuracy | ~94% |
| Final Training Loss | ~0.08 |

> Since the dataset is intentionally small, these results demonstrate successful learning of the training corpus rather than general-purpose language modeling.

---

# 💬 Sample Predictions

## Next Word Prediction

| Input | Prediction |
|--------|------------|
| i love | deep |
| machine learning is | powerful |
| deep learning is | amazing |
| gpt is | decoder |
| language model predicts | next |
| masked attention prevents | future |

---

## Autoregressive Text Generation

**Input**

```text
i love
```

**Output**

```text
i love deep learning
```

---

**Input**

```text
machine learning
```

**Output**

```text
machine learning is powerful
```

---

**Input**

```text
decoder transformer
```

**Output**

```text
decoder transformer generates text
```

---

**Input**

```text
gpt
```

**Output**

```text
gpt predicts next token
```

---

**Input**

```text
students learn
```

**Output**

```text
students learn artificial intelligence
```

---

# 📷 Screenshots

Add screenshots of:

- Dataset creation
- Tokenization output
- Model summary
- Training progress
- Text generation examples

---

# ⚙ Installation

Clone the repository

```bash
git clone https://github.com/yourusername/gpt-style-text-generator.git

cd gpt-style-text-generator
```

Install dependencies

```bash
pip install -r requirements.txt
```

---

# 🚀 Running the Project

```bash
python src/gpt_style_text_generator.py
```

The script demonstrates the complete workflow:

- Dataset preparation
- Tokenization
- Vocabulary creation
- Embedding generation
- Masked attention
- Model construction
- Training
- Next-word prediction
- Autoregressive text generation

---

# ⚙ Configuration

Current implementation uses:

- Decoder-only Transformer architecture
- Embedding dimension: 32
- Two Transformer blocks
- Sequence length: 6
- TensorFlow/Keras backend

---

# 🚀 Future Improvements

Potential enhancements include:

- Larger training datasets
- Byte Pair Encoding (BPE) tokenizer
- Temperature sampling
- Top-k / Top-p sampling
- Beam search decoding
- Model checkpointing
- Attention visualization
- Configurable hyperparameters
- TensorBoard integration
- Streamlit inference interface
- Hugging Face dataset support

---

# 📚 Learning Outcomes

This project provided practical experience with:

- Transformer internals
- Decoder-only language models
- Self-attention mechanisms
- Autoregressive generation
- NLP preprocessing
- Deep learning model implementation
- TensorFlow model development

---

# 📄 License

This project is licensed under the MIT License.

---

## 👨‍💻 Author

**Niraj Nale**

B.Tech Robotics & Automation  
MIT World Peace University, Pune

---

⭐ If you found this project interesting, consider giving it a star.
