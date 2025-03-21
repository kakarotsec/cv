# Aria Fatah - CV

<a href="https://jekyll-themes.com/ariafatah0711/cv">
  <img
    src="https://img.shields.io/badge/featured%20on-JT-red.svg"
    height="20"
    alt="Jekyll Themes Shield"
  />
</a>

[![Website](https://img.shields.io/badge/Website-ariaf.my.id-blue)](https://ariaf.my.id/cv)

## 📌 Tentang
Repositori ini berisi CV saya yang dibuat menggunakan Jekyll. Template awal berasal dari [heartsker/resume](https://github.com/heartsker/resume) dan telah dimodifikasi sesuai kebutuhan.

## 🚀 Menjalankan Secara Lokal
Pastikan Jekyll sudah terinstal di sistem. Jika belum, bisa mengikuti panduan instalasi di [Jekyll Docs](https://jekyllrb.com/docs/installation/).

Jalankan perintah berikut untuk menjalankan server lokal:
```bash
jekyll serve
```
Atau dengan port dan host khusus:
```bash
jekyll serve --host 0.0.0.0 --port 4000
```

## ⚙️ Konfigurasi
Konfigurasi utama berada di `_config.yml`. Berikut beberapa pengaturan yang bisa diubah:

```yaml
title: ariaf.my.id
title_path: ariaf.my.id/cv
url: "https://ariaf.my.id"
baseurl: "/cv"
```
- **`title` atau `title_path`**: Gunakan salah satu sesuai kebutuhan.
- **`url` dan `baseurl`**: Sesuaikan jika ingin mengubah path.
- **Navigasi dan footer**: Ubah sesuai preferensi.

## 📊 Data
Untuk mengubah informasi dalam CV, edit file di dalam folder `_data/`, seperti:
- `education.yml` → Pendidikan
- `certifications.yml` → Sertifikasi
- `experience.yml` → Pengalaman Kerja
- `honors.yml` → Penghargaan
- `skills.yml` → Keterampilan

### Contoh Data Per File
#### `_data/certifications.yml`
```yaml
certifications:
  - name: IDCamp Front-End Developer Mahir
    path: cert/FE - IDCamp Mahir-14.pdf
    year: "2023"
    subcerts:
      - name: Belajar Dasar Pemrograman Web
        path: cert/dicoding/fe1_Belajar%20Dasar%20Pemrograman%20Web.pdf
        year: "2024 - 2027"
```

#### `_data/education.yml`
```yaml
educations:
  - school: "SMK Harapan Bangsa"
    link: "https://www.smkharapanbangsa.sch.id/"
    degree: "Student"
    duration: "2022 - 2025 (perkiraan)"
    major: "Teknik Komputer dan Jaringan"
    mobilitas: "networking, linux, mikrotik, cisco"
```

#### `_data/experience.yml`
```yaml
experiences:
  - title: IT Support
    company: PT Jarvis Integrasi Solusi
    link: https://www.linkedin.com/company/jarvis-integrasi-solusi/
    duration: Juli 2024 - Agustus 2024 (2 bulan)
    location: JRP4+H38, Tanah Baru, Kecamatan Beji, Kota Depok, Jawa Barat 16426
    description: |
      Saat PKL di PT Jarvis, saya membantu tim IT dalam troubleshooting, instalasi sistem, dukungan pengguna, dan pemeliharaan jaringan, meningkatkan keterampilan problem-solving serta pemahaman peran IT Support.
```

#### `_data/honors.yml`
```yaml
honors:
  - name: Olimpiade Jaringan MikroTik tingkat Nasional
    path: cert/lomba/3_ojm_2024.jpg
    date: 2024 Oct
    rank: 3rd Place Winner
```

#### `_data/skills.yml`
```yaml
skills:
  networking:
    - name: Cisco
      level: "■■■□□"
      description: Intermediate
    - name: MikroTik
      level: "■■■■□"
      description: Advanced
```

## 🛠️ Konversi ke PDF (Opsional)
Jika ingin mengonversi website ke PDF (hanya untuk uji coba, tidak digunakan di versi final), gunakan perintah berikut:
```bash
wkhtmltopdf --enable-local-file-access --print-media-type _site/index.html resume.pdf
```

## 📄 Lisensi
Proyek ini menggunakan [MIT License](https://github.com/heartsker/resume/blob/gh-pages/LICENSE).
