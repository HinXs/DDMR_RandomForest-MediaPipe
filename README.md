# ✨ DDMR RandomForest MediaPipe

[![Python](https://img.shields.io/badge/language-Python-blue.svg)](https://www.python.org/)

> Proyek ini menggabungkan Random Forest dengan MediaPipe untuk mengontrol robot berdasarkan deteksi pose.

## ✨ Fitur Utama

* **Deteksi Pose Real-time:** Menggunakan MediaPipe untuk mendeteksi pose manusia secara real-time dari input video atau gambar.
* **Klasifikasi Gerakan:**  Menggunakan model Random Forest yang terlatih untuk mengklasifikasikan pose yang terdeteksi ke dalam berbagai gerakan atau perintah untuk robot.
* **Kontrol Robot:**  Menerjemahkan klasifikasi gerakan menjadi perintah kontrol untuk robot, memungkinkan interaksi berbasis gerakan.
* **Model Random Forest yang Terlatih:**  Menggunakan model `rf_pose_model.pkl` yang telah dilatih sebelumnya untuk melakukan klasifikasi pose.
* **Penggunaan `shared_vars.py`:** Mengelola variabel bersama yang digunakan oleh berbagai bagian program untuk memastikan sinkronisasi data.
* **Simulator Robot (`PROGRAM_DDMR_ESP.py`):**  Menyediakan simulasi dari logika kontrol robot, sehingga pengembangan dan pengujian dapat dilakukan tanpa perangkat keras robot yang sebenarnya.  (Detail lebih lanjut tentang simulasi ini dibutuhkan untuk deskripsi yang lebih komprehensif).
* **Penggunaan `project_Mobot_DDMR.zip` (Potensial):**  File zip ini mungkin berisi aset tambahan atau kode sumber yang terkait dengan proyek robot, membutuhkan pemeriksaan lebih lanjut untuk detail fitur.


## 🛠️ Tumpukan Teknologi

| Kategori          | Teknologi | Catatan                               |
|----------------------|------------|---------------------------------------|
| Bahasa Pemrograman | Python      | Bahasa utama untuk pengembangan.       |
| Perpustakaan       | MediaPipe   | Untuk deteksi pose real-time.          |
| Perpustakaan       | scikit-learn (diasumsikan) | Untuk model Random Forest.      |


## 🏛️ Tinjauan Arsitektur

Arsitektur proyek ini terdiri dari beberapa komponen utama:  detektor pose MediaPipe, model klasifikasi Random Forest, dan sebuah simulator robot.  MediaPipe memproses input visual dan menghasilkan data pose. Data pose ini kemudian dimasukkan ke model Random Forest untuk mengklasifikasikan gerakan.  Akhirnya, simulator robot (atau robot nyata jika diimplementasikan) menerima perintah berdasarkan klasifikasi dan melaksanakannya. Detail arsitektur yang lebih rinci memerlukan pemeriksaan lebih lanjut terhadap kode sumber.

## 🚀 Memulai

1. **Kloning Repositori:**
   ```bash
   git clone https://github.com/HinXs/DDMR_RandomForest-MediaPipe.git
   cd DDMR_RandomForest-MediaPipe
   ```

2. **Instalasi Dependensi:**  
   ```bash
   update soon.
   ```

3. **Menjalankan Simulator:**
   ```bash
   python PROGRAM_DDMR_ESP.py
   ```


## 📂 Struktur File

```
/
├── # Fungsi simulator robot.txt
├── PROGRAM_DDMR_ESP.py      # Simulasi robot (Perlu verifikasi lebih lanjut)
├── README.md                 # File README
├── project_Mobot_DDMR.zip   # Potensial berisi aset tambahan (Perlu verifikasi lebih lanjut)
├── rf_pose_model.pkl        # Model Random Forest yang telah terlatih
└── shared_vars.py           # Variabel bersama
```

* **/:** Direktori utama proyek.
* **PROGRAM_DDMR_ESP.py:**  Mengandung logika utama untuk simulasi robot.
* **rf_pose_model.pkl:**  File yang berisi model Random Forest yang telah dilatih.
* **shared_vars.py:** File yang berisi variabel bersama yang digunakan oleh berbagai bagian program.
* **project_Mobot_DDMR.zip:**  File program esp8266 untuk menjalankan DDMR menggunakan ESP8266.



