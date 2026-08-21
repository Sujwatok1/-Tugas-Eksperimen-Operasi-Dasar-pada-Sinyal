# Operasi Dasar pada Sinyal dan Citra

## Informasi Mahasiswa

| Keterangan    | Detail                        |
| ------------- | ----------------------------- |
| Nama          | Anasufi Ajwa Nazli N.         |
| NIM           | 452024611015                  |
| Program Studi | Teknik Informatika            |
| Mata Kuliah   | Pengolahan Sinyal Digital     |
| Universitas   | Universitas Darussalam Gontor |

---

## Deskripsi Project

Project ini merupakan implementasi berbagai operasi dasar pada sinyal 1D dan citra 2D menggunakan bahasa pemrograman Python. Eksperimen dilakukan untuk memahami konsep dasar Pengolahan Sinyal Digital (PSD), khususnya operasi penjumlahan, penggeseran, amplifikasi, superposisi, dan pengujian sistem linier.

Melalui project ini dilakukan visualisasi, analisis, dan pengujian terhadap berbagai operasi pada sinyal diskrit serta citra digital untuk melihat pengaruh perubahan parameter terhadap hasil yang diperoleh.

---

## Tujuan Project

* Mengimplementasikan operasi penjumlahan pada sinyal dan citra.
* Mengimplementasikan operasi penggeseran (shift) pada sinyal dan citra.
* Mengimplementasikan operasi amplifikasi (scaling) pada sinyal dan citra.
* Menguji sifat homogenitas dan additivitas sistem.
* Membandingkan sistem linier dan non-linier.
* Memahami hubungan operasi dasar dengan konsep superposisi.
* Menghubungkan teori dengan aplikasi nyata dalam pengolahan sinyal digital.

---

## Library yang Digunakan

Project ini menggunakan beberapa library Python berikut:

* NumPy
* Matplotlib
* OpenCV (cv2)
* SciPy

Instalasi library:

```bash
pip install numpy matplotlib opencv-python scipy
```

---

## Cara Menjalankan Project

### 1. Clone Repository

```bash
https://github.com/Sujwatok1/-Tugas-Eksperimen-Operasi-Dasar-pada-Sinyal.git
```

### 2. Masuk ke Folder Project

```bash
cd operasi-dasar-sinyal-citra
```

### 3. Install Dependency

```bash
pip install -r requirements.txt
```

### 4. Jalankan Jupyter Notebook

```bash
jupyter notebook
```

Buka file:

```text
notebook/operasi_sinyal_citra.ipynb
```

Kemudian pilih:

```text
Kernel → Restart & Run All
```

---

## Struktur Folder Project

```text
operasi-dasar-sinyal-citra/
│
├── notebook/
│   └── operasi_sinyal_citra.ipynb
│
├── images/
│   ├── image1.jpg
│   └── image2.jpg
│
├── report/
│   └── laporan.pdf
│
├── README.md
│
└── requirements.txt
```

---

## Ringkasan Hasil Eksperimen

### 1. Operasi Penjumlahan Sinyal

Penjumlahan dua sinyal menghasilkan sinyal baru yang merupakan kombinasi dari kedua sinyal masukan. Perubahan amplitudo bergantung pada nilai masing-masing sinyal pada setiap indeks waktu.

### 2. Operasi Penggeseran Sinyal

Penggeseran dengan nilai positif menghasilkan delay (geser ke kanan), sedangkan nilai negatif menghasilkan advance (geser ke kiri). Operasi ini sering digunakan dalam simulasi keterlambatan transmisi sinyal.

### 3. Operasi Amplifikasi Sinyal

Amplifikasi dilakukan dengan mengalikan sinyal dengan faktor skalar α. Nilai α yang lebih besar dari 1 memperbesar amplitudo, sedangkan 0 < α < 1 memperkecil amplitudo sinyal.

### 4. Operasi Penjumlahan Citra

Penjumlahan dua citra menghasilkan peningkatan brightness dan dapat digunakan pada aplikasi image blending. Sebelum dijumlahkan, kedua citra harus memiliki ukuran yang sama.

### 5. Operasi Penggeseran Citra

Translasi citra mengubah posisi objek tanpa mengubah bentuk objek. Teknik ini banyak digunakan dalam augmentasi data pada machine learning dan computer vision.

### 6. Operasi Amplifikasi Citra

Amplifikasi citra meningkatkan nilai intensitas pixel sehingga citra menjadi lebih terang. Jika nilai pixel melebihi batas maksimum, diperlukan clipping untuk menjaga rentang pixel tetap valid.

### 7. Uji Sistem Linier

Dua sistem diuji:

**T₁(x) = 2x**

* Memenuhi homogenitas
* Memenuhi additivitas
* Termasuk sistem linier

**T₂(x) = x²**

* Tidak memenuhi homogenitas
* Tidak memenuhi additivitas
* Termasuk sistem non-linier

---

## Studi Kasus

### Brightness Enhancement pada Citra Digital

#### Permasalahan

Citra yang terlalu gelap menyebabkan informasi visual sulit diamati dan dianalisis.

#### Solusi

Melakukan amplifikasi nilai pixel menggunakan faktor pengali tertentu sehingga brightness meningkat.

#### Kelebihan

* Mudah diterapkan
* Komputasi ringan
* Efektif meningkatkan visibilitas objek

#### Keterbatasan

* Dapat menyebabkan overexposure
* Noise ikut diperkuat
* Detail area terang dapat hilang

---

## Kesimpulan

Berdasarkan eksperimen yang telah dilakukan, operasi penjumlahan, penggeseran, dan amplifikasi merupakan operasi dasar yang sangat penting dalam Pengolahan Sinyal Digital. Operasi-operasi tersebut menjadi fondasi berbagai teknik lanjutan seperti filtering, image blending, augmentasi data, audio processing, dan sistem komunikasi digital.

Hasil pengujian juga menunjukkan bahwa suatu sistem dapat dikatakan linier apabila memenuhi sifat homogenitas dan additivitas. Konsep sistem linier sangat penting karena berkaitan langsung dengan prinsip superposisi yang menjadi dasar banyak metode analisis sinyal modern.

Melalui project ini diperoleh pemahaman bahwa operasi sederhana pada sinyal dan citra memiliki peran besar dalam berbagai aplikasi teknologi yang digunakan saat ini.

---

## Referensi

1. Oppenheim, A. V., Willsky, A. S., & Nawab, S. H. *Signals and Systems*.
2. Gonzalez, R. C., & Woods, R. E. *Digital Image Processing*.
3. Dokumentasi NumPy: https://numpy.org
4. Dokumentasi Matplotlib: https://matplotlib.org
5. Dokumentasi OpenCV: https://opencv.org
