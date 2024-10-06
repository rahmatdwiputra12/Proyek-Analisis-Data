# Dashboard
Proyek ini menyediakan dashboard berbasis Python yang bisa dijalankan di komputer lokal atau di Google Colab.

## Prasyaratan

Sebelum menjalankan dashboard, pastikan kamu sudah memenuhi beberapa syarat:
-Python 3.x: Pastikan kamu sudah menginstal versi Python yang sesuai.
-Library Python yang dibutuhkan: Instal semua library yang diperlukan menggunakan pip.
-Untuk menginstal semua dependensi yang dibutuhkan, jalankan perintah ini di terminal:
pip install -r requirements.txt

## Langkah Menjalankan di Komputer Lokal
-Unduh atau clone repositori yang berisi file dashboard.py atau cukup download file tersebut.
-Instal dependensi dengan menjalankan perintah berikut:
pip install -r requirements.txt
-Setelah semua dependensi terpasang, jalankan script dashboard dengan perintah:
python dashboard.py
-Buka browser, dan akses alamat lokal yang ditunjukkan (biasanya http://127.0.0.1:8050 atau serupa) untuk melihat tampilan dashboard.

## Langkah Menjalankan di Google Colab
-Unggah file dashboard.py ke sesi Google Colab yang kamu buka.
-Instal library yang dibutuhkan di dalam notebook Colab dengan menjalankan perintah berikut:
-Jalankan script dashboard.py di dalam Colab menggunakan perintah:
!python dashboard.py
-Akses dashboard di Colab: Agar dashboard bisa diakses, kamu perlu menggunakan ngrok untuk membuat alamat publik. Instal library pyngrok terlebih dahulu:
!pip install pyngrok
-Impor dan setup ngrok untuk menghubungkan dashboard ke alamat publik:
from pyngrok import ngrok
public_url = ngrok.connect(8050)
print(f"Dashboard bisa diakses di {public_url}")
