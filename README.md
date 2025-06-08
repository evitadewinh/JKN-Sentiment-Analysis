# Analisis Sentimen Berbasis Aspek Ulasan Mobile JKN  
## Membandingkan Kinerja Algoritma SVM dan Naive Bayes

Aplikasi **Mobile JKN** dari **BPJS Kesehatan** telah menjadi sarana penting bagi masyarakat Indonesia dalam mengakses layanan kesehatan. Meskipun penggunaannya luas, masih terdapat banyak ulasan negatif dari pengguna yang menunjukkan kendala teknis dan pengalaman yang kurang optimal. Oleh karena itu, proyek ini bertujuan untuk melakukan **Aspect-Based Sentiment Analysis (ABSA)** terhadap ulasan aplikasi Mobile JKN dan membandingkan kinerja dua algoritma machine learning: **Support Vector Machine (SVM)** dan **Naive Bayes (NB)**.

##  Tujuan Penelitian
- Menganalisis sentimen pengguna aplikasi Mobile JKN berdasarkan aspek tertentu.
- Membandingkan performa algoritma SVM dan Naive Bayes dalam klasifikasi sentimen.

##  Metodologi

### 🔹 Dataset
- **Jumlah data**: 10.752 ulasan dari Google Play Store
- **Format**: Teks mentah (berbahasa Indonesia)

### 🔹 Langkah-langkah Analisis
1. **Preprocessing Teks**  
   - Case Folding, Normalisasi, Stopword Removal, dan Stemming.
2. **Ekstraksi Aspek**  
   - Menggunakan **Count Vectorizer** untuk representasi fitur.
3. **Klasifikasi Sentimen**  
   - Menggunakan algoritma:
     - Support Vector Machine (SVM)
     - Naive Bayes (Multinomial)
4. **Evaluasi Model**  
   - Metrik: Accuracy, Precision, Recall, dan F1-Score  
   - Skema pembagian data: 10:90 hingga 90:10 (train:test)


## Hasil dan Temuan
Model Support Vector Machine (SVM) menghasilkan akurasi pengujian sebesar 93,91%, dengan jumlah prediksi benar sebanyak 2.020 dan prediksi salah sebanyak 131. Dari hasil cross-validation sebanyak 10 kali, akurasi model SVM bervariasi antara 92,24% hingga 94,14%, dengan rata-rata akurasi sebesar 93,21%. Meskipun performa SVM cukup baik dan stabil, hasil ini masih berada sedikit di bawah model Naive Bayes.

Sementara itu, model Naive Bayes menunjukkan performa yang lebih unggul dengan akurasi pengujian sebesar 95,03%, menghasilkan 2.044 prediksi benar dan hanya 107 prediksi salah. Akurasi dari hasil cross-validation berkisar antara 93,86% hingga 95,03%, dengan rata-rata akurasi sebesar 94,42%. Hal ini menunjukkan bahwa Naive Bayes memiliki kinerja yang lebih tinggi dan lebih konsisten dibandingkan SVM dalam mengklasifikasikan sentimen ulasan pengguna terhadap aplikasi Mobile JKN.

## Kesimpulan
Naive Bayes menunjukkan **kinerja terbaik** dalam klasifikasi sentimen ulasan aplikasi Mobile JKN, baik dari sisi akurasi maupun konsistensi. Temuan ini penting sebagai dasar untuk **evaluasi aplikasi** yang berorientasi pada **pengalaman pengguna**. Penelitian lanjutan disarankan menggunakan **data yang lebih seimbang** dan **algoritma lanjutan** seperti deep learning.

