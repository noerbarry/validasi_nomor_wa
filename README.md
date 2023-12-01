# Validasi Nomor WhatsApp
Deskripsi Kode Python untuk Validasi Nomor Telepon di WhatsApp (Simulasi)
Deskripsi
Kode Python ini bertujuan untuk melakukan validasi nomor telepon di WhatsApp menggunakan API WhatsApp (hanya simulasi). Kode ini membaca daftar nomor telepon dari file CSV dan mencoba melakukan permintaan ke API WhatsApp untuk memeriksa apakah nomor tersebut aktif di WhatsApp atau tidak. Perlu diperhatikan bahwa ini hanya merupakan simulasi dan tidak mengakses langsung API WhatsApp yang sebenarnya.

# Instruksi Penggunaan
1. Pastikan Python telah terpasang di lingkungan Anda.
2. Unduh atau kloning repositori ini.
3. Persiapkan file CSV yang berisi daftar nomor telepon dengan header kolom 'Phone_Number'.
5. Ganti path file CSV pada kode dengan path file Anda.
6. Jalankan kode dengan menjalankan skrip Python pada lingkungan Anda.

![alt text](https://github.com/noerbarry/validasi_nomor_wa/blob/main/Screen%20Shot%202023-11-25%20at%2002.09.39.png?raw=true)


# Keterangan
- Kode menggunakan pustaka requests untuk membuat permintaan ke API WhatsApp (simulasi).
- Kode ini mensimulasikan respons dari API WhatsApp berdasarkan logika tertentu untuk menghasilkan hasil validasi.
- Hasil yang ditampilkan hanyalah simulasi dan tidak merepresentasikan status aktual nomor telepon di WhatsApp.



# CARA KEDUA Validasi Nomor WhatsApp REAL

## Deskripsi
Program ini memvalidasi nomor WhatsApp menggunakan API dari `pabar-validasi-nomor-wa.vercel.app`. Program ini membaca nomor telepon dari file CSV dan mengirimkan permintaan validasi nomor WhatsApp untuk setiap nomor yang dibaca.

## Penggunaan

### Instalasi
1. Pastikan Python telah terinstal di komputer Anda.
2. Pastikan sudah memasang library `requests`. Jika belum, Anda dapat memasangnya menggunakan pip dengan perintah berikut:
   ```bash
   pip install requests

## Menjalankan Kode
Pastikan Anda memiliki file CSV dengan nomor telepon yang ingin divalidasi.
Ganti csv_file_path pada kode dengan path file CSV Anda.
Jalankan kode dengan menjalankan script Python yang telah Anda buat.
 ```bash
import csv
import requests

# Fungsi untuk memvalidasi nomor WhatsApp
def validate_whatsapp_number(number):
    # ... (kode fungsi validasi nomor WhatsApp)

# Ganti dengan path file CSV Anda
csv_file_path = '/content/nomor.csv'

# ... (bagian membaca nomor telepon dari file CSV)

 

## Fungsi untuk memvalidasi nomor WhatsApp
def validate_whatsapp_number(number):
    # ... (kode fungsi validasi nomor WhatsApp)

## Ganti dengan path file CSV Anda
csv_file_path = '/content/nomor.csv'

## ... (bagian membaca nomor telepon dari file CSV)

## Fungsi validate_whatsapp_number(number)
Fungsi ini digunakan untuk memvalidasi nomor WhatsApp dengan mengirimkan permintaan ke API yang disediakan.
```
Parameter:

number (str): Nomor telepon yang ingin divalidasi.
Output:

Jika respons berhasil (status code 200), fungsi ini akan mengembalikan respons dalam format JSON.
Jika respons gagal, fungsi ini akan mengembalikan pesan berisi informasi bahwa permintaan gagal dengan kode status yang sesuai.
Catatan
Pastikan file CSV Anda memiliki data yang valid. Pastikan juga koneksi internet tersedia saat menjalankan program untuk melakukan permintaan ke API.

![alt text](https://github.com/noerbarry/validasi_nomor_wa/blob/main/Screen%20Shot%202023-11-26%20at%2010.04.21.png?raw=true)
Note : contoh file csv tersedia di github


# Cara lain dengan Export Hasilnya ke csv
![alt text](https://github.com/noerbarry/validasi_nomor_wa/blob/main/Screen%20Shot%202023-12-01%20at%2016.49.44.png)

# Validasi Nomor WhatsApp ke File CSV

Program ini menggunakan API eksternal untuk memvalidasi nomor WhatsApp yang diberikan dalam file CSV dan menyimpan hasil validasi ke dalam file CSV baru.

## Cara Penggunaan

1. Pastikan Anda memiliki Python yang terinstal di komputer Anda.
2. Unduh atau salin kode dari file `validasi_nomor_whatsapp.py`.
3. Pastikan Anda memiliki file CSV yang berisi nomor telepon yang akan divalidasi. Pastikan format nomor sesuai dengan yang diharapkan.
4. Ganti `csv_file_path` pada kode dengan lokasi dari file CSV yang ingin Anda validasi.
5. Jalankan program dengan perintah `python validasi_nomor_whatsapp.py`.
6. Hasil validasi akan disimpan ke dalam file `hasil_validasi_nomor.csv`.

## Keterangan

- Program ini menggunakan API eksternal untuk memvalidasi nomor WhatsApp.
- Setiap baris dalam file CSV hasil validasi akan memiliki dua kolom: nomor dan status.
- Jika terjadi kesalahan pada validasi nomor, pesan kesalahan yang diberikan adalah "invalid format number".
- Batas maksimal jumlah nomor yang akan diperiksa adalah 400.

## Catatan

Pastikan komputer Anda terhubung ke internet selama proses validasi nomor WhatsApp untuk memungkinkan program mengakses API eksternal.




## Selengkapnya :  
https://github.com/noerbarry/validasi_nomor_wa/blob/main/Validasi_nomor_WA.ipynb

## JIKA MENGGUNAKAN POSTMAN
### WhatsApp Number Validation - Postman Collection
Deskripsi
Koleksi ini menyediakan request untuk validasi nomor WhatsApp menggunakan endpoint
https://pabar-validasi-nomor-wa.vercel.app/api/validate.


### Langkah-langkah Penggunaan
### Instalasi dan Penggunaan
1. Pastikan Anda telah mengunduh dan menginstal aplikasi Postman.
2. Impor koleksi ini ke dalam aplikasi Postman.

### Environment Variables
Koleksi ini menggunakan beberapa environment variables:

- base_url: Berisi URL dasar untuk endpoint API.
- phone_number: Berisi nomor telepon WhatsApp yang ingin divalidasi.
- country_code: Berisi kode negara yang sesuai dengan nomor telepon yang ingin divalidasi.
- Pastikan untuk menyesuaikan nilai variabel ini sebelum mengirimkan request.

### Endpoint dan Request
- Endpoint URL: {{base_url}}/api/validate

Request
- Metode: GET
- Parameter Query:
  target: Isi dengan {{phone_number}}.
  countryCode: Isi dengan {{country_code}}.

### Pengiriman Request
1. Pastikan nilai environment variables telah diatur dengan benar.
2. Pilih request "Validate WhatsApp Number" di dalam koleksi.
3. Klik "Send" untuk mengirimkan request ke endpoint yang ditentukan.

## Semoga bermanfaat 
Jika ingin kontribusi silakan akses (https://trakteer.id/edukasi_ai/link)

