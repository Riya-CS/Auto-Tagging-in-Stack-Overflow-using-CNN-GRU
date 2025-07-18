# Auto-Tagging-in-Stack-Overflow-using-CNN-GRU
An intelligent hybrid deep learning system for automatically predicting relevant tags for Stack Overflow posts using NLP, CNN, and GRU. Achieves over 81% accuracy with top-10 tag predictions.

📚 Built during a research internship at PES University | 📽️ Includes demo video and research paper

## 📄 Abstract

Manually tagging questions on Stack Overflow can be inconsistent and time-consuming. This project proposes an automated system using a **hybrid Convolutional Neural Network (CNN) and Gated Recurrent Unit (GRU)** architecture to predict the most appropriate tags for a given question. The model enhances the tagging process by utilizing advanced NLP techniques to achieve improved accuracy and tagging consistency.

This research was conducted under the **CDSAML Summer Internship at PES University**, and the findings have been presented in our paper:

📘 *"Automating Tag Prediction in Stack Overflow Using Machine Learning and Deep Learning Techniques"*

## 🎬 Demo

A short video demo is included showing the model successfully predicting relevant tags for technical queries. The predicted tags appear within the **top 10**, demonstrating the system’s robustness and practical effectiveness.



https://github.com/user-attachments/assets/9000a5fb-37e2-43b8-bcdd-c5b2554503bd


## 🧱 Model Architecture

- **Embedding Layer** – Word embeddings to capture semantic meaning.
- **CNN Layers** – Extract local textual features and n-gram patterns.
- **GRU Layers** – Model long-term dependencies across sequences.
- **Dense Layer (Sigmoid)** – Multi-label classification to output multiple tags.

The hybrid model balances spatial (CNN) and temporal (GRU) representations for effective tag prediction.

## 📊 Key Results

| Dataset Size | Accuracy (%) |
|--------------|--------------|
| 10K Samples  | 70.80%       |
| 150K Samples | 81.03%       |

✅ Tags are correctly predicted **within top 10 suggestions** for real user queries.

## 📦 Project Content
├── auto-tagging-in-stack-overflow-using-cnn-gru.ipynb # Kaggle-compatible notebook
├── demo.mp4 # Tag prediction demo video
└── README.md

## ⚙️ How to Run (Kaggle Instructions)

> This project runs fully on **Kaggle** using GPU support.

1. Upload the `auto-tagging-in-stack-overflow-using-cnn-gru.ipynb` to [Kaggle Notebooks](https://www.kaggle.com/code).
2. Enable GPU.
3. Run all cells. (Data is loaded and preprocessed within the notebook.)

📌 *Note: The datasets are from Kaggle and Hugging Face but are not bundled due to licensing restrictions.*

## 📚 Paper Highlights

- Compared classical ML models (Naive Bayes, SVM, Random Forest, KNN) with DL models (LSTM, CNN, GRU, BERT).
- Achieved superior performance using **CNN + GRU hybrid model**.
- Top 10 tags focus due to high frequency and coverage.
- Multi-label binarization used for tag encoding.

## 💡 Future Work

- Expand beyond top 10 tags for richer prediction.
- Explore attention mechanisms and transformer-based models (e.g., BERT+CNN).
- Integrate real-time API or web UI for live tag suggestion.

## 🧠 Authors & Contributors

- **Riya C. Sapkale**
- Pranav Acharya
- Shreya M. Hegde
- Shreya Kiran
- Ashwini M. Joshi

PES University, Bangalore, India  
📬 riyacsapkale@gmail.com

## 🏫 Acknowledgements

This research was conducted at the **Centre for Data Sciences & Applied Machine Learning (CDSAML), PES University** under the guidance of **Dr. Shylaja S S**. We thank the faculty and research mentors for their support and infrastructure.

## 📜 Citation

```bibtex
@inproceedings{stacko-autotagging-2025,
  title={Automating Tag Prediction in Stack Overflow Using Machine Learning and Deep Learning Techniques},
  author={Sapkale, Riya C and Acharya, Pranav and Hegde, Shreya M and Kiran, Shreya and Joshi, Ashwini M},
  year={2025},
  institution={PES University},
  journal={ICTIS 2025}
}
```
