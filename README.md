# TIM Anomali SCP-03

## Deskripsi Project
Project ini merupakan solusi untuk kompetisi BDC Case 1 mengenai multiclass text classification terhadap tweet terkait Program Makan Bergizi Gratis (MBG). 

Model dibangun untuk mengklasifikasikan tweet ke dalam 8 kategori:
- Anggaran
- Kualitas Pangan
- Distribusi
- Ekonomi
- Tata Kelola
- Sasaran Penerima
- Politik
- Lainnya

Metode yang digunakan meliputi preprocessing teks, vectorization, pelatihan model machine learning, dan inferensi untuk menghasilkan prediksi pada data uji.

---

## Struktur File

### Notebook & Source Code
- `Case1_TIM Anomali SCP-03.ipynb`
  - Notebook utama yang berisi seluruh proses mulai dari preprocessing hingga prediksi.

- `case1_TIM Anomali SCP-03.py`
  - Versi Python script dari notebook.

---

## Dataset
Dataset yang digunakan berasal dari panitia kompetisi BDC Case 1.

File dataset:
- `case_1_labeled_data.xlsx`
- `case_1_text_to_predict.xlsx`
- `case_1_template_sheet.xlsx`

Dataset tidak disertakan di repository untuk menjaga ketentuan kompetisi.

---

## Tahapan Pengerjaan

### 1. Data Loading
Membaca dataset training dan testing dari file `.xlsx`.

### 2. Preprocessing
Tahapan preprocessing meliputi:
- Case folding
- Cleaning text
- Remove punctuation
- Remove URL
- Remove mention/hashtag
- Tokenization
- Stopword removal
- Stemming

### 3. Feature Extraction
Mengubah data teks menjadi representasi numerik menggunakan teknik vectorization.

### 4. Model Training
Melakukan pelatihan model klasifikasi multiclass menggunakan data training.

### 5. Evaluation
Evaluasi model menggunakan metrik:
- Balanced Accuracy

### 6. Prediction
Model digunakan untuk memprediksi label pada data testing.

### 7. Export Submission
Hasil prediksi disimpan dalam format `.xlsx` sesuai template yang diberikan panitia.

---

## Cara Menjalankan Project

### 1. Install Dependencies
```bash
pip install -r requirements.txt
