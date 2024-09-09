# Web Scraping & GraphQL Assignment

## Deskripsi

Project ini bertujuan untuk melakukan web scraping dari website [Books to Scrape](http://books.toscrape.com/) dan menggunakan GraphQL API untuk mengakses data negara dari [Countries GraphQL API](https://countries.trevorblades.com/). Project ini dilakukan sebagai bagian dari tugas data engineering bootcamp.

## Teknologi yang Digunakan

- **Python**: Untuk implementasi web scraping dan penggunaan GraphQL.
- **Libraries**:
  - `requests`: Untuk mengambil halaman web dan API.
  - `BeautifulSoup`: Untuk mem-parsing HTML dan ekstrak data dari website.
  - `pandas`: Untuk memproses dan menyimpan data ke dalam format CSV.
- **Google Colab**: Sebagai environment untuk menjalankan kode Python.
- **GitHub**: Untuk version control dan penyimpanan hasil.

## Struktur Repository

- `Abil_Farabil_Web_scraping_GraphQL_Assignment.ipynb`: Notebook yang berisi kode Python untuk scraping data buku dan penggunaan GraphQL API. [Link to Notebook](Abil_Farabil_Web_scraping_GraphQL_Assignment.ipynb)
- `books_scraped_clean.csv`: File CSV hasil scraping dari website Books to Scrape. [Link to CSV](books_scraped_clean.csv)
- `countries_data.csv`: File CSV hasil query GraphQL yang berisi data negara, benua, dan bahasa. [Link to CSV](countries_data.csv)

## Langkah-Langkah

### 1. **Mengambil Data Buku**
   - Mengambil halaman web menggunakan `requests.get`.
   - Parsing HTML dengan `BeautifulSoup`.
   - Mengekstrak judul buku, harga, dan rating.

### 2. **Perbaikan Kode Scraping Buku**
   - **Penanganan Encoding dan Simbol Mata Uang**: Memastikan harga ditampilkan dengan simbol mata uang `£` tanpa karakter encoding tambahan.
   - **Konversi Rating dari Kata Menjadi Angka**: Rating buku dikonversi ke angka 1-5 untuk konsistensi dan kemudahan analisis.

### 3. **Mengambil Data Negara dengan GraphQL**
   - Menggunakan [Countries GraphQL API](https://countries.trevorblades.com/) untuk mengambil data negara, kode, benua, dan bahasa.
   - Menulis query GraphQL untuk mengambil data dan memproses hasil dengan `pandas`.
   - Menyimpan hasil dalam file CSV `countries_data.csv`.

## Hasil Scraping dan GraphQL

### Data Buku:
Data yang berhasil diekstrak dari website mencakup informasi berikut:
- **Title**: Judul buku.
- **Price**: Harga buku dalam Pound Sterling (£).
- **Rating**: Rating buku dalam format numerik (1-5).

### Data Negara:
Data negara yang diambil melalui GraphQL mencakup:
- **Code**: Kode negara.
- **Name**: Nama negara.
- **Continent**: Benua tempat negara berada.
- **Language**: Bahasa yang digunakan di negara tersebut.

### Visualisasi

**Proses Web Scraping dan GraphQL:**
![Diagram Alur](images/diagram_alur_proses.png)

**Contoh Hasil CSV:**
![Hasil CSV](images/screenshot_countries_data.png)

## Perbaikan yang Dilakukan

- Mengatasi masalah encoding yang menyebabkan simbol tidak diinginkan pada harga buku.
- Menjaga simbol mata uang agar tetap terlihat pada kolom harga.
- Mengubah rating dari bentuk kata menjadi angka untuk memudahkan analisis data.
- Menggunakan prefix pada nama kolom untuk menghindari konflik nama saat menggunakan GraphQL.

## File Terkait

- [Abil_Farabil_Web_scraping_GraphQL_Assignment.ipynb](Abil_Farabil_Web_scraping_GraphQL_Assignment.ipynb): Berisi kode scraping versi awal dan setelah perbaikan, serta penggunaan GraphQL.
- [books_scraped_clean.csv](books_scraped_clean.csv): File CSV dengan data hasil scraping yang sudah diperbaiki.
- [countries_data.csv](countries_data.csv): File CSV hasil query GraphQL yang berisi data negara.

## Cara Menjalankan Kode

1. Clone repository ini.
2. Buka file notebook `Abil_Farabil_Web_scraping_GraphQL_Assignment.ipynb` di Google Colab atau Jupyter Notebook.
3. Jalankan sel-sel kode untuk melihat hasil scraping, penggunaan GraphQL, dan proses perbaikan yang telah dilakukan.

## Kesimpulan

Proses scraping ini berhasil mengekstrak data buku dari website [Books to Scrape](http://books.toscrape.com/) dan mengambil data negara menggunakan GraphQL API. Hasil yang diperoleh akurat dan siap digunakan untuk analisis lebih lanjut.

## Referensi

- [Books to Scrape](http://books.toscrape.com/): Sumber data scraping.
- [Countries GraphQL API](https://countries.trevorblades.com/): Sumber data GraphQL.
- [BeautifulSoup Documentation](https://www.crummy.com/software/BeautifulSoup/bs4/doc/): Panduan penggunaan BeautifulSoup.
- [Requests Documentation](https://docs.python-requests.org/en/latest/): Panduan penggunaan library requests.
- [GraphQL Documentation](https://graphql.org/learn/): Panduan dasar penggunaan GraphQL.
