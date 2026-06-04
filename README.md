```python
import os

# Let's create a beautifully styled README.md file optimized for a GitHub profile repository,
# completely using emojis, clear tables, and a professional yet aesthetic developer layout.

readme_content = """# 📸 Face & Eye Detection Project Using OpenCV 👁️✨

> **Tugas Praktikum 14 - Pengolahan Citra Digital (Semester 4)** > *A Real-Time & Static Computer Vision Application built with Python and Haar Cascade Classifiers.* 🛡️🚀

---

## 🌟 Features & Highlights

* 🤖 **Real-Time Webcam Tracking**: Capture and record live face frames instantly with adaptive compression.
* 🎯 **Smart Region of Interest (ROI)**: Isolates the face grid to maximize eye detection accuracy and reduce processing overhead.
* 📁 **Local Deployment Ready**: Optimized paths natively tailored for VS Code (No Google Colab cloud locks!).
* 📊 **Visual Analytics**: Direct output render using Matplotlib plots for precise biometrics bounding.

---

## 📂 Repository Structure


```

```text
README.md generated successfully!

```text
📁 praktikum_14/
│
├── 📁 data/
│   ├── 📄 haarcascade_frontalface_default.xml  # 🏷️ Trained model for face recognition
│   └── 📄 haarcascade_eye.xml                  # 🏷️ Trained model for eye tracking
│
├── 🖼️ andrew.jpg                               # 📸 Static input sample picture
├── 🖼️ face.jpg                                 # 📤 Output: Detected face frame
├── 🖼️ face_and_eyes.jpg                        # 📤 Output: Combined biometric mapping
│
├── 🐍 tugas1_webcam.py                         # 💻 Live webcam tracking script
├── 🐍 tugas2_gambar.py                         # 💻 Static face detection script
└── 🐍 tugas3_mata.py                           # 💻 Integrated face & eye ROI script

```

---

## 🚀 Getting Started

### 🛠️ Prerequisites & Installation

Make sure you have Python 3.x installed on your workstation. Run the command below inside your VS Code terminal to sync all core dependencies:

```bash
pip install opencv-python numpy matplotlib

```

### 🎮 Running the Scripts

| Task Type | Execution Command | Control Key | Description |
| --- | --- | --- | --- |
| **🎥 Live Webcam** | `py tugas1_webcam.py` | Press **`q`** to Exit | Boots camera feed, tracks faces, and logs up to 100 sample vectors. |
| **🖼️ Static Photo** | `py tugas2_gambar.py` | Close Window | Maps face coordinates on `andrew.jpg` and exports `face.jpg`. |
| **👁️ ROI Analytics** | `py tugas3_mata.py` | Close Window | Runs optimized sub-grid scanning for face and eyes simultaneously. |

---

## 🔬 Core Concepts & Architecture

### 🧠 Haar Cascade Classifiers

The system leverages **Haar-like features**, computing the pixel intensity differences between adjacent rectangular regions. It acts as a cascading framework, meaning it filters non-faces rapidly in early stages to save processing bandwidth.

### 🎯 Region of Interest (ROI) Isolation

```text
[ Full Digital Frame ] ➡️ Detect Face ➡️ Crop Face Boundaries (ROI) ➡️ Scan Eyes ONLY inside ROI
                                                                               │
                                                                               └── ❌ Background Noise Ignored!

```

By deploying **ROI Slicing**, the eye detection algorithm ignores background noise (e.g., wall textures, shadows), boosting performance speed and preventing false-positive data spikes.

---

## 🎨 Visualization Gallery

| Original Input (`andrew.jpg`) | Face Detection Result | Integrated Face & Eye ROI Mapping |
| --- | --- | --- |
| 👤 *[Insert Image]* | 🔴 Bounding Box Activated | ⚪ Precision Bounded Frames |

---

## ⚙️ Technologies Used

* `Python 3.x` 🐍
* `OpenCV (cv2)` 👁️
* `NumPy` 🔢
* `Matplotlib` 📊

---

with open("README.md", "w", encoding="utf-8") as f:
f.write(readme_content)

print("README.md generated successfully!")

```
Tentu, ini sudah saya buatkan file **`README.md`** khusus untuk repositori GitHub kamu. Desainnya sudah dibuat sangat *clean*, menggunakan banyak emoji agar interaktif, *eye-catching*, serta memiliki penataan teks yang *aesthetic* khas programmer profesional.

Berikut adalah file markdown (`.md`) yang bisa langsung kamu unduh dan masukkan ke dalam proyekmu:

Your Markdown (MD) file is ready
[file-tag: code-generated-file-0-1780558408328167764]

---

Jika kamu ingin melihat bagaimana tampilannya atau ingin menyalin teks mentahnya (*raw code*), berikut adalah visualisasi teks dari isi file GitHub `README.md` tersebut:

```markdown
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
