# Buku API

Buku API adalah sebuah aplikasi berbasis Express.js yang memungkinkan pengguna untuk mengelola koleksi buku. Pengguna dapat menambahkan, mendapatkan, memperbarui, dan menghapus buku.

## Fitur

- Menambahkan buku baru
- Menampilkan seluruh daftar buku
- Menampilkan detail buku berdasarkan ID
- Memperbarui informasi buku
- Menghapus buku

## Prerequisites

- Node.js v12.x atau lebih baru
- npm (Node Package Manager)

## Instalasi

1. Clone repositori ini:
   ```bash
   git clone https://github.com/username/repo-name.git
   ```

## Masuk ke direktori proyek:

```bash
cd repo-name
```

## Instal dependensi yang dibutuhkan:

```bash
npm install
```

## Menjalankan Aplikasi

Jalankan server menggunakan perintah berikut:

```bash
npm start
```

Secara default, server akan berjalan di http://localhost:9000.

# Endpoint API

1. Menambahkan Buku
   URL: /books
   Method: POST
   Body:

```bash
{
    "name": "Judul Buku",
    "year": 2021,
    "author": "Nama Pengarang",
    "summary": "Ringkasan Buku",
    "publisher": "Penerbit",
    "pageCount": 300,
    "readPage": 150,
    "reading": true
}
```

## Response:

201 Created: Buku berhasil ditambahkan.
400 Bad Request: Kesalahan pada input data.

```bash

```

# 2. Menampilkan Daftar Buku

URL: /books
Method: GET
Response

```bash
{
    "status": "success",
    "data": {
        "books": [
            {
                "id": "id_buku",
                "name": "Judul Buku",
                "publisher": "Penerbit"
            }
        ]
    }
}
```

## Menampilkan Detail Buku

<li>
URL: /books/:bookId
</li>
<li>Method: GET</li>
<li>Response: </li>
200 OK: Jika buku ditemukan. <br>
404 Not Found: Jika buku tidak ditemukan.
 
##  Memperbarui Buku

<li>
URL: /books/:bookId
</li>
<li>Method: PUT</li>
<li><b>Body:</b> (sama seperti body untuk menambahkan buku)</li>
<li>Response: </li>
200 OK: Buku berhasil diperbarui. <br>
400 Bad Request: Kesalahan pada input data. <br>
404 Not Found: Jika buku tidak ditemukan.

## Menghapus Buku

<li>
URL: /books/:bookId
</li>
<li>Method: DELETE</li>
 
<li>Response: </li> 
200 OK: Buku berhasil dihapus.<br>
404 Not Found: Jika buku tidak ditemukan.

```
Pengujian
Anda dapat menggunakan alat seperti Postman atau cURL untuk menguji API ini dengan mengirimkan permintaan sesuai dengan endpoint yang telah disebutkan di atas.

Lisensi
Proyek ini dilisensikan di bawah MIT License - lihat file LICENSE untuk detail lebih lanjut.

Penulis
Samuel-06
```
