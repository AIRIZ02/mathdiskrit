---
title: analisis graph

---

# Analisa graph

## Pengertian analisis graph
Analisis Graph adalah proses mempelajari dan memahami struktur serta hubungan di dalam sebuah graph yaitu kumpulan elemen yang terdiri dari nodes (simpul) dan edges (sisi), yang digunakan untuk merepresentasikan jaringan atau hubungan antara entitas.

## social network analysis

### pengertian social network analysis
Social Network Analysis (SNA) adalah metode untuk menganalisis hubungan, pola interaksi, dan struktur jaringan dalam suatu kelompok atau komunitas. SNA digunakan untuk memahami bagaimana individu, organisasi, atau entitas lainnya saling terhubung melalui jaringan sosial.


![Cuplikan layar 2024-11-23 132457](https://hackmd.io/_uploads/Bk4dHlyQye.png)

![image](https://hackmd.io/_uploads/Hk8aBxkXyg.png)

#### Social network

terdapat node yang mewakili orang atau individu atau aktor. Relasi  antar objek  dapat dinyatakan dengan link atau edges yang terjadi antara aktor tersebut Social network terdiri dari banyak aktor yang mempunyai relasi satu sama lain hingga membentuk peta jaringan sosial yang dinyatakan dengan graph

* Tidak semua node dalam jaringan adalah penting (aktor). 
* Mencari node yang paling penting dalam suatu jaringan.
*  Centrality adalah penentuan aktor menggunakan ukuran pada Social Network Centrality dalam teori graf dan social network. Dibagi menjadi empat jenis, 
1. degree centrality, 
2. betweeness centrality, 
3. closeness centrality, 
4. eigenvector centrality

## Degree Centrality

* Degree centrality adalah jumlah edge yang terkoneksi pada suatu node yang mewakili interaksi.
* Pentingnya node ditentukan oleh jumlah node yang berdekatan dengan node tersebut
Lebih besar derajatnya (degree), maka lebih penting node itu dalam suatu jaringan 
Hanya sebagian kecil node yang memiliki derajat tinggi dalam jaringan 
* Mengukur jumlah koneksi langsung yang dimiliki oleh sebuah node.
* Node dengan derajat tinggi biasanya dianggap penting.



![image](https://hackmd.io/_uploads/S1g2KgkXke.png)

Untuk  node 1, degree centrality adalah 3;
Normalisasi degree centrality adalah  
3/(9-1)=3/8.

## Closeness Centrality

### pengertian Closeness Centrality
Closenes centrality adalah nilai kedekatan antara satu node dengan node lain dalam jaringan dengan menghitung rata-rata dari jarak relasi node-node tersebut. Skor closeness centrality mewakili kecepatan dalam penyebaran informasi. Mengukur kedekatan sebuah node dengan node lainnya,
Node dengan closeness tinggi dapat dengan cepat menyebarkan informasi.


Contoh Closeness Centrality 
![image](https://hackmd.io/_uploads/S17e7WJmJe.png)
![image](https://hackmd.io/_uploads/BJhjQ-kQ1x.png)
![image](https://hackmd.io/_uploads/HJR27ZyXyl.png)

Node 4  lebih central  dari node 3

## Betweenness Centrality
* Skor betweeness Centrality mewakili seberapa besar informasi yang tersebar dari suatu aktor. Semakin besar skor, artinya aktor tersebut semakin berperan dalam penyebaran informasi 
* Semakin banyak lintasan yang harus melewati persimpangan itu (misal tidak ada jalan alternatif), maka semakin penting arti persimpangan tersebut. Hal ini menandakan seberapa besar suatu node diperlukan sebagai penghubung dalam penyebaran informasi di dalam jaringan
* Ukuran ini juga dapat digunakan untuk mengidentifikasi boundary spanners, yaitu orang atau node yang berperan sebagai penghubung (jembatan) antara dua komunitas
* Menghitung jumlah lintasan terpendek yang melewati suatu node
* Node dengan  betweenness  tinggi  adalah  penting dalam komunikasi dan penyebaran informasi
* Mengukur seberapa sering sebuah node menjadi penghubung di antara node lain.
Penting untuk memahami pengaruh dalam jaringan.



