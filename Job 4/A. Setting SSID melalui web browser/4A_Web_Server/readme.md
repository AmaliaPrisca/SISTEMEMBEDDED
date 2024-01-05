# A. Setting SSID dan Password Wi-Fi ESP32 melalui Web Server

### a. Rangkaian dan Flowchart
Rangkaian pada percobaan ini adalah sebagai berikut

![job4 a](https://github.com/AmaliaPrisca/SISTEMEMBEDDED/assets/145273945/7aafe1e9-3dd1-4b4a-8c5b-857617709292)

### b. Source Code
Kode program : <a href="https://github.com/AmaliaPrisca/SISTEMEMBEDDED/blob/master/Job%204/A.%20Setting%20SSID%20melalui%20web%20browser/4A_Web_Server/4A_Web_Server.ino">klik di sini</a>

### c. Hasil dan Pembahasan
<p align="justify">Percobaan A, melakukan pengaturan SSID dan password Wi-Fi pada ESP32 melalui sebuah Web Server. ESP32 akan menampilkan daftar SSID Wi-Fi yang tersedia di serial monitor. Program berupaya untuk terhubung ke jaringan Wi-Fi yang telah disimpan di EEPROM, yang merupakan memori non-volatile. Jika koneksi Wi-Fi tidak berhasil atau tombol fisik pada pin D15 (GPIO15) ditekan, program akan memulai proses konfigurasi sebagai titik akses (Access Point) untuk mengonfigurasi ulang kredensial Wi-Fi. Terdapat beberapa fungsi utama, seperti testWifi(void) yang menguji koneksi Wi-Fi dan melaporkan statusnya, launchWeb(void) yang membuka server web lokal untuk konfigurasi Wi-Fi, setupAP(void) yang menginisialisasi titik akses jika koneksi ke jaringan Wi-Fi tidak dapat dilakukan atau tombol fisik ditekan, dan createWebServer(void) yang membuat halaman web untuk konfigurasi kredensial Wi-Fi, termasuk tombol pemindaian jaringan Wi-Fi dan formulir untuk mengatur SSID serta kata sandi Wi-Fi baru. Implementasi menggunakan library WebServer untuk membuat server web lokal pada port 80.


### d. Hasil Setting SSID dan Password Wi-Fi ESP32 melalui Web Server
#### a. ![1](https://github.com/AmaliaPrisca/SISTEMEMBEDDED/assets/145273945/f22b0dcb-4424-4615-ab39-0188e639228d)
#### b. ![2](https://github.com/AmaliaPrisca/SISTEMEMBEDDED/assets/145273945/8fe77da1-10ca-4af1-845f-c64a656030b2)
#### c. ![3](https://github.com/AmaliaPrisca/SISTEMEMBEDDED/assets/145273945/1e430bd3-76bd-43f8-bd9a-f845e6eaad4e)



