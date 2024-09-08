# Web Scraping Assignment

## Deskripsi

Project ini bertujuan untuk melakukan web scraping dari website [Books to Scrape](http://books.toscrape.com/) untuk mengekstrak data buku seperti judul, harga, dan rating. Project ini dilakukan sebagai bagian dari tugas data engineering bootcamp.

## Teknologi yang Digunakan

- **Python**: Untuk implementasi web scraping.
- **Libraries**:
  - `requests`: Untuk mengambil halaman web.
  - `BeautifulSoup`: Untuk mem-parsing HTML dan ekstrak data.
  - `pandas`: Untuk memproses dan menyimpan data ke dalam format CSV.
- **Google Colab**: Sebagai environment untuk menjalankan kode Python.
- **GitHub**: Untuk version control dan penyimpanan hasil.

## Struktur Repository

- `Abil_Farabil - Web_scraping - Assignment.ipynb`: Notebook yang berisi kode Python untuk scraping data, baik versi awal maupun setelah perbaikan. [Link to Notebook](Abil_Farabil_Web_scraping_Assignment.ipynb)
- `books_scraped_clean.csv`: File CSV hasil scraping yang berisi data buku dengan kolom `Title`, `Price`, dan `Rating`. [Link to CSV](books_scraped_clean.csv)

## Langkah-Langkah

1. **Mengambil Data**:
   - Mengambil halaman web menggunakan `requests.get`.
   - Parsing HTML dengan `BeautifulSoup`.
   - Mengekstrak judul buku, harga, dan rating.

2. **Perbaikan Kode**:
   - **Penanganan Encoding dan Simbol Mata Uang**: Memastikan harga ditampilkan dengan simbol mata uang `£` tanpa karakter encoding tambahan.
   - **Konversi Rating dari Kata Menjadi Angka**: Rating buku dikonversi ke angka 1-5 untuk konsistensi dan kemudahan analisis.

3. **Menyimpan Hasil**:
   - Data yang diekstrak disimpan dalam bentuk DataFrame menggunakan `pandas` dan diekspor ke file `books_scraped_clean.csv`.

## Hasil Scraping

Data yang berhasil diekstrak dari website mencakup informasi berikut:
- **Title**: Judul buku.
- **Price**: Harga buku dalam Pound Sterling (£).
- **Rating**: Rating buku dalam format numerik (1-5).

## Perbaikan yang Dilakukan

- Mengatasi masalah encoding yang menyebabkan simbol tidak diinginkan pada harga buku.
- Menjaga simbol mata uang agar tetap terlihat pada kolom harga.
- Mengubah rating dari bentuk kata menjadi angka untuk memudahkan analisis data.

## File Terkait

- [Abil_Farabil - Web_scraping - Assignment.ipynb](Abil_Farabil_Web_scraping_Assignment.ipynb): Berisi kode scraping versi awal dan setelah perbaikan.
- [books_scraped_clean.csv](books_scraped_clean.csv): File CSV dengan data hasil scraping yang sudah diperbaiki.

## Cara Menjalankan Kode

1. Clone repository ini.
2. Buka file notebook `Abil_Farabil - Web_scraping - Assignment.ipynb` di Google Colab atau Jupyter Notebook.
3. Jalankan sel-sel kode untuk melihat hasil scraping dan proses perbaikan yang telah dilakukan.

## Kesimpulan

Proses scraping ini berhasil mengekstrak data buku dari website [Books to Scrape](http://books.toscrape.com/) dengan hasil yang akurat setelah dilakukan perbaikan pada encoding dan format data. File hasil (`books_scraped_clean.csv`) siap digunakan untuk analisis lebih lanjut.

## Referensi

- [Books to Scrape](http://books.toscrape.com/): Sumber data scraping.
- [BeautifulSoup Documentation](https://www.crummy.com/software/BeautifulSoup/bs4/doc/): Panduan penggunaan BeautifulSoup.
- [Requests Documentation](https://docs.python-requests.org/en/latest/): Panduan penggunaan library requests.
