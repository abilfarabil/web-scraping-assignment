# Web Scraping & GraphQL Assignment

## Deskripsi

Project ini bertujuan untuk melakukan web scraping dari website [Books to Scrape](http://books.toscrape.com/) untuk mengekstrak data buku serta menggunakan GraphQL API untuk mengakses data negara dari [Countries GraphQL API](https://countries.trevorblades.com/). Project ini dikembangkan sebagai bagian dari tugas data engineering bootcamp dan menjadi portofolio saya dalam bidang data engineering.

## Teknologi yang Digunakan

- **Python**: Untuk implementasi web scraping dan GraphQL.
- **Libraries**:
  - `requests`: Untuk mengambil halaman web dan API.
  - `BeautifulSoup`: Untuk parsing HTML dan ekstrak data dari website.
  - `pandas`: Untuk memproses dan menyimpan data ke dalam format CSV.
- **Google Colab**: Sebagai environment untuk menjalankan kode Python.
- **GitHub**: Untuk version control dan penyimpanan hasil.

## Struktur Repository

- `Abil_Farabil - Web_scraping - GraphQL - Assignment.ipynb`: Notebook yang berisi kode Python untuk web scraping dan penggunaan GraphQL API. [Link to Notebook](Abil_Farabil_Web_scraping_GraphQL_Assignment.ipynb)
- `books_scraped_clean.csv`: File CSV hasil scraping dari website Books to Scrape, berisi data buku dengan kolom `Title`, `Price`, dan `Rating`. [Link to CSV](data/books_scraped_clean.csv)
- `countries_data.csv`: File CSV hasil query GraphQL yang berisi data negara dengan kolom `Code`, `Name`, `Continent`, dan `Language`. [Link to CSV](data/countries_data.csv)

## Langkah-Langkah

### 1. Mengambil Data Buku dari Books to Scrape
   - **Proses**: Mengambil halaman web menggunakan `requests.get`, parsing HTML dengan `BeautifulSoup`, dan mengekstrak data buku.
   - **Output**: Menampilkan beberapa baris data hasil scraping yang disimpan dalam `books_scraped_clean.csv`.

   ![Screenshot Kode Scraping Buku](images/1_Kode_Scraping_Buku.png)
   ![Screenshot Kode Scraping Buku](images/2_Kode_Scraping_Buku.png)

### 2. Hasil Data Buku
   - **Deskripsi**: Hasil scraping buku disimpan dalam format CSV dengan kolom `Title`, `Price`, dan `Rating`.
   
   ![Hasil Data Buku](images/3_Hasil_Data_Buku.png)

### 3. Mengambil Data Negara Menggunakan GraphQL
   - **Proses**: Menggunakan [Countries GraphQL API](https://countries.trevorblades.com/) untuk mengambil data negara, kode, benua, dan bahasa.
   - **Output**: Menampilkan data hasil query GraphQL yang diproses menjadi DataFrame.

   ![Screenshot Kode GraphQL](images/4_Kode_GraphQL.png)
   ![Screenshot Kode GraphQL](images/5_Kode_GraphQL.png)

### 4. Hasil Data Negara
   - **Deskripsi**: Hasil query GraphQL disimpan dalam format CSV dengan kolom `Code`, `Name`, `Continent`, dan `Language`.

   ![Hasil Data Negara](images/6_Hasil_Data_Negara.png)

## Kesimpulan

Proses scraping ini berhasil mengekstrak data buku dari website [Books to Scrape](http://books.toscrape.com/) dan mengambil data negara menggunakan GraphQL API dari [Countries GraphQL API](https://countries.trevorblades.com/). Hasil yang diperoleh akurat dan siap digunakan untuk analisis lebih lanjut. Project ini menunjukkan kemampuan dalam menggunakan berbagai teknik untuk mengakses dan memproses data dari sumber yang berbeda, serta mendokumentasikan hasil secara profesional di GitHub.

## Referensi

- [Books to Scrape](http://books.toscrape.com/): Sumber data scraping buku.
- [Countries GraphQL API](https://countries.trevorblades.com/): Sumber data negara melalui GraphQL.
- [BeautifulSoup Documentation](https://www.crummy.com/software/BeautifulSoup/bs4/doc/): Panduan penggunaan BeautifulSoup.
- [Requests Documentation](https://docs.python-requests.org/en/latest/): Panduan penggunaan library requests.
- [GraphQL Documentation](https://graphql.org/learn/): Panduan dasar penggunaan GraphQL.
