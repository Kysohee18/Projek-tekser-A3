# 🎲 RandoQuest - Random Challenge 

> **Final Project Teknologi Server - Kelompok A3**
> Platform generator tantangan acak berbasis komunitas untuk kegiatan *ice breaking*. dan sesuai dengan  proposal yang ada yaitu dapat berjalan di server melalui docker
---

## Fitur Utama

Aplikasi ini mengusung konsep **Open Access** (Tanpa Login) namun tetap terkontrol.

* **🎲 Gacha Mode:** Algoritma pengacakan tantangan yang adil dan cepat.
* **📝 Open Contribution:** Siapa saja dapat menambahkan tantangan baru ke database.
* **✏️ Community Moderation:** User dapat memperbaiki *typo* atau level kesulitan secara langsung.
* **🗑️ Hard Delete:** Mekanisme penghapusan permanen untuk konten spam/tidak pantas.
* **🛡️ Secure Network:** Akses database terisolasi, hanya dapat dijangkau oleh aplikasi internal.
---

## 💻 Cara Menjalankan

Pastikan **Docker Desktop** sudah berjalan di komputer Anda.

### 1. Clone Repository
```bash
git clone [https://github.com/Kysohee18/Projek-tekser-A3.git](https://github.com/Kysohee18/Projek-tekser-A3.git)
cd Projek-tekser-A3
RUN DOCKER
docker compose up --build


.
├── database/
│   └── init.sql         # Skema Database & Data Dummy (Auto-seed)
├── nginx/
│   └── nginx.conf       # Konfigurasi Reverse Proxy & Security
├── src/                 # Source Code Backend (Node.js)
├── views/               # Source Code Frontend (EJS Views)
├── public/              # Aset Statis (CSS/Images)
├── docker-compose.yml   # Orkestrasi Service Multi-Container
└── README.md            # Dokumentasi Proyek