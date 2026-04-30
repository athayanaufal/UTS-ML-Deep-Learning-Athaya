# 🎓 UTS Machine Learning & Deep Learning 2025/2026

Repositori ini berisi pengerjaan proyek Ujian Tengah Semester (UTS) untuk mengevaluasi dan membandingkan performa antara metode **Machine Learning Konvensional** dan **Deep Learning**.

---

## 👤 Profil Mahasiswa

- **Nama:** Athaya Naufal Pranastya
- **NIM:** 1202220001
- **Repositori:** [UTS-ML-Deep-Learning-Athaya](https://github.com/athayanaufal/UTS-ML-Deep-Learning-Athaya.git)

---

## 📌 Deskripsi Proyek

Proyek ini melakukan studi komparatif pada tiga domain data yang berbeda (Tabular, Image, dan Text). Fokus utama adalah menganalisis:

1.  **Performa:** Akurasi dan F1-Score pada setiap model.
2.  **Efisiensi:** Waktu training dan penggunaan sumber daya.
3.  **Kompleksitas:** Perbandingan antara _Feature Engineering_ manual vs otomatis.

---

## 📊 Metodologi Komparatif

| Domain Data | Dataset         | ML Konvensional (Baseline)   | Deep Learning (Bonus/Advanced)          |
| :---------- | :-------------- | :--------------------------- | :-------------------------------------- |
| **Tabular** | Titanic         | Random Forest / XGBoost      | Multi-Layer Perceptron (MLP)            |
| **Image**   | MNIST           | HOG Feature Extraction + SVM | Deep Convolutional Neural Network (CNN) |
| **Text**    | Disaster Tweets | TF-IDF + Logistic Regression | Bidirectional LSTM (Bi-LSTM)            |

---

## 📂 Struktur Repositori

Organisasi file dalam repositori ini dirancang agar mudah diperiksa oleh penguji:

```text
├── Kasus_1_Tabular/
│   └── Kasus1.ipynb          # Prediksi Survival Penumpang Titanic
├── Kasus_2_Image/
│   └── Kasus2.ipynb          # Klasifikasi Digit Tulisan Tangan
├── Kasus_3_Text/
│   └── Kasus3.ipynb          # Deteksi Berita Bencana via Tweet
├── requirements.txt          # Daftar dependencies library Python
└── README.md                 # Panduan dan dokumentasi utama
## 📥 Pengambilan Data (Data Acquisition)

Seluruh dataset dalam proyek ini ditarik secara otomatis menggunakan **Kaggle API**. Hal ini dilakukan untuk memastikan integritas data dan kemudahan reproduksi (reproducibility).

### Daftar Dataset yang Digunakan:
1. **Kasus 1:** [Titanic - Machine Learning from Disaster](https://www.kaggle.com/c/titanic)
2. **Kasus 2:** [Digit Recognizer (MNIST)](https://www.kaggle.com/c/digit-recognizer)
3. **Kasus 3:** [NLP with Disaster Tweets](https://www.kaggle.com/c/nlp-getting-started)

### Prosedur Otomatisasi:
Dataset diunduh menggunakan library `kagglehub`. Jika Anda menjalankan notebook untuk pertama kali, library ini akan mendownload file `.csv` yang diperlukan ke dalam folder cache lokal atau path yang ditentukan secara dinamis.
```
### 2. Konfigurasi Kredensial Kaggle
Agar fungsi `kagglehub` dapat mengakses kompetisi di Kaggle, Anda wajib menyetujui "Rules" di setiap halaman kompetisi terlebih dahulu. Kemudian, masukkan API Key Anda pada blok kode berikut di awal notebook:
```python
import os
os.environ['KAGGLE_USERNAME'] = "isi_username_anda"
os.environ['KAGGLE_KEY'] = "isi_key_api_anda"