# Deteksi dan Tracking Kendaraan Menggunakan YOLO

## Proyek UAS – Computer Vision

---

## Deskripsi Proyek

Proyek ini merupakan implementasi sistem **deteksi dan tracking kendaraan pada lalu lintas jalan** menggunakan metode **Computer Vision berbasis deep learning YOLO (You Only Look Once)**. Sistem mampu mendeteksi beberapa jenis kendaraan seperti **mobil, motor, bus, dan truk** dari citra maupun video, serta melacak pergerakan kendaraan antar frame menggunakan **ID unik**.

Proyek ini dikembangkan sebagai bagian dari **Ujian Akhir Semester (UAS) Mata Kuliah Computer Vision**, dengan mengintegrasikan materi pertemuan **1 hingga 15**, mulai dari pengolahan citra dasar hingga **object detection dan tracking berbasis deep learning**.

---

## Fitur Utama

* Deteksi kendaraan secara real-time menggunakan YOLO
* Tracking kendaraan antar frame video menggunakan ID unik
* Mendukung input berupa gambar dan video
* Visualisasi bounding box dan label kelas kendaraan
* Menggunakan preprocessing Computer Vision (filtering, edge detection, dan segmentation)

---

## Teknologi yang Digunakan

* **Python**
* **YOLO (Ultralytics)**
* **OpenCV**
* **NumPy**
* **Matplotlib**
* **Jupyter Notebook**

---

## Cara Penggunaan

### 1️. Persiapan Environment

Pastikan Python telah terinstal, kemudian install library yang dibutuhkan dengan perintah berikut:

```bash
pip install ultralytics opencv-python matplotlib numpy
```

Jika menggunakan **Google Colab**, jalankan cell instalasi library terlebih dahulu sebelum menjalankan program utama.

---

### 2️. Menyiapkan Model

Pastikan file model hasil training YOLO (`best.pt`) tersedia dan berada pada path yang sesuai dengan konfigurasi notebook.

Model ini digunakan sebagai hasil **fine-tuning** dari pretrained YOLO untuk mendeteksi kendaraan.

---

### 3. Menjalankan Deteksi pada Gambar

* Masukkan file gambar dengan format `.jpg`, `.jpeg`, atau `.png`
* Jalankan notebook utama

Sistem akan melakukan:

* Membaca gambar input
* Melakukan preprocessing citra
* Menampilkan hasil deteksi kendaraan dalam bentuk **bounding box dan label kelas**

---

### 4️. Menjalankan Deteksi dan Tracking pada Video

* Masukkan file video dengan format `.mp4`
* Jalankan cell deteksi video pada notebook

Sistem akan:

* Mendeteksi kendaraan pada setiap frame video
* Memberikan **ID unik** pada setiap kendaraan
* Menampilkan hasil tracking secara visual

---

## Penjelasan Singkat Sistem

Alur kerja sistem secara umum adalah sebagai berikut:

1. Input berupa citra atau video lalu lintas
2. Preprocessing citra untuk meningkatkan kualitas input
3. Object Detection menggunakan YOLO untuk mendeteksi dan mengklasifikasikan kendaraan
4. Object Tracking untuk melacak kendaraan antar frame
5. Output berupa visualisasi bounding box, label kelas, dan ID kendaraan

Pendekatan ini memungkinkan sistem bekerja secara **cepat dan akurat**, serta tetap stabil pada kondisi lalu lintas yang padat.


