# Contributing Guide

Terima kasih sudah berkontribusi pada repository **Praktikum 3 Teknologi Big Data — Batch Data Analytics + Visualization Layer**.

Dokumen ini menjelaskan cara berkontribusi dengan rapi, aman, dan konsisten agar struktur project tetap terjaga.

## Tujuan Repository

Repository ini digunakan untuk mendokumentasikan hasil praktikum yang berfokus pada:

- Analytics Layer dengan PySpark
- Serving Layer dalam format CSV
- Visualization Layer dengan Pandas + Matplotlib
- Dashboard KPI menggunakan Power BI

## Aturan Umum Kontribusi

Sebelum melakukan perubahan, pastikan bahwa:

- Struktur folder project tetap rapi
- Perubahan relevan dengan praktikum 3
- Script dapat dijalankan ulang tanpa error
- File yang tidak perlu seperti virtual environment tidak ikut ter-push
- Output yang dihasilkan tetap sesuai dengan modul praktikum
## Cara Berkontribusi

### 1. Fork atau Clone Repository
Clone repository ke lokal:
```bash
git clone <url-repository>
cd bigdata-project
```
### 2. Aktifkan Environment
Gunakan virtual environment yang sudah disiapkan:
```bash
source .venv/bin/activate
```
### 3. Buat Branch Baru
Gunakan branch terpisah untuk setiap perubahan.

Contoh:
```bash
git checkout -b feat/update-visualization

# atau

git checkout -b fix/analytics-script

# atau

git checkout -b docs/update-readme
```
### 4. Pastikan Script Bisa Dijalankan
Sebelum commit, pastikan perubahan dapat dijalankan ulang.

Untuk analytics layer:
```bash
python scripts/analytics_layer.py
```
Untuk visualization layer:
```bash
python scripts/visualization_layer.py
```
Pastikan output terbentuk sesuai harapan, misalnya:
```bash
data/serving/total_revenue/
data/serving/top_products/
data/serving/category_revenue/
data/serving/avg_transaction/
reports/category_revenue.png
```
### 5. Commit dengan Pesan yang Jelas
Gunakan format commit yang singkat dan deskriptif.

Contoh:
```bash
git add .
git commit -m "feat: add visualization layer script"
```
Contoh lain:
```bash
git commit -m "fix: correct total revenue formatting for power bi"
git commit -m "docs: update readme praktikum 3"
git commit -m "chore: clean gitignore and remove venv tracking"
```
### 6. Push ke Branch
```bash
git push origin nama-branch
```
## Standar Perubahan yang Diperbolehkan
Kontribusi diperbolehkan untuk hal-hal berikut:

- Perbaikan script analytics
- Perbaikan script visualisasi
- Penambahan dokumentasi
- Perbaikan README
- Penataan struktur screenshot
- Perbaikan .gitignore
- Penyempurnaan dashboard dan dokumentasi hasil

## Hal yang Sebaiknya Tidak Di-push
Jangan push file atau folder berikut:

- .venv/
- __pycache__/
- *.pyc
- *:Zone.Identifier
- file sementara editor
- file hasil cache yang tidak dibutuhkan

Contoh isi `.gitignore` yang direkomendasikan:
```bash
.venv/
__pycache__/
*.pyc
*:Zone.Identifier
```
## Panduan Dokumentasi
Jika kamu menambahkan dokumentasi atau screenshot, pastikan:

- Nama file jelas dan konsisten
- Screenshot mudah dipahami
- Dashboard terlihat utuh
- Folder output `data/serving` terdokumentasi
- Terminal execution disertakan bila perlu

Contoh nama file screenshot yang baik:

- analytics_layer_terminal.png
- data_serving_folder.png
- dashboard_powerbi.png
- category_revenue_plot.png

## Checklist Sebelum Push
Sebelum push, cek kembali:

- Script berjalan tanpa error
- Struktur folder tetap rapi
- Tidak ada `.venv` yang ikut ter-track
- Tidak ada file `Zone.Identifier`
- README dan dokumentasi sudah diperbarui jika perlu
- Output praktikum tetap sesuai tujuan

## Pelaporan Masalah
Jika menemukan masalah, catat dengan jelas:

- bagian yang error
- pesan error
- langkah untuk mereproduksi
- screenshot jika diperlukan

## Catatan
Kontribusi yang baik adalah kontribusi yang:

- mudah dipahami
- dapat dijalankan ulang
- tidak merusak struktur project
- membantu memperjelas proses praktikum dan hasil akhir

Terima kasih sudah menjaga repository ini tetap rapi dan profesional.
