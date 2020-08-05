1. Docker Engine adalah 

teknologi kontainerisasi sumber terbuka untuk membangun dan membuat wadah aplikasi Anda. Docker Engine bertindak sebagai aplikasi server-klien dengan:

Server dengan proses daemon yang sudah berjalan lama dockerd.
API yang menentukan antarmuka yang dapat digunakan oleh program untuk berbicara dan memerintahkan daemon Docker.
Docker klien antarmuka baris perintah (CLI).
CLI menggunakan Docker API untuk mengontrol atau berinteraksi dengan daemon Docker melalui scripting atau perintah CLI langsung. Banyak aplikasi Docker lainnya menggunakan API dan CLI yang mendasarinya. Daemon membuat dan mengelola objek Docker, seperti gambar, wadah, jaringan, dan volume.

Untuk detail lebih lanjut, lihat Arsitektur Docker.

Panduan pengguna Docker
Untuk mempelajari tentang Docker lebih detail dan untuk menjawab pertanyaan tentang penggunaan dan implementasi, lihat halaman ikhtisar di "memulai".

Panduan pemasangan
Bagian instalasi menunjukkan kepada Anda bagaimana menginstal Docker pada berbagai platform.

Catatan rilis
Ringkasan perubahan dalam setiap rilis dalam seri saat ini sekarang dapat ditemukan di halaman Notes Release terpisah

Kebijakan Penghentian Fitur
Karena ada perubahan pada Docker, ada kalanya fitur yang ada perlu dihapus atau diganti dengan fitur yang lebih baru. Sebelum fitur yang ada dihapus, ia dilabeli sebagai "usang" dalam dokumentasi dan tetap di Docker untuk setidaknya 3 rilis stabil kecuali ditentukan secara eksplisit sebaliknya. Setelah waktu itu dapat dihapus.

Pengguna diharapkan untuk mencatat daftar fitur yang sudah usang setiap rilis dan merencanakan migrasi mereka jauh dari fitur-fitur tersebut, dan (jika berlaku) ke fitur penggantian sesegera mungkin.

Daftar lengkap fitur yang sudah usang dapat ditemukan di halaman Fitur yang sudah tidak digunakan lagi.

Perizinan
Docker dilisensikan di bawah Lisensi Apache, Versi 2.0. Lihat LICENSE untuk teks lisensi lengkap.

sumber daya untuk pengembang aplikasi yang ingin membangun aplikasi baru menggunakan Docker.

Prasyarat
Bekerja melalui modul pembelajaran di Mulai untuk memahami cara membuat gambar dan menjalankannya sebagai aplikasi kemas.

Kembangkan aplikasi baru di Docker
Jika Anda baru saja mulai mengembangkan aplikasi baru di Docker, lihat sumber daya ini untuk memahami beberapa pola paling umum untuk mendapatkan manfaat maksimal dari Docker.

Gunakan multi-stage build untuk menjaga gambar Anda ramping
Kelola data aplikasi menggunakan volume dan bind mount
Skala aplikasi Anda dengan Kubernetes
Skala aplikasi Anda sebagai layanan Swarm
Praktik terbaik pengembangan aplikasi umum
Pelajari tentang pengembangan aplikasi khusus bahasa dengan Docker
Docker untuk lab pengembang Java
Port aplikasi node.js ke lab Docker
Aplikasi Ruby on Rails di lab Docker
Dockerize aplikasi .Net Core
Dockerize aplikasi ASP.NET Core dengan SQL Server di Linux menggunakan Docker Compose
Pengembangan lanjutan dengan SDK atau API
Setelah Anda dapat menulis Dockerfiles atau Compose file dan menggunakan Docker CLI, bawa ke level berikutnya dengan menggunakan 
Docker Engine SDK untuk Go / Python atau gunakan HTTP API secara langsung.

2. Virtualisasi tingkat OS mengacu pada paradigma sistem operasi di mana kernel memungkinkan adanya beberapa instance ruang pengguna yang terisolasi. 
Contoh seperti itu, disebut wadah (LXC, wadah Solaris, Docker), Zona (wadah Solaris), server pribadi virtual (OpenVZ), partisi, lingkungan virtual (VE), 
kernel virtual (DragonFly BSD), atau penjara (penjara FreeBSD atau penjara chroot) ), [1] mungkin terlihat seperti komputer nyata dari sudut pandang program yang
berjalan di dalamnya. Program komputer yang berjalan pada sistem operasi biasa dapat melihat semua sumber daya (perangkat yang terhubung, file dan folder, pembagian 
jaringan, daya CPU, kemampuan perangkat keras yang dapat diukur) dari komputer tersebut. Namun, program yang berjalan di dalam wadah hanya dapat melihat konten dan
perangkat kontainer yang ditugaskan ke wadah.

Pada sistem operasi mirip Unix, fitur ini dapat dilihat sebagai implementasi lanjutan dari mekanisme chroot standar, yang mengubah folder root yang terlihat untuk 
proses yang sedang berjalan dan anak-anaknya. Selain mekanisme isolasi, kernel sering menyediakan fitur manajemen sumber daya untuk membatasi dampak aktivitas satu 
wadah pada wadah lain.

Istilah kontainer, sementara yang paling populer mengacu pada sistem virtualisasi tingkat OS, kadang-kadang secara ambigu digunakan untuk merujuk pada lingkungan 
mesin virtual yang lebih penuh yang beroperasi dalam berbagai tingkat konser dengan OS host, mis. Wadah Microsoft Hyper-V.

Operasi
Pada sistem operasi biasa untuk komputer pribadi, sebuah program komputer dapat melihat (meskipun mungkin tidak dapat mengakses) semua sumber daya sistem. Mereka termasuk:

Kemampuan perangkat keras yang dapat digunakan, seperti CPU dan koneksi jaringan
Data yang dapat dibaca atau ditulis, seperti file, folder, dan berbagi jaringan
Periferal yang terhubung dapat berinteraksi dengannya, seperti webcam, printer, pemindai, atau faks
Sistem operasi mungkin dapat mengizinkan atau menolak akses ke sumber daya tersebut berdasarkan program mana yang meminta mereka dan akun pengguna dalam 
konteks yang dijalankannya. Sistem operasi juga dapat menyembunyikan sumber daya tersebut, sehingga ketika program komputer menyebutkannya, mereka tidak muncul dalam 
hasil enumerasi. Namun demikian, dari sudut pandang pemrograman, program komputer telah berinteraksi dengan sumber daya tersebut dan sistem operasi telah mengatur 
tindakan interaksi.

Dengan virtualisasi sistem operasi, atau containerisasi, dimungkinkan untuk menjalankan program di dalam wadah, yang hanya dialokasikan sebagian sumber daya ini. 
Suatu program yang mengharapkan untuk melihat seluruh komputer, setelah dijalankan di dalam sebuah wadah, hanya dapat melihat sumber daya yang dialokasikan dan 
percaya bahwa hanya itu yang tersedia. Beberapa wadah dapat dibuat di setiap sistem operasi, yang masing-masingnya dialokasikan sumber daya komputer. 
Setiap wadah dapat berisi sejumlah program komputer. Program-program ini dapat berjalan secara bersamaan atau terpisah, dan bahkan dapat berinteraksi satu sama lain.

Penggunaan
Virtualisasi tingkat sistem operasi umumnya digunakan dalam lingkungan hosting virtual, di mana ia berguna untuk mengalokasikan sumber daya perangkat keras yang 
terbatas secara aman di antara sejumlah besar pengguna yang saling curiga. Administrator sistem juga dapat menggunakannya untuk mengkonsolidasikan perangkat keras 
server dengan memindahkan layanan pada host yang berbeda ke dalam wadah di satu server.

Skenario khas lainnya termasuk memisahkan beberapa program untuk memisahkan wadah untuk meningkatkan keamanan, kemandirian perangkat keras, dan menambahkan fitur 
manajemen sumber daya. Namun, peningkatan keamanan yang disediakan oleh penggunaan mekanisme chroot, sama sekali tidak ada. Implementasi virtualisasi tingkat 
sistem operasi yang mampu melakukan migrasi langsung juga dapat digunakan untuk menyeimbangkan muatan dinamis kontainer antara node dalam sebuah cluster.

Atas
Virtualisasi tingkat sistem operasi biasanya membebankan lebih sedikit overhead daripada virtualisasi penuh karena program dalam 
partisi virtual tingkat OS menggunakan antarmuka panggilan sistem normal sistem operasi dan tidak perlu dikenakan emulasi atau 
dijalankan dalam mesin virtual perantara, seperti halnya kasus dengan virtualisasi penuh (seperti VMware ESXi, QEMU, atau Hyper-V) dan 
paravirtualization (seperti Xen atau User-mode Linux). 
Bentuk virtualisasi ini juga tidak memerlukan dukungan perangkat keras untuk kinerja yang efisien.

Fleksibilitas
Virtualisasi tingkat sistem operasi tidak sefleksibel pendekatan virtualisasi lainnya karena tidak dapat meng-host sistem operasi tamu yang berbeda dari host, 
atau kernel tamu yang berbeda. Misalnya, dengan Linux, distribusi yang berbeda baik-baik saja, tetapi sistem operasi lain seperti Windows tidak dapat di-host. 
Sistem operasi menggunakan sistematika input variabel tunduk pada batasan dalam arsitektur yang divirtualisasikan. Metode adaptasi termasuk cloud-server 
relay analytics menjaga lingkungan virtual level OS dalam aplikasi ini.

Solaris sebagian mengatasi batasan yang dijelaskan di atas dengan fitur zona bermereknya, yang memberikan kemampuan untuk menjalankan lingkungan dalam wadah yang 
mengemulasi versi Solaris 8 atau 9 yang lebih lama dalam host Solaris 10. Zona bermerek Linux (disebut zona bermerek "lx") juga tersedia pada sistem Solaris 
berbasis x86, menyediakan ruang pengguna Linux yang lengkap dan dukungan untuk pelaksanaan aplikasi Linux; selain itu, Solaris menyediakan utilitas yang diperlukan 
untuk menginstal Red Hat Enterprise Linux 3.x atau CentOS 3.x Linux di dalam zona "lx".Namun, pada 2010 zona bermerek Linux telah dihapus dari Solaris; 
pada tahun 2014 mereka diperkenalkan kembali di Illumos, yang merupakan garpu open source Solaris, mendukung kernel Linux 32-bit.
