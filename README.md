# UTS-ML-Deep-Learning-Athaya
Proyek UTS Machine Learning &amp; Deep Learning
**Nama:** [Athaya Naufal Pranastya]  
**NIM:** [1202220001]  
**Repositori:** [https://github.com/athayanaufal/UTS-ML-Deep-Learning-Athaya.git]

## 📌 Deskripsi Proyek
Proyek ini merupakan implementasi tugas UTS untuk mata kuliah Machine Learning & Deep Learning. Fokus utama penelitian ini adalah melakukan studi komparatif antara algoritma **Machine Learning Konvensional** dan **Deep Learning** pada tiga domain data yang berbeda: Tabular, Image (Gambar), dan Text (Teks).

Tujuan dari proyek ini adalah untuk menganalisis performa, efisiensi komputasi, dan kompleksitas dari kedua pendekatan tersebut di setiap kasus.

---

## 📂 Struktur Repositori
```text
├── Kasus_1_Tabular/
│   └── Kasus1.ipynb      # Klasifikasi Survival Titanic
├── Kasus_2_Image/
│   └── Kasus2.ipynb      # Pengenalan Angka Tulisan Tangan
├── Kasus_3_Text/
│   └── Kasus3.ipynb         # Analisis Sentimen Tweet Bencana
├── requirements.txt                      # Daftar pustaka (dependencies)
└── README.md                             # Panduan proyek

🛠️ Ringkasan Metodologi
Kasus 1: Tabular (Titanic)
Baseline: Random Forest / XGBoost (Konvensional).

Deep Learning: Multi-Layer Perceptron (MLP).

Target: Prediksi keselamatan penumpang berdasarkan fitur demografis.

Kasus 2: Image (MNIST)
Baseline: HOG Feature Extraction + SVM (Konvensional).

Deep Learning: Deep Convolutional Neural Network (CNN).

Target: Klasifikasi angka 0-9 dari gambar 28x28 piksel.

Kasus 3: Text (Disaster Tweets)
Baseline: TF-IDF Vectorizer + Logistic Regression (Konvensional).

Deep Learning: Bidirectional Long Short-Term Memory (Bi-LSTM).

Target: Mendeteksi tweet yang menginformasikan bencana nyata vs non-bencana.

## Cara Menjalankan Notebook
Notebook ini menggunakan `kagglehub` untuk mengunduh dataset secara otomatis. 

### Persyaratan:
1. Pastikan library terinstall: `pip install -r requirements.txt`
2. **Kaggle API Credentials:**
   Untuk menjalankan proses download otomatis, Anda perlu memasukkan API Key Kaggle Anda pada cell pertama di setiap notebook:
   ```python
   import os
   os.environ['KAGGLE_USERNAME'] = "USERNAME_ANDA"
   os.environ['KAGGLE_KEY'] = "KEY_ANDA"