# 🎬 IMDB Movie Review Sentiment Analysis

A deep learning web application built with **TensorFlow**, **Simple RNN**, and **Streamlit** that predicts whether a movie review expresses **Positive** or **Negative** sentiment.

---

## 🚀 Demo

🌐 **Live App**

https://rnn-project-deployment-imdb-sentiment-analysis-abhoy.streamlit.app/

---

## ✨ Features

- Predicts movie review sentiment
- Simple RNN based neural network
- IMDB Dataset
- Interactive Streamlit UI
- Confidence Score
- Clean and responsive interface

---

## 🧠 Model Architecture

```
Input Review
      │
      ▼
Preprocessing
      │
      ▼
Embedding Layer
      │
      ▼
Simple RNN
      │
      ▼
Dense Layer (Sigmoid)
      │
      ▼
Positive / Negative
```

---

## 📂 Project Structure

```
RNN_project_deployment_imdb_sentiment_analysis/
│
├── main.py
├── simple_rnn_imdb.keras
├── requirements.txt
├── README.md
└── assets/
    └── streamlit-python-version-fix.png
```

---

## ⚙️ Installation

Clone the repository

```bash
git clone https://github.com/abhoy-ghosh/RNN_project_deployment_imdb_sentiment_analysis.git

cd RNN_project_deployment_imdb_sentiment_analysis
```

Create a virtual environment

```bash
conda create -n imdb_rnn python=3.11
```

Activate it

```bash
conda activate imdb_rnn
```

Install dependencies

```bash
pip install -r requirements.txt
```

Run the application

```bash
streamlit run main.py
```

---

## 📦 Requirements

- Python 3.11
- TensorFlow
- Streamlit
- NumPy

---

# 🚨 Streamlit Cloud Deployment Issue

While deploying the application on **Streamlit Community Cloud**, you may encounter an installation error similar to:

```
Error installing requirements

installer returned a non-zero exit code
```

or

```
No matching distribution found for tensorflow
```

This is **not a problem with the application code**.

The issue occurs because Streamlit Cloud may choose a Python version that is **not yet supported by TensorFlow**.

---

## ✅ Solution

Open your deployed application.

Click

```
⋮  →  Settings
```

Open the deployment logs and check which Python version is being used.

If the log shows an unsupported version (for example Python 3.14), change it to **Python 3.11**.

After changing the Python version, reboot the application.

---

## 📸 Example

![Python Version Fix](https://github.com/Abhoy-Ghosh/RNN_project_deployment_imdb_sentiment_analysis/blob/main/%7B33973863-FA31-4AC1-B5C9-E686888DB1BE%7D.png)

---

## Why does this happen?

TensorFlow only provides official wheels for supported Python versions.

If Streamlit deploys the application using an unsupported Python version, pip cannot install TensorFlow, resulting in

```
ERROR: No matching distribution found for tensorflow
```

Changing the deployment Python version to **3.11** resolves the issue.

---

## 🛠 Tech Stack

- Python
- TensorFlow / Keras
- Simple RNN
- Streamlit
- NumPy

---

## Dataset

The model is trained using the **IMDB Movie Review Dataset** provided by TensorFlow.

---

## Future Improvements

- Bidirectional LSTM
- GRU Model
- Attention Mechanism
- Better Text Preprocessing
- Explainable Predictions

---

## 👨‍💻 Author

**Abhoy Ghosh**

GitHub:
https://github.com/Abhoy-Ghosh

---

⭐ If you found this project useful, consider giving it a star.
