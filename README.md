# Studi Kasus: Sinergi IMK & Visualisasi Data Risiko Cuaca Sumatera

Berdasarkan kuliah umum **"Human-Computer Interaction & Data Visualization"** dalam rangkaian *Informatics Practitioner Lecture Series* (19 Oktober 2026) oleh **Dr. Arafat Febriandirza** (Senior Researcher & Chief of Research Group for Human-Computer Interaction & Visualization, **Badan Riset dan Inovasi Nasional / BRIN** — diselenggarakan oleh Program Studi Informatika, **Universitas Bengkulu**).

Pesan utama materi: visualisasi data yang efektif membutuhkan prinsip Interaksi Manusia dan Komputer (IMK) yang berpusat pada pengguna (*User-Centered Design* / *"Pengguna bukanlah Anda"*), memahami keterbatasan memori kerja manusia ($7 \pm 2$ *chunk*), memanfaatkan *preattentive visual attributes*, menerapkan prinsip persepsi Gestalt, serta mematuhi standar aksesibilitas **WCAG (POUR)** dan etika visualisasi tanpa manipulasi skala.

## Hubungan dengan Materi

| Poin Materi Kuliah Umum | Implementasi pada Proyek Ini |
| :--- | :--- |
| **User-Centered Design (UCD) & *User Persona*** | Menyediakan 3 mode *User Persona* interaktif (*Warga & Lansia*, *Stakeholder Daerah/BPBD*, dan *Peneliti BRIN*) yang mengubah penyajian informasi sesuai kebutuhan pengguna |
| **Psikologi Kognitif ($7 \pm 2$ *Chunk* & *Preattentive Attributes*)** | Mereduksi tabel data mentah multi-variabel menjadi 4 *chunk* kategori risiko dengan kode warna, ukuran titik, dan simbol bentuk redundan (`✓`, `▲`, `◆`, `■`) |
| **Prinsip Persepsi Gestalt** | Menerapkan *Enclosure*, *Proximity*, *Similarity*, dan *Figure/Ground* pada pengelompokan kontrol filter, KPI, dan peta interaktif |
| **Aksesibilitas WCAG (POUR) & Keberagaman Pengguna** | Audit matematis rasio kontras luminansi WCAG 2.1 ($\ge 7.0:1$ / lulus AAA), tombol **Palet Ramah Buta Warna (Okabe-Ito)**, dan **Mode Teks Besar (A+)** untuk lansia |
| **5 Prinsip Desain Interaksi & Etika Visualisasi** | Umpan balik (*feedback*) instan pada setiap filter, *affordance* tombol yang jelas, serta grafik batang berskala jujur (*zero-baseline*) tanpa *dark patterns* |
| **Otomasi Cloud** | GitHub Actions memperbarui data hidrometeorologi dari API Open-Meteo setiap 6 jam secara otomatis |

## Menjalankan Secara Lokal

```bash
pip install -r requirements.txt
python pipeline_hci_vis.py
