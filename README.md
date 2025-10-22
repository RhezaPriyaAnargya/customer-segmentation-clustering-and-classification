# Customer Segmentation Clustering 🎯

> **Analisis Segmentasi Pelanggan menggunakan Machine Learning untuk Optimalisasi Strategi Marketing**

[![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)](https://www.python.org/)
[![Pandas](https://img.shields.io/badge/Pandas-1.3+-green.svg)](https://pandas.pydata.org/)
[![Scikit-learn](https://img.shields.io/badge/Scikit--learn-1.0+-orange.svg)](https://scikit-learn.org/)
[![Matplotlib](https://img.shields.io/badge/Matplotlib-3.5+-red.svg)](https://matplotlib.org/)
[![Seaborn](https://img.shields.io/badge/Seaborn-0.11+-purple.svg)](https://seaborn.pydata.org/)

## 📋 Deskripsi Proyek

Proyek ini mengimplementasikan **Customer Segmentation** menggunakan teknik clustering untuk menganalisis perilaku pelanggan dan mengidentifikasi segmen pasar yang berbeda. Analisis ini membantu bisnis dalam merancang strategi marketing yang tepat sasaran dan meningkatkan customer experience.

### 🎯 Tujuan
- Mengidentifikasi pola perilaku pelanggan berdasarkan demografis dan spending behavior
- Membuat segmentasi pelanggan yang akurat menggunakan unsupervised learning
- Memberikan insights untuk strategi marketing yang data-driven
- Membandingkan performa algoritma clustering yang berbeda

## 🔧 Teknologi yang Digunakan

- **Python 3.8+**
- **Pandas** - Data manipulation dan analysis
- **NumPy** - Numerical computing
- **Matplotlib & Seaborn** - Data visualization
- **Scikit-learn** - Machine learning algorithms
- **SciPy** - Scientific computing untuk hierarchical clustering

## 📊 Dataset

Dataset berisi informasi pelanggan dengan fitur:
- `CustomerID` - ID unik pelanggan
- `Age` - Usia pelanggan
- `Annual_Income` - Pendapatan tahunan (dalam ribuan)
- `Spending_Score` - Skor pengeluaran (0-100)
- `Gender` - Jenis kelamin
- `City` - Kota tempat tinggal

## 🚀 Metodologi

### 1. **Data Preprocessing**
- ✅ Penanganan missing values dengan median imputation
- ✅ Penghapusan data duplikat
- ✅ Standardisasi format data (Gender, City)
- ✅ Deteksi dan penanganan outliers menggunakan IQR method
- ✅ Feature engineering (Income_per_Age ratio)

### 2. **Exploratory Data Analysis (EDA)**
- 📈 Analisis distribusi usia pelanggan
- 📊 Korelasi antar fitur numerik
- 🎨 Visualisasi scatter plot berdasarkan gender
- 📋 Analisis spending score per kota

### 3. **Clustering Analysis**

#### **K-Means Clustering**
- Implementasi K-Means dengan 3 cluster
- Visualisasi cluster centers
- Analisis karakteristik setiap cluster

#### **Hierarchical Clustering**
- Menggunakan Ward linkage method
- Dendrogram analysis untuk menentukan jumlah cluster optimal
- Perbandingan dengan hasil K-Means

## 📈 Hasil Analisis

### 🎯 3 Segmen Pelanggan Teridentifikasi:

| Cluster | Nama Segmen | Karakteristik | Strategi Marketing |
|---------|-------------|---------------|-------------------|
| **0** | 🛍️ **High Spenders** | Spending Score tinggi (60-100), Income rendah-sedang | Promosi produk premium dengan cicilan |
| **1** | 💎 **High Income Earners** | Income tinggi (80-140k), Spending bervariasi | Produk eksklusif dan layanan VIP |
| **2** | 💰 **Conservative Spenders** | Spending Score rendah (0-40), Income rendah-sedang | Produk value-for-money dan loyalitas |

### 📊 Key Insights:
- **Konsistensi algoritma**: K-Means dan Hierarchical Clustering menghasilkan 3 cluster yang optimal
- **Independensi fitur**: Age, Income, dan Spending Score relatif independen (korelasi lemah)
- **Opportunity**: Tidak ada korelasi langsung antara income dan spending behavior

## 🏃‍♂️ Cara Menjalankan

### Prerequisites
```bash
pip install pandas matplotlib seaborn scikit-learn scipy jupyter
```

### Menjalankan Analisis
1. Clone repository ini
```bash
git clone https://github.com/username/customer-segmentation-clustering.git
cd customer-segmentation-clustering
```

2. Jalankan Jupyter Notebook
```bash
jupyter notebook app.ipynb
```

3. Atau jalankan script Python
```bash
python app.py
```

## 📁 Struktur Proyek

```
customer-segmentation-clustering/
│
├── app.ipynb                 # Main analysis notebook
├── customers_dirty.csv       # Raw dataset
├── customers_new.csv         # Cleaned dataset
├── README.md                 # Project documentation
├── .gitignore               # Git ignore rules
└── requirements.txt         # Python dependencies
```

## 🔮 Pengembangan Selanjutnya

- [ ] Implementasi algoritma clustering lainnya (DBSCAN, Gaussian Mixture)
- [ ] Automated hyperparameter tuning
- [ ] Real-time clustering pipeline
- [ ] Interactive dashboard dengan Streamlit/Dash
- [ ] A/B testing framework untuk validasi strategi marketing

## 📝 Kesimpulan Bisnis

Analisis clustering ini memberikan **foundation yang solid** untuk:
- 🎯 **Personalisasi marketing** yang meningkatkan conversion rate
- 💰 **Optimalisasi budget** dengan targeting yang tepat sasaran
- 📈 **Peningkatan customer lifetime value** melalui strategi yang disesuaikan
- 🚀 **Competitive advantage** melalui customer intimacy yang lebih baik

## 👥 Kontribusi

Kontribusi sangat diterima! Silakan:
1. Fork repository ini
2. Buat feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit changes (`git commit -m 'Add some AmazingFeature'`)
4. Push ke branch (`git push origin feature/AmazingFeature`)
5. Buka Pull Request

## 📄 Lisensi

Distributed under the MIT License. See `LICENSE` for more information.


⭐ **Jika proyek ini membantu, jangan lupa beri star!** ⭐
