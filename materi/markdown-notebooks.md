---
jupytext:
  formats: md:myst
  text_representation:
    extension: .md
    format_name: myst
    format_version: 0.13
    jupytext_version: 1.11.5
kernelspec:
  display_name: Python 3
  language: python
  name: python3
---

# HIMPUNAN

Mengutip dari buku "Teori Himpunan" oleh Darwanto dkk, himpunan adalah kumpulan objek atau benda yang didefinisikan secara jelas, di mana setiap anggotanya dapat dibedakan dari yang bukan bagian himpunan tersebut.
Dalam himpunan, setiap objek disebut sebagai anggota atau elemen. Anggota himpunan ditandai dengan "∈", sementara yang bukan anggota ditandai dengan "∉", sebagaimana dilansir dari laman CNN Indonesia.

Contohnya:
A = {harimau, anjing, kucing, kelinci}
Maka, himpunan A adalah himpunan hewan berkaki empat dengan n(A) = 4
Kelinci ∈ A (kelinci adalah anggota himpunan A, dan ayam ∉ A (ayam bukan anggota himpunan 


## Identitas Himpunan
Identitas adalah persamaan yang berlaku universal untuk semua elemen dalam suatu himpunan . Misalnya, persamaan a + b = b+a adalah identitas untuk bilangan riil karena berlaku untuk semua bilangan riil a dan b. Kumpulan sifat himpunan dalam teorema berikut seluruhnya terdiri dari identitas himpunan.

### $\Diamond$ Hukum Identitas

### 1. Himpunan $A \cup \emptyset = A$

$A \cup \emptyset = \{ x \mid x \in A \text{ atau } x \in \emptyset \}$


Karena 
$x \in \emptyset$ adalah kondisi yang tidak mungkin terjadi (karena $\emptyset$ tidak memiliki elemen), maka gabungan ini hanya akan berisi elemen-elemen dari 

$A \cup \emptyset = \{ x \mid x \in A \}$

Ini setara dengan himpunan $A$ itu sendiri

**Definisi**:
- $\cup$ adalah simbol untuk operasi union (gabungan) dalam teori himpunan.
- $\emptyset$ adalah himpunan kosong, yaitu himpunan yang tidak memiliki elemen.
- $A$ adalah himpunan apa pun.

**Penjelasan**:
Operasi union antara himpunan $A$ dan himpunan kosong  $\emptyset$ berarti kita menggabungkan semua elemen dari kedua himpunan tersebut. Karena $\emptyset$ tidak memiliki elemen, maka gabungan dari $A$ dan $\emptyset$ hanya akan berisi elemen-elemen dari $A$ itu sendiri.

Secara formal:
$A \cup \emptyset = A$

Artinya, jika Anda menggabungkan himpunan $A$ dengan himpunan kosong, hasilnya tetap $A$. Himpunan kosong tidak mempengaruhi hasil gabungan karena tidak ada elemen yang ditambahkan.

**Contoh:**
Jika $𝐴 =\{1,2,3\},\text {maka} 𝐴 \cup \emptyset =\{1,2,3\}$

### 2. Himpunan $A \cap U = A$

**$A \cap U = \{ x \mid x \in A \text{ dan } x \in U \}$**

Karena $𝑈$ adalah ruang semesta yang mencakup semua elemen yang relevan, setiap elemen $𝑥$ dari $𝐴$ juga merupakan elemen dari $𝑈$,ini menyatakan bahwa irisan antara $𝐴$ dan $𝑈$ adalah himpunan $𝐴$ itu sendiri,karena $𝑈$ tidak mengubah himpunan $𝐴$

**Definisi**:
- $\cap$ adalah simbol untuk operasi irisan (intersection) dalam teori himpunan.
- $U$ biasanya digunakan untuk menyebut himpunan semesta, yaitu himpunan yang memuat semua elemen yang relevan dalam konteks tertentu.
- $A$ adalah himpunan apa pun.

**Penjelasan**:
Operasi irisan antara himpunan $A$ dan himpunan semesta $U$ berarti kita mencari elemen yang ada di kedua himpunan tersebut. Karena $U$ adalah himpunan semesta, semua elemen dari $A$ sudah tentu termasuk dalam $U$.

Secara formal:
$A \cap U = A$

Artinya, jika Anda mengambil irisan himpunan $A$ dengan himpunan semesta $U$, hasilnya adalah himpunan $A$ itu sendiri. Ini karena $U$ mencakup semua elemen yang ada dalam $A$, sehingga irisan dari $A$ dengan $U$ tidak menghilangkan elemen apa pun dari $A$.

**Contoh:**

Jika $𝑈$ $=\{1,2,3,4,5\}$ dan $𝐴$ $=/{1,2,3/}$, maka $A \cap U=\{1,2,3\}$.

### Kesimpulan

1. Gabungan himpunan $A$ dengan himpunan kosong $\emptyset$ menghasilkan himpunan $A$ itu sendiri.
2. Irisan himpunan $A$ dengan himpunan semesta $U$ juga menghasilkan himpunan $A$ itu sendiri.

### $\Diamond$ Hukum Dominasi
### 1. Hukum Gabungan  $A \cup U = U$

**Pernyataan:**

$A\cup U=\{ x \mid x \in A atau x \in U\}$

Karena $𝑈$ adalah ruang semesta yang mencakup semua elemen, maka kondisi $𝑥 \in 𝑈$ selalu benar jika $𝑥$ berada di $𝑈$,Karena $𝑥 \in 𝑈$ mencakup semua elemen dalam konteks tersebu

**Penjelasan:**

- **Gabungan (Union):** Gabungan antara dua himpunan $A$ dan $U$, ditulis sebagai $A \cup U$, adalah himpunan yang berisi semua elemen yang ada di $A$ atau di $U$ atau di keduanya.

- **Ruang Semesta $U$:** Ruang semesta $U$ adalah himpunan yang mencakup semua elemen yang relevan dalam konteks tertentu. Dengan kata lain, $U$ adalah himpunan yang mencakup semua elemen yang mungkin dalam sistem yang sedang dibahas.

**Contoh:**

Misalkan $U$ adalah ruang semesta yang mencakup semua bilangan bulat dari 1 hingga 10, dan $A$ adalah himpunan bilangan genap dari 1 hingga 10. Jadi, kita punya:

$U = \{1, 2, 3, 4, 5, 6, 7, 8, 9, 10\}$
$A = \{2, 4, 6, 8, 10\}$

Gabungan $A \cup U$ akan mencakup semua elemen dalam $U$, karena $U$ sudah mencakup semua elemen dalam $A$ dan lebih banyak lagi. Jadi:
$A \cup U = U$

Dalam hal ini:

$\{2, 4, 6, 8, 10\} \cup \{1, 2, 3, 4, 5, 6, 7, 8, 9, 10\} = \{1, 2, 3, 4, 5, 6, 7, 8, 9, 10\}$

### 2. Hukum Irisan dengan Himpunan Kosong: $A \cap \emptyset = \emptyset$

**Pernyataan:**

$A \cap \emptyset =\{x \mid x \in A dan x \in \emptyset \}$

Karena tidak ada elemen yang berada di $\emptyset$, kondisi $𝑥 \in \emptyset$ selalu salah. Dengan demikian, irisan $𝐴 \cap \emptyset$ tidak mengandung elemen apapun

**Penjelasan:**

- **Irisan (Intersection):** Irisan antara dua himpunan $A$ dan $\emptyset$, ditulis sebagai $A \cap \emptyset$, adalah himpunan yang berisi semua elemen yang ada di kedua himpunan tersebut.

- **Himpunan Kosong $\emptyset$:** Himpunan kosong adalah himpunan yang tidak memiliki elemen sama sekali. Dengan kata lain, tidak ada elemen $x$ yang memenuhi kondisi $x \in \emptyset$.

**Contoh:**

Misalkan $A$ adalah himpunan bilangan genap dari 1 hingga 10, dan $\emptyset$ adalah himpunan kosong:

$A = \{2, 4, 6, 8, 10\}$

$\emptyset = \{\}$

Irisan $A \cap \emptyset$ akan selalu menjadi himpunan kosong karena tidak ada elemen yang ada di $\emptyset$ yang juga bisa berada di $A$. Jadi:
$A \cap \emptyset = \emptyset$
Dalam hal ini:
$\{2, 4, 6, 8, 10\} \cap \{\} = \{\}$

### Kesimpulan

- **$A \cup U =U$ :** Gabungan antara himpunan $A$ dengan ruang semesta $U$ adalah ruang semesta $U$ itu sendiri, karena ruang semesta sudah mencakup semua elemen yang mungkin.

- **$A \cap \emptyset = \emptyset$:** Irisan antara himpunan $A$ dan himpunan kosong $\emptyset$ adalah himpunan kosong $\emptyset$, karena tidak ada elemen di himpunan kosong yang dapat beririsan dengan elemen di $A$. 

Kedua hukum ini adalah dasar penting dalam teori himpunan dan membantu dalam menyederhanakan ekspresi himpunan serta dalam pemahaman dasar tentang bagaimana operasi himpunan berfungsi.

### $\Diamond$ Hukum idempoten
### 1. Irisan Himpunan dengan Diri Sendiri: $𝐴 \cap 𝐴$
**Pernyataan:**

$A \cap A =\{x \mid x \in A dan x \in A \}$

Karena $𝑥 \in 𝐴$ dan $𝑥 \in 𝐴$ hanya memberikan $𝑥 \in 𝐴$

**Penjelasan:**

Irisan (Intersection): Irisan antara dua himpunan $𝐴$ dan $𝐵$, yang ditulis sebagai $𝐴 \cap 𝐵$, adalah himpunan yang berisi semua elemen yang ada di kedua himpunan tersebut.

Irisan dengan Diri Sendiri: Ketika kita melakukan irisan himpunan $𝐴$ dengan dirinya sendiri $𝐴 \cap 𝐴$ , kita mencari elemen yang ada di $𝐴$ dan juga di $𝐴$ lagi. Karena $𝐴$ adalah himpunan yang sama di kedua sisi, hasilnya adalah himpunan $A$ itu sendiri.

Contoh:

Misalkan $A=\{1,2,3\}. \text{maka}: A∩A=\{1,2,3\}$

### 2. Gabungan Himpunan dengan Diri Sendiri: $A \cup A$

**Pernyataan:**

$A \cup A = \{ x \mid x \in A \text{ atau } x \in A \} = A$

Karena $𝑥 \in 𝐴$ atau $𝑥 \in 𝐴$ hanya memberikan $𝑥 \in 𝐴$,

**Penjelasan:**

Gabungan (Union): Gabungan antara dua himpunan 𝐴 dan 𝐵, yang ditulis sebagai $𝐴 \cup 𝐵$, adalah himpunan yang berisi semua elemen yang ada di $𝐴$ atau di $𝐵$ atau di keduanya.

Gabungan dengan Diri Sendiri: Ketika kita melakukan gabungan himpunan $𝐴$ dengan dirinya sendiri $(𝐴∪𝐴)$, kita mencari elemen yang ada di $𝐴$ atau di $𝐴$ lagi. Karena himpunan $𝐴$ yang digabungkan dengan dirinya sendiri tidak menambah elemen baru, hasilnya adalah himpunan $𝐴$ itu sendiri.

Contoh:

Misalkan 
$A=\{1,2,3\}$. Maka: $𝐴∪𝐴=\{1,2,3\}$

**Kesimpulan:**

- Irisan dengan Diri Sendiri (𝐴∩𝐴): Menghasilkan himpunan itu sendiri, 𝐴, karena setiap elemen yang ada di 𝐴 pasti berada di 𝐴 lagi.
- Gabungan dengan Diri Sendiri (𝐴∪𝐴): Menghasilkan himpunan itu sendiri, 𝐴, karena gabungan himpunan 𝐴 dengan dirinya sendiri tidak menambah elemen baru.

Kedua hukum ini menunjukkan bahwa operasi himpunan dengan diri sendiri tidak mengubah himpunan, baik dalam hal irisan maupun gabungan.

Tentu! Hukum terkait himpunan komplemen dari komplemen adalah salah satu hukum dasar dalam teori himpunan. Mari kita bahas dengan rinci.

### $\Diamond$ Hukum Komplementasi

### Komplemen dari Komplemen Himpunan: $\overline{\overline{A}} = A$

**Pernyataan:**

$\overline{\overline{A}} = \{ x \mid x \in U \text{ dan } x \notin \overline{A} \} = \{ x \mid x \in U \text{ dan } x \in A \} = A$

**Penjelasan:**

- **Komplemen Himpunan $A (\overline{A)}$**: Komplemen dari himpunan $A$ adalah himpunan semua elemen yang tidak berada di $A$, tetapi berada di ruang semesta $U$. Dalam notasi set-builder, ini dapat dinyatakan sebagai:
  
  $\overline{A} = \{ x \mid x \in U \text{ dan } x \notin A \}$

- **Komplemen dari Komplemen**: Jika kita mengambil komplemen dari $\overline{A}$, kita mencari himpunan semua elemen yang tidak berada di $\overline{A}$. Namun,$\overline{A}$ sendiri adalah himpunan elemen yang tidak berada di $A$. Jadi, komplemen dari $\overline{A}$ adalah himpunan yang kembali ke himpunan $A$, karena semua elemen di luar $A$ adalah elemen dari $\overline{A}$, dan komplemennya adalah himpunan $A$ itu sendiri.

**Matematis:**

1. Misalkan $U$ adalah ruang semesta.
2. Komplemen $A$ adalah: 
   
   $\overline{A} = U \setminus A$

3. Komplemen dari $\overline{A}$ adalah:
   
   $\overline{\overline{A}} = U \setminus \overline{A}$

   Karena $\overline{A} = U \setminus A$, maka:

   $\overline{\overline{A}} = U \setminus (U \setminus A)$

**Contoh:**

Misalkan $U = \{1, 2, 3, 4, 5\} dan A = \{2, 4\}$.

1. Komplemen dari $A$ dalam $U$ adalah:
   
   $\overline{A} = \{1, 3, 5\}$

2. Komplemen dari $\overline{A}$ adalah
   
   $\overline{\overline{A}} = U \setminus \{1, 3, 5\} = \{2, 4\}$

Jadi:

$\overline{\overline{A}} = A$


### Kesimpulan

- **Komplemen dari Komplemen $(\overline{\overline{A}})$**: Menghasilkan himpunan asli $A$. Ini berarti jika Anda mengambil komplemen dari himpunan komplemen, Anda akan kembali ke himpunan awal.
- **Hukum ini**: Menunjukkan bahwa operasi komplemen adalah operasi invers, yaitu melakukan komplemen dua kali akan kembali ke himpunan yang asli.

Hukum ini penting dalam teori himpunan dan logika karena menunjukkan sifat invers dari operasi komplemen. Ini juga merupakan dasar untuk memahami hubungan antara himpunan dan operasi logika dalam matematika dan ilmu komputer.

### $\Diamond$ Hukum Komutatif Dalam Himpunan

Tentu! Hukum komutatif adalah salah satu hukum dasar dalam teori himpunan dan aljabar yang menjelaskan bahwa urutan operasi tidak mempengaruhi hasil. Hukum ini berlaku untuk operasi gabungan (union) dan irisan (intersection) dalam teori himpunan, serta untuk operasi penjumlahan dan perkalian dalam aljabar

### 1. Hukum Komutatif untuk Gabungan (Union):$A \cup B = B \cup A$

**Pernyataan:**

$A \cup B = \{ x \mid x \in A \text{ atau } x \in B \}=B \cup A = \{ x \mid x \in B \text{ atau } x \in A \}$

**Penjelasan:**
- Hukum komutatif untuk gabungan menyatakan bahwa gabungan dari dua himpunan $A$ dan $B$ tidak terpengaruh oleh urutan himpunan. Dengan kata lain, gabungan $A$ dengan $B$ menghasilkan himpunan yang sama dengan gabungan $B$ dengan $A$.

**Contoh:**
Jika $A = \{1, 2\}$ dan $B = \{2, 3\}$, maka:

$A \cup B = \{1, 2, 3\}$

$B \cup A = \{1, 2, 3\}$

Jadi:

$A \cup B = B \cup A$

### 2. Hukum Komutatif untuk Irisan (Intersection): $A \cap B = B \cap A$

**Pernyataan:**

$A \cap B = \{ x \mid x \in A \text{ dan } x \in B \} = B \cap A = \{ x \mid x \in B \text{ dan } x \in A \}$

**Penjelasan:**
- Hukum komutatif untuk irisan menyatakan bahwa irisan dari dua himpunan $A$ dan $B$ tidak terpengaruh oleh urutan himpunan. Dengan kata lain, irisan $A$ dengan $B$ menghasilkan himpunan yang sama dengan irisan $B$ dengan $A$.

**Contoh:**

Jika $A = \{1, 2\}$ dan $B = \{2, 3\}$, maka:

$A \cap B = \{2\}$

$B \cap A = \{2\}$

Jadi:

$A \cap B = B \cap A$

### Kesimpulan

- **Hukum Komutatif untuk Gabungan (Union):** Mengatakan bahwa $A \cup B = B \cup A$.
- **Hukum Komutatif untuk Irisan (Intersection):** Mengatakan bahwa $A \cap B = B \cap A$.
- **Hukum Komutatif dalam Aljabar:** Mengatakan bahwa urutan dalam penjumlahan dan perkalian tidak mempengaruhi hasil, yaitu $a + b = b + a$ dan $a \cdot b = b \cdot a$.

Hukum komutatif adalah dasar penting dalam berbagai cabang matematika, memastikan bahwa urutan operasi tidak mempengaruhi hasil akhir.

Hukum asosiatif dalam teori himpunan adalah prinsip yang menunjukkan bahwa cara kita mengelompokkan himpunan saat melakukan operasi gabungan (union) atau irisan (intersection) tidak mempengaruhi hasil akhir. Hukum ini berlaku untuk operasi gabungan dan irisan dan sangat mirip dengan hukum asosiatif dalam aljabar.

### $\Diamond$ Hukum Asosiatif dalam Teori Himpunan

### 1. Hukum Asosiatif untuk Gabungan (Union): $(A \cup B) \cup C = A \cup (B \cup C)$**

**Pernyataan:**

$(A \cup B) \cup C = \{ x \mid x \in (A \cup B) \text{ atau } x \in C \}$ = $A \cup (B \cup C) = \{ x \mid x \in A \text{ atau } x \in (B \cup C) \}$

**Penjelasan:**

- Hukum asosiatif untuk gabungan menyatakan bahwa gabungan dari tiga himpunan tidak terpengaruh oleh cara kita mengelompokkan himpunan-himpunan tersebut. Baik kita menggabungkan $A$ dengan $B$ terlebih dahulu dan kemudian dengan $C$, atau kita menggabungkan $B$ dengan $C$ terlebih dahulu dan kemudian dengan $A$, hasilnya akan tetap sama.

**Contoh:**

Jika $A = \{1\}$, $B = \{2\}$, dan $C = \{3\}$, maka:

$(A \cup B) \cup C = \{1\} \cup \{2\} \cup \{3\} = \{1, 2, 3\}$

$A \cup (B \cup C) = \{1\} \cup (\{2\} \cup \{3\}) = \{1, 2, 3\}$

Jadi, kita dapat menyimpulkan:

$(A \cup B) \cup C = A \cup (B \cup C)$

### 2. Hukum Asosiatif untuk Irisan (Intersection): $(A \cap B) \cap C = A \cap (B \cap C)$

**Pernyataan:**

$(A \cap B) \cap C = \{ x \mid x \in A \text{ dan } x \in B \text{ dan } x \in C \}$  = $A \cap (B \cap C) = \{ x \mid x \in A \text{ dan } x \in B \text{ dan } x \in C \}$

**Penjelasan:**

- Hukum asosiatif untuk irisan menyatakan bahwa irisan dari tiga himpunan tidak terpengaruh oleh cara kita mengelompokkan himpunan-himpunan tersebut. Baik kita mengiris $A$ dengan $B$ terlebih dahulu dan kemudian dengan $C$, atau kita mengiris $B$ dengan $C$ terlebih dahulu dan kemudian dengan $A$, hasilnya akan tetap sama.

**Contoh:**

Jika $A = \{1, 2\}$, $B = \{2, 3\}$, dan $C = \{2, 4\}$, maka:

$(A \cap B) \cap C = (\{1, 2\} \cap \{2, 3\}) \cap \{2, 4\} = \{2\} \cap \{2, 4\} = \{2\}$

$A \cap (B \cap C) = \{1, 2\} \cap (\{2, 3\} \cap \{2, 4\}) = \{1, 2\} \cap \{2\} = \{2\}$

Jadi, kita dapat menyimpulkan:

$(A \cap B) \cap C = A \cap (B \cap C)$


### Kesimpulan

- **Hukum Asosiatif untuk Gabungan (Union):** Mengatakan bahwa gabungan dari tiga himpunan $A$, $B$, dan $C$ tidak terpengaruh oleh cara kita mengelompokkan himpunan-himpunan tersebut.
  
  $(A \cup B) \cup C = A \cup (B \cup C)$

- **Hukum Asosiatif untuk Irisan (Intersection):** Mengatakan bahwa irisan dari tiga himpunan $A$, $B$, dan $C$ tidak terpengaruh oleh cara kita mengelompokkan himpunan-himpunan tersebut.
  
  $(A \cap B) \cap C = A \cap (B \cap C)$

Hukum asosiatif memastikan bahwa cara pengelompokan himpunan dalam operasi gabungan dan irisan tidak mempengaruhi hasil akhir, yang merupakan prinsip penting dalam teori himpunan dan aljabar.


### $\Diamond$ Hukum Distributif dalam Teori Himpunan


### 1.Hukum Distributif Union terhadap Intersection: $A \cup (B \cap C) = (A \cup B) \cap (A \cup C)$

**Pernyataan:**

$A \cup (B \cap C) = (A \cup B) \cap (A \cup C) = \{x \mid x \in A dan (x \in B atau x \in C)\}=\{x \mid(x 
\in A dan x \in B) atau (x \in A dan x \in C)\}$

**Penjelasan:**
- **Sisi Kiri**: $A \cup (B \cap C)$
  - Ini berarti kita mengambil gabungan dari himpunan $A$ dengan irisan $B$ dan $C$. Artinya, kita akan menyertakan semua elemen yang ada di $A$ ditambah semua elemen yang ada di $B$ dan $C$ secara bersamaan.

- **Sisi Kanan**: $(A \cup B) \cap (A \cup C)$
  - Ini berarti kita pertama-tama mengambil gabungan $A$ dengan $B$, dan gabungan $A$ dengan $C$, lalu kita mengambil irisan dari kedua gabungan tersebut. Artinya, kita akan menyertakan elemen-elemen yang ada di kedua gabungan tersebut.

**Contoh:**

Misalkan $A = \{1, 2\}$,$B = \{2, 3\}$, dan $C = \{3, 4\}$.

- **Sisi Kiri**:
  
  $B \cap C = \{3\}$
  
  $A \cup (B \cap C) = \{1, 2\} \cup \{3\} = \{1, 2, 3\}$

- **Sisi Kanan**:
  
  $A \cup B = \{1, 2\} \cup \{2, 3\} = \{1, 2, 3\}$
  
  $A \cup C = \{1, 2\} \cup \{3, 4\} = \{1, 2, 3, 4\}$
  
  $(A \cup B) \cap (A \cup C) = \{1, 2, 3\} \cap \{1, 2, 3, 4\} = \{1, 2, 3\}$

Kedua sisi menghasilkan himpunan yang sama: $\{1, 2, 3\}$.

### 2.Hukum Distributif Intersection terhadap Union: $A \cap (B \cup C) = (A \cap B) \cup (A \cap C)$

**Pernyataan:**

$A \cap (B \cup C) = (A \cap B) \cup (A \cap C) = \{x \mid x \in A dan (x \in B atau x \in C)\}=\{x \mid(x 
\in A dan x \in B) atau (x \in A dan x \in C)\}$

**Penjelasan:**
- **Sisi Kiri**: $A \cap (B \cup C)$
  - Ini berarti kita mengambil irisan dari himpunan $A$ dengan gabungan $B$ dan $C$. Artinya, kita mencari elemen yang ada di $A$ dan juga ada di gabungan $B$ dan $C$.

- **Sisi Kanan**: $(A \cap B) \cup (A \cap C)$
  - Ini berarti kita pertama-tama mengambil irisan $A$ dengan $B$, dan irisan $A$ dengan $C$, lalu kita gabungkan hasil irisan tersebut. Artinya, kita akan menyertakan elemen-elemen yang ada di $A$ dan juga ada di $B$ atau di $C$.

**Contoh:**

Misalkan $A = \{1, 2, 3\}$,$B = \{2, 3, 4\}$, dan $C = \{3, 4, 5\}$.

- **Sisi Kiri**:
  
  $B \cup C = \{2, 3, 4\} \cup \{3, 4, 5\} = \{2, 3, 4, 5\}$
  
  $A \cap (B \cup C) = \{1, 2, 3\} \cap \{2, 3, 4, 5\} = \{2, 3\}$

- **Sisi Kanan**:
  
  $A \cap B = \{1, 2, 3\} \cap \{2, 3, 4\} = \{2, 3\}$
  
  $A \cap C = \{1, 2, 3\} \cap \{3, 4, 5\} = \{3\}$
  
  $(A \cap B) \cup (A \cap C) = \{2, 3\} \cup \{3\} = \{2, 3\}$

Kedua sisi menghasilkan himpunan yang sama: $\{2, 3\}$.

### Kesimpulan

Hukum-hukum distributif ini memastikan bahwa operasi gabungan (union) dan irisan (intersection) dalam teori himpunan bersifat konsisten dan dapat dipertukarkan, memungkinkan kita untuk menyederhanakan ekspresi himpunan dan melakukan manipulasi yang lebih kompleks dengan cara yang sistematis.


### $\Diamond$ Hukum De Morgan dalam Teori Himpunan

Hukum De Morgan untuk himpunan terdiri dari dua hukum yang saling berhubungan. Mereka memberikan cara untuk mengekspresikan negasi dari gabungan dan irisan himpunan dalam bentuk yang berbeda.

### 1.Hukum De Morgan untuk Gabungan: $\overline{A \cup B} = \overline{A} \cap \overline{B}$

**Pernyataatn**

$\overline{A \cup B} = \overline{A} \cap \overline{B}=\{x \mid x \notin A \cup B\}=\{x \mid x \notin A \text{ dan }x \notin B\}$

**Penjelasan**: 
- $A \cup B$ adalah himpunan yang terdiri dari semua elemen yang berada di $A$, di $B$, atau di kedua himpunan tersebut.
- Negasi dari $A \cup B$ , yang ditulis sebagai $ \overline{A}$, adalah himpunan yang terdiri dari semua elemen yang tidak berada di $A \cup B$.
- $\overline A$ adalah himpunan yang terdiri dari semua elemen yang tidak berada di $A$, dan $\overline B$ adalah himpunan yang terdiri dari semua elemen yang tidak berada di $B$.
- Jadi, $\overline{A}  \cap \overline B$ adalah himpunan yang terdiri dari semua elemen yang tidak berada di $A$ dan juga tidak berada di $B$.

**Contoh**:
- Misalkan $A = \{1, 2, 3\}$ dan $B = \{3, 4, 5\}$. 
- Maka $A \cup B = \{1, 2, 3, 4, 5\}$.
- Negasi dari $A \cup B$ dalam konteks semesta $U = \{1, 2, 3, 4, 5, 6\}$ adalah $\{6\}$.
- $\overline{A} = \{4, 5, 6\}$ dan $\overline B = \{1, 2, 6\}$.
- Jadi $\overline{A} \cap \overline B = \{6\}$, yang sesuai dengan $(\overline{A \cup B})$.

### 2.Hukum De Morgan untuk Irisan: $\overline{A \cap B} = \overline{A} \cup \overline{B}$

**Pernyataan**

$\overline{A \cap B} = \overline{A} \cup \overline{B}=\{x \mid x \notin A \cap B\}=\{x \mid x \notin A \text{ atau }x \notin B\}$

**Penjelasan**:
- $A \cap B$ adalah himpunan yang terdiri dari semua elemen yang berada di kedua himpunan $A$ dan $B$.
- Negasi dari $A \cap B$, yang ditulis sebagai $(\overline{A \cap B})$, adalah himpunan yang terdiri dari semua elemen yang tidak berada di $A \cap B$.
- $\overline{A}$ adalah himpunan yang terdiri dari semua elemen yang tidak berada di $A$, dan $\overline{B}$ adalah himpunan yang terdiri dari semua elemen yang tidak berada di $B$.
- Jadi, $\overline{A} \cup \overline{B}$  adalah himpunan yang terdiri dari semua elemen yang tidak berada di $A$ atau tidak berada di $B$.

**Contoh**:
- Dengan $A = \{1, 2, 3\}$ dan  $B = \{3, 4, 5\} \
- $A \cap B = \{3\}$.
- Negasi dari $A \cap B$  dalam konteks semesta $U = \{1, 2, 3, 4, 5, 6\}$ adalah $\{1, 2, 4, 5, 6\}$.
- $\overline A = \{4, 5, 6\}$ dan $\overline B = \{1, 2, 6\}$.
- Jadi $\overline{A \cup B} = \{1, 2, 4, 5, 6\}$, yang sesuai dengan $(\overline{A \cap B})$.


### Kesimpulan

Hukum De Morgan membantu dalam memanipulasi dan memahami negasi dari operasi gabungan dan irisan pada himpunan. Ini sangat berguna dalam teori himpunan, logika proposisional, dan berbagai aplikasi matematika dan komputer. Dengan memahami hukum ini, Anda dapat lebih mudah mengelola dan bekerja dengan berbagai operasi himpunan dan logika.


### $\Diamond$ Hukum Penyerapan dalam Himpunan

### 1. Hukum Penyerapan 1: $A \cup (A \cap B) = A$
**Pernyataan**:

$A \cup (A \cap B) = \{ x \mid x \in A \text{ atau } (x \in A \text{ dan } x \in B) \}$

**Penjelasan**:
- Jika kita menggabungkan himpunan $A$ dengan irisan antara $A$ dan $B$, hasilnya tetap himpunan $A$.
- Ini karena semua elemen dari $A$ sudah ada di $A$ dan elemen dari $A \cap B$ juga sudah termasuk dalam $A$.

**Contoh**:
- Misalkan $A = \{1, 2, 3\}$ dan $B = \{3, 4, 5\}$.
- Hitung irisan: $A \cap B = \{3\}$.
- Hitung gabungan: 
  
  $A \cup (A \cap B) = A \cup \{3\} = \{1, 2, 3\} = A.$

### 2. Hukum Penyerapan 2: $A \cap (A \cup B) = A$
**Pernyataan**:

$A \cap (A \cup B) = \{ x \,|\, x \in A \text{ dan } (x \in A \text{ atau } x \in B) \}$

**Penjelasan**:
- Jika kita mengambil irisan antara himpunan $A$ dan gabungan $A$ dengan $B$, hasilnya akan tetap $A$.
- Semua elemen dalam $A$ pasti ada dalam $A \cup B$.


**Contoh**:
- Misalkan $A = \{2, 4, 6\}$ dan $B = \{1, 4, 5\}$.
- Hitung gabungan: $A \cup B = \{1, 2, 4, 5, 6\}$.
- Hitung irisan: 

  $A \cap (A \cup B) = A \cap \{1, 2, 4, 5, 6\} = \{2, 4, 6\} = A.$


### Kesimpulan

Hukum penyerapan menunjukkan bahwa operasi gabungan dan irisan dari himpunan tidak mengubah isi himpunan tersebut. Hukum ini membantu dalam menyederhanakan ekspresi himpunan.

### $\diamond$ Hukum Komplement dalam Himpunan

Hukum komplement dalam teori himpunan menjelaskan hubungan antara sebuah himpunan dan komplementnya. Berikut adalah dua hukum utama yang berkaitan dengan komplement:

### 1. Hukum Komplement 1: $A \cup \overline{A} = U$
**Pernyataan**:

$A \cup \overline{A} = \{ x \mid x \in A \text{ atau } x \notin A \}$

**Penjelasan**:
- Himpunan $A$ digabungkan dengan komplementnya $\overline{A}$ (semua elemen yang tidak ada dalam $A$) akan menghasilkan himpunan semesta $U$.
- Ini berarti bahwa setiap elemen di himpunan semesta pasti ada di $A$ atau di komplement $A$.

#### 2. Hukum Komplement 2: $A \cap \overline{A} = \emptyset$
**Pernyataan**:

$A \cap \overline{A} = \{ x \mid x \in A \text{ dan } x \notin A \}$

**Penjelasan**:
- Himpunan $A$ dan komplementnya $\overline{A}$ tidak memiliki elemen yang sama, sehingga irisan antara keduanya adalah himpunan kosong $\emptyset$.
- Artinya, tidak ada elemen yang bisa menjadi anggota $A$ sekaligus anggota komplementnya.

### Contoh

Misalkan:
- Himpunan semesta $U = \{1, 2, 3, 4, 5\}$
- Himpunan $A = \{2, 3\}$
- Komplement $\overline{A} = \{1, 4, 5\}$ (elemen yang tidak ada di $A$)

#### Menggunakan Hukum Komplement 1
- Gabungan:
  
  $A \cup \overline{A} = \{2, 3\} \cup \{1, 4, 5\} = \{1, 2, 3, 4, 5\} = U$

#### Menggunakan Hukum Komplement 2
- Irisan:
  
  $A \cap \overline{A} = \{2, 3\} \cap \{1, 4, 5\} = \emptyset$

### Kesimpulan

- **Hukum Komplement 1**: Gabungan himpunan dan komplementnya menghasilkan himpunan semesta, menunjukkan bahwa semua elemen terwakili.
- **Hukum Komplement 2**: Irisan himpunan dan komplementnya adalah himpunan kosong, menunjukkan bahwa tidak ada elemen yang tumpang tindih antara keduanya.
