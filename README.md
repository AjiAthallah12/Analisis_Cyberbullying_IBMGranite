# 🧠 Cyberbullying Classification and Summarization with IBM Granite  

Analisis data tweet terkait *cyberbullying* menggunakan model **IBM Granite** melalui pendekatan **Data Classification** dan **Data Summarization**.  
Proyek ini bertujuan untuk mengidentifikasi pola, tren, serta klasifikasi teks yang berkaitan dengan perilaku *cyberbullying* di media sosial menggunakan *Large Language Model (LLM)* IBM Granite.  

---

## 📊 Project Overview  
Proyek ini merupakan implementasi *machine learning pipeline* untuk mengolah data teks mentah dari Twitter.  
Langkah-langkah utama yang dilakukan meliputi:  
1. **Data Preparation** — membaca, membersihkan, dan menormalkan data mentah dalam format `.csv`.  
2. **Data Classification** — mengidentifikasi jenis dan kategori *cyberbullying* pada setiap tweet menggunakan model **IBM Granite**.  
3. **Data Summarization** — menghasilkan ringkasan konteks umum dari kumpulan tweet terkait isu *cyberbullying*.  
4. **Visualization** — menampilkan hasil analisis dalam bentuk grafik dan tabel untuk memperlihatkan distribusi dan tren *cyberbullying*.  

---

## 🧾 Raw Dataset Submission  
**Dataset:** Cyberbullying Tweets Dataset  
**Source:** Dataset publik untuk analisis teks terkait cyberbullying  
**Format:** `.csv`  
**Purpose:** Analisis klasifikasi dan peringkasan data teks *cyberbullying* menggunakan IBM Granite  

**Raw Dataset Link:**  
🔗 [CBTweets.csv (GitHub RAW)](https://github.com/AjiAthallah12/Analisis_Stunting_IBMGranite/raw/refs/heads/main/CBTweets.csv)

---

## 📊 Insight & Findings
Analisis dilakukan setelah proses klasifikasi dengan IBM Granite menghasilkan label utama:
- **Cyberbullying**
- **Sensitive / Aggressive**
- **Non-Cyberbullying**

Beberapa temuan utama:
- Kategori **Cyberbullying** mendominasi sekitar _x%_ dari total data.
- Tweet yang tergolong **Sensitive** memiliki rata-rata panjang teks lebih tinggi daripada kategori lain.
- Kata-kata umum yang muncul pada kategori **Cyberbullying** mencerminkan ekspresi negatif dan ejekan.
- Distribusi panjang teks menunjukkan variasi signifikan antara kategori.

Visualisasi yang dihasilkan:
- Distribusi kategori (bar chart)  
- Panjang teks per kategori (boxplot)  
- WordCloud kata dominan per kategori  

Contoh grafik dan hasil analisis dapat dilihat di notebook `DataSummarization.ipynb`.

---

## 🤖 AI Support Explanation
Analisis ini menggunakan **model IBM Granite** melalui layanan **Replicate API**, yang mendukung *text classification* dan *summarization*.  
Peran AI di proyek ini mencakup:
- **Klasifikasi teks otomatis:** model IBM Granite mendeteksi pola kalimat dan mengelompokkan tweet berdasarkan konteks.
- **Summarization dan interpretasi hasil:** LLM membantu merangkum hasil klasifikasi menjadi insight deskriptif.
- **Pipeline otomatis:** kode Python mengelola batch request untuk mematuhi batasan rate limit pada versi free-tier Replicate API (maks. 6 request/menit).

Dengan bantuan IBM Granite, proses analisis menjadi **lebih cepat, konsisten, dan skalabel**, meskipun dataset mencapai ribuan baris.

---
