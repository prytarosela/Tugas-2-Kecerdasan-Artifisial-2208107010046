# Tugas-2-Kecerdasan-Artifisial-2208107010046

# Klasifikasi Gambar Bunga Menggunakan Convolutional Neural Network (CNN)

Proyek ini bertujuan untuk mengklasifikasikan gambar bunga ke dalam lima kategori (`daisy`, `dandelion`, `rose`, `sunflower`, `tulip`) menggunakan model Convolutional Neural Network (CNN).

## Fitur
- **Pengelolaan Dataset**: Secara otomatis membagi dataset menjadi data training dan validasi.
- **Arsitektur Model**: CNN sederhana dengan tiga lapisan konvolusi, lapisan pooling, dan lapisan dense.
- **Visualisasi Training**: Grafik untuk memantau loss dan akurasi selama proses training.
- **Penyimpanan Model**: Model yang sudah dilatih disimpan di Google Drive.
- **Logging**: Dukungan TensorBoard untuk log training secara mendetail.

## Langkah-Langkah
1. **Mount Google Drive**  
   Pastikan akses ke dataset dan folder penyimpanan:
   ```python
   from google.colab import drive
   drive.mount('/content/drive')
   ```

2. **Persiapan Dataset**  
   Susun dataset di Google Drive dengan struktur berikut:  
   ```
   Dataset/
       flowers/
           daisy/
           dandelion/
           rose/
           sunflower/
           tulip/
   ```

3. **Jalankan Kode**  
   Eksekusi skrip Python di Google Colab sesuai langkah-langkah yang disediakan.

4. **Training**  
   Model akan dilatih selama 5 epoch, dengan log training dapat dilihat menggunakan TensorBoard.

5. **Evaluasi dan Simpan Model**  
   Evaluasi performa model pada data validasi, lalu simpan model ke Google Drive:
   ```python
   model.save('/content/drive/My Drive/Dataset/flowers_cnn_model.h5')
   ```

## Hasil
- **Akurasi Validasi Akhir**: ~63%
- **Grafik Training**:
  - Grafik *Loss*: Training vs Validasi
  - Grafik *Accuracy*: Training vs Validasi

## Persyaratan
- Python 3.7+
- TensorFlow 2.x
- Matplotlib

## Struktur Folder
```
tensorboard_logs/
    train/
    validation/
Screenshot/
SourceCode.ipynb
```

## Catatan
- Akurasi validasi dapat bervariasi tergantung dataset.
- Untuk meningkatkan akurasi, tambahkan data atau coba fine-tuning hyperparameter.

Selamat mencoba! 🌼🌻🌹
