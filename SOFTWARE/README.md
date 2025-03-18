# Software Development
## _Welcome to IoT Dashboard Friends_

Pada laman ini setidaknya akan membahas perihal website developing, mulai dari UI/UX design, frontend, dan backend. 

Selayang pandang untuk pembuatan website ini setidaknya kita perlu beberapa hal:
1. Frontend Development
Di bagian ini, temen temen akan fokus membahas tampilan/interface dari dashboard kita setidaknya ada beberapa hal yang perlu dipersiapkan, antara lain HTML, CSS, dan JavaScript
2. Backend Devlopment
Bagian ini gimana cara ngehubuungin antara database dan frontendnya. Jadi ini sebagai jembatannya, karena akan menggunakan raspi jadi kemungkinan besar bisa pakai algoritma mqtt nanti atau websocket yang support atau bahkan pake HTTP. Kita lihat perkembangannya
3. Database Devlopment
Bagian ini lebih untuk membuat gudang/storing data sehingga bisa dapat diolah dan ditampilkan pada dashboard kita


# _Draft Network_
Pada network nanti kurang lebih alurnya seperti pada blok diagram berikut:

![Topologi](https://github.com/user-attachments/assets/4b5e0089-8049-4669-97ea-c39919bd6547)

Raspi akan upload data sensor dengan protokol mqtt yang bakal store di database laragon untuk nyimpen data sensor tadi. Setelah disimpan, data tadi bakal difetch pakai HTTP buat dashboardnya ambil data. 
* P.S: Databse ini bisa dibicarain lebih lanjut ya laragon ini salah satu opsi karena dia lokal dan udah umum developmentnya
# _Selamat Bekerja Semua_

