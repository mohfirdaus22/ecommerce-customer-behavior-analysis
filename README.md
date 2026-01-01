# E-Commerce Customer Behavior & Profitability Analysis

## Project Overview
**Role:** Data Analyst  
**Tools:** Microsoft Excel (Cleaning & Pivot), Power BI (Dashboarding)  
**Dataset:** 5,000 Transaction Records (2023-2024)

### Business Problem
Perusahaan E-commerce ingin memahami pola perilaku pelanggan untuk meningkatkan profitabilitas. Tantangan utamanya adalah mengevaluasi apakah strategi diskon saat ini efektif, mengidentifikasi segmen pelanggan yang paling bernilai, dan memahami preferensi penggunaan perangkat (device) pelanggan.

---

## Executive Summary (Key Findings)
Berdasarkan analisis terhadap 5.000 data transaksi, ditemukan bahwa perusahaan memiliki **Retensi Pelanggan yang sangat kuat (~60%)**, namun strategi **pemberian diskon saat ini justru menggerus profitabilitas** tanpa memberikan kenaikan volume penjualan yang signifikan.

### 1. Inefisiensi Strategi Diskon
* **Temuan:** Rata-rata profit pesanan **tanpa diskon ($984)** jauh lebih tinggi dibandingkan pesanan **dengan diskon ($899)**.
* **Masalah:** Pemberian diskon saat ini menyebabkan penurunan margin keuntungan sebesar **~8.6%** per transaksi, sementara rata-rata nilai belanja (Total Amount) antara yang diskon dan tidak diskon hampir sama.
* **Insight:** Diskon yang diberikan tidak efektif mendorong pelanggan untuk membelanjakan uang lebih banyak (upselling).

### 2. Perilaku Pengguna & Platform (The "Mobile Whales")
* **Temuan:** Pengguna **Mobile** memiliki rata-rata pembelanjaan tertinggi ($1,005) dibandingkan pengguna Desktop ($964) dan Tablet ($921).
* **Insight:** Pelanggan bernilai tinggi (High-Value Customers) lebih nyaman bertransaksi melalui ponsel.

### 3. Loyalitas Pelanggan (Retention)
* **Temuan:** 59.8% transaksi berasal dari **Returning Customers** (2.990 pesanan) vs 40.2% New Customers.
* **Insight:** Bisnis ini memiliki basis pelanggan setia yang sangat sehat. Fokus strategi harus pada menjaga loyalitas ini (retention) daripada hanya membakar uang untuk akuisisi pelanggan baru.

### 4. Performa Produk
* **Cash Cow:** Kategori **Electronics** adalah penyumbang Revenue dan Profit terbesar (~$2.3M).
* **Rising Star:** Kategori **Home & Garden** menempati posisi kedua dengan performa yang solid (~$908k).

---

## Business Recommendations
Berdasarkan data di atas, berikut adalah rekomendasi strategis untuk manajemen:

1.  **Evaluasi Ulang Strategi Diskon:**
    * Hentikan diskon "bakar uang" yang tidak menaikkan Basket Size.
    * Ubah menjadi strategi **Bundling** atau **Minimum Spend** (misal: "Diskon 10% untuk pembelian di atas $1.500") untuk memaksa kenaikan rata-rata nilai belanja.
2.  **Mobile-First Optimization:**
    * Pastikan UI/UX aplikasi mobile berjalan sempurna karena pengguna mobile adalah penyumbang rata-rata revenue terbesar. Alokasikan budget marketing lebih besar untuk Mobile Ads.
3.  **Loyalty Program untuk Returning Customers:**
    * Mengingat 60% pelanggan adalah *Returning*, buat program loyalitas tiering (Silver/Gold/Platinum) untuk menjaga mereka agar tidak pindah ke kompetitor.

---

## Technical Process (Methodology)

### 1. Data Cleaning & Preparation
* **Standardisasi:** Mengonversi format tanggal menjadi format standar `YYYY-MM-DD`.
* **Duplikasi:** Melakukan pengecekan duplikasi berdasarkan `Order_ID` (Hasil: 0 duplikat ditemukan).
* **Missing Values:** Memastikan tidak ada *null values* di kolom kritis (Harga, Quantity, Customer ID).

### 2. Feature Engineering
Menambahkan kolom baru untuk mempermudah analisis:
* `Profit_Estimation`: Menghitung estimasi keuntungan per transaksi.
* `Age_Group`: Mengelompokkan usia pelanggan (<25, 25-34, 35-44, dst) untuk analisis demografi.
* `Year` & `Month`: Ekstraksi dari tanggal pesanan untuk analisis tren waktu.

### 3. Exploratory Data Analysis (EDA)
Menggunakan Excel Pivot Tables untuk menganalisis:
* Korelasi antara Diskon vs Profitabilitas.
* Distribusi demografi pelanggan.
* Analisis metode pembayaran dan tipe perangkat.

### 4. Visualization
Membuat Dashboard interaktif menggunakan **Power BI** untuk memvisualisasikan Metrik Kunci (KPIs).

---

## Dashboard Preview
*(Note: Silakan masukkan screenshot dashboard Power BI kamu di sini)*

![Dashboard Customer Behavior](/assets/Ecommerce-customer-behavior-analysis.png)
![Dashboard Profitability & Performance](/assets/Profitability-&-Business-Performance-Analysis.png)

---

**Author:** [mohfirdaus22]  
