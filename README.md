# Power Consumption of Tetouan City Dataset

Repositori ini berisi dataset tentang konsumsi daya di kota Tetouan, Maroko. Data ini dikumpulkan dari tiga zona jaringan distribusi yang berbeda di kota tersebut.

## 📝 Deskripsi

Dataset ini mencakup data konsumsi daya yang dicatat setiap 10 menit selama tahun 2017. Selain data konsumsi daya untuk tiga zona berbeda, dataset ini juga menyertakan variabel cuaca yang relevan seperti suhu, kelembaban, kecepatan angin, dan aliran radiasi matahari.

Data ini sangat berguna untuk tugas-tugas analisis deret waktu (*time series*), peramalan (*forecasting*), dan pemodelan regresi untuk memprediksi penggunaan energi berdasarkan faktor cuaca.

## 🗂️ Detail Dataset

  * **Nama File**: `Tetuan City power consumption.csv`
  * **Format**: CSV (Comma-Separated Values)
  * **Jumlah Baris**: 52416
  * **Jumlah Kolom**: 9
  * **Frekuensi Data**: Setiap 10 menit
  * **Periode Waktu**: 1 Januari 2017 - 30 Desember 2017

## 📊 Informasi Atribut (Kolom)

| Nama Kolom | Tipe Data | Deskripsi |
| :--- | :--- | :--- |
| `DateTime` | Object (String) | Tanggal dan waktu pencatatan (format: `MM/DD/YYYY HH:mm`) |
| `Temperature` | float64 | Suhu dalam satuan Celcius (°C) |
| `Humidity` | float64 | Kelembaban relatif dalam persen (%) |
| `Wind Speed` | float64 | Kecepatan angin dalam satuan m/s |
| `general diffuse flows`| float64 | Aliran radiasi matahari difus umum (kW/m²) |
| `diffuse flows` | float64 | Aliran radiasi matahari difus (kW/m²) |
| `Zone 1 Power Consumption`| float64 | Konsumsi daya di Zona 1 (kW) |
| `Zone 2 Power Consumption`| float64 | Konsumsi daya di Zona 2 (kW) |
| `Zone 3 Power Consumption`| float64 | Konsumsi daya di Zona 3 (kW) |

## 🚀 Contoh Penggunaan

Berikut adalah contoh sederhana cara memuat dan melihat dataset ini menggunakan Python dengan library `pandas`.

```python
import pandas as pd

# Muat dataset dari file CSV
file_path = 'Tetuan City power consumption.csv'
df = pd.read_csv(file_path)

# Tampilkan 5 baris pertama dari dataset
print("Data Awal:")
print(df.head())

# Tampilkan informasi dasar tentang dataset
print("\nInformasi Dataset:")
df.info()

# Tampilkan ringkasan statistik
print("\nStatistik Deskriptif:")
print(df.describe())
```

## 🙏 Sitasi

Jika Anda menggunakan dataset ini dalam penelitian atau proyek Anda, harap mengutip sumber aslinya:

Salam, A., & El Hibaoui, A. (2018). Comparison of Machine Learning Algorithms for the Power Consumption Prediction: Case of a Tetouan city. In *Proceedings of the 2nd International Conference on Big Data, Advanced Wireless and Communication (BDAW '18)*. Association for Computing Machinery, New York, NY, USA, Article 19, 1–5. DOI: [https://doi.org/10.1145/3233207.3233228](https://www.google.com/search?q=https://doi.org/10.1145/3233207.3233228)

## 🌐 Sumber

Dataset ini tersedia di UCI Machine Learning Repository:
[https://archive.ics.uci.edu/dataset/849/power+consumption+of+tetouan+city](https://archive.ics.uci.edu/dataset/849/power+consumption+of+tetouan+city)
