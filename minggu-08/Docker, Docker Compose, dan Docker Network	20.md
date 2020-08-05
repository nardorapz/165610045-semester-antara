Penggunaan
Virtualisasi tingkat sistem operasi umumnya digunakan dalam lingkungan hosting virtual, di mana ia berguna untuk mengalokasikan sumber daya perangkat keras yang 
terbatas secara aman di antara sejumlah besar pengguna yang saling curiga. Administrator sistem juga dapat menggunakannya untuk mengkonsolidasikan perangkat keras 
server dengan memindahkan layanan pada host yang berbeda ke dalam wadah di satu server.

Skenario khas lainnya termasuk memisahkan beberapa program untuk memisahkan wadah untuk meningkatkan keamanan, kemandirian perangkat keras, 
dan menambahkan fitur manajemen sumber daya. Namun, peningkatan keamanan yang disediakan oleh penggunaan mekanisme chroot, sama sekali tidak ada. 
Implementasi virtualisasi tingkat sistem operasi yang mampu melakukan migrasi langsung juga dapat digunakan untuk menyeimbangkan 
muatan dinamis kontainer antara node dalam sebuah cluster.

Atas Virtualisasi tingkat sistem operasi biasanya membebankan lebih sedikit overhead daripada virtualisasi penuh karena program dalam 
partisi virtual tingkat OS menggunakan antarmuka panggilan sistem normal sistem operasi dan tidak perlu dikenakan emulasi atau dijalankan 
dalam mesin virtual perantara, seperti halnya kasus dengan virtualisasi penuh (seperti VMware ESXi, QEMU, atau Hyper-V) dan paravirtualization 
(seperti Xen atau User-mode Linux). Bentuk virtualisasi ini juga tidak memerlukan dukungan perangkat keras untuk kinerja yang efisien.

Fleksibilitas
Virtualisasi tingkat sistem operasi tidak sefleksibel pendekatan virtualisasi lainnya karena tidak dapat meng-host sistem operasi tamu yang berbeda dari host, 
atau kernel tamu yang berbeda. Misalnya, dengan Linux, distribusi yang berbeda baik-baik saja, tetapi sistem operasi lain seperti Windows tidak dapat di-host. 
Sistem operasi menggunakan sistematika input variabel tunduk pada batasan dalam arsitektur yang divirtualisasikan. Metode adaptasi termasuk cloud-server relay
analytics menjaga lingkungan virtual level OS dalam aplikasi ini.

Solaris sebagian mengatasi batasan yang dijelaskan di atas dengan fitur zona bermereknya, yang memberikan kemampuan untuk menjalankan lingkungan dalam wadah yang 
mengemulasi versi Solaris 8 atau 9 yang lebih lama dalam host Solaris 10. 
Zona bermerek Linux (disebut zona bermerek "lx") juga tersedia pada sistem Solaris berbasis x86, menyediakan ruang pengguna Linux yang lengkap 
dan dukungan untuk pelaksanaan aplikasi Linux; selain itu, Solaris menyediakan utilitas yang diperlukan 
untuk menginstal Red Hat Enterprise Linux 3.x atau CentOS 3.x Linux di dalam zona "lx".Namun, pada 2010 zona bermerek Linux 
telah dihapus dari Solaris; pada tahun 2014 mereka diperkenalkan kembali di Illumos, 
yang merupakan garpu open source Solaris, mendukung kernel Linux 32-bit.

Penyimpanan
Beberapa implementasi menyediakan mekanisme copy-on-write (CoW) tingkat file. (Paling umum, sistem file standar dibagi di antara partisi, 
dan partisi yang mengubah file secara otomatis membuat salinannya sendiri.) Ini lebih mudah untuk membuat cadangan, lebih hemat-ruang dan lebih mudah untuk 
di-cache daripada penyalinan tingkat blok. Skema -write umum pada virtualizers seluruh sistem. Namun, virtualisasi seluruh sistem dapat bekerja dengan sistem file 
non-asli dan membuat dan memutar kembali snapshot dari seluruh kondisi sistem.
