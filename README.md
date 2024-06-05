# Palm-vein-detection

Repository ini digunakan untuk memnuhi tugas pengelolahan citra digital

# Identifikasi Pembuluh Darah Vena pada Telapak Tangan

Proyek ini mengimplementasikan identifikasi pembuluh darah telapak tangan menggunakan teknik pengolahan citra dengan Jupyter. Proyek ini menggunakan OpenCV dan SciPy untuk memproses citra dan mengekstrak fitur-fitur pembuluh darah.

## Daftar Isi

- [Instalasi](#instalasi)
- [Penggunaan](#penggunaan)
- [Fitur](#fitur)
- [Kontribusi](#kontribusi)

## Instalasi

1. Clone repositori ini:
    ```bash
    git clone https://github.com/MHafidafandi/Palm-vein-detection
    ```
2. Masuk ke direktori proyek:
    ```bash
    cd palm-vein-detection
    ```
3. Buat virtual environment:
    ```bash
    python -m venv env
    ```
4. Aktifkan virtual environment:
    - Windows:
      ```bash
      .\env\Scripts\activate
      ```
    - MacOS/Linux:
      ```bash
      source env/bin/activate
      ```
5. Instal dependensi yang diperlukan:
    ```bash
    pip install -r requirements.txt
    ```

## Penggunaan

1. Pastikan Anda sudah menginstal semua dependensi.
2. Jalankan script utama di Jupyter Notebook atau simpan dalam file Python dan jalankan:
    ```bash
    python Main.py
    ```

## Fitur

- **Peningkatan Kontras**: Meningkatkan kontras citra untuk memperjelas pembuluh darah.
- **Konversi Grayscale**: Mengubah citra RGB menjadi grayscale.
- **Segmentasi Citra**: Menerapkan threshold untuk membuat citra biner.
- **Deteksi Kontur**: Menemukan kontur pada citra biner.
- **Ekstraksi Landmark**: Menemukan titik-titik penting pada kontur.
- **Rotasi dan Penyelarasan**: Menyelaraskan citra berdasarkan landmark.
- **Ekstraksi ROI**: Mengekstraksi region of interest (ROI) dari citra yang diselaraskan.
- **Filter Gabor**: Menerapkan filter Gabor untuk menonjolkan pembuluh darah.
- **Normalisasi dan CLAHE**: Menormalkan citra dan menerapkan CLAHE untuk meningkatkan kontras lokal.
- **Binarisasi**: Mengubah citra hasil CLAHE menjadi citra biner.

## Kontribusi

Kontribusi sangat terbuka! Silakan fork repositori ini dan buat pull request dengan perubahan yang ingin Anda ajukan.

1. Fork repositori ini.
2. Buat branch fitur (`git checkout -b fitur-anda`).
3. Commit perubahan Anda (`git commit -m 'Menambahkan fitur'`).
4. Push ke branch (`git push origin fitur-anda`).
5. Buat pull request.