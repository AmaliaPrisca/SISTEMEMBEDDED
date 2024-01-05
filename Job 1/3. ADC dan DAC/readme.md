# C. ADC (Analog to Digital Converter) dan DAC (Digital to Analog Converter)

## 1. ADC dan DAC | Membaca Nilai Analog dari Potensiometer

### a. Rangkaian dan Flowchart
Rangkaian pada percobaan ini adalah sebagai berikut

![Screenshot 2023-11-28 153328](https://github.com/AmaliaPrisca/SISTEMEMBEDDED/assets/145273945/c74b7a68-7be4-48ff-806c-48b9baa88e8c)
<br>
![ADC DAC](https://github.com/AmaliaPrisca/SISTEMEMBEDDED/assets/145273945/46018fb0-cdff-4e4a-a3e0-7bb515659b26)


### b. Source Code
Kode program : <a href="ADC%20dan%20DAC/ADC%20dan%20DAC/ADC_1/ADC_1.ino">klik di sini</a>

### c. Hasil dan Pembahasan
<p align="justify">Dalam fungsi setup(), program menginisialisasi komunikasi serial dengan Serial.begin(115200) dan memberikan jeda waktu selama 1 detik menggunakan delay(1000). Pada fungsi loop(), beberapa langkah utama dijalankan. Pertama, program membaca nilai analog dari potensiometer menggunakan fungsi analogRead(potPin) dan menyimpannya dalam variabel potValue. Selanjutnya, nilai potensiometer tersebut ditampilkan di Serial Monitor dengan menggunakan Serial.println(potValue). Terdapat juga delay sebesar 500 ms menggunakan delay(500) agar nilai potensiometer tidak berubah terlalu cepat, memudahkan pemantauan melalui Serial Monitor.

https://github.com/AmaliaPrisca/SISTEMEMBEDDED/assets/145273945/8e0ae1a1-4f3f-4e88-9979-907662f3beea


## 2. ADC dan DAC | Mengatur Kecerahan LED Menggunakan Potensiometer

### a. Rangkaian dan Flowchart
Rangkaian pada percobaan ini adalah sebagai berikut

![Screenshot 2023-11-28 153328](https://github.com/AmaliaPrisca/SISTEMEMBEDDED/assets/145273945/c74b7a68-7be4-48ff-806c-48b9baa88e8c)
<br>
![ADC DAC (2)](https://github.com/AmaliaPrisca/SISTEMEMBEDDED/assets/145273945/8f5da861-d7f2-443f-a9e0-115e346ece90)



### b. Source Code
Kode program : <a href="ADC%20dan%20DAC/ADC%20dan%20DAC/ADC_2/ADC_2.ino">klik di sini</a>

### c. Hasil dan Pembahasan
<p align="justify">Dalam fungsi setup(), program menginisialisasi komunikasi serial dengan baudrate 115200 dan melakukan konfigurasi modul PWM untuk mengontrol LED. Pengaturan PWM melibatkan menetapkan frekuensi (freq), channel PWM (ledChannel), dan resolusi (resolution). Setelahnya, program menghubungkan saluran PWM ke pin output analog yang terhubung ke LED. Pada fungsi loop(), program membaca nilai analog dari potensiometer menggunakan analogRead(analogInPin) dan menyimpannya dalam variabel sensorValue. Nilai ini kemudian di-mapping dengan fungsi map() dari rentang nilai analog (0 hingga 4095) ke rentang nilai PWM (0 hingga 255). Nilai tersebut digunakan untuk mengatur kecerahan LED melalui fungsi analogWrite(analogOutPin, outputValue).

https://github.com/AmaliaPrisca/SISTEMEMBEDDED/assets/145273945/3fb04282-50db-4dd2-ab63-31d177334de4

