# 🎯 Analisis Sentimen Big Data Ulasan Skintific Official Store (Tokopedia)
# 📖 Overview
Proyek ini merupakan Tugas Akhir yang berfokus pada analisis Big Data ulasan konsumen untuk 10 produk utama dari Skintific Official Store di platform e-commerce Tokopedia. Tujuannya adalah untuk mengukur tingkat kepuasan pelanggan secara kuantitatif melalui klasifikasi sentimen (Positif, Negatif, Netral) menggunakan pendekatan Machine Learning (ML) dan Natural Language Processing (NLP).
# 🛠️ Metodologi (Teknis)
Proses pemodelan sentimen dilakukan melalui serangkaian tahapan teknis utama:
1. Pengumpulan Data: Menggunakan teknik Web Scraping/Web Crawling untuk mengumpulkan ulasan, rating, dan detail produk.
2. Preprocessing Data: Pembersihan teks yang komprehensif, termasuk normalisasi teks, stopword removal (menggunakan list Bahasa Indonesia), dan Stemming (menggunakan Pustaka Sastrawi).
3. Pelabelan Sentimen Otomatis: Ulasan diterjemahkan dan dilabeli menggunakan pustaka TextBlob berdasarkan polaritas teks (polarity > 0, polarity < 0, polarity = 0).
4. Ekstraksi Fitur: Representasi teks menjadi fitur numerik menggunakan metode Term Frequency-Inverse Document Frequency (TF-IDF).
5. Pemodelan ML: Melatih model klasifikasi Multinomial Naive Bayes pada dataset yang dibagi dengan rasio 80% (Data Latih) : 20% (Data Uji).
6. Pustaka Kunci: Pandas, NumPy, Scikit-learn, TextBlob, Sastrawi.
# 📈 Hasil (Kuantitas)
Setelah pelatihan dan evaluasi, model sentimen memberikan hasil sebagai berikut:

Metrik|Nilai
* Jumlah Total Ulasan Dikerjakan|5147
* Akurasi Model Naive Bayes|79.86%
* Dominasi Sentimen Positif|75.6% dari total ulasan.
* Kata Kunci Positif Dominan|"cocok", "kulit", "bagus", "cepat".
* F1-Score (Kelas Positif)|0.93 (menunjukkan performa yang kuat dalam identifikasi Positif).

