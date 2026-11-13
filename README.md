# Zona Rawan dan Peluang Blooming Alga – KJA Waduk Cirata

Peta web interaktif hasil penelitian tentang zona rawan dan peluang blooming alga di area keramba jaring apung (KJA) Waduk Cirata, Jawa Barat, pada grid 250 m.

- `index.html`: peta interaktif (Leaflet). Lapisan: zona rawan blooming, titik panas Getis-Ord Gi\*, frekuensi blooming per musim, peluang blooming (nowcast, prakiraan 5 dan 10 hari), ketidakpastian, indeks keterpaparan risiko, skenario iklim, NDCI teramati, dan kepadatan struktur KJA.
- `kinerja.html`: kinerja dan validasi model, uji statistik, diagnostik, dan batasan.
- `unduh/`: keluaran model dalam CSV dan GeoJSON.

## Data dan metode singkat

- Citra Sentinel-2 L1C 2016–2026 (ESA Copernicus, melalui Google Earth Engine), dikoreksi atmosfer dengan pendekatan MAIN-sederhana (Page dkk. 2019, *Remote Sensing of Environment* 231: 111284).
- Blooming didefinisikan sebagai NDCI ≥ persentil 90 periode 2016–2022. Ini anomali indeks klorofil relatif, bukan konsentrasi klorofil-a dalam µg/L.
- Iklim harian: ERA5-Land (ECMWF) dan CHIRPS (UCSB-CHG). Batas waduk: JRC Global Surface Water.
- Model: gradient boosting dengan kalibrasi isotonik; kerangka mengikuti Mahdiyasa dkk. (2026, *Natural Hazards Research*).
- Zona rawan: frekuensi blooming per sel dari seluruh pengamatan citra 2016–2026 dan statistik Getis-Ord Gi\*.

## Batasan

Peta ini hasil penelitian dan bukan peringatan resmi. Data iklim hingga 31 Oktober 2026; peta tidak diperbarui otomatis. Validasi lapangan terbatas pada data sekunder dari publikasi.
