---
title: deret rekursif

---

# Deretan (sequence) 

**Deretan** adalah suatu urutan atau susunan elemen atau objek yang disusun secara teratur berdasarkan suatu aturan tertentu. Elemen dalam deretan biasanya berupa angka, huruf, simbol, atau objek lainnya, dan urutannya dapat didasarkan pada pola, nilai, atau hubungan tertentu

* **Definisi**: Sebuah **deretan** adalah fungsi dari subset suatu himpunan bilangan bulat (biasanya **N** atau **P**) ke sebuah himpunan **S**.
contoh :
$N = \{1, 2, 3, 4, … \}$
$S \text{ misalnya } \{2, 4, 6, 8, \dots\},   \{1/3, 1/5, 1/7, \dots \},  dsb$
* Notasi deretan: $\{a_n\}$

## Pembuktian Rumus Deret

**Soal:**
Buatlah Pembuktian Rumus Berikut :

$$\sum_{k=0}^{n} ar^k \text{ }(r \neq 0)$$

**Jawab :**
Rumus yang diberikan adalah bentuk dari **deret geometri**:

$$S_n = \sum_{k=0}^n ar^k = a + ar + ar^2 + \dots + ar^n$$

dengan $( r \neq 0 )$ dan $( r \neq 1 )$. Untuk membuktikan rumus tertutup dari deret ini, kita dapat menggunakan langkah berikut:

---

### Pembuktian Rumus Deret Geometri:
**Langkah 1: Tulis deretnya**  
Mulai dengan bentuk deret geometri:

$$S_n = a + ar + ar^2 + \dots + ar^n$$

**Langkah 2: Kalikan $( S_n )$ dengan rasio $( r )$**  
Kalikan kedua sisi persamaan dengan $( r )$:

$$rS_n = ar + ar^2 + ar^3 + \dots + ar^{n+1}$$

**Langkah 3: Kurangi kedua persamaan**  
Kurangi $( S_n )$ dengan $( rS_n )$:

$$S_n - rS_n = (a + ar + ar^2 + \dots + ar^n) - (ar + ar^2 + \dots + ar^{n+1})$$

Semua suku di kanan akan saling menghilangkan, kecuali $( a )$ dan $( ar^{n+1} )$:

$$S_n (1 - r) = a - ar^{n+1}$$

**Langkah 4: Sederhanakan persamaan**  
Faktor $( S_n )$:

$$S_n = \frac{a(1 - r^{n+1})}{1 - r}, \quad \text{dengan \( r \neq 1 \)}.$$

---

### Hasil Akhir:
Rumus tertutup dari deret geometri adalah:
$$S_n = \frac{a(1 - r^{n+1})}{1 - r}, \quad \text{untuk \( r \neq 1 \)}.$$

Rumus ini sangat berguna dalam banyak aplikasi matematika, termasuk analisis keuangan dan pemodelan data.

---

**Soal :**
Buatlah Pembuktian Rumus Berikut : 

$$\sum_{k=1}^n k$$

**Jawab :**
Rumus yang diberikan adalah jumlah bilangan bulat dari \( k = 1 \) hingga \( n \), yaitu:

$$\sum_{k=1}^n k = 1 + 2 + 3 + \dots + n$$

Rumus ini memiliki bentuk tertutup yang dinyatakan sebagai:

$$\sum_{k=1}^n k = \frac{n(n+1)}{2}$$

Berikut adalah pembuktiannya:

---

### Pembuktian:
**Langkah 1: Tulis deretnya dua kali dengan urutan terbalik**  
Tulis jumlah $( S )$ dua kali, satu dalam urutan asli, dan satu dalam urutan terbalik:

$$S = 1 + 2 + 3 + \dots + n$$

$$S = n + (n-1) + (n-2) + \dots + 1$$

**Langkah 2: Tambahkan kedua persamaan**  
Tambahkan kedua persamaan tersebut secara baris demi baris:

$$2S = (1 + n) + (2 + (n-1)) + (3 + (n-2)) + \dots + (n + 1)$$

Setiap pasangan menghasilkan jumlah $(n + 1)$, dan ada total $( n )$ pasangan:

$$2S = n(n+1)$$

**Langkah 3: Sederhanakan**  
Bagi kedua sisi persamaan dengan 2 untuk mendapatkan $( S )$:

$$S = \frac{n(n+1)}{2}$$

---

### Hasil Akhir:
Rumus jumlah bilangan bulat dari 1 hingga \( n \) adalah:

$$\sum_{k=1}^n k = \frac{n(n+1)}{2}.$$

Rumus ini sering digunakan dalam teori bilangan, kombinatorika, dan aplikasi lainnya.

---
**Soal :**
Buatlah Pembuktian Rumus Berikut

$$\sum_{k=1}^n k^2$$

**Jawab :**
Rumus yang ditampilkan adalah bentuk jumlah kuadrat dari bilangan bulat pertama hingga $(n)$, yaitu:

$$\sum_{k=1}^n k^2$$

Rumus umumnya adalah:

$$\sum_{k=1}^n k^2 = \frac{n(n+1)(2n+1)}{6}.$$

**Pembuktian**
Pembuktian rumus ini dapat dilakukan menggunakan **induksi matematika**.

---

**Langkah 1: Basis Induksi**
Untuk $( n = 1 )$, hitunglah sisi kiri dan sisi kanan.

- Sisi kiri:

$$\sum_{k=1}^1 k^2 = 1^2 = 1.$$

- Sisi kanan:

$$\frac{1(1+1)(2(1)+1)}{6} = \frac{1 \cdot 2 \cdot 3}{6} = 1.$$

Jadi, basis induksi benar.

---

**Langkah 2: Asumsi Induksi**
Misalkan rumus benar untuk $( n = m )$, yaitu:

$$\sum_{k=1}^m k^2 = \frac{m(m+1)(2m+1)}{6}.$$

---

**Langkah 3: Pembuktian untuk $n = m+1$**
Tambahkan suku berikutnya ($(m+1)^2$) pada kedua sisi asumsi induksi:

$$\sum_{k=1}^{m+1} k^2 = \sum_{k=1}^m k^2 + (m+1)^2.$$

Dari asumsi induksi:

$$\sum_{k=1}^{m+1} k^2 = \frac{m(m+1)(2m+1)}{6} + (m+1)^2.$$

Faktor $(m+1)$ dari kedua suku:

$$\sum_{k=1}^{m+1} k^2 = \frac{(m+1) \left[ m(2m+1) + 6(m+1) \right]}{6}.$$

Sederhanakan ekspresi dalam kurung:

$$m(2m+1) + 6(m+1) = 2m^2 + m + 6m + 6 = 2m^2 + 7m + 6.$$

Faktorkan:

$$2m^2 + 7m + 6 = (m+2)(2m+3).$$

Substitusikan kembali:

$$\sum_{k=1}^{m+1} k^2 = \frac{(m+1)(m+2)(2m+3)}{6}.$$

Ini sesuai dengan bentuk rumus untuk $n = m+1$. Maka, langkah induksi terbukti.

---

### Kesimpulan
Dengan basis dan langkah induksi terbukti, rumus:

$$\sum_{k=1}^n k^2 = \frac{n(n+1)(2n+1)}{6}$$
benar untuk semua bilangan bulat $n \geq 1$.