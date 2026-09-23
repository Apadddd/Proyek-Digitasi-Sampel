# Proyek-Digitasi-Sampel

## 📖 Tentang Proyek
Proyek ini bertujuan untuk melakukan pemetaan area persawahan, lebih tepatnya berfokus pada sawah padi di Kecamatan Sugio, Kabupaten Lamongan. Setelah tahapan pemetaan spasial dan digitasi area (poligon) diselesaikan menggunakan perangkat lunak QGIS, alur kerja proyek ini dirancang agar dapat dilanjutkan ke tahap ekstraksi *dataset*. Pembuatan *dataset* tersebut memanfaatkan *plugin* Deepness untuk menghasilkan data latih berbasis citra spasial.

## 📂 Struktur File (Sampel Pengerjaan)
Repositori ini memuat beberapa file yang menjadi representasi sebagian (*sample*) dari hasil pengerjaan, di antaranya:
*   **`Digitasi.qgz`**: File *project* utama QGIS yang menyimpan ruang kerja pemetaan.
*   **`Petak 1.shp`, `.dbf`, `.prj`, `.shx`**: Kesatuan data *shapefile* (vektor) yang memuat hasil digitasi petak sawah.
*   **`Sugio_01.jpg` & `Sugio_01.kmz`**: File citra serta referensi spasial.
*   **`Sugio_01_modified.tif.aux.xml`**: File *metadata* untuk citra raster TIFF.
*   **`tile_img_0_1.png` & `tile_mask_0_1.png`**: Sampel hasil *dataset* citra dan *masking* (*defect*/target area) yang telah diekstrak.

## 🚀 Langkah Penggunaan (Manual Book)

Berikut adalah tata cara untuk membuka dan mengoperasikan proyek pemetaan ini:

1. **Persiapan Perangkat Lunak**: Pastikan Anda telah mengunduh dan menginstal aplikasi QGIS versi terbaru melalui web resminya (https://qgis.org/).
2. **Unduh Proyek**: Unduh repositori ini dalam bentuk arsip dengan menekan tombol **Code > Download ZIP** pada halaman GitHub.
3. **Ekstrak File**: Ekstrak file `.zip` yang telah diunduh ke dalam direktori lokal di komputer Anda.
4. **Buka Project QGIS**: Buka folder hasil ekstraksi tersebut, lalu lakukan klik ganda (*double-click*) pada file bernama `Digitasi.qgz`. Jika asosiasi file sudah benar, QGIS akan otomatis terbuka dan memuat layer pemetaan.
5. **Pembuatan Dataset dengan Deepness**: 
   - Apabila pengguna (*user*) ingin melakukan proses pembuatan *dataset* lanjutan dari hasil digitasi, pengguna wajib menginstal *plugin* **Deepness**.
   - Instalasi dapat dilakukan di dalam QGIS melalui menu **Plugins > Manage and Install Plugins**, lalu cari "Deepness" dan pasang.
