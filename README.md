# 🧠 Turkish Hate Speech Detection with BERT Models

This project uses pretrained BERT models to classify Turkish tweets as containing hate speech or not. It leverages `transformers`, `PyTorch`, and evaluation tools like confusion matrices and classification reports.

The project also improves the results of the first project that focuses on the same topic. You can visit here: [Hate Speech Detection on Turkish Tweets](https://github.com/1eclerc/Hate-Speech-Detection-on-Turkish-Tweets)

---

## 📌 Project Overview

- **Language**: Turkish 
- **Task**: Binary text classification (`Hate Speech` vs `Non-Hate Speech`)
- **Models Used**:
  - [`VRLLab/TurkishBERTweet`](https://huggingface.co/VRLLab/TurkishBERTweet)
  - [`dbmdz/bert-base-turkish-cased`](https://huggingface.co/dbmdz/bert-base-turkish-cased)

---

## 🗃️ Dataset

The dataset was loaded from an Excel file containing Turkish tweets preprocessed with Zemberek.

| Column         | Description            |
|----------------|------------------------|
| `Tweet_Zemberek` | Preprocessed tweet text |
| `Label`        | 0 (non-hate) or 1 (hate) |

---

## 🧪 Model Pipeline

1. **Tokenization** with BERT tokenizer
2. **Dataset split**: 80% training, 20% validation
3. **Custom PyTorch Dataset** for loading tweet-label pairs
4. **Training Loop** with AdamW optimizer and GPU acceleration
5. **Evaluation**: Confusion matrix & classification report

---

## 🔬 Example Results

### Confusion Matrix  
📊 Model performance visualized using Seaborn heatmaps

### Classification Report
Includes:
- Precision
- Recall
- F1-score
- Accuracy

---

## 🚀 How to Run

1. Install dependencies:
```bash
pip install torch transformers scikit-learn pandas matplotlib seaborn openpyxl tqdm
```

2. Load your `.xlsx` dataset under the expected format
3. Run the notebook

---

## 🛠 Tech Stack

- Python 🐍
- PyTorch ⚡
- Huggingface Transformers 🤗
- Matplotlib & Seaborn 📊
- Jupyter Notebook 📒

---

## 🙋‍♂️ Contributors

Made with ❤️ by [Your Name](https://github.com/yourusername)

---

## 📄 License

MIT License
