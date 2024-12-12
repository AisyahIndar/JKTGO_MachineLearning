# JKTGO_MachineLearning

# Model Rekomendasi Wisata dan Hotel

Proyek ini adalah sistem rekomendasi dan ini adalah path Machine Learning untuk wisata dan hotel dari project JKTGo!. Sistem ini menggunakan dataset wisata dan hotel untuk memberikan rekomendasi berdasarkan input pengguna seperti kategori wisata, harga, rating, dan lokasi.

## Deskripsi Proyek

Proyek ini terdiri dari dua sistem rekomendasi utama:

1. **Tourism Recommender**: Memberikan rekomendasi wisata berdasarkan kategori wisata, harga, dan rating.
2. **Hotel Recommender**: Memberikan rekomendasi hotel berdasarkan rating bintang, harga, rating pengguna, dan lokasi.

Kedua sistem ini dibangun menggunakan Neural Network dengan arsitektur deep learning yang menggabungkan fitur numerik dan kategorikal untuk menghasilkan prediksi yang lebih akurat.

## Fitur

- Rekomendasi wisata berdasarkan kategori (misalnya budaya, alam, belanja, dll).
- Rekomendasi hotel berdasarkan rating, harga, dan lokasi.
- Filter pencarian yang fleksibel (misalnya harga minimum/ maksimum, rating minimum).
- Penggunaan model deep learning untuk memproses fitur numerik dan kategorikal.

## Teknologi yang Digunakan

- **Python**: Bahasa pemrograman utama.
- **TensorFlow/Keras**: Digunakan untuk membangun model neural network.
- **Scikit-learn**: Digunakan untuk preprocessing data, termasuk encoding dan scaling.
- **Pandas**: Digunakan untuk manipulasi dan analisis data.
- **NLTK**: Digunakan untuk pemrosesan teks dan ekstraksi entitas.
- **Matplotlib**: Digunakan untuk visualisasi (jika diperlukan).

## Instalasi

### Persyaratan

1. Python 3.7 atau lebih baru.
2. Paket-paket Python berikut:
    - TensorFlow
    - Scikit-learn
    - Pandas
    - NLTK
    - Matplotlib

### Langkah-langkah Instalasi

1. **Clone repository ini ke komputer Anda**:
    ```bash
    git clone https://github.com/username/nama-repository.git
    cd nama-repository
    ```

2. **Install dependencies**:
    Jika Anda menggunakan `pip`, buat virtual environment dan install dependencies:
    ```bash
    python -m venv venv
    source venv/bin/activate  # Untuk Linux/MacOS
    venv\Scripts\activate  # Untuk Windows
    pip install -r requirements.txt
    ```

    File `requirements.txt` yang berisi dependensi dapat dibuat dengan perintah:
    ```bash
    pip freeze > requirements.txt
    ```

3. **Download dataset**:
    - Pastikan Anda sudah memiliki dataset yang diperlukan. Dataset yang digunakan adalah `cleaned_dataset_wisata.csv` dan `cleaned_dataset_hotel.csv`. Anda dapat mengunduhnya dan menaruhnya di folder yang sesuai.

## Penggunaan

Untuk menjalankan chatbot rekomendasi:

1. Jalankan script Python:
    ```bash
    python chatbot.py
    ```

2. Chatbot akan meminta input pengguna. Anda dapat mengetikkan pertanyaan seperti:
    - "Rekomendasikan wisata alam"
    - "Rekomendasikan hotel bintang 3"
    - "Rekomendasikan wisata murah"
    - "Rekomendasikan hotel di Jakarta"

    Ketik "keluar" untuk menghentikan chatbot.

## Menyimpan dan Memuat Model

- **Menyimpan model**: Setelah melatih model, model akan disimpan menggunakan Keras `model.save()` ke dalam file `.h5`:
    ```python
    self.model.save_model('tourism_recommender.h5')
    ```

- **Memuat model**: Anda bisa memuat model yang telah disimpan menggunakan:
    ```python
    self.model.load_model('tourism_recommender.h5')
    ```
## Struktur Direktori
```bash
/JKTGO_MachineLearning 
│
├── datasets/
│   ├── cleaned_dataset_wisata.csv
│   └── cleaned_dataset_hotel.csv
├──  Cleaned_dataset.ipynb 
├── Model Chatbot.ipynb 
└── README.md


