# PRAKTIKUM 3 BATCH DATA ANALYTICS & VISUALIZATION LAYER
<p align="center">
  <img alt="Python" src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" />
</p>

## Tim Developer

| Peran | Nama | NIM | Profil GitHub |
| :--- | :--- | :--- | :--- |
| **Pengembang Proyek** | M. Kaspul Anwar | 230104040212 | [![](https://img.shields.io/badge/GitHub-M.KaspulAnwar-181717?style=flat&logo=github)](https://github.com/mkaspulanwar) |
| **Dosen Pengampu** | Muhayat, M. IT | - | [![](https://img.shields.io/badge/GitHub-Muhayat,M.IT-181717?style=flat&logo=github)](https://github.com/muhayat-lab) |

---

## Struktur Folder Project
Struktur folder mengikuti standar data lake berlapis agar alur kerja jelas dan mudah dikembangkan.
```markdown
bigdata-project/
├── .venv
├── screenshots
├── data/
│   ├── raw/                          # Data mentah (CSV) sebagai source of truth
│   ├── clean/                        # Data bersih (Parquet) termasuk output partisi
│   │   ├── parquet/                  # Output clean utama dalam Parquet
│   │   └── partitioned_by_category/  # Output clean yang dipartisi (contoh: category)
│   └── curated/                      # Dataset terkurasi (hasil agregasi/metrik bisnis)
│       ├── category_revenue/         # Revenue per category
│       ├── top_products/             # Top produk terlaris
│       └── avg_transaction/          # Rata-rata transaksi per customer
├── logs/                             # Log eksekusi pipeline untuk debugging dan audit
└── scripts/                          # Script PySpark pipeline
    └── batch_pipeline_enterprise.py  # Script utama Week 2
```

## Bukti Screenshots

Berikut dokumentasi proses praktikum 2 batch data ingestion & processing with spark:

<table>
<tr>
<td align="center"><b>Dashboard Power BI</b></td>
<td align="center"><b>Folder Serving Dataset</b></td>
</tr>
<tr>
<td><img src="screenshots_powerbi/dashboard_powerbi.png"/></td>
<td><img src="screenshots_powerbi/data_serving.png"/></td>
</tr>

<tr>
<td align="center"><b>Script Analytics Layer</b></td>
<td align="center"><b>Script Analytics Layer</b></td>
</tr>
<tr>
<td><img src="screenshots_powerbi/analytics_layer1.png"/></td>
<td><img src="screenshots_powerbi/analytics_layer2.png"/></td>
</tr>
</table>

---
