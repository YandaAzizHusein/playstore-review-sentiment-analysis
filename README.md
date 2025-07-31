# Playstore Review Sentiment Analysis

Analisis sentimen pada ulasan pengguna di Google Play Store bertujuan untuk mengidentifikasi opini positif, negatif, atau netral terhadap aplikasi tertentu. Proyek ini memanfaatkan teknik *Natural Language Processing (NLP)* dan *machine learning* untuk membangun model klasifikasi yang dapat mengevaluasi persepsi pengguna secara otomatis.

---

## 🎯 Tujuan Proyek

- Mengekstrak dan membersihkan data review pengguna aplikasi di Google Play Store.
- Menganalisis distribusi sentimen pengguna (positif, netral, negatif).
- Membangun model klasifikasi berbasis teks untuk prediksi sentimen.
- Visualisasi hasil analisis secara interaktif dan informatif.

---

## 📊 Dataset

- **Sumber**: Google Play Store Reviews
- **Fitur**:
  - `Review`: teks ulasan pengguna
  - `Sentiment`: label target (Positive / Neutral / Negative)
  - `Translated_Review`: hasil translasi (opsional)
  - `App`, `Rating`, `Version`, dll

---

## 🔧 Teknologi yang Digunakan

- Python 3.x
- Pandas, NumPy
- NLTK, Sastrawi (tokenisasi dan stemming Bahasa Indonesia)
- scikit-learn (TF-IDF, Naive Bayes, Logistic Regression)
- Matplotlib, Seaborn, WordCloud
- Jupyter Notebook

---

## 🔍 Alur Analisis

1. **Preprocessing Teks**
   - Lowercase, remove stopwords, stemming
   - Tokenisasi menggunakan Sastrawi/regex
   - Bersihkan angka, simbol, emoji

2. **EDA (Exploratory Data Analysis)**
   - Distribusi sentimen
   - Kata populer per label (wordcloud)
   - Korelasi rating vs sentimen

3. **Ekstraksi Fitur**
   - TF-IDF Vectorizer
   - Unigram dan Bigram (opsional)

4. **Modeling**
   - Naive Bayes (Multinomial)
   - Logistic Regression
   - Support Vector Machine (SVM)
   - Evaluasi: akurasi, precision, recall, f1-score

5. **Visualisasi & Interpretasi**
   - Confusion Matrix
   - WordCloud positif/negatif
   - ROC Curve (opsional)

---

## 📈 Hasil Sementara

- **Model Terbaik**: Logistic Regression (akurasi ~86%)
- Naive Bayes bekerja baik untuk baseline ringan
- WordCloud menunjukkan fokus review pada fitur dan performa aplikasi

> *Catatan*: Angka akurasi & metrik evaluasi akan tergantung pada preprocessing dan pembagian data.

---

## 🗂️ Struktur Folder

```
playstore-review-sentiment-analysis/
├── data/                 # Dataset asli & hasil pembersihan
├── notebooks/            # EDA, Preprocessing, Modeling
├── model/                # Model yang disimpan (pickle/joblib)
├── visualization/        # Gambar hasil WordCloud & grafik
├── utils/                # Preprocessing & pipeline tools
├── README.md             # Dokumen ini
└── requirements.txt      # Library yang dibutuhkan
```

---

## 📦 Cara Menjalankan

```bash
# Setup environment
pip install -r requirements.txt

# Buka notebook
jupyter notebook notebooks/sentiment_analysis_playstore.ipynb
```

---

## 📎 Lisensi

Proyek ini untuk tujuan edukatif. Dataset berasal dari sumber publik.  
Lisensi kode: MIT

---

## 🙋 Kontributor

Yanda Aziz Husein  
[GitHub](https://github.com/YandaAzizHusein) · [LinkedIn](https://linkedin.com/in/...)  
