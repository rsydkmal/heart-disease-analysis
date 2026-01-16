# Heart Disease Exploratory Data Analysis (EDA)

## 📌 Project Overview
Project ini bertujuan untuk melakukan **Exploratory Data Analysis (EDA)** pada dataset *Heart Disease Prediction* guna memahami karakteristik data, pola distribusi variabel, serta hubungan antara fitur-fitur medis dengan kondisi penyakit jantung.  
Hasil EDA ini digunakan sebagai fondasi sebelum masuk ke tahap preprocessing dan pemodelan prediktif.

---

## 📂 Dataset
- **Nama file:** `Heart_Disease_Prediction.csv`
- **Jumlah data:** 270 observasi
- **Jumlah fitur:** 14 kolom
- **Target variable:** `Heart Disease` (Presence / Absence)

Dataset berisi informasi medis pasien seperti usia, tekanan darah, kolesterol, denyut jantung maksimum, hasil EKG, serta indikator klinis lainnya yang relevan dengan risiko penyakit jantung.

---

## 🧪 Tahapan Analisis
Analisis dilakukan secara bertahap untuk memastikan pemahaman data yang komprehensif:

1. **Import library dan load dataset**
2. **Pemeriksaan struktur data**
   - Jumlah baris dan kolom
   - Tipe data setiap variabel
   - Pemeriksaan missing values
3. **Statistik deskriptif**
   - Rata-rata, median, nilai minimum dan maksimum
4. **Analisis distribusi variabel numerik**
   - Age  
   - Blood Pressure (BP)  
   - Cholesterol  
   - Max Heart Rate  
   - ST depression  
5. **Analisis distribusi variabel kategorikal**
   - Sex  
   - Chest pain type  
   - Exercise angina  
   - Heart Disease  
6. **Analisis hubungan variabel numerik dengan penyakit jantung**
   - Menggunakan boxplot untuk membandingkan distribusi antar kelas target

---

## 📊 Insight Utama dari EDA

### 1. Kualitas Data
- Tidak ditemukan missing value pada seluruh dataset
- Data siap digunakan untuk analisis lanjutan tanpa imputasi awal

### 2. Distribusi Variabel Numerik
- **Age** menunjukkan distribusi mendekati normal dengan konsentrasi usia 50–60 tahun
- **Cholesterol** memiliki distribusi right-skewed dengan beberapa nilai ekstrem di atas 400
- **Max Heart Rate** cenderung lebih rendah pada pasien dengan penyakit jantung
- **ST depression** menunjukkan perbedaan yang cukup jelas antara pasien dengan dan tanpa penyakit jantung

Outlier **tidak dihapus pada tahap EDA** karena dalam konteks medis, nilai ekstrem dapat merepresentasikan kondisi klinis nyata, bukan kesalahan pencatatan.

### 3. Distribusi Variabel Kategorikal
- Pasien laki-laki mendominasi dataset
- Beberapa tipe nyeri dada memiliki frekuensi lebih tinggi dan berpotensi berkaitan dengan penyakit jantung
- Distribusi target *Heart Disease* relatif seimbang, sehingga dataset cukup baik untuk pemodelan klasifikasi

### 4. Hubungan dengan Penyakit Jantung
Variabel **Age**, **Cholesterol**, **Max HR**, dan **ST depression** menunjukkan perbedaan distribusi yang cukup signifikan antara pasien dengan dan tanpa penyakit jantung, sehingga berpotensi menjadi fitur penting dalam model prediksi.

---

## 🧠 Kesimpulan
Exploratory Data Analysis menunjukkan bahwa dataset memiliki kualitas yang baik dan mengandung sinyal kuat terkait faktor risiko penyakit jantung.  
Hasil EDA ini menjadi dasar yang solid untuk tahap selanjutnya seperti preprocessing data dan pembangunan model machine learning.

---

## 🛠️ Tools & Library
- Python
- Pandas
- Matplotlib
- Seaborn
- Jupyter Notebook (VS Code)

---

## 📌 Next Step
- Feature engineering
- Scaling dan encoding
- Model building dan evaluasi