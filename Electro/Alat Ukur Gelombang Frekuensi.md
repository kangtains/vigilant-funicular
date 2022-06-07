# Alat Ukur Gelombang Frekuensi

Frekuensi ialah jumlah gelombang atau getaran yang dihasilkan tiap detik.

![](https://kangtain.com/images/8/84/U-Alatukurgel02.png)

Amplitudo atau nilai puncak suatu sinyal adalah ukuran seberapa besar tegangan. Amplitudo sinyal merupakan setengah dari nilai puncak ke puncak. Gelombang dengan nilai amplitudo sebesar 5 V dan nilai puncak ke puncak sebesar 10 V.

![](https://kangtain.com/images/6/62/Alatukurgel03.png)

**Periode** (`T`) adalah lamanya waktu yang dibutuhkan oleh sinyal untuk membentuk satu gelombang penuh. Periode disimbolkan dengan huruf T, dan satuan dari periode dinyatakan dalam detik atau second (s). Gelombang dengan nilai periode sebesar 1/2 detik.

## Gelombang Frekuensi

Adaptor atau power suplay menggunakan trafo Center Tape

![](https://kangtain.com/images/0/0f/Alatukurgel01.png)

Dari dua definisi tersebut terdapat pengertian, bahwa jika suatu gelombang penuh mempunyai perioda sebesar T detik maka banyaknya gelombang penuh yang terjadi setiap detiknya ( f ) adalah: 

![](https://kangtain.com/images/e/e3/Alatukurgel04.png)

Dimana `f` adalah frekuensi dalam cycle/secon atau Herzt (`Hz`) dan `T` adalah Perioda dalam detik.

## Sumber Gelombang

### Osilator

Osilator memanfaatkan sinyal derau / noise yang berasal dari penguat itu sendiri. Saat Penguat diberikan suplay tegangan, sinyal derau / noise akan terjadi, kemudian diumpanbalik ke Penguat, maka Osilasi akan terjadi.

![](https://kangtain.com/images/6/6a/Alatukurgel05.png)

### Osilator flip-flop 2 transistor

Yang membuat rangkaian flip-flop 2 transistor ini memiliki 2 kondisi saling bergantian antara cut-off dan saturasi adalah rangkaian RC pada kedua transistor.

Dengan asumsi bahwa transistor TR1 berada pada posisi cut-off (OFF) dan TR2 dalam kondisi saturasi (ON) maka C2 akan melakukan pengisian muatan melalui R2 ke ground melalui kolektor emitor TR2, kemudian pada saat muatan telah penuh maka transistor TR1 mendapat bias maju sehingga berubah menjadi saturasi (ON) kondisi ini akan memaksa berubah kondisi transistor TR2 menjadi cut-off (OFF) dengan cepat sehingga muatan C2 akan dilepas melalui basis TR1 dan pada saat yang sama C1 mengisi muatan sampai penuh melalui R3 ke ground melalui kolektor emitor TR1.

![](https://kangtain.com/images/c/c3/Alatukurgel06.png)

Dengan asumsi bahwa transistor Q1 berada pada posisi cut-off (OFF) dan Q2 dalam kondisi saturasi (ON) maka C2 akan melakukan pengisian muatan melalui R3 ke ground melalui kolektor emitor Q2.

![](https://kangtain.com/images/e/e0/Alatukurgel07.png)

Saat muatan C2 penuh, maka cukup untuk memberikan bias maju pada transistor Q1 sehingga menjadi saturasi (ON) kondisi ini memaksa transistor Q2 menjadi cut-off (OFF) sehingga muatan C2 dibuang melalui basis Q1 dan selanjutnya C1 mulai mengisi muatan melalui R2 ke ground melalui kolektor emitor Q1.

![](https://kangtain.com/images/b/bc/Alatukurgel08.png)

Kondisi 2 keadaan pada kedua transistor yang selalu cut off dan saturasi secara bergantian ini memberikan output berupa pulsa yang terus menerus dengan frekuensi ditentukan oleh kecepatan waktu pengisian dan pengosongan kapasitor umpan balik kedua bagian. Frekuesi pulsa yang dihasilkan rangkaian flip-flop 2 transistor (astabil multivibrator) sbb: 

![](https://kangtain.com/images/e/e3/Alatukurgel04.png)

![](https://kangtain.com/images/6/68/Alatukurgel09.png)