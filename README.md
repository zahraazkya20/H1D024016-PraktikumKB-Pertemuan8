# Praktikum Kecerdasan Buatan - Pertemuan 8
## Jaringan Syaraf Tiruan 3: Klasifikasi Rock-Paper-Scissors dengan CNN

**NIM:** H1D024016  
**Nama:** Zahratul Askia  
**Mata Kuliah:** Praktikum Kecerdasan Buatan Shift F  

---

## 📋 Deskripsi Proyek

Proyek ini merupakan implementasi **Convolutional Neural Network (CNN)** menggunakan TensorFlow/Keras untuk mengklasifikasikan gambar tangan membentuk batu (rock), kertas (paper), atau gunting (scissors). Dataset yang digunakan adalah [Rock Paper Scissors Dataset dari Kaggle](https://www.kaggle.com/datasets/drgfreeman/rockpaperscissors).

Model CNN yang dibangun memiliki arsitektur:
- 3 lapisan konvolusi (Conv2D) dengan filter 32, 64, 128 dan ukuran kernel 3x3.
- Setiap lapisan konvolusi diikuti oleh MaxPooling2D (2x2).
- Flatten layer dan Dense layer (512 unit) dengan aktivasi ReLU.
- Output layer Dense (3 unit) dengan aktivasi Softmax.

**Hasil akhir yang dicapai:**  
- Akurasi validasi: **98.17%**  
- Loss validasi: 0.0424

---

## 📁 Struktur Folder
├── .venv/ # Virtual environment (dibuat otomatis)  
├── rockpaperscissors/ # Folder dataset (HARUS persis ini)  
│ ├── rock/  
│ ├── paper/  
│ └── scissors/  
├── main.py # Kode program CNN  
└── README.md # File ini  

> **Penting:** Nama folder dataset **wajib** `rockpaperscissors` dan berada di level yang sama dengan `main.py`.

---

## Cara Install & Jalankan

### Prasyarat
- Python 3.8 atau lebih baru [download python.org](https://python.org)
- Git (opsional, untuk clone repositori)

### Langkah-langkah

1. **Clone repositori** (atau download file `main.py`):
```bash
git clone [https://github.com/username/NIM-PraktikumKB-Pertemuan8.git](https://github.com/zahraazkya20/H1D024016-PraktikumKB-Pertemuan8.git)
cd NIM-PraktikumKB-Pertemuan8
```
2. Buat dan aktifkan virtual environment (disarankan):
Windows (PowerShell):
```bash
python -m venv .venv
.\.venv\Scripts\Activate
```
Mac / Linux:
```bash
python3 -m venv .venv
source .venv/bin/activate
```
3. Install library yang diperlukan:
```bash
pip install tensorflow numpy pandas
```
4. Siapkan dataset:
- Unduh dataset dari Kaggle (https://www.kaggle.com/datasets/drgfreeman/rockpaperscissors).
- Ekstrak file ZIP sehingga menghasilkan folder rockpaperscissors.
- Pindahkan folder rockpaperscissors ke dalam folder proyek (samping main.py).
5. Jalankan program:
```bash
python main.py
```
