# 🧠 Attention Is All You Need — NLP Project

A comprehensive implementation and comparison of modern neural network architectures in **Natural Language Processing (NLP)** using **PyTorch** and **HuggingFace Transformers**.

---

## 🔍 Tasks Covered

- 🗂 **Text Classification**  
- 🔄 **Sequence-to-Sequence Translation** (e.g., French to English)  
- ❓ **Question Answering**  
- ✍️ **Text Generation**

---

## 📚 Background

### 🧮 Recurrent Neural Networks (RNNs)
RNNs process sequential data by maintaining a hidden state that captures temporal patterns. They’re effective for language modeling, translation, and text generation.  
**Limitations**: Vanishing gradient problem, poor long-term memory  
**Improvement**: **Bidirectional RNNs** read sequences both forward and backward to capture richer context.

### 🔁 Encoder-Decoder Architecture
A classical **Seq2Seq** approach using RNNs:
- **Encoder**: Compresses input into a fixed context vector  
- **Decoder**: Generates the output from the context

![Encoder-Decoder](/Images/attention_research_1.webp)

### ⚡ Transformers (Vaswani et al., 2017)
Replaces recurrence with **self-attention** mechanisms for parallelism and modeling long-range dependencies.  
Key components:
- Multi-head self-attention  
- Positional encoding  
- Scalable parallel training  

### 🧠 BERT (Bidirectional Encoder Representations from Transformers)
A deep, pre-trained Transformer encoder using:
- **Masked Language Modeling (MLM)**  
- **Next Sentence Prediction (NSP)**  
It generates **context-aware embeddings** fine-tuned for various NLP tasks.

![BERT and GPT](/Images/Bert%20GPT.jpeg)

---

## 📂 Project Structure

```bash
attention-is-all-you-need/
│
├── Classify text with BERT/                       # Fine-tune BERT for classification
├── Generating Text Using a Transformer Decoder-Only Model/  # GPT-style generation
├── Images/                                        # Visualizations
├── Machine Translation French to English/         # Seq2Seq & Transformer-based translation
├── Question-Answering with a Multi-Layer Bidirectional RNN/ # QA with Bi-RNN
├── Simple RNN Encode-Decoder for Translation/     # RNN-based translation
├── Text Generation with RNN/                      # Language modeling with RNN
├── Attention_is_all_you_need.pdf                  # Original Transformer paper
└── README.md                                      # Project overview
