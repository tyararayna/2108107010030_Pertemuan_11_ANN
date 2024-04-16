# Tugas-3-2108107010030

Nama : Tyara Raynasari

NPM : 2108107010030
## Deskripsi Data

### Poin 1 
Data yang digunakan dalam proyek ini merupakan data bank besar di eropa dengan beberapa karakteristik dari masing-masing customer tersebut. Dalam dataset ini, terdapat sekitar 10.000 data dengan 14 kolom didalamnya. Proses yang dilakukan adalah klasifikasi, sehingga nantinya kita ingin memprediksi apakah model deep learning (DL) bisa memprediksi status keluar tidaknya nasabah karena berdasarkan data-data di atas tingkat keluar nasabah tiba tiba meningkat (churn rate) . 

Link menuju dataset : https://www.megabagus.id/download/data-ann/

Berikut merupakan beberapa kolom yang terdapat dalam dataset Bank Eropa : 

- RowNumber = menunjukkan ia baris ke berapa.
- CustomerId = identitas unik setiap costumer.
- Surname = nama belakang pelanggan.
- CreditScore = skor kredit yang diberikan oleh bank. Hanya bank yang tahu cara menghitung skor ini.
- Geography = negara domisili nasabah.
- Gender = jenis kelamin.
- Age = usia.
- Tenure = berapa lama (dalam tahun) mereka sudah menjadi nasabah bank.
- Balance = tabungan nasabah saat ini (atau saat terakhir sebelum keluar sebagai nasabah).
- NumberOfProduct = berapa banyak produk bank yang dimiliki oleh nasabah pada saat ini (atau saat terakhir).
- HasCrCard = kondisi apakah saat ini nasabah memiliki kartu kredit di bank ini (1) atau tidak (0).
- IsActiveMember = kondisi apakah pelanggan saat ini aktif (1) menjadi member aktif atau tidak (0). Hanya bank yang tahu cara membuat status ini, misal apakah nasabah aktif melakukan transaksi di bulan terakhir, apakah memiliki pinjaman di bulan terakhir, dan seterusnya.
- EstimatedSalary = estimasi gaji yang dibuat oleh bank. Tentu saja bank tidak tahu gaji asli dari nasabah, tapi bank sudah membuat perkiraan gaji berdasarkan pola keluar masuknya uang nasabah tersebut.
- Exited = status apakah nasabah ini tetap di bank (0) atau keluar dari bank (1).

### Poin 2 
Data yang digunakan dalam proyek ini merupakan data harga laptop dengan beberapa karakteristik dari masing-masing laptop tersebut. Dalam dataset ini, terdapat sekitar 1000 data dengan 7 kolom didalamnya. Data ini dapat diunduh dari situs Kaggle.

Link menuju dataset : https://www.kaggle.com/datasets/mrsimple07/laptoppriceprediction/data 

Berikut merupakan beberapa kolom yang terdapat dalam dataset Laptop Price Prediction : 

- Brand = merupakan nama-nama brand laptop, seperti Dell, HP, Lenovo, Asus, dan Acer.
- Processor_Speed = merupakan kecepatan pada processor tiap laptop antara 1.5 dan 4.0 GHz.
- RAM_size = merupakan ukuran RAM yaitu 4GB, 8GB, 16GB dan 32GB.
- Storage_Capacity = merupakan ukuran kapasitas dari laptop yaitu 256GB, 512GB, dan 1000GB (1TB).
- Screen_Size = merupakan ukuran layar dari laptop antara 11 sampai 17 inch.
- Weight = merupakan berat laptop mulai dari 2 kg sampai 5 kg.
- Price = merupakan label dari data yaitu harga laptop sesuai dengan fitur-fitur lainnya.

Output **Poin2.ipynb** ini untuk membandingkan nilai akurasi antara model dengan SVR dan model dengan ANN.

Berdasarkan hasil output :

R-squared dari model SVR: **0.9682939700117195**

Model SVR mampu menjelaskan sekitar 96.83% variabilitas dalam data yang diamati. Dengan nilai R^2 yang tinggi seperti ini, dapat diinterpretasikan bahwa model SVR memberikan perkiraan yang sangat baik terhadap variabel target.


R-squared dari model ANN: **0.9831003930913376**

Ini menunjukkan bahwa model Artificial Neural Network (ANN) memiliki kemampuan yang lebih baik dalam menjelaskan data, dengan R^2 sebesar 98.31%. Hal ini menunjukkan bahwa ANN mampu menghasilkan prediksi yang lebih akurat dibandingkan dengan model SVR dalam kasus yang sama.

Secara keseluruhan, kedua model tersebut memiliki kinerja yang baik, tetapi model ANN sedikit lebih baik dalam menjelaskan variabilitas data. Namun, selain R^2, selalu penting untuk mempertimbangkan metrik evaluasi lainnya dan membandingkan keduanya untuk mendapatkan pemahaman yang lebih lengkap tentang kinerja model.

## Langkah menjalankan repository ini : 

1. Membuat virtual enviroment di dalam repository ini. Open in terminal kemudian jalankan : 
```bash
python3 -m venv nama_env
```
2. Aktifkan virtual environment pada terminal dalam lingkungan kode. Jalankan :
```bash
source nama_env/bin/activate
```
3. Install semua library yang ada dalam file requirements.txt. Jalankan : 
```bash
pip install -r requirements.txt
```
4. Jalankan semua kode Poin1.ipynb dan Poin2.ipynb dengan memilih kernel terlebih dahulu. Pilih nama_env yang telah dibuat sebelumnya. 

5. Lihat output dan analisis hasilnya. 
