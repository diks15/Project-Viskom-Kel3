# Pre-Trained Object Detection menggunakan OpenCV Yolov4 X MQTT-ESP32
#### Disusun oleh kelompok 6 mata kuliah Computer Vision

[![forthebadge made-with-python](http://ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/) [![](https://img.shields.io/badge/python-3.8.10-blue.svg)](https://www.python.org/downloads/)
[![Github all releases](https://img.shields.io/github/downloads/Naereen/StrapDown.js/total.svg)](https://GitHub.com/Naereen/StrapDown.js/releases/)
Proyek ini menggabungkan teknologi Pre-Trained Object Detection menggunakan OpenCV dengan model YOLOv4 dan platform ESP32 yang mendukung protokol MQTT. Dengan menggunakan kombinasi ini, proyek ini dapat mendeteksi objek dalam waktu nyata dan mengirimkan data deteksi melalui protokol MQTT ke perangkat ESP32.

## Features
Fitur utama yang dihadarkan yaitu sebagai berikut:
- Implementasi teknologi Pre-Trained Object Detection menggunakan OpenCV dan    model YOLOv4 untuk mendeteksi objek dalam citra atau video
- Integrasi dengan platform ESP32 yang mendukung protokol MQTT untuk mengirimkan data deteksi secara real-time ke perangkat tersebut
- Kemampuan untuk mengakses data deteksi melalui MQTT dan menggunakannya untuk pengambilan keputusan atau tindakan lebih lanjut di perangkat ESP32
- Dapat digunakan dalam berbagai aplikasi seperti pemantauan keamanan, penghitungan orang, pengenalan objek, dan lainnya

## Tech

Aplikasi dan alat ini dibangun dengan menggunakan :

- [OpenCV] https://opencv.org/ - Library open-source populer untuk pengolahan citra dan video yang mendukung berbagai fungsi pemrosesan, termasuk deteksi objek. Digunakan untuk implementasi teknologi Pre-Trained Object Detection menggunakan model YOLOv4.
- [YOLOv4] - Model deteksi objek real-time yang sangat akurat dan efisien dalam mengidentifikasi objek dalam citra atau video. Digunakan sebagai model Pre-Trained Object Detection dalam proyek ini.
- [MQTT] (Message Queuing Telemetry Transport) https://mqtt.org/ - Protokol ringan dan handal yang digunakan untuk pertukaran pesan antara perangkat dalam Internet of Things (IoT). Digunakan untuk mengirimkan data deteksi objek secara real-time dari OpenCV ke perangkat ESP32.
- [ESP32] - Platform pengembangan mikrokontroler yang memiliki kemampuan WiFi dan Bluetooth, serta dukungan untuk protokol MQTT. Digunakan sebagai perangkat penerima data deteksi objek dan dapat melakukan tindakan atau pengambilan keputusan berdasarkan data yang diterima.
- Visual Studio Code https://code.visualstudio.com/ - Editor teks yang canggih dengan dukungan untuk pengembangan aplikasi web dan IoT.
- Arduino IDE https://wiki-content.arduino.cc/en/software - Lingkungan pengembangan terpadu untuk pemrograman mikrokontroler Arduino.

Dengan menggunakan kombinasi Aplikasi di atas, proyek ini mengimplementasikan Pre-Trained Object Detection menggunakan model YOLOv4 dengan OpenCV. Selain itu, pengiriman data deteksi objek secara real-time dilakukan melalui protokol MQTT ke perangkat ESP32. Pengembangan aplikasi ini dapat dilakukan menggunakan Visual Studio Code yang memberikan kemudahan dalam mengedit dan membangun kode.

## Requirement

- Install GIT_
- Python 3.8.10_
- Arduino IDE 1.8.x_
- autopep8==1.7.0
- dnspython==2.2.1
- numpy==1.23.4
- opencv-contrib-python==4.5.3.56
- paho-mqtt==1.6.1
- pycodestyle==2.9.1
- setuptools==44.0.0
- toml==0.10.2
- urllib3==1.26.12

## Installation

Pertama, buka repository dan salin link github ini, kemudian buka git bash pada device, lalu ketikan

```sh
git clone https://github.com/diks15/Project-Viskom-Kel3.git
```

Setelah project di donwload buka folder pada device lalu membuka folder tersebut melalui git bash, lalu ketikan

```sh
code .
```
Folder project akan otomatis membuka melalui visual studio code

Setelah itu, kembali lagi ke git bash untuk menginstall beberapa virtual environtment

- Install
```sh
pip install virtualenv
```
- Create
```sh
 virtualenv -p python3.8.10 yolov4
```
- Install
```sh
pip install virtualenv
```
- Activate
```sh
source yolov4/Scripts/activate
```
Lakukan  dengan berurutan, setelah itu buka code editor Visual Studio Code dan pergi ke terminal yang ada di Visual Studio Code
Untuk Menjalankan aplikasi, ada dua bagian, yaitu dengan terkoneksi melalui MQTT dan tidak terkoneksi ke MQTT
- With MQTT
```sh
python yolov4_mqtt.py
```
- Whitout MQTT
```sh
python yolov4.py
```
## Demonstrasi

Berikut link youtube yang berisi video demonstrasi dari aplikasi yang dibuat, untuk dapat diikuti oleh pengguna
- Demo ke 1 (Without MQTT)
https://youtu.be/WuTvR-BgOXY

- Demo ke 1 (With MQTT)
https://youtu.be/o5yy9dyDLYg

## Referensi

Aplikasi yang dirancang oleh Kelompok 6 merupakan pengembangan dari : https://github.com/Asadullah-Dal17/yolov4-opencv-python
