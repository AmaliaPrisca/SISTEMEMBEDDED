# A. Koneksi MQTT Broker

### 1. Rangkaian
Rangkaian pada percobaan ini adalah sebagai berikut

![1](https://github.com/AlfinIzza01/Sistem-Embedded/assets/94149476/33cb40f8-d5f7-4028-aca8-c88399477e97)

### 2. Hasil dan Pembahasan
Instal paket MQTT untuk Node-RED dengan perintah npm install node-red-contrib-mqtt. Buka Node-RED melalui browser dan tambahkan node MQTT ke alur. Konfigurasikan node MQTT dengan mengatur server MQTT, termasuk alamat broker, port, dan opsi lainnya. Tambahkan node pengirim dan penerima, sambungkan keduanya, dan konfigurasi topik yang ingin Anda gunakan. Deploy alur untuk menerapkan konfigurasi. Monitor pesan di tab "Debug" untuk memastikan tidak ada masalah. Uji koneksi dengan mengirim pesan dari node pengirim dan memastikan bahwa pesan diterima oleh node penerima. 

![2](https://github.com/AlfinIzza01/Sistem-Embedded/assets/94149476/5f73463e-5dde-40f0-bfbe-40178b8343e9)
