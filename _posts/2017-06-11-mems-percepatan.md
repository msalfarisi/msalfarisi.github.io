---
title: 'Sensor Percepatan Berbasis MEMS'
date: 2017-06-11
permalink: /posts/2017/06/mems-accelerometer/
tags:
  - 1000guru
  - mems
  - science
---

Teman-teman tentu mempunyai smartphone atau ponsel pintar, bukan? Pernahkah terpikirkan oleh teman-teman mengapa ketika kita memutar ponsel dengan sudut 90°, orientasi layar pada ponsel akan berubah dari potrait ke landscape ataupun sebaliknya? Kira-kira dari mana ponsel ini mengetahui kalau dia sedang kita putar? Jawabannya adalah karena di dalam ponsel kita tertanam sensor percepatan atau dikenal sebagai akselerometer yang bisa mendeteksi adanya percepatan.

Pada kasus ponsel yang diputar, akselerometer mendeteksi hilangnya percepatan gravitasi pada satu sumbu serta munculnya percepatan gravitasi di sumbu yang lain, sehingga sistem di layar ponsel bisa menyesuaikan orientasinya. Pada edisi ini kita akan bahas mengenai salah satu jenis akselerometer yang paling banyak digunakan di kehidupan kita, yaitu akselerometer berbasis micro electro-mechanical systems (MEMS). Pada majalah 1000guru edisi Agustus 2016, MEMS telah dibahas sebagai mesin yang sangat kecil dan biasanya berperan sebagai sensor untuk mendeteksi suatu besaran. Dalam artikel kali ini, dibahas mengenai kegunaan MEMS dalam mendeteksi dan mengukur besaran percepatan, atau biasa juga disebut akselerometer MEMS (MEMS accelerometer).

Prinsip kerja dari akselerometer MEMS sangatlah sederhana. Bayangkan sebuah sistem pegas bermassa seperti ditunjukkan pada gambar. Jika kita gerakkan sistem pegas bermassa, akan terjadi perubahan panjang pegas. Menurut hukum Hooke dan hukum Newton, perubahan panjang pegas pada sistem tersebut berbanding lurus dengan besar percepatan yang dikenakan pada sistem yang sama. Oleh karenanya, ketika kita mendeteksi perubahan panjang pegas, kita bisa mendapatkan besaran percepatan yang bekerja pada sistem tersebut. Pada MEMS, sistem pegas bermassa ini disebut juga resonator karena sistem ini dapat bergerak bolak-balik di sekitar suatu titik kesetimbangan.

Ketika kita kenakan gaya sebesar F pada massa yang kita punya, dengan k sebagai konstanta pegas, m sebagai besaran massa dan x adalah besarnya perpindahan massa yang dihasilkan, kita akan memiliki 3 persamaan matematis sesuai hukum Hooke dan hukum Newton sebagai berikut:

$F = k x$

ΣF = m a

m a = k x

Pada proses pendeteksian percepatan, pergerakan massa dikonversi menjadi besaran listrik, sehingga diperlukan struktur tambahan selain massa dan pegas. Mekanisme yang paling umum digunakan adalah mekanisme kapasitor, yakni dengan memanfaatkan fenomena bahwa besar kapasitansi antara 2 pelat berbanding terbalik dengan jarak antara keduanya. Dengan mendeteksi perubahan besar kapasitansi antara dua pelat, perubahan panjang pegas bisa dideteksi dan dikonversikan menjadi besarnya percepatan yang dikenakan pada sistem yang kita miliki. Misalnya kita memiliki C sebagai besarnya kapasitansi kapasitor, ϵ0 adalah konstanta permitivitas, S adalah luas pelat atau elektrode yang digunakan, dan d adalah jarak antara kedua pelat tersebut, kita akan memiliki hubungan matematis sebagai berikut:

C =  ϵ0 S / d

Ketika tidak ada percepatan yang dikenakan pada akselerometer MEMS yang kita miliki, nilai d1 (jarak antara pelat biru dengan pelat bermassa seperti pada gambar) akan sama dengan nilai d2 (jarak antara pelat merah dengan pelat bermassa). Dengan demikian, nilai C1 (kapasitansi antara pelat biru dan dengan pelat bermassa) juga akan sama dengan nilai C2 (kapasitansi antara pelat merah dan dengan pelat bermassa). Sementara itu, ketika ada percepatan yang dikenakan pada akselerometer MEMS, nilai d1 dan d2 akan berbeda, sehingga besar C1 dan C2 juga akan berbeda.

Perpindahan massa diukur secara tidak langsung dengan mengukur perubahan kedua kapasitansi dan perbedaan di antara besar keduanya (selisih nilai antara C1 dan C2). Dengan mengukur perbedaan antara besar kedua kapasitansi, kita bisa mendapatkan bilangan yang lebih besar untuk perpindahan massa yang kecil sehingga sensornya lebih sensitif. Akselerometer MEMS sendiri didesain sedemikian rupa sehingga mampu mendeteksi percepatan dari semua arah. Hal inilah yang membuat strukturnya menjadi semakin rumit.

Selain digunakan pada ponsel pintar, saat ini akselerometer MEMS juga digunakan pada beberapa perangkat seperti remote control pada Nintendo-Wii, perangkat pengukur aktivitas seismik getaran permukaan bumi, perangkat pengukur aktivitas biologis dalam tubuh manusia, dan juga perangkat pemantauan aktivitas mesin pada proses produksi industri.

Pada tahun 2015, sebuah tim mahasiswa yang berasal dari Tohoku University menjadi juara pada International Contest of Application in Nano-micro Technology (iCAN) dengan membuat anywhere sado. Kontes ini merupakan kontes tahunan berskala internasional yang bertujuan untuk merangkai MEMS menjadi sebuah sistem tertentu yang bisa diikuti oleh siswa SMA maupun perguruan tinggi.


Sado merupakan kosakata bahasa Jepang yang artinya adalah upacara minum teh tradisional ala Jepang. Pada upacara minum teh di Jepang, ada teknik tertentu dalam mengaduk teh agar dapat menghasilkan cita rasa spesial. Biasanya pembuat (pengaduk) teh profesional perlu berlatih selama berbulan-bulan di bawah bimbingan seorang pelatih sebelum agar bisa menyajikan teh dengan cita rasa spesial tersebut.

Ketua dari tim mahasiswa yang berasal dari Tohoku University ini merupakan salah satu orang yang telah terlatih dalam menyajikan teh pada upacara minum teh selama bertahun-tahun. Ia merumuskan beberapa parameter yang penting dalam proses pengadukan teh, mulai dari frekuensi pengadukan, arah adukan, hingga temperatur air. Berbagai parameter ini bisa diukur dengan memasangkan akselerometer MEMS dan beberapa jenis MEMS lainnya pada alat pengaduk teh. Kemudian, data yang direkam dari MEMS tersebut dapat digunakan oleh siapapun untuk belajar mengaduk teh dengan baik dan benar. Teman-teman mungkin sekarang jadi tertarik untuk membuat alat tertentu dengan MEMS?

### Bahan bacaan:
* Chollet, Franck, Liu, Haobing. A (not so) short introduction to MEMS. http://memscyclopedia.org/
* Esashi, Masayoshi. はじめてのMEMS (Introduction to MEMS). 工業調査会, 2009.
* http://www.memsjournal.com/2010/12/motion-sensing-in-the-iphone-4-mems-accelerometer.html

Telah diterbitkan di Rubrik Teknologi Majalah 1000guru edisi Oktober 2017.
