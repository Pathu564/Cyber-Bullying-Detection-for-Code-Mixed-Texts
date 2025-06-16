# 🛡️ Cyber-Bullying Detection for Code-Mixed Texts  
A machine learning project for detecting **cyber-bullying / hate speech** in **code-mixed texts** using a multimodal approach (text + emojis).

---

## 📌 Description  
This project leverages Natural Language Processing (NLP) and Deep Learning to classify **code-mixed sentences** (like Hinglish, Tanglish) as either **bullying** or **non-bullying**, by analyzing both:

- 📝 Text content using MuRIL + DConvBiLSTM  
- 😊 Emojis using emoji2vec + Ensemble Classifier  

---

## 🚀 Features

- Detects bullying in **mixed-language** social media content  
- Processes and analyzes **emojis** separately from text  
- Uses a **dual-model fusion** for improved accuracy  
- Clean **interactive interface** using `ipywidgets` in Google Colab  
- Confidence scores displayed for **each model** used  

---

## 🧠 Models Used

| Component        | Model Used                      |
|------------------|----------------------------------|
| Text Embedding   | Google MuRIL (BERT-based)        |
| Text Classifier  | Custom DConvBiLSTM               |
| Emoji Embedding  | emoji2vec (pretrained)           |
| Emoji Classifier | Ensemble (Random Forest, etc.)   |

---

## 📁 Files Needed (Upload to Google Drive)

```
/MyDrive/bully_detection/
│
├── dconvbilstm_bully_model.pth           # Trained text classification model
├── emoji_ensemble_model_fixed.pkl        # Trained emoji ensemble model
└── emoji2vec.bin                         # Pretrained emoji embeddings
```

---

## ▶️ How to Run

1. **Launch the notebook** in Google Colab.  
2. **Connect to Google Drive** to access the necessary model files.  
3. **Execute all cells** to initialize the interface.  
4. 💬 Enter a sentence (with or without emojis) and click **Predict** to see the results.

---

## 🔍 Sample Output

```
📝 Extracted Text: tu kya kar rha hai 🤔
😊 Extracted Emojis: 🤔
📝 Text Model Confidence (Bully): 64.12%
😊 Emoji Model Confidence (Bully): 50.43%
🧠 Final Prediction: Bully (Confidence: 57.27%)
```

---

## 🛠️ Tech Stack

- Python  
- PyTorch  
- Transformers (`transformers` by HuggingFace)  
- Gensim  
- emoji  
- ipywidgets  
- joblib  

---

## 📦 Installation (Optional - for local setup)

```bash
git clone https://github.com/Pathu564/Cyber-Bullying-Detection-for-Code-Mixed-Texts.git
cd Cyber-Bullying-Detection-for-Code-Mixed-Texts


```
## ✅ To-Do

- [ ] Add support for real-time deployment (e.g., Flask or Streamlit)  
- [ ] Improve model performance with larger dataset  
- [ ] Add Hindi transliteration module for code-mixed parsing  

---

## 📜 License

This project is for educational and research purposes. Pretrained models like MuRIL and emoji2vec retain their original licenses.
```
