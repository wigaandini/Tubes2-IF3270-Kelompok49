# Tugas Besar 2 IF3270 Pembelajaran Mesin
## Convolutional Neural Network dan Recurrent Neural Network

### Deskripsi Repository

Repository ini berisi implementasi **Convolutional Neural Network (CNN)** dan **Recurrent Neural Network (RNN)** from scratch untuk Tugas Besar 2 mata kuliah IF3270 Pembelajaran Mesin. Tugas ini mencakup implementasi forward propagation untuk tiga arsitektur neural network:

- **CNN** - untuk image classification menggunakan dataset CIFAR-10
- **Simple RNN** - untuk text classification menggunakan dataset NusaX-Sentiment (Bahasa Indonesia)
- **LSTM** - untuk text classification menggunakan dataset NusaX-Sentiment (Bahasa Indonesia)

### Struktur Repository

```
.
├── doc/
│   └── Tubes2_13521049_13522013_13522053   # Laporan tugas dalam format PDF
├── src/
│   ├── result_lstm/            # Hasil model LSTM
│   ├── result_rnn/             # Hasil model Simple RNN
│   ├── cnn.ipynb              # Implementasi dan eksperimen CNN
│   ├── lstm.ipynb             # Implementasi dan eksperimen LSTM
│   └── simple_rnn.ipynb       # Implementasi dan eksperimen Simple RNN
└── README.md                   # File dokumentasi ini
```

### Requirements

Sebelum menjalankan program, pastikan Anda telah menginstall dependencies berikut:

```bash
pip install tensorflow
pip install keras
pip install numpy
pip install pandas
pip install matplotlib
pip install seaborn
pip install scikit-learn
pip install datasets
```

### Cara Setup dan Run Program

#### 1. Clone repository
```bash
git clone https://github.com/wigaandini/Tubes2-IF3270-Kelompok49.git
cd Tubes2-IF3270-Kelompok49
```

#### 2. Install dependencies yang disebutkan sebelumnya

#### 3. Jalankan model dan eksperimen

**CNN (CIFAR-10 Image Classification):**
```bash
jupyter notebook src/cnn.ipynb
```
- Jalankan semua cell untuk melatih model CNN

**Simple RNN (Text Classification):**
```bash
jupyter notebook src/simple_rnn.ipynb
```
- Jalankan semua cell untuk melatih model Simple RNN

**LSTM (Text Classification):**
```bash
jupyter notebook src/lstm.ipynb
```
- Jalankan semua cell untuk melatih model LSTM

### Fitur Implementasi

#### CNN Features:
- Forward propagation from scratch
- Analisis pengaruh jumlah layer konvolusi (3 variasi)
- Analisis pengaruh banyak filter per layer (3 variasi)
- Analisis pengaruh ukuran filter (3 variasi)
- Analisis pengaruh jenis pooling layer (Max vs Average)
- Evaluasi menggunakan macro F1-score

#### RNN & LSTM Features:
- Forward propagation from scratch
- Backward propagation from scratch
- Text preprocessing (tokenization & embedding)
- Analisis pengaruh jumlah layer (3 variasi)
- Analisis pengaruh jumlah cell per layer (3 variasi)
- Analisis pengaruh arah RNN/LSTM (bidirectional vs unidirectional)
- Evaluasi menggunakan macro F1-score

### Dataset

- **CNN**: CIFAR-10 (40k training, 10k validation, 10k test)
- **RNN & LSTM**: NusaX-Sentiment dataset (Bahasa Indonesia)

### Metodologi

1. **Training dengan Keras**: Melatih model menggunakan framework Keras dengan optimizer Adam dan loss function Sparse Categorical Crossentropy
2. **Forward Propagation from Scratch**: Implementasi ulang forward propagation tanpa menggunakan framework deep learning
3. **Validasi**: Membandingkan hasil implementasi from scratch dengan hasil Keras menggunakan macro F1-score
4. **Analisis Hyperparameter**: Eksperimen dengan berbagai konfigurasi untuk memahami pengaruh hyperparameter

### Pembagian Tugas

| Nama | NIM | Kontribusi |
|------|-----|------------|
| Brian Kheng | 13521049 | - Implementasi CNN from scratch |
| Denise Felicia Tiowanni | 13522013 | - Implementasi Simple RNN from scratch |
| Erdianti Wiga Putri Andini | 13522053 | - Implementasi LSTM from scratch |