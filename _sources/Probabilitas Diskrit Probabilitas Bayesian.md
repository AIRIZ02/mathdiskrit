---
title: Probabilitas Diskrit Probabilitas Bayesian

---

# Probabilitas Diskrit & Probabilitas Bayesian 
## Definisi
### Probabilitas Diskrit
**Probabilitas diskrit** adalah variabel acak yang dapat mengambil nilai tertentu (biasanya bilangan bulat). Contohnya termasuk pelemparan dadu.
### Probabilitas Bayesian 
**Probabilitas Bayesian** adalah pendekatan dalam teori probabilitas yang menggabungkan informasi baru dengan pengetahuan sebelumnya untuk memperbarui kepercayaan terhadap suatu hipotesis. Ini didasarkan pada Teorema Bayes, yang menyatakan bahwa probabilitas suatu hipotesis $H$ setelah melihat data $X$ (dikenal sebagai posterior probability).
Dapat dihitung dengan **rumus**:
$P(H \mid X) = \frac{P(X \mid H) \cdot P(H)} {P(X)}$ 
Keterangan: 
$P(H \mid X)$ = probabilitas hipotesis setelah data diperoleh (posterior).
$P(H)$ = probabilitas awal hipotesis (prior).
$P(X \mid H)$ = probabilitas data jika hipotesis benar.
$P(X)$ = total probabilitas data 24. 

## Teorema Bayes
### 1. Prior 
**Prior probability** adalah distribusi probabilitas yang mencerminkan keyakinan atau pengetahuan awal tentang suatu parameter sebelum data baru diperoleh **(apa yang kita ketahui sebelum ada data baru. Misalnya, hanya 1% orang yang sakit)**.
Ini menggambarkan asumsi atau informasi yang sudah ada mengenai parameter yang sedang dianalisis. Misalnya, jika kita memperkirakan kemungkinan suatu penyakit, prior dapat didasarkan pada data epidemiologi sebelumnya atau studi populasi.
### 2. Likelihood
**Likelihood** adalah cara untuk membandingkan dugaan mana yang paling mungkin benar, berdasarkan data yang kita lihat. 
Misalnya: Melempar koin 10 kali dan mendapatkan 7 kali "kepala". Lalu kamu ingin tahu, apakah koin itu "adil" (peluang kepala dan ekornya sama, yaitu 50%-50%) atau tidak? 
maka, 
* Kamu menduga peluang kepala adalah 50%. Likelihood mengecek apakah dugaan ini cocok dengan hasil 7 kepala tadi.
* Kalau tidak cocok, kamu bisa mencoba dugaan lain, seperti 70%, 80%, dan seterusnya, sampai menemukan yang paling cocok.

### 3. Posterior
**Posterior probability** adalah distribusi probabilitas yang diperoleh setelah menggabungkan informasi dari prior dan likelihood. Ini mencerminkan keyakinan kita tentang parameter setelah mempertimbangkan data yang baru diperoleh **(keyakinan kita setelah memperbarui informasi dengan data baru)**.

**Bayesian ini seperti mengatakan**: "Kita mulai dengan tebakan awal (prior), lalu melihat bukti baru (data), dan akhirnya memperbarui keyakinan kita (posterior)."

## Contoh Soal


| No. | Usia | Tekanan Darah | Penyakit (H/T) |
| ----| -----| --------      | --------       |
| 1.  | Muda | Normal        | T              |
| 2.  | Muda | Tinggi        | T              |
| 3.  | Paruh Baya | Normal  | T              |
| 4.  | Paruh Baya | Tinggi  | H              |
| 5.  | Tua  | Normal        | H              |
| 6.  | Tua  | Sangat Tinggi | H              |
| 7.  | Muda | Normal        | T              |
| 8.  | Tua  | Tinggi        | H              |
1. Hitunglah probabilitas Hipertensi terhadapa usia paruh baya tekanan darah sangat tinggi
2. Hitunglah probabilitas Tidak Hipertensi terhadap usia paruh baya tekanan darah sangat tinggi
### Jawaban Menggunakan Rumus Naive Bayes
#### Informasi Awal: 
1. Total data $(N) = 8$
2. Probabilitas prior:
* $P(H) = 4/8 = 0.5$
* $P(T) = 4/8 = 0.5$
#### Probabilitas Kondisional
1. Probabilitas $P(\text{Usia Paruh Baya} \mid H) :$
*  Dari 4 data Hipertensi, Usia Paruh Baya muncul 1 kali (Baris 4).
* $P(\text{Usia Paruh Baya} \mid H) = 1/4 = 0.25$ 
2. Probabilitas $P(\text{Sangat Tinggi} \mid H) :$
* Dari 4 data Hipertensi (H), Tekanan Darah Sangat Tinggi muncul 1 kali.
* $P(\text{Sangat Tinggi} \mid H) = \frac{1 + 1}{4 + 3} = \frac{2}{7}\approx 0.286$
3. Probabilitas $P(\text{Usia Paruh Baya} \mid T) :$
* Dari 4 data Tidak Hipertensi (T), Usia Paruh Baya muncul 1 kali.
* $P(\text{Paruh Baya} \mid T) = \frac{\text{Frekuensi Paruh Baya pada } T}{\text{Total Frekuensi } T} = \frac{1}{4} = 0.25$
4. Probabilitas $P(\text{Sangat Tinggi} \mid T) :$
* Dari 4 data Tidak Hipertensi (T), Tekanan Darah Sangat Tinggi muncul 0 kali.
* $P(\text{Sangat Tinggi} \mid T) = \frac{0 + 1}{4 + 3} = \frac{1}{7} \approx 0.143$ 
#### Probabilitas Posterior (Naive Bayes)
1. Untuk Hipertensi (H):
$P(H \mid \text{Paruh Baya, Sangat Tinggi}) = P(\text{Paruh Baya} \mid H) \cdot P(\text{Sangat Tinggi} \mid H)$
maka = $0.25 . 0.286 . 0.5 = 0.03575$
2. Untuk Tidak Hipertensi (T): 
$P(T \mid \text{Paruh Baya, Sangat Tinggi}) = P(\text{Paruh Baya} \mid T) \cdot P(\text{Sangat Tinggi} \mid T)$ 
maka = $0.25 . 0.143 . 0.5 = 0.017875$
#### Normalisasi Untuk menghitung probabilitas akhir:
$\text{Total} = P(H \mid \ldots) + P(T \mid \ldots) = 0.03575 + 0.017875 = 0.053625$
Probabilitas Hipertensi (H): 
$P(H \mid \ldots) = \frac{0.03575}{0.053625} \approx 0.666 \, (66.6\%)$  
Probabilitas Tidak Hipertensi ( T ):
$P(T \mid \ldots) = \frac{0.017875}{0.053625} \approx 0.333 \, (33.3\%)$
#### Kesimpulan
* Probabilitas seseorang dengan **usia paruh baya** dan **tekanan darah sangat tinggi** mengalami **Hipertensi** adalah 66.6%.
* Probabilitas **Tidak Hipertensi** adalah 33.3%.
### Jawaban Menggunakan Rumus Teorema Bayes
**Teorema Bayes** digunakan untuk menghitung probabilitas posterior $P(H \mid X)$ berdasarkan probabilitas prior dan probabilitas kondisional.
**Rumus umum**: 
$P(H \mid X) = \frac{P(X \mid H) \cdot P(H)}{P(X)}$ 
keterangan: 
* $P(H \mid X)$ : Probabilitas seseorang memiliki Hipertensi (H) diberikan data $X$ (fitur yang diamati seperti Usia Paruh Baya dan Tekanan Darah Sangat Tinggi).
* $P(X \mid H)$ : Probabilitas mengamati $X$ jika seseorang memiliki Hipertensi.
* $P(H)$ : Probabilitas prior Hipertensi (H).
* Probabilitas mengamati $X$, dihitung sebagai total probabilitas untuk semua kategori (Hipertensi dan Tidak Hipertensi).

**Penerapan Teorema Bayes** dalam Masalah Ini Kita ingin menghitung probabilitas posterior untuk:
1. Hipertensi $P(H \mid \text{Paruh Baya, Sangat Tinggi})$ 
2. Tidak Hipertensi $P(T \mid \text{Paruh Baya, Sangat Tinggi})$ 

#### Data:
* $X$ = Paruh Baya, Sangat Tinggi
* Probabilitas prior
* $P(H)$ = 0.5
* $P(T)$ = 0.5 
* Probabilitas kondisional dihitung menggunakan Laplace Smoothing.

#### Langkah 1: Hitung $P(X \mid H)$ dan $P(X \mid T)$
* $P(X \mid H)$ = $P(\text {Paruh Baya} \mid H)$ . $P(\text {Sangat Tinggi} \mid H)$ 
$= 0.25 . 0.286 = 0.0715$
* $P(X \mid T)$ = $P(\text {Paruh Baya} \mid T)$ . $P(\text {Sangat Tinggi} \mid T)$ 
$= 0.25 . 0.143 = 0.03575$

#### Langkah 2: Hitung Probabilitas Prior $(P(H) dan P(T))$ 
* $P(H) = 0.5$
* $P(T) = 0.5$

#### Langkah 3: Hitung $P(X)$ (Normalisasi Total Probabilitas)
$P(X)$ = $P(X \mid H).P(H)+P(X \mid T).P(T)$
$= (0.0715 . 0.5)+(0.03575 . 0.5)=0.03575+0.017875= 0.053625$
#### Langkah 4: Hitung Posterior Menggunakan Teorema Bayes
* Hipertensi 
$P(H \mid X)$ = $P(X \mid H) \frac{P(X \mid H).P(H)}{P(X)}$ 
$= \frac{0.03575. 0.5}{0.053625}$ = $\frac{0.017875}{0.053625} \approx 0.333 (33.3\%)$ 
#### Kesimpulan
* Probabilitas Hipertensi $P(H \mid X) = 66.6\%$
* Probabilitas Tidak Hipertensi $P(T \mid X) = 33.3\%$

