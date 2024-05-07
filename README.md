# 1.2
![alt text](img/Screen%20Shot%202024-05-07%20at%2007.44.31.png)
Fungsi async akan berjalan di luar fungsi utama yang menjalankanny, sehingga hey hye bisa saja berjalan sebelum dua output lain karena ia berada di luar fungsi async, jadi ia bisa dicetak saat fungsi async masih menunggu.

# 1.3
![alt text](img/Screen%20Shot%202024-05-07%20at%2009.41.40.png)
Banyak spawner membuat lebih banyak task yang dapat dilakukan karena lebih banyak task yang dimasukkan kedalam queue. Karena spawner tidak di drop, program tidak mati dengan sendirinya karena ia berasumsi masih ada pengiriman data dari spawner. 

Saat suatu fungsi spawn dipanggil, terbuat task baru yang dimasukkan kedalam task sender. Executor akan mengambil satu task dari sender dan mengekeskusinya, dan mengulangi hal tsb sampai spawner drop/interaksi selesai. 
