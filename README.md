# Manpower Recommendation AI for Cleaning Teams

---

## Ringkasan Proyek

Proyek ini adalah **Final Project** dari **Purwadhika Data Science Bootcamp** yang bertujuan untuk mengembangkan sistem rekomendasi berbasis **kecerdasan buatan (AI)**. Sistem ini dirancang untuk **memprediksi dan merekomendasikan kebutuhan jumlah *manpower* tim *cleaning service*** pada fasilitas properti (gedung perkantoran, pusat perbelanjaan, apartemen, dll.) secara optimal.

Manajemen *cleaning service* sering menghadapi tantangan dalam menentukan jumlah staf yang tepat untuk memastikan kebersihan optimal tanpa pemborosan sumber daya. Sistem ini hadir untuk mengatasi masalah tersebut dengan menganalisis berbagai faktor dan memberikan rekomendasi yang akurat, sehingga membantu operasional menjadi lebih efisien dan efektif.

## Fitur Utama

* **Prediksi *Manpower***: Memprediksi jumlah *manpower* yang dibutuhkan berdasarkan parameter input.
* **Analisis Faktor**: Mengidentifikasi dan menganalisis faktor-faktor kunci yang memengaruhi kebutuhan *manpower* (misalnya, luas area, jenis fasilitas, frekuensi pembersihan, tingkat kunjungan, dll.).
* **Rekomendasi Optimal**: Memberikan rekomendasi jumlah *manpower* yang efisien dan efektif.
* **Antarmuka Pengguna (Opsional)**: Jika ada, jelaskan singkat antarmuka yang dibuat (misalnya, Streamlit, Flask Web App).

## Tujuan Proyek

* Mengimplementasikan pengetahuan Data Science yang diperoleh selama bootcamp.
* Membangun model AI yang robust dan akurat untuk kasus nyata.
* Memberikan solusi inovatif untuk masalah manajemen *cleaning service* di fasilitas properti.
* Meningkatkan efisiensi operasional dan kualitas kebersihan.

## Teknologi yang Digunakan

* **Bahasa Pemrograman**: Python
* **Library Utama**:
    * `pandas` (Manipulasi Data)
    * `numpy` (Komputasi Numerik)
    * `scikit-learn` (Model Machine Learning: Regresi, Klasifikasi, dll.)
    * `matplotlib` & `seaborn` (Visualisasi Data)
    * `streamlit` / `flask` (Jika ada *web app* sebagai antarmuka)
    * (Tambahkan library lain yang kamu gunakan, seperti `xgboost`, `lightgbm`, `tensorflow`, `pytorch` jika relevan)
* **Lingkungan Pengembangan**: Jupyter Notebook, VS Code
* **Manajemen Paket**: `pip`

## Struktur Proyek
.
├── data/
│   ├── raw_data.csv        # Data mentah
│   └── processed_data.csv  # Data yang sudah dibersihkan/diproses
├── notebooks/
│   ├── 01_data_exploration.ipynb
│   ├── 02_feature_engineering.ipynb
│   ├── 03_model_training.ipynb
│   └── 04_model_evaluation.ipynb
├── src/
│   ├── data_preprocessing.py   # Skrip untuk preprocessing data
│   ├── model_training.py       # Skrip untuk melatih model
│   └── prediction.py           # Skrip untuk melakukan prediksi
├── models/
│   └── best_model.pkl          # Model yang sudah dilatih dan disimpan
├── app/ (Opsional, jika ada Streamlit/Flask app)
│   └── app.py                  # Skrip utama aplikasi web
├── README.md                   # File ini
├── requirements.txt            # Daftar dependensi proyek
└── LICENSE                     # Lisensi proyek (opsional)

.
## Instalasi dan Penggunaan

Ikuti langkah-langkah berikut untuk menjalankan proyek ini di lingkungan lokal Anda:

1.  **Clone Repositori:**
    ```bash
    git clone [https://github.com/namamu/nama-repo-kamu.git](https://github.com/namamu/nama-repo-kamu.git)
    cd nama-repo-kamu
    ```

2.  **Buat Virtual Environment (Disarankan):**
    ```bash
    python -m venv venv
    source venv/bin/activate  # Linux/macOS
    # atau
    .\venv\Scripts\activate   # Windows
    ```

3.  **Instal Dependensi:**
    ```bash
    pip install -r requirements.txt
    ```

4.  **Menjalankan Notebook (untuk Eksplorasi/Pengembangan):**
    ```bash
    jupyter notebook
    ```
    Buka file `.ipynb` di folder `notebooks/` untuk melihat alur kerja proyek.

5.  **Menjalankan Aplikasi (Jika Ada):**
    Jika ada aplikasi Streamlit:
    ```bash
    streamlit run app/app.py
    ```
    Jika ada aplikasi Flask:
    ```bash
    python app/app.py
    ```

## Data

Dataset yang digunakan untuk proyek ini (jelaskan secara singkat sumber data atau jenis data yang digunakan, misalnya data operasional historis, data luas area, dll.). Data ini disimpan di direktori `data/`.

## Metodologi

* **Pengumpulan Data**: Jelaskan bagaimana data dikumpulkan atau disimulasikan.
* **Data Preprocessing**: Langkah-langkah pembersihan data, penanganan *missing values*, *outliers*, dan *encoding* kategori.
* **Eksplorasi Data (EDA)**: Analisis statistik dan visualisasi untuk memahami pola dan hubungan dalam data.
* **Feature Engineering**: Pembuatan fitur-fitur baru dari data yang ada untuk meningkatkan kinerja model.
* **Pemilihan Model**: Pemilihan algoritma *machine learning* yang sesuai (misalnya, Regresi Linear, Random Forest Regressor, Gradient Boosting, dll.).
* **Pelatihan dan Evaluasi Model**: Melatih model dengan data latih dan mengevaluasi kinerja menggunakan metrik yang relevan (misalnya, MAE, MSE, R2-score untuk regresi).
* **Hyperparameter Tuning**: Optimalisasi parameter model untuk mendapatkan performa terbaik.

## Hasil dan Analisis

* Sebutkan performa model terbaik yang dicapai (misalnya, "Model terbaik mencapai R2-score sebesar X% pada data uji").
* Diskusikan *feature importance* jika relevan (fitur apa yang paling memengaruhi rekomendasi *manpower*).
* Jelaskan implikasi hasil dan bagaimana sistem ini dapat membantu manajemen fasilitas.

## Tantangan dan Pembelajaran

* Sebutkan beberapa tantangan yang dihadapi selama proyek (misalnya, kualitas data, pemilihan model yang kompleks, *deployment*).
* Apa saja pelajaran penting yang didapat dari proses ini?

## Pengembangan Selanjutnya (Future Work)

* Integrasi dengan sistem manajemen properti yang ada.
* Penambahan fitur *real-time monitoring* dan penyesuaian rekomendasi.
* Eksplorasi model yang lebih kompleks (misalnya, *time-series forecasting* jika data memiliki aspek waktu yang kuat).
* Penyempurnaan UI/UX aplikasi (jika ada).
* Validasi model dengan data operasional riil yang lebih besar.

## Kontributor

* **Nama Lengkap Anda** - [LinkedIn Anda](link-linkedin-anda) | [GitHub Anda](link-github-anda)

## Lisensi

Proyek ini dilisensikan di bawah [Nama Lisensi, contoh: MIT License]. Lihat file `LICENSE` untuk detail lebih lanjut.

---

Terima kasih telah melihat proyek saya! Jangan ragu untuk memberikan *feedback* atau pertanyaan.
