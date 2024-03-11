# Queue

queue atau antrian adalah struktur data linier dalam pemograman yang bersifat FIFO (First In First Out). Artinya data pertama yang masuk akan menjadi data pertama yang keluar. Untuk logikannya seperti ketika kita menganti sesuatu (misalnya mengantri sembako), maka siapa yang mengantri dulu dialah yang pertama mendapatkan sembako terlebih dahulu. Untuk visualisasinya bisa lihat di link berikut [visualisasi-queue](https://visualgo.net/en/list?slide=1).
![image](https://upload.wikimedia.org/wikipedia/commons/thumb/5/52/Data_Queue.svg/800px-Data_Queue.svg.png)

Dari gambar diatas, kita bisa melihat bahwa data yang masuk mengantri dibelakang, sedangkan data yang keluar yang berada didepan, jadi seperti ada pintu masuk di _back_ dan pintu keluar di _front_. Kemudian _back_ lebih dikenal dengan istilah _tail_, sedangkan _front_ dikenal dengan head.

## Fungsi-fungsi pada queue

1. `isEmpty` fungsi untuk mengecek apakah data masih kosong.
1. `isFull` fungsi untuk mengecek apakah data sudah full.
1. `enqueue` fungsi untuk menambahkan data paling belakang.
1. `dequeue` fungsi untuk menghapus data paling awal.
1. `tampil` fungsi untuk mencetak semua data.
1. `clear` fungsi untuk membersihkan/menghapus semua data.
