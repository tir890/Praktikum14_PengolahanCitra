# 📸 Face & Eye Detection Project Using OpenCV 👁️✨

> **Tugas Praktikum 14 - Pengolahan Citra Digital (Semester 4)** > *A Real-Time & Static Computer Vision Application built with Python and Haar Cascade Classifiers.* 🛡️🚀

---

## 🌟 Features & Highlights

* 🤖 **Real-Time Webcam Tracking**: Menyalakan camera feed secara instan, mendeteksi pergerakan wajah, dan melakukan auto-crop sampel gambar secara adaptif.
* 🎯 **Smart Region of Interest (ROI)**: Membatasi ruang pencarian koordinat mata hanya di dalam area wajah demi menghemat beban komputasi dan melipatgandakan akurasi.
* 📁 **Local Deployment Ready**: Konfigurasi path file yang fleksibel dan dioptimalkan khusus untuk VS Code lokal (bebas dari error path cloud Google Colab).
* 📊 **Visual Analytics**: Output rendering grafis menggunakan plot boks Matplotlib untuk pemetaan spasial biometrik yang presisi.

---

## 📂 Repository Structure

```text
📁 praktikum_14/
│
├── 📁 data/
│   ├── 📄 haarcascade_frontalface_default.xml  # 🏷️ Model latih untuk deteksi wajah depan
│   └── 📄 haarcascade_eye.xml                  # 🏷️ Model latih untuk deteksi organ mata
│
├── 🖼️ andrew.jpg                               # 📸 Citra input statis untuk uji coba
├── 🖼️ face.jpg                                 # 📤 Hasil ekspor deteksi wajah tunggal
├── 🖼️ face_and_eyes.jpg                        # 📤 Hasil ekspor pemetaan wajah + mata
│
├── 🐍 tugas1_webcam.py                         # 💻 Script tracking wajah interaktif via Webcam
├── 🐍 tugas2_gambar.py                         # 💻 Script deteksi wajah citra statis
└── 🐍 tugas3_mata.py                           # 💻 Script terintegrasi deteksi wajah & mata (ROI)

```

---

## 🚀 Getting Started

### 🛠️ Prerequisites & Installation

Pastikan komputer kamu sudah terpasang Python 3.x. Jalankan baris perintah berikut di dalam terminal VS Code untuk menginstal semua pustaka inti yang dibutuhkan:

```bash
pip install opencv-python numpy matplotlib

```

### 🎮 Running the Scripts

| Jenis Tugas | Perintah Eksekusi | Tombol Kontrol | Deskripsi Fungsional |
| --- | --- | --- | --- |
| **🎥 Live Webcam** | `py tugas1_webcam.py` | Tekan **`q`** untuk Keluar | Booting kamera, deteksi wajah *real-time*, dan rekam hingga 100 sampel. |
| **🖼️ Static Photo** | `py tugas2_gambar.py` | Silang Jendela Grafik | Memetakan koordinat wajah pada `andrew.jpg` lalu mengekspor `face.jpg`. |
| **👁️ ROI Analytics** | `py tugas3_mata.py` | Silang Jendela Grafik | Pemindaian sub-grid teroptimasi untuk wajah dan kedua mata sekaligus. |

---

## 🔬 Core Concepts & Architecture

### 🧠 Haar Cascade Classifiers

Sistem ini memanfaatkan **Haar-like features**, yang menghitung perbedaan nilai intensitas piksel di antara area persegi panjang digital yang berdekatan. Algoritma ini bekerja dalam format *Cascading* (beringkat), sehingga area non-wajah akan langsung dieliminasi sejak tahap awal demi menghemat memori RAM komputer.

### 🎯 Region of Interest (ROI) Isolation

```text
[ Bingkai Citra Utuh ] ➡️ Deteksi Kotak Wajah ➡️ Potong Batas Wajah (ROI) ➡️ Cari Mata HANYA di Dalam ROI
                                                                                         │
                                                                                         └── ❌ Noise Latar Belakang Diabaikan!

```

Dengan menerapkan teknik **ROI Slicing**, algoritma pencarian mata tidak perlu memindai seluruh background gambar (seperti tekstur tembok atau bayangan baju), sehingga performa program menjadi jauh lebih cepat dan akurat.

---

## ⚙️ Technologies Used

* `Python 3.x` 🐍
* `OpenCV (cv2)` 👁️
* `NumPy` 🔢
* `Matplotlib` 📊

---

### Sumber Yang digunakan

- https://github.com/kipr/opencv/blob/master/data/haarcascades/haarcascade_frontalface_default.xml
