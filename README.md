# 📰 Text Summarization using Seq2Seq with Attention (LSTM)

<p align="center">
  <img src="https://img.shields.io/badge/DeepLearning-LSTM-red?style=for-the-badge">
  <img src="https://img.shields.io/badge/NLP-TextSummarization-blue?style=for-the-badge">
  <img src="https://img.shields.io/badge/Model-Attention-green?style=for-the-badge">
  <img src="https://img.shields.io/badge/Status-Completed-success?style=for-the-badge">
</p>

---

##  Overview
This project focuses on **automatic text summarization of news articles** using deep learning.<br>
It implements **Sequence-to-Sequence (Seq2Seq) models with attention mechanisms** to generate human-like summaries.

The system reduces long news articles into short, meaningful summaries, solving the problem of **information overload in digital journalism**.

---

##  Objectives
- Generate coherent and meaningful summaries<br>
- Implement Seq2Seq LSTM models with attention<br>
- Compare Bahdanau and Luong attention mechanisms<br>
- Compare with Transformer model (T5)<br>
- Evaluate performance using ROUGE metrics<br>

---

##  Dataset
- Dataset Used: **CNN/DailyMail Dataset**<br>
- Contains:<br>
  - News Articles (Input)<br>
  - Highlights (Target Summary)<br>

- Dataset Split:<br>
  - Training: 287,113<br>
  - Validation: 13,368<br>
  - Test: 11,490   

 Articles are long (~700–800 words) while summaries are short (3–5 sentences), making it a **high compression task**.

---

##  Workflow
- Data Preprocessing<br>
- Tokenization & Padding<br>
- Seq2Seq Model Building<br>
- Attention Mechanism Integration<br>
- Model Training<br>
- Evaluation using ROUGE Scores<br>

---

##  Model Architecture

### 🔹 Seq2Seq LSTM
- Encoder: Processes input article<br>
- Decoder: Generates summary word-by-word<br>

### 🔹 Attention Mechanisms
- **Bahdanau Attention** → Better context understanding<br>
- **Luong Attention** → Faster & efficient computation<br>

 Attention helps model focus on important words instead of compressing everything into one vector.

---

##  Advanced Model
- T5 Transformer Model<br>
- Uses self-attention for better long-range dependencies<br>

✔ T5 outperforms LSTM models in fluency and accuracy 

---

##  Preprocessing Steps
- Lowercasing text<br>
- Removing special characters<br>
- Removing extra spaces<br>
- Adding tokens:<br>
  - `startseq` (start of summary)<br>
  - `endseq` (end of summary)<br>
- Tokenization using Keras Tokenizer<br>
- Padding sequences to fixed length  

---

##  Hyperparameters
- Vocabulary Size: 50,000<br>
- Max Article Length: 400<br>
- Max Summary Length: 50<br>
- Embedding Size: 128<br>
- LSTM Units: 128<br>
- Epochs: 20<br>
- Batch Size: 64 

---

## Evaluation Metrics
- ROUGE-1 → Word overlap<br>
- ROUGE-2 → Bigram overlap<br>
- ROUGE-L → Longest common subsequence 
---

## Results
- Attention improves Seq2Seq performance significantly<br>
- Bahdanau captures better context<br>
- Luong is computationally efficient<br>
- T5 performs best overall<br>

---

## 📊 Visualizations
- Training vs Validation Loss<br>
- ROUGE Score Comparison<br>
- Generated Summary Examples<br>

---

##  Tech Stack
- Python <br>
- TensorFlow / Keras<br>
- NumPy & Pandas<br>
- Matplotlib<br>
- Transformers (HuggingFace)<br>
- Rouge Score<br>

---
## ⚠️ Limitations
- LSTM struggles with very long sequences<br>
- Repetition issues in generated summaries<br>
- Lower ROUGE-2 scores<br>
## Future Improvements
- Use BART / PEGASUS models<br>
- Add Beam Search decoding<br>
- Use Pointer-Generator Networks<br>
- Deploy as web application<br>
## Why This Project Stands Out
✔ Real-world NLP problem<br>
✔ Deep Learning + Attention Mechanism<br>
✔ Comparison with Transformer (T5)<br>
✔ End-to-end pipeline<br>
