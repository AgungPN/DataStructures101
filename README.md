# Daftar Isi

- [Search](#searching)
- [Sort](#sorting)
- [Linked List](#linked-list)
- [Queu](#queue)
- [Stack](#stack)
- [Tree](#tree)

# Sorting

## Daftar algoritma sort yang di kerjakan

1. Chellenge Bubble Sort
2. Chellenge Exchange Sort
3. Bubble Sort
4. Insertion Sort
5. Selection Sort

## Sorting

Sorting adalah proses pengurutan data. _Ascending_ adalah pengurutan data dari kecil ke besar. Sedangkan _descending_ adalah pengurutan data dari besar ke kecil. Untuk visualisasi metode pengurutan bisa lihat di link berikut [visualisasi-sorting](https://visualgo.net/en/sorting).

## Metode Pengurutan

ada banyak sekali metode pengurutan, diantarannya sebagai berikut:

### Bubble Sort

![image](https://user-images.githubusercontent.com/99482764/155095410-0787c9d2-29ee-4a2e-a8a4-8d81186bcf93.png)
Burbble mengurutkan data dengan membandingkan data sekarang dengan data berikutnya. Jika yang dicari _ascanding_, maka ketika <br>`data sekarang > data berikutnya` akan ditukar. Begitu pula sebaliknya untuk _descending_ hanya tinggal ubah dari `>` menjadi `<`. Metode ini seolah-olah mengeser data dari kiri ke kanan atau sebaliknya. Kita bisa memulai membandingkan data dari paling awal/paling akhir. Bubble akan berhenti jika semua data telah diurutkan dan tidak ada pertukaran data yang bisa dilakukan lagi.

### Selection Sort

![image](https://user-images.githubusercontent.com/99482764/155095944-3d6eb274-5cbb-4f47-ac55-b6977a03024b.png)
Selection Sort merupakan metode sorting yang mengkombinasikan _searching_ dan _sorting_. Untuk setiap putaran akan dibandingkan data dari `min_index` dengan data index berikutnya. Jika `data min_index > data index berikutnya` maka akan diubah nilai dari `min_index` dengan index berikutnya(untuk _descending_ ubah simbol `>`). Setelah pembandingan data sampai pada index terakhir/perulangan selesai, maka tukar data saat ini dengan data `min_index` yang berisi data paling kecil. Untuk lebih jelas silahkan liat visualisasi diatas tadi.

### Insertion Sort

![image](https://user-images.githubusercontent.com/99482764/155095864-44507a79-f2af-4995-bdd8-af8a35f65ffb.png)
Insertion Sort merupakan metode pengurutan data yang paling cepat diantara kedua metode diatas. Insorting sort bisa diibaratkan seperti pengurutan kartu, selembar demi selembar kartu diambil lalu ditempatkan/disisipkan pada tempat yang seharusnya. Begitu juga pada sorting, data akan diurutkan dimulai dari data kedua sampai akhir. Jika ditemukkan data yang lebih kecil, maka akan disisipkan di tempatnya. Pada proses ini data-data yang lain akan bergeser ke belakang.

---

# Searching

## Penjelasan Searching

searching adalah proses pencarian data dari kumpulan data. Kumpulan data bisa berupa elemen-elemen array, mencari nomer dari range nomer tertentu, database, dan lain-lain. Ada banyak sekali metode pencarian data pada pemrograman, yang paling sering dipakai ialah **_Sequential Searching_** dan **_Binary Searching_**. Untuk melihat secara visualisasi perbedaan antara keduannya menggunakan link berikut [Searching Sorted List](https://www.cs.usfca.edu/~galles/visualization/Search.html). Untuk melihat penjelasan detailnya silahkan baca penjelasan dibawah.

## Sequential Searching

Sequential Searching merupakan metode pencarian data yang paling sederhana. Prinsip pencariannya dengan mengecek data satu persatu secara urut. Artinya jika datanya ada banyak, misal datanya ada `1000` lalu yang dicari data ke `999`, maka akan dicek datannya satu persatu dari `1-999`. Meskipun begitu ada beberapa kelebihan dari Sequential Searching salah satunnya ketika datannya tidak urut itu tidak menjadi masalah.
ALgoritma pencariannya sebagai berikut:

1. Lakukan perulangan untuk mencari data.
2. Jika `data != data yang dicari`, maka akan berpindah ke data berikutnya.
3. Jika `data == data yang dicari`, maka pencarian selesai.
4. Jika sampai data habis tapi **_data yang dicari_** tidak ditemukan, maka data tidak ada.

## Binary Searching

Binary Searching merupakan metode pencarian data secara **_biner_**. Artinya jika data yang dicari melebihi nilai tengah maka setelah tengah akan bernilai `1` dan sebelum nilai tengah akan bernilai `0` atau diabaikan. Sebelum mencari data menggunakan metode Binary Searching kita harus mengurutkan data terlebih dahulu, jika tidak pencarian tidak akan berjalan dengan baik. Kelebihan dari Binary Searching ialah pencariannya lebih cepat, karena tidak mengecek datanya satu persatu, langsung eliminasi **_1/2_** data seperti penjelasan diatas.
Algoritma pencariannya sebagai berikut:

1. Urutkan data
2. Lakukan perulangan untuk mencari data.
3. Cari _data tengah_ `(posisi awal + posisi akhir)/2`.
4. Lalu bandingkan _data tengah_ dengan _data yang dicari_.
5. Jika `data yang dicari > data tengah`, maka `posisi awal = data tengah + 1` lalu ulang algoritma dari nomer 3.
6. Jika `data yang dicari < data tengah`, maka `posisi akhir = data tengah - 1` lalu ulang algoritma dari nomer 3.
7. Jika `data yang dicari == data tengah`, maka pencarian selesai.
8. Jika sampai data habis tapi **_data yang dicari_** tidak ditemukkan, maka data tidak ada.

---

# Linked List

Linked list merupakan sekumpulan node yang saling terhubung yang dihubungkan melalui pointer/link secara berurutan. Sederhanannya, setiap node yang ada akan dihubungkan dengan node lain dengan memanfaatkan pointer. Pada setiap node terdapat dua bagian, bagian awal untuk data(data boleh lebih dari 1), lalu bagian kedua berupa alamat node berikutnya. Linked list juga merupakan dasar dari database, artinya jika kita memahami linked list maka kita memahami dasar dari pembuatan database. Untuk membaca data di linked list kita harus selalu memulai dengan data head berlanjut ke data selanjutnya, tidak seperti array yang bisa membaca data dengan spesifik index tertentu. Untuk gambaran pengunaan linked list bisa lihat link berikut [visualisasi-linked-list](https://visualgo.net/en/list?slide=1)

## Materi yang perlu dipelajari sebelum linked list

1. dasar-dasar pemograman (pada kasus ini terutama bahasa C).
1. struct, dengan struct memungkinkan kita bekerja dengan satu record yang terdapat banyak field. Karena itulah untuk membuat node kita memerlukan struct.
1. pointer, dengan pointer kita bisa membuat data secara dinamis sekaligus untuk menghubungkan antar node kita memerlukan pointer.

## Jenis-jenis Linked list

### Single Linked List

> single linked list merupakan jenis linked list yang paling simple, yang mana datanya dimulai dari head berlanjut ke data berikutnya sampai node terakhir yang mengarah ke alamat `NULL`, yang artinya data berakhir. <br>  
> ![image](https://media.geeksforgeeks.org/wp-content/uploads/singly-linkedlist.png)

### Double Linked List

> dengan menggunakan double linked list kita tidak hanya bisa pindah ke alamat selanjutnya (_next_), tapi juga ke alamat sebelumnya (_previous_) dan data terakhir akan mengarah ke alamat `NULL` > ![image](https://media.geeksforgeeks.org/wp-content/cdn-uploads/gq/2014/03/DLL1.png)

### Circular Linked List

> circular linked list itu seperti single linked list, tetapi tidak ada data terakhir. Hal tersebut terjadi karena data terakhir akan dihubungkan dengan data pertama hingga membentuk suatu _circle_.
> ![image](https://media.geeksforgeeks.org/wp-content/uploads/CircularLinkeList.png)

---

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

---

# Stack

stack atau tumpukan adalah struktur data linier dalam pemograman yang bersifat LIFO (Last In First Out). Artinya data yang terakhir masuk ke struktur data, maka menjadi data pertama yang akan keluar. Untuk visualisasinya bisa liat link berikut pada bagian stack [visualisasi-stack](https://visualgo.net/en/list?slide=1).
![image](https://cdn.programiz.com/sites/tutorial2program/files/stack-operations.png)
Disini top digunakan sebagai penanda banyaknya data, dengan begitu bisa digunakan untuk menentukkan apakah data _kosong_ atau _full_.

## fungsi-fungsi pada stack

1. `push` = digunakan untuk `menambah data` stack paling atas.
1. `pop` = digunakan untuk `mengambil data` stack paling atas.
1. `clear` = digunakan untuk `mengosongkan data` stack.
1. `isEmpty` = digunakan untuk `mengecek` apakah data stack `kosong`.
1. `isFull` = digunakan untuk `mengecek` apakah data stack `penuh`.

---

# Tree

tree merupakan kumpulan node yang membentuk sebuah _tree_ atau pohon, yang diawali oleh _root_ dan diakhiri oleh _leaf_. Tree dibedakn menjadi 2 jenis, **statik** yang datanya tetap, dan **dinamis** yang datanya bisa di rubah-rubah. Untuk lebih jelas lihat visualisasi pada link ini [visualisasi-tree](http://btv.melezinek.cz/binary-search-tree.html)  
<br>![terminologi-tree](https://4.bp.blogspot.com/-kRRhE_q3Rrs/WlmGpBrKlJI/AAAAAAAABRc/evU6gm5v-8UCbJeN8EQ8Tf21B-p_uYA2gCLcBGAs/s1600/Capture.JPG)

> **_Binary tree_**, semua node(_kecuali leaf_) memiliki 2 _child_. dan disebelah kanan adalah child yang memiliki nilai lebih besar dari _parent_, dan sebelah kiri yang memiliki nilai lebih kecil.

## Operasi-perasi Tree

1. `create` membentuk tree baru yang kosong.
1. `clear` menghapus semua node pada tree.
1. `empty` mengetahui apakah tree kosong.
1. `insert` menambah node kedalah tree.
1. `find` mencari node pada tree.
1. `traverse` kunjungan terhadap node-node dalam tree, dah setiap node hanya dikunjungi 1x.
1. `count` menghitung jumlah node pada tree.
1. `height` mengetahui kedalaman tree.
1. `find min and max` mencari nilai terkecil dan terbesar.
1. `child` mengetahui anak dari sebuah node(jika punya).

## Jenis Transverse

1. `PreOrder`: cetak node yang dikunjungi, kunjungi left, kunjungi right (tengah, kiri, kanan)
1. `InOrder`: kunjungi left, cetak node yang dikunjungi, kunjungi right (kiri, tengah, kanan)
1. `PostOrder`: kunjungi left, kunjungi right, cetak node yang dikunjungi (kiri, kanan, tengah)
