# 📝 Sentiment Analysis on Instagram Comments

Proyek ini bertujuan untuk melakukan **analisis sentimen** pada komentar Instagram terkait kebijakan Presiden Joko Widodo. Dataset dikumpulkan secara mandiri melalui web scraping dengan **Data Miner**, kemudian dianalisis menggunakan pendekatan **machine learning (SVM)** dan **lexicon-based**.

---

## ⚙️ Tahapan Proyek
1. **Data Collection**
   - Data komentar Instagram diperoleh dengan tools **Data Miner**.  
   - Komentar difokuskan pada postingan terkait **Peraturan Presiden No. 75 Tahun 2024**.  

2. **Preprocessing**
   - Case folding
   - Normalisasi  
   - Removal (punctuation, angka, URL, emoji, mention, hashtag, stopwords)  
   - Tokenisasi  
   - Stemming

3. **Feature Extraction**
   - **TF-IDF** digunakan untuk representasi teks numerik.  

4. **Sentiment Analysis Approaches**
   - **Lexicon-Based** (dengan kamus sentimen Bahasa Indonesia)  
   - **Support Vector Machine (SVM)** dengan empat kernel:  
     - Linear  
     - Polynomial  
     - RBF (Radial Basis Function)  
     - Sigmoid  

---

## 📊 Evaluasi
Model dievaluasi menggunakan:  
- **Accuracy**  
- **Precision, Recall, F1-score**  
- **Confusion Matrix**

### 📌 Hasil Perbandingan Akurasi SVM Kernel
| Kernel      | Akurasi |
|-------------|---------|
| Linear      | 84%     |
| Polynomial  | 82%     |
| RBF         | 83%     |
| Sigmoid     | 79%     |

---

## ☁️ Wordcloud Sentimen

Berikut visualisasi Wordcloud Negatif berdasarkan hasil preprocessing dan pelabelan sentimen:

  ![Wordcloud Negatif](images/wordcloud.png)
