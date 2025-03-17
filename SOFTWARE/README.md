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

## _Draft Network Topology_
-> Block Diagramnya kurang lebih begini yang kita propose yah
![Topologi](https://github.com/user-attachments/assets/a10d6632-dd5e-4b29-8564-f471ed34edf1)

-> Penjelasan
Jadi disini kita bakal pakai MQTT sama HTTP buat komunikasi dan node red sebagai gatewaynya. Kurang lebih sama seperti di blok diagram yang diatas itu
1. Raspi bakal upload data bacaan sensor via mqtt
2. Node Red bakal subscribe ke MQTT raspi dan jadi jembatan untuk nanti disimpan ke dalam InfluxDB. Kenapa harus ada InfluxDB? karena influxDB ini fungsinya jadi database kita dan sifatnya si DB ini udah timeseries dan umum digunakan
3. Nah buat dashboarbnya ngambil data dari DB tadi itu pakai HTTP request pakai query yang ada
4. Tertampil deh datanya di dashboard
P.S. Kita bakal coba tanpa framework kaya react.js soalnya berat buat laptop, dan takutnya pas demo harus pakai laptop si usernya. Jadi kita coba buat from scrstch

# _Selamat Bekerja Semua_

