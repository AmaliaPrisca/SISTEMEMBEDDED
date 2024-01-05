<<<<<<< HEAD:Job 4/Job 4/A. Setting SSID melalui web browser/readme.md
# A.  Setting SSID dan Password Wi-Fi ESP32 melalui Web Server


### a. Rangkaian dan flowchart
Rangkaian pada percobaan ini adalah sebagai berikut

![1](https://github.com/Muhmdwild/Sistem-Embeded/assets/150982519/05287890-4b87-4390-9368-c54fc4187734)

</br>


### b. Source Code
Kode program : <a href="A.%20Setting%20SSID%20melalui%20web%20browser/4A_Web_Server">di sini</a>

### c. Hasil dan Pembahasan
Pada percobaan A, melakukan pengaturan SSID dan password Wi-Fi pada ESP32 melalui sebuah Web Server. ESP32 akan menampilkan daftar SSID Wi-Fi yang tersedia di serial monitor. Program berupaya untuk terhubung ke jaringan Wi-Fi yang telah disimpan di EEPROM, yang merupakan memori non-volatile. Jika koneksi Wi-Fi tidak berhasil atau tombol fisik pada pin D15 (GPIO15) ditekan, program akan memulai proses konfigurasi sebagai titik akses (Access Point) untuk mengonfigurasi ulang kredensial Wi-Fi. Terdapat beberapa fungsi utama, seperti testWifi(void) yang menguji koneksi Wi-Fi dan melaporkan statusnya, launchWeb(void) yang membuka server web lokal untuk konfigurasi Wi-Fi, setupAP(void) yang menginisialisasi titik akses jika koneksi ke jaringan Wi-Fi tidak dapat dilakukan atau tombol fisik ditekan, dan createWebServer(void) yang membuat halaman web untuk konfigurasi kredensial Wi-Fi, termasuk tombol pemindaian jaringan Wi-Fi dan formulir untuk mengatur SSID serta kata sandi Wi-Fi baru. Implementasi menggunakan library WebServer untuk membuat server web lokal pada port 80.

![1](https://github.com/Muhmdwild/Sistem-Embeded/assets/150982519/90d8a9bf-db1f-4aad-b66f-fe88727a9fec)

![2](https://github.com/Muhmdwild/Sistem-Embeded/assets/150982519/7726b4f4-7469-4534-8956-c934cbda5835)

![3](https://github.com/Muhmdwild/Sistem-Embeded/assets/150982519/23f7e16a-b775-42fa-9f20-e68a666146a6)
=======
# JOBSHEET 4 -  TRANSMISI DATA MENGGUNAKAN PROTOKOL HTTP DAN MQTT
## Tujuan
1) Mahasiswa dapat memahami cara kerja protokol HTTP dan MQTT untuk 
transmisi data (akuisisi data dan kendali) pada Platform IoT Node-Red.
2) Mahasiswa dapat merancang dan melakukan konfigurasi pada perangkat 
Internet of Things (IoT) menggunakan protokol HTTP dan MQTT untuk 
monitoring dan kendali melalui Platform IoT Node-Red.


## Dasar Teori
<p align="justify">Internet of Things (IoT) telah mengubah cara kita terhubung dengan perangkat sehari-hari, memungkinkan segala sesuatu, mulai dari mobil hingga peralatan rumah tangga, untuk terkoneksi ke internet. Platform IoT merupakan lingkungan yang memungkinkan pengembangan produk dan solusi IoT dengan efisiensi. Ini melibatkan pengumpulan, penyimpanan, visualisasi, dan manajemen data dari berbagai sumber, serta kontrol perangkat.

<p align="justify">Sebelum membangun platform IoT, ada beberapa pertimbangan penting, seperti protokol komunikasi yang digunakan, jenis koneksi, jaringan yang akan diadopsi, dan format data. HTTP merupakan protokol jaringan yang umum digunakan untuk sistem informasi terdistribusi dan pengelolaan website. Di sisi lain, MQTT adalah protokol komunikasi yang ringan, dirancang untuk komunikasi mesin ke mesin (M2M). MQTT bersifat open source, memiliki overhead protokol rendah, dan cocok untuk transmisi data dari node sensor ke server, dengan konsumsi daya rendah, kinerja baik pada latency tinggi, dan bandwidth kecil..</p>


**Sub-job** pada jobsheet ini, antara lain:
1. Setting SSID dan Password Wi-Fi ESP32 melalui Web Server


## Alat dan Bahan
**Alat dan bahan** yang digunakan dalam jobsheet ini, antara lain:
1) ESP32 dan Server Node-Red
2) Breadboard
3) Kabel jumper
4) Sensor DHT 11
5) LED (5)
6) Resistor 330,1K Ohm (@ 3)


> [!NOTE]  
> *Buka folder-folder subjob untuk melihat laporan percobaan*
>>>>>>> 89d9af985df0ac6188707e44f7c960678f9d13fc:Job 4/A. Setting SSID melalui web browser/readme.md
