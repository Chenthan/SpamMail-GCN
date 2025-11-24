# 📧 SpamMail-GCN

### **Graph Convolutional Network (GCN) for Spam Email Classification**

SpamMail-GCN is a lightweight research project that explores how **Graph Neural Networks (GNNs)**, specifically **GCNs**, can be used for email spam detection. Instead of traditional text-classification pipelines, this project treats the email dataset as a **graph**, where relationships between emails are encoded and learned.

---

## 🚀 Features

* Custom 2-layer Graph Convolutional Network (GCN) implementation
* Graph-based email representation
* Modular training pipeline
* Easy inference script
* Output folder includes performance screenshots and graphs

---

## 📊 Model Performance

**Training Accuracy:** ~97.76%
**Test Accuracy:** ~87.50%
**Final Loss:** ~0.0528

See the `Output/` folder for detailed visualizations.

---

## 🧠 Project Architecture

```
SpamMail-GCN
│
├── GCN.py                 # Core GCN model (2-layer & batched variants)
├── trainer.py             # Training loop + evaluation
├── train_funcs.py         # Optimization & batching utilities
├── preprocessing_funcs.py # Graph construction + data preprocessing
├── classify.py            # Inference script
├── Output/                # Plots & screenshots
└── .gitignore
```

---

## 🏗️ How It Works

1. **Preprocessing** – Emails are converted into vectors and graphs.
2. **Graph Construction** – Nodes represent emails; edges represent semantic similarity.
3. **GCN Layers:**

```
X'  = ReLU(A_hat * X * W1)
X'' = ReLU(A_hat * X' * W2)
logits = FC(X'')
```

4. **Training** – Adam optimizer + cross-entropy loss.
5. **Inference** – Run `python classify.py` to classify new samples.

---

## 🛠️ Setup & Usage

### Install dependencies

```
pip install torch numpy matplotlib
```

### Train the model

```
python trainer.py
```

### Run inference

```
python classify.py
```

---

## 📦 Outputs

The `Output/` folder contains:

* Accuracy graphs
* Loss curves
* Console output screenshots

---
