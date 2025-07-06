# 🧠 Customer Lifetime Value Prediction

Proyek ini bertujuan untuk menganalisis perilaku pelanggan dan memprediksi **Customer Lifetime Value (CLV)** menggunakan berbagai algoritma **machine learning** dan mengevaluasi penerimaan pelanggan terhadap kampanye pemasaran.

Dataset yang digunakan berasal dari Kaggle:  
👉 [Customer Personality Analysis](https://www.kaggle.com/datasets/imakash3011/customer-personality-analysis/data)

---

## 📦 Dataset Overview

Dataset ini berisi data pelanggan dari perusahaan pemasaran langsung. Kolom-kolom utama meliputi:

| Fitur             | Deskripsi |
|------------------|-----------|
| `ID`             | ID unik untuk setiap pelanggan |
| `Year_Birth`     | Tahun kelahiran pelanggan |
| `Education`      | Tingkat pendidikan pelanggan |
| `Marital_Status` | Status pernikahan |
| `Income`         | Pendapatan tahunan |
| `Kidhome`        | Jumlah anak kecil di rumah |
| `Teenhome`       | Jumlah remaja di rumah |
| `Dt_Customer`    | Tanggal pertama menjadi pelanggan |
| `Recency`        | Hari sejak pembelian terakhir |
| `MntWines` hingga `MntGoldProds` | Total pembelian per kategori produk |
| `NumWebPurchases`, dll | Jumlah pembelian melalui kanal tertentu |
| `AcceptedCmp1`–`AcceptedCmp5` | Indikator penerimaan kampanye 1–5 |
| `Response`       | Penerimaan kampanye terakhir |
| `Z_CostContact`, `Z_Revenue` | Nilai tetap (tidak informatif) |
| `Complain`       | Apakah pelanggan pernah komplain |

---

## 🎯 Tujuan Proyek

- Menganalisis perilaku pelanggan berdasarkan pengeluaran dan aktivitas belanja.
- Membuat model klasifikasi untuk memprediksi apakah pelanggan akan menerima kampanye.
- Membuat model regresi untuk memprediksi **TotalSpend (CLV)**.
- Membandingkan performa model:
  - `LinearRegression`
  - `GradientBoostingRegressor`
  - `XGBoost`
  - `RandomForestRegressor`

---

## 🧪 Evaluasi Model

Setiap model dievaluasi menggunakan metrik:

- **Regresi**: RMSE, MAE, R²
- **Klasifikasi**: Accuracy, Precision, Recall, F1-score

Visualisasi yang disediakan:
- Korelasi antar fitur
- Distribusi CLV (TotalSpend)
- Distribusi error per model
- Scatter plot: Prediksi vs Nilai Asli

---

## 🚀 Cara Menjalankan Proyek

1. **Clone repositori**:
   ```bash
   git clone https://github.com/username/customer-clv-prediction.git
   cd customer-clv-prediction
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
4. Jalankan notebook:
   ```bash
   jupyter notebook notebooks/CLV_Analysis.ipynb

📌 Catatan Tambahan
- Z_CostContact dan Z_Revenue dihapus dari modeling karena berisi nilai tetap.
