# tree

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
