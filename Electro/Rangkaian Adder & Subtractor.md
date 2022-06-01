## Rangkaian ADDER

Rangkaian Adder (penjumlah) adalah rangkaian elektronika digital yang digunakan untuk menjumlahkan dua buah angka (dalam sistem bilangan biner), sementara itu di dalam komputer rangkaian adder terdapat pada mikroprosesor dalam blok **ALU** (*Arithmetic Logic Unit*).


Sistem bilangan yang digunakan dalam rangkaian adder adalah:

- Sistem bilangan Biner (memiliki bilangan dasar 2)
- Sistem bilangan Desimal (memiliki bilangan dasar 10)

### Half-adder

Berdasarkan dua input A dan B, outputnya adalah S (sum) yang dihitung berdasarkan implementasi operasi logika XOR dari A dan B. Selain Output S (sum), output lain adalah C (carry) yang dihasilkan dari implementasi operasi logika AND. Disimpulkan S menyatakan hasil penjumlahan input A dan B, sedangakan C adalah menyatakan Carry (sisa) dari penjumlahan tersebut.

![](https://blog.kangtain.com/wp-content/uploads/Adder-Subtractor-1.png)

Dari tabel kebenaran di atas dapat dilihat bahwa cara kerja dari rangkaian half adder menyerupai rumus dasar pemjumlahan:


- 0 + 0 = 0 carry 0
- 0 + 1 = 1 carry 0
- 1 + 0 = 1 carry 0
- 1 + 1 = 0 carry 1

Pada rangkaian half adder penjumlahan yang dilakukan hanya melibatkan carry out (sisa hasil penjumlahan). Padahal pada kenyataanya sering dijumpai bahwa dalam penjumlahan selalu melibatkan carry in (sisa hasil penjumlahan yang harus ditambahkan pada bilangan berikutnya).

### Full-adder

Berdasarkan dua input seperti half-adder, Full-adder mampu menampung Carry (sisa) dari hasil penjumlahan sebelumnya.

## Rangkaian SUBTRACTOR

Sama seperti rangkaian penjumlahan biner, pada rangkaian pengurangan biner juga dapat dibagi menjadi half subtractor dan full subtractor. Rangkaian half subtractor merupakan dasar untuk menyusun atau membuat rangkaian full subtractor. Jadi untuk dapat memahami rangkaian full subtraktor, terlebih dahulu memahami prinsip dasar dari rangkaian half subtractor.

Rangkaian Subtractor di dalam komputer terdapat pada mikroprosesor dalam blok ALU (Arithmetic Logic Unit).

Sistem bilangan yang digunakan dalam rangkaian adder adalah:

- Sistem bilangan Biner (memiliki bilangan dasar 2)
- Sistem bilangan Desimal (memiliki bilangan dasar 10)

### Half-Subtractor

Berdasarkan dua input X dan Y, outputnya adalah D (difference) yang dihitung berdasarkan implementasi operasi logika XOR dari X dan Y. Selain Output D (difference), output lain adalah B (borrow) yang dihasilkan dari implementasi operasi logika AND dan NOT.

Disimpulkan D menyatakan hasil pengurangan input X dan Y, sedangakan B (borrow) adalah menyatakan digit pinjam dari pengurangan tersebut.

![](https://blog.kangtain.com/wp-content/uploads/Adder-Subtractor_2.png)

Dari tabel kebenaran di atas dapat dilihat bahwa cara kerja dari rangkaian half Subtractor serupa rumus dasar pengurangan:

- 0 - 0 = 0 borrow 0
- 0 - 1 = 1 borrow 1
-1 - 0 = 1 borrow 0
- 1 - 1 = 0 borrow 0

Pada rangkaian half Subtractor pengurangan yang dilakukan hanya melibatkan borrow out (digit pinjam). Padahal pada kenyataanya sering dijumpai bahwa dalam pengurangan selalu melibatkan borrow in (digit pinjam yang harus dikurangkan pada bilangan berikutnya).

### Full-Subtractor

Berdasarkan dua input seperti half-Subtractor, Full- Subtractor mampu mengurangkan borrow (digit pinjam) dari hasil pengurangan sebelumnya.