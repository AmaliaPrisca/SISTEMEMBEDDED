# JOBSHEET 2.1 -  JARINGAN SENSOR NIRKABEL MENGGUNAKAN ESP-NOW
## Tujuan
1) Mahasiswa dapat memahami konsep topologi jaringan sensor nirkabel berbasis ESP-NOW.
2) Mahasiswa dapat melakukan konfigurasi berbagai topologi ESP-NOW.
3) Mahasiswa dapat menganalisis dan menentukan topologi ESP-NOW,sesuai dengan studi kasus proyek

## Dasar Teori
<p align="justify">ESP-NOW adalah protokol yang dikembangkan oleh Espressif, yang memungkinkan banyak 
perangkat untuk berkomunikasi satu sama lain tanpa menggunakan Wi-Fi. Protokol ini mirip 
dengan konektivitas nirkabel 2.4GHz berdaya rendah. Pendifinisian alamat (MAC Address) 
pada masing-masing ESP32 diperlukan pada awal konfigurasi. Setelah konfigurasi alamat 
selesai dilakukan, jaringan peer-to-peer akan terbentuk dan perangkat tidak perlu melakukan 
handshaking kembali ketika akan berkomunikasi. Hal ini memunjukkan bahwa setelah 
perangkat ESP32 saling terpasang satu sama lain, koneksi akan tetap ada. Dengan kata lain, 
jika tiba-tiba salah satu ESP32 kehilangan daya atau diatur ulang, ketika restart, secara 
otomatis akan terhubung ke pasangan ESP32 yang telah terdefinisi alamatnya untuk 
melanjutkan komunikasi.


**Sub-job** pada jobsheet ini, antara lain:
##### A. Memperoleh MAC Address ESP32 Receiver
##### B. ESP-NOW One-Way Point-to-Point Communication
##### C. One-Way, One-to-Many Communication
##### D. One-Way, Many-to-One Communication
##### E. Two-Way Communication


## Alat dan Bahan
**Alat dan bahan** yang digunakan dalam jobsheet ini, antara lain:
1) ESP32
2) Breadboard
3) Kabel jumper
4) Resistor 10K Ohm
   
> [!NOTE]  
> *Buka folder-folder subjob untuk melihat laporan percobaan*
