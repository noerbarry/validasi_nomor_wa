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

import csv
import requests

# Fungsi untuk memvalidasi nomor WhatsApp
def validate_whatsapp_number(number):
    # ... (kode fungsi validasi nomor WhatsApp)

# Ganti dengan path file CSV Anda
csv_file_path = '/content/nomor.csv'

# ... (bagian membaca nomor telepon dari file CSV)

Fungsi validate_whatsapp_number(number)
Fungsi ini digunakan untuk memvalidasi nomor WhatsApp dengan mengirimkan permintaan ke API yang disediakan.

Parameter:

number (str): Nomor telepon yang ingin divalidasi.
Output:

Jika respons berhasil (status code 200), fungsi ini akan mengembalikan respons dalam format JSON.
Jika respons gagal, fungsi ini akan mengembalikan pesan berisi informasi bahwa permintaan gagal dengan kode status yang sesuai.
Catatan
Pastikan file CSV Anda memiliki data yang valid. Pastikan juga koneksi internet tersedia saat menjalankan program untuk melakukan permintaan ke API.

Selengkapnya : https://colab.research.google.com/drive/1O9BISXD_-MFUp0293CUzYuwQLQ2Qb-8e?usp=sharing

Semoga bermanfaat 
Jika ingin kontribusi silakan akses (https://trakteer.id/edukasi_ai/link)

