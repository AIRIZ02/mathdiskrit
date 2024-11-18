---
title: Cetrality Graph

---

# Cetrality Graph

# Social Network Analysis 
merupakan bidang kajian yang mengekplorasitentang hubungan manusia dengan menggunakan teori graf. Implementasi Social Network Analysis dapat menjelaskan relasi atau hubungan antar aktor melalui visualisasi berbentuk graf.

![image](https://hackmd.io/_uploads/SkvbK1ufkx.png)
![image](https://hackmd.io/_uploads/ryyNK1dMyl.png)
Social network 
terdapat node yang mewakili 
orang atau individu atau aktor. 
Relasi  antar objek  dapat dinyatakan dengan link 
atau edges yang terjadi antara aktor tersebut 
Social network terdiri dari banyak aktor 
yang mempunyai relasi satu sama lain hingga
membentuk peta jaringan sosial yang dinyatakan dengan 
graph

# Definisi
Tidak semua node dalam jaringan adalah penting  (aktor)
Mencari node yang paling penting dalam suatu jaringan
Centrality adalah penentuan aktor menggunakan ukuran pada Social Network Centrality dalam teori graf dan social network .Dibagi menjadi empat jenis, 
- degree centrality, 
- betweeness centrality, 
- closeness centrality 
- eigenvector centrality

# Degree Centrality
Degree centrality adalah jumlah edge yang terkoneksi pada suatu node yang mewakili interaksi.

Pentingnya node ditentukan oleh jumlah node yang berdekatan dengan node tersebut
- Lebih besar derajatnya (degree), maka lebih penting node itu dalam suatu jaringan 
- Hanya sebagian kecil node yang memiliki derajat tinggi dalam jaringan 

Degree Centrality : 
![image](https://hackmd.io/_uploads/BkflcJuGJe.png)

Normalisasi  Degree Centrality :
![image](https://hackmd.io/_uploads/B1TGq1dGkg.png)

# Closeness Centrality
Closenes centrality adalah nilai kedekatan antara satu node dengan node lain dalam jaringan dengan menghitung rata-rata dari jarak relasi node-node tersebut. Skor closeness centrality mewakili kecepatan dalam penyebaran informasi.

Average Distance:
![image](https://hackmd.io/_uploads/S1cDcJOfkg.png)

# Betweenness Centrality
Skor betweeness Centrality mewakili seberapa besar informasi yang tersebar dari suatu aktor. Semakin besar skor, artinya aktor tersebut semakin berperan dalam penyebaran informasi 

Semakin banyak lintasan yang harus melewati persimpangan itu (misal tidak ada jalan alternatif), maka semakin penting arti persimpangan tersebut. Hal ini menandakan seberapa besar suatu node diperlukan sebagai penghubung dalam penyebaran informasi di dalam jaringan

Ukuran ini juga dapat digunakan untuk mengidentifikasi boundary spanners, yaitu orang atau node yang berperan sebagai penghubung (jembatan) antara dua komunitas
