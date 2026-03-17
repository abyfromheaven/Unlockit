# 🔓 UnlockKit - Python Brute Force Toolkit

[![Python Version](https://img.shields.io/badge/python-3.x-blue.svg?style=flat-square&logo=python)](https://www.python.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg?style=flat-square)](https://opensource.org/licenses/MIT)
[![Bootcamp](https://img.shields.io/badge/Bootcamp-ID--Networkers-red?style=flat-square)](https://https://www.idn.id//)
[![Cyber Security](https://img.shields.io/badge/Focus-Cyber%20Security-black?style=flat-square&logo=target)](https://id-networkers.com/)

**UnlockKit** adalah toolkit berbasis Python yang ringan dan edukatif, dirancang untuk membuka proteksi file yang dikunci dengan password menggunakan metode brute force. Proyek ini merupakan bagian dari tugas **Bootcamp Online Cyber Security di ID-Networkers**.

---

## 🎯 Deskripsi Proyek
Proyek ini dibuat sebagai bentuk implementasi praktis dari materi keamanan siber, khususnya dalam memahami mekanisme *password cracking* dan *brute force* pada file terkompresi. Versi awal mendukung cracking file **ZIP** dan akan terus dikembangkan untuk mendukung format lain.

## 🚀 Fitur Utama
- ⚡ **Fast & Lightweight:** Menggunakan modul bawaan Python.
- 📂 **ZIP Cracking:** Brute force file ZIP menggunakan wordlist kustom.
- 🛠️ **Error Handling:** Penanganan error yang lengkap untuk file rusak atau tidak ditemukan.
- 📖 **Interactive CLI:** Antarmuka baris perintah yang mudah digunakan bagi pemula.

---

## 🛠️ Instalasi & Penggunaan

Ikuti langkah-langkah di bawah ini untuk menjalankan alat ini di lingkungan lokal Anda:

### 1️⃣ Kloning Repositori
Clone proyek ini ke mesin lokal Anda:
```bash
git clone https://github.com/abyfromheaven/Unlockit.git
cd unlockkit
```

### 2️⃣ Persiapan Lingkungan (Opsional namun Disarankan)
Gunakan virtual environment untuk menjaga sistem Anda tetap bersih:
```bash
# Windows
python -m venv venv
venv\Scripts\activate

# Linux/macOS
python3 -m venv venv
source venv/bin/activate
```

### 3️⃣ Instalasi Dependensi
Saat ini, proyek hanya menggunakan library standar Python (`zipfile`), sehingga tidak ada instalasi tambahan yang diperlukan. Namun, jika di masa depan ada update:
```bash
# Jika ada file requirements.txt
pip install -r requirements.txt
```

### 4️⃣ Cara Menjalankan
Pastikan Anda memiliki file ZIP target dan file wordlist (seperti `rockyou.txt` atau daftar password lainnya).
```bash
python3 main.py
```

### 5️⃣ Contoh Input di Terminal
```text
=== Alat Brute Force Kata Sandi ZIP ===
Masukkan path ke file ZIP: data_rahasia.zip
Masukkan path ke file wordlist: wordlist.txt
Mulai brute force pada "data_rahasia.zip" menggunakan wordlist "wordlist.txt"...
```

---

## 🔍 Detail Teknis: `main.py`
Skrip ini bekerja dengan mencoba mengekstrak file ZIP menggunakan setiap baris kata sandi yang ada di dalam wordlist yang diberikan.

- **`brute_force_zip()`**: Logika utama untuk iterasi wordlist dan percobaan dekripsi.
- **`main()`**: Handler input pengguna dan manajemen alur eksekusi.

---

## 🚧 Roadmap Pengembangan
- [ ] 📦 Tambahkan dukungan file **RAR** (`rarfile`)
- [ ] 📄 Tambahkan dukungan file **PDF** (`pikepdf`)
- [ ] 🖥️ Antarmuka GUI (CustomTkinter)
- [ ] 🧵 Implementasi Multi-threading untuk kecepatan maksimal
- [ ] 🌐 Web Interface (Flask/FastAPI)

---

## ⚠️ Disclaimer
> [!IMPORTANT]
> Proyek ini dibuat **HANYA UNTUK TUJUAN EDUKASI**. Jangan gunakan alat ini untuk mengakses file atau sistem tanpa izin yang sah. Penulis tidak bertanggung jawab atas penyalahgunaan alat ini.

---

## 👨‍💻 Kontribusi & Kredit
Dibuat sebagai bagian dari tugas:
**Bootcamp Online Cyber Security - ID-Networkers**

---

## 📜 Lisensi
Proyek ini dilisensikan di bawah [MIT License](https://opensource.org/licenses/MIT).
