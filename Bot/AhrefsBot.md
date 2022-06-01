**AhrefsBot** adalah Web Crawler yang mendukung database tautan 12 triliun untuk perangkat pemasaran online Ahrefs. Itu terus-menerus merayapi web untuk mengisi basis data kami dengan tautan baru dan memeriksa status tautan yang ditemukan sebelumnya untuk memberikan data paling komprehensif dan terkini kepada pengguna kami.

Data tautan yang dikumpulkan oleh Ahrefs Bot dari web digunakan oleh ribuan pemasar digital di seluruh dunia untuk merencanakan, melaksanakan, dan memantau kampanye pemasaran online mereka.

Data ini memiliki nilai yang sangat besar bagi komunitas SEO karena membantu profesional pemasaran untuk lebih memahami algoritme dasar dari mesin pencari terbesar di dunia sehingga mereka dapat mengoptimalkan situs web yang sesuai. Setiap 24 jam perayap kami mengunjungi lebih dari 6 miliar halaman web dan memperbarui indeks Ahrefs setiap 15-30 menit.

Menurut studi pihak ketiga baru-baru ini tentang “bot yang baik”, AhrefsBot adalah perayap paling aktif kedua setelah Googlebot.

## Apa yang dilakukan AhrefsBot di situs web Anda?

AhrefsBot merayapi situs web Anda membuat catatan tautan keluar dan menambahkannya ke basis data kami. Ini akan merayapi ulang situs web Anda secara berkala untuk memeriksa status terkini dari tautan yang ditemukan sebelumnya.

Perayap kami tidak mengumpulkan atau menyimpan informasi lain tentang situs web Anda. Ini tidak memicu iklan di situs web Anda dan tidak akan menambahkan angka ke lalu lintas Google Analytics Anda.

## Bagaimana cara mengontrol AhrefsBot di situs web Anda?

Seperti disebutkan di atas, AhrefsBot secara ketat mengikuti file `robots.txt` di situs web Anda. Jadi Anda dapat sepenuhnya mengontrolnya di situs web Anda jika Anda membutuhkannya.

Untuk mengubah frekuensi AhrefsBot mengunjungi situs Anda, Anda dapat menentukan penundaan minimum yang dapat diterima antara dua permintaan berturut-turut dari bot kami di file `robots.txt` Anda:

```shell
User-agent: AhrefsBot
Crawl-Delay: [value]
```

Dimana nilai Crawl-Delay adalah waktu dalam detik.

Jika karena alasan tertentu Anda ingin mencegah AhrefsBot mengunjungi situs Anda, masukkan dua baris berikut ke dalam file `robots.txt` di server Anda:

```shell
User-agent: AhrefsBot
Disallow: /
```

Harap perhatikan bahwa AhrefsBot mungkin memerlukan waktu untuk memilih perubahan pada file `robots.txt` Anda. Ini akan dilakukan sebelum setiap perayapan terjadwal berikutnya.

Harap perhatikan juga bahwa jika `robots.txt` Anda berisi kesalahan dan AhrefsBot tidak akan dapat mengenali perintah Anda, ia akan terus merayapi situs web Anda seperti sebelumnya.

##### Source
- [ahrefsdotcom](https://ahrefs.com/robot)