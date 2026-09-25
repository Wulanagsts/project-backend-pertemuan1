# Backend API Service — Dasar Pemrograman Backend (KK112105)

Proyek REST API sederhana menggunakan **Flask**, dibuat untuk mata kuliah **Dasar Pemrograman Backend (KK112105)** — STIKOM PGRI Banyuwangi.

Tugas ini merupakan **Praktikum Mandiri 1**, dengan penambahan endpoint `/api/v1/status` pada proyek Flask pertemuan 1.

## 📋 Deskripsi

Aplikasi ini menyediakan beberapa endpoint REST API yang menampilkan informasi status server, data akademik, dan profil mahasiswa (dummy) dalam format JSON.

## 🛠️ Teknologi

- Python 3
- Flask

## 📁 Struktur Proyek

```
.
├── app.py
├── requirements.txt
├── .gitignore
└── README.md
```

## ⚙️ Instalasi & Menjalankan

1. **Clone repository**
   ```bash
   git clone <url-repository-anda>
   cd <nama-folder>
   ```

2. **Buat virtual environment (opsional tapi disarankan)**
   ```bash
   python -m venv venv
   source venv/bin/activate      # Linux/Mac
   venv\Scripts\activate         # Windows
   ```

3. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

4. **Jalankan aplikasi**
   ```bash
   python app.py
   ```

5. Aplikasi akan berjalan di `http://127.0.0.1:5000`

## 📡 Daftar Endpoint

| Method | Endpoint             | Deskripsi                                      |
|--------|-----------------------|-------------------------------------------------|
| GET    | `/`                    | Root / health check service                    |
| GET    | `/api/v1/info`         | Informasi akademik & perkuliahan                |
| GET    | `/api/v1/mahasiswa`    | Profil data mahasiswa (dummy)                   |
| GET    | `/api/v1/status`       | Status operasional server (waktu & versi Python)|

### Contoh Response `/api/v1/status`

```json
{
  "status": "success",
  "data": {
    "server_status": "operational",
    "timestamp": "2026-09-25T10:00:00.000000+00:00",
    "python_version": "3.x.x"
  }
}
```

## 👤 Informasi Mahasiswa

- **Mata Kuliah:** Dasar Pemrograman Backend (KK112105)
- **Institusi:** STIKOM PGRI Banyuwangi
- **Tugas:** Praktikum Mandiri 1 — Penambahan endpoint `/api/v1/status`

## 📄 Lisensi

Proyek ini dibuat untuk keperluan tugas akademik.