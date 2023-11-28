# C. Mengakses Sensor RFID (SPI Communication)
## 1. DHT Single Wire
### a. Rangkaian dan Flowchart
Rangkaian pada percobaan ini adalah sebagai berikut
![Screenshot 2023-11-28 150701](https://github.com/AmaliaPrisca/SISTEMEMBEDDED/assets/145273945/bf06a46e-8b6d-46a5-b4a0-bfca9c7d108b)



### b. Source Code
Kode program : <a href="GPIO_1.2/GPIO_1.ino">di sini</a>

### c. Hasil dan Pembahasan
Percobaan B, dilakukan akses terhadap Sensor DHT 11 (Single Wire / BUS) di mana jika suhu ruangan mencapai 30 derajat Celsius, ESP32 akan menyalakan LED Merah dan buzzer secara beep (blink). Jika suhu berada di bawah 30 derajat, ESP32 akan mematikan buzzer dan menyalakan LED dalam bentuk running LED, mirip dengan yang dilakukan pada Percobaan A. 
Cara kerja program dimulai dengan membuka komunikasi serial dan mencetak pesan "DHT11 Embedded System Test". Di dalam loop utama, program membaca nilai suhu dan kelembaban dari sensor DHT. Jika pembacaan gagal, program akan mencetak pesan kesalahan. Selanjutnya, program menghitung dan menampilkan indeks panas. Berdasarkan nilai suhu, program mengontrol LED dan buzzer. Jika suhu lebih dari 36°C, LED Merah (LEDM) dan buzzer akan menyala dengan interval 500 ms menyala dan 500 ms mati. Sedangkan jika suhu tidak lebih dari 36°C, LED Hijau (LEDH), LED Kuning (LEDK), LED Merah (LEDM), dan LED Biru (LEDB) akan menyala berurutan dengan interval 500 ms menyala dan 500 ms mati.
### d. Hasil Sensor RFID
https://github.com/AmaliaPrisca/SISTEMEMBEDDED/assets/145273945/35f9cd18-9ddb-4531-9359-a94ca0379cd3

