### Milestone 2: Credit Risk Scoring Analysis & Prediction

## Repository Outline
1. P1M2_gugun_gunawan.ipynb: Notebook utama yang berisi proses End-to-End Machine Learning mulai dari EDA, Preprocessing, Cross Validation, hingga Hyperparameter Tuning.

2. P1M2_gugun_gunawan_inf.ipynb: Notebook khusus untuk melakukan Inference (pengujian model dengan data baru).

3. P1M2_gugun_gunawan_conceptual.txt: File teks yang berisi jawaban atas pertanyaan konsep (Bagging, Random Forest vs Boosting, Cross Validation).

4. best_rf_credit_model.pkl: Model Random Forest terbaik yang sudah di-save (disimpan di Google Drive karena ukuran file).

5. deployment: Folder yang berisi source code untuk aplikasi web berbasis Streamlit.

6. url.txt: Berisi link dataset, link model di Google Drive, dan link aplikasi deployment.

## Problem Background
Industri keuangan menghadapi risiko kerugian besar akibat nasabah yang gagal bayar (default). Proses penilaian kredit secara manual seringkali memakan waktu lama, subjektif, dan sulit untuk dikembangkan secara skala besar. Proyek ini bertujuan untuk mendigitalisasi dan mengotomatisasi proses credit scoring menggunakan algoritma Machine Learning agar keputusan pemberian pinjaman menjadi lebih cepat, objektif, dan akurat berdasarkan data historis nasabah.
## Project Output
Machine Learning Model: Model klasifikasi yang mampu memprediksi probabilitas gagal bayar nasabah.

Web Application: Dashboard interaktif berbasis Streamlit yang memungkinkan Credit Analyst memasukkan data calon nasabah dan mendapatkan hasil prediksi (ACC/Reject) secara instan.
## Data
* Sumber Data: Credit Risk Dataset - Kaggle.

* Karakteristik Data:

* Terdiri dari 32,581 baris data sebelum dibersihkan.

* Memiliki 12 kolom fitur (campuran numerik dan kategorikal).

* Missing Values: Ditemukan pada kolom loan_int_rate (suku bunga) dan person_emp_length.

* Target: loan_status (0: Lancar, 1: Gagal Bayar).
## Method
Proyek ini menggunakan metode Supervised Learning (Classification). Langkah-langkah teknis yang dilakukan meliputi:

* Exploratory Data Analysis (EDA) untuk menemukan pola risiko.

* Preprocessing Pipeline menggunakan ColumnTransformer (Imputation, Scaling, dan Encoding).

* Model Comparison: Membandingkan 5 algoritma (KNN, SVM, Decision Tree, Random Forest, dan AdaBoost) menggunakan Cross Validation.

* Model Improvement: Melakukan Hyperparameter Tuning dengan GridSearchCV pada model terbaik.

## Stacks
* Bahasa Pemrograman: Python 3.x

* Data Manipulation: Pandas, NumPy 1.26.4, plotly 5.9.0

* Visualization: Matplotlib 3.7.0, Seaborn .12.2

* Machine Learning: Scikit-Learn 1.6.1

* Model Export: Joblib

* Deployment: Streamlit 1.54.0, HuggingFace/Render

## Reference
* Dataset: [Kaggle Credit Risk Dataset](https://www.kaggle.com/datasets/laotse/credit-risk-dataset)

* Deployment URL: https://huggingface.co/spaces/gun1205/credit-risk-prediction-gunawan
* Model Link: https://drive.google.com/file/d/1LB928tQDFN-2DSMQz_jo_7BQxBi9oyRA/view?usp=drive_link

---

**Referensi tambahan:**
- [Basic Writing and Syntax on Markdown](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)
- [Contoh readme](https://github.com/fahmimnalfrzki/Swift-XRT-Automation)
- [Another example](https://github.com/sanggusti/final_bangkit) (**Must read**)
- [Additional reference](https://www.freecodecamp.org/news/how-to-write-a-good-readme-file/)