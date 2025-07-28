🇬🇧 English-to-French Translation using Seq2Seq Models

This project presents two neural machine translation models for English-to-French translation using Sequence-to-Sequence (Seq2Seq) architectures in TensorFlow and Keras.

🗂 Project Files

eng-fra-seq2seq-basic-v1.ipynb

A fully working encoder-decoder model with:

Word embeddings and LSTM layers

Teacher forcing during training

Evaluation using BLEU scores

Training accuracy/loss curves

Sample translations for qualitative inspection


fra-seq2seq-basic-with-attention-v2.ipynb

An experimental attention-based extension featuring:

Additive Attention mechanism

Stable training with improved accuracy

Training curves 

Incomplete inference logic — still under development



---

✅ Basic Seq2Seq Model (Stable)

📌 Highlights

Encoder-decoder using LSTM

Embedding layers for source and target sequences

Teacher forcing applied during training

Evaluation using BLEU scores and manual inspection


📊 Results

Final Training Accuracy: ~35%

BLEU Score: Measured on 100 test samples

Training Curves: Accuracy and loss plotted over epochs (see notebook)



---

⚠ Attention Model (Experimental)

📌 Additions

Adds Additive Attention to focus on relevant encoder outputs



📈 Status

Training Accuracy: ~89%

Inference: Still unstable; predictions may be repetitive or semantically incorrect



---

📚 Dataset

File: fra.txt

Source:(https://www.manythings.org/anki/fra-eng.zip)

Used: Top 10,000 English–French sentence pairs



---

🧪 Evaluation

Metric: BLEU Score via nltk.translate.bleu_score

Qualitative Analysis: Sample predictions reviewed manually

Visualizations:

Training accuracy/loss plots





---

🧰 Requirements

Python 3.7+

TensorFlow 2.x

NumPy

Matplotlib

NLTK


🔧 Install Dependencies

pip install tensorflow numpy matplotlib nltk


---

🚀 How to Run

1. download fra.txt and place it in the working directory.


2. Open either notebook in Jupyter Notebook or convert them to Python scripts.


3. Run cells step by step. Use predict_sample() or predict_samples() to test your model’s translations.




---

🧠 Author Notes

The basic model is a strong reference for implementing Seq2Seq models.

The attention-based model is experimental, with better training performance but pending improvements for reliable inference.

All key visualizations (training curves, BLEU scores) are included in the notebooks.
