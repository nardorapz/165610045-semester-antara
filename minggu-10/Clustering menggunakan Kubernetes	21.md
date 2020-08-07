Kubernetes adalah platform open-source portabel, dapat diperluas, untuk mengelola beban kerja dan layanan dalam container, yang memfasilitasi konfigurasi dan otomatisasi deklaratif. Ini memiliki ekosistem yang besar dan berkembang pesat. Layanan, dukungan, dan alat Kubernetes tersedia secara luas.
Halaman ini adalah ringkasan Kubernetes.

Kubernetes adalah platform open-source portabel, dapat diperluas, untuk mengelola beban kerja dan layanan dalam container, yang memfasilitasi konfigurasi dan otomatisasi deklaratif. Ini memiliki ekosistem yang besar dan berkembang pesat. Layanan, dukungan, dan alat Kubernetes tersedia secara luas.

Nama Kubernetes berasal dari bahasa Yunani yang berarti juru mudi atau pilot. Google open-source proyek Kubernetes pada tahun 2014. Kubernetes menggabungkan lebih dari 15 tahun pengalaman Google dalam menjalankan beban kerja produksi dalam skala besar dengan gagasan dan praktik terbaik dari komunitas.

Era penyebaran tradisional: Sejak awal, organisasi menjalankan aplikasi di server fisik. Tidak ada cara untuk menentukan batas sumber daya untuk aplikasi di server fisik, dan ini menyebabkan masalah alokasi sumber daya. Misalnya, jika beberapa aplikasi berjalan di server fisik, mungkin ada contoh di mana satu aplikasi akan menggunakan sebagian besar sumber daya, dan akibatnya, aplikasi lain akan berkinerja buruk. Solusi untuk ini adalah menjalankan setiap aplikasi di server fisik yang berbeda. Tetapi ini tidak berskala karena sumber daya kurang dimanfaatkan, dan mahal bagi organisasi untuk memelihara banyak server fisik.

Era penyebaran virtual: Sebagai solusi, virtualisasi diperkenalkan. Hal ini memungkinkan Anda untuk menjalankan beberapa Mesin Virtual (VM) pada CPU server fisik tunggal. Virtualisasi memungkinkan aplikasi untuk diisolasi antara VM dan menyediakan tingkat keamanan karena informasi dari satu aplikasi tidak dapat diakses secara bebas oleh aplikasi lain.

Virtualisasi memungkinkan pemanfaatan sumber daya yang lebih baik di server fisik dan memungkinkan skalabilitas yang lebih baik karena aplikasi dapat ditambahkan atau diperbarui dengan mudah, mengurangi biaya perangkat keras, dan banyak lagi. Dengan virtualisasi, Anda dapat menyajikan sekumpulan sumber daya fisik sebagai sekumpulan mesin virtual sekali pakai.

Setiap VM adalah mesin lengkap yang menjalankan semua komponen, termasuk sistem operasinya sendiri, di atas perangkat keras tervirtualisasi.

Era penerapan kontainer: Penampung mirip dengan VM, tetapi mereka memiliki properti isolasi yang santai untuk berbagi Sistem Operasi (OS) di antara aplikasi. Karena itu, wadah dianggap ringan. Mirip dengan VM, container memiliki sistem file, CPU, memori, ruang proses, dan lainnya sendiri. Karena dipisahkan dari infrastruktur yang mendasarinya, mereka portabel di cloud dan distribusi OS.

Container menjadi populer karena memberikan manfaat tambahan, seperti:

Pembuatan dan penerapan aplikasi tangkas: meningkatkan kemudahan dan efisiensi pembuatan gambar container dibandingkan dengan penggunaan gambar VM.
Pengembangan berkelanjutan, integrasi, dan penerapan: menyediakan pembuatan dan penerapan gambar container yang andal dan sering dengan rollback yang cepat dan mudah (karena kekekalan gambar).
Pemisahan perhatian Dev dan Ops: buat gambar container aplikasi pada waktu build / rilis daripada waktu penerapan, sehingga memisahkan aplikasi dari infrastruktur.
Pengamatan tidak hanya menampilkan informasi dan metrik tingkat OS, tetapi juga kesehatan aplikasi dan sinyal lainnya.
Konsistensi lingkungan di seluruh pengembangan, pengujian, dan produksi: Berjalan di laptop seperti halnya di cloud.
Portabilitas distribusi Cloud dan OS: Berjalan di Ubuntu, RHEL, CoreOS, lokal, cloud publik utama, dan di mana pun.
Manajemen aplikasi-sentris: Meningkatkan tingkat abstraksi dari menjalankan OS pada perangkat keras virtual untuk menjalankan aplikasi pada OS menggunakan sumber daya logis.
Layanan mikro yang digabungkan, didistribusikan, elastis, dan dibebaskan secara longgar: aplikasi dipecah menjadi bagian-bagian yang lebih kecil dan independen dan dapat digunakan dan dikelola secara dinamis - bukan tumpukan monolitik yang dijalankan pada satu mesin satu tujuan besar.
Isolasi sumber daya: kinerja aplikasi yang dapat diprediksi.
Pemanfaatan sumber daya: efisiensi dan kepadatan tinggi.
Mengapa Anda membutuhkan Kubernetes dan apa fungsinya
Kontainer adalah cara yang baik untuk menggabungkan dan menjalankan aplikasi Anda. Dalam lingkungan produksi, Anda perlu mengelola container yang menjalankan aplikasi dan memastikan tidak ada waktu henti. Misalnya, jika sebuah wadah turun, wadah lain harus dimulai. Bukankah lebih mudah jika perilaku ini ditangani oleh sistem?

Begitulah cara Kubernetes datang untuk menyelamatkan! Kubernetes memberi Anda kerangka kerja untuk menjalankan sistem terdistribusi dengan tangguh. Ini menangani penskalaan dan failover untuk aplikasi Anda, menyediakan pola penerapan, dan banyak lagi. Misalnya, Kubernetes dapat dengan mudah mengelola penerapan canary untuk sistem Anda.

Kubernetes memberi Anda:
Penemuan layanan dan penyeimbangan beban
Kubernetes dapat mengekspos kontainer menggunakan nama DNS atau menggunakan alamat IP mereka sendiri. Jika lalu lintas ke sebuah kontainer tinggi, Kubernetes dapat menyeimbangkan muatan dan mendistribusikan lalu lintas jaringan sehingga penerapannya stabil.
Orkestrasi penyimpanan
Kubernetes memungkinkan Anda untuk secara otomatis memasang sistem penyimpanan pilihan Anda, seperti penyimpanan lokal, penyedia cloud publik, dan banyak lagi.
Peluncuran dan rollback otomatis
Anda dapat menggambarkan keadaan yang diinginkan untuk wadah yang digunakan menggunakan Kubernetes, dan itu dapat mengubah keadaan aktual ke keadaan yang diinginkan pada tingkat yang terkontrol. Misalnya, Anda dapat mengotomatiskan Kubernetes untuk membuat container baru untuk penerapan Anda, menghapus container yang ada, dan mengadopsi semua sumber dayanya ke container baru.
Pengepakan tempat sampah otomatis
Anda memberi Kubernetes sekumpulan node yang dapat digunakan untuk menjalankan tugas dalam container. Anda memberi tahu Kubernetes berapa banyak CPU dan memori (RAM) yang dibutuhkan setiap container. Kubernetes dapat memuat wadah ke node Anda untuk memanfaatkan sumber daya Anda sebaik mungkin.
Penyembuhan diri
Kubernet memulai ulang wadah yang gagal, menggantikan wadah, membunuh kontainer yang tidak menanggapi pemeriksaan kesehatan yang ditentukan pengguna Anda, dan tidak mengiklankannya kepada klien sampai siap untuk melayani.
Manajemen rahasia dan konfigurasi.

Apa yang bukan Kubernetes
Kubernetes bukanlah sistem PaaS (Platform as a Service) tradisional yang inklusif. Karena Kubernetes beroperasi pada level container dan bukan pada level hardware,
Kubernetes menyediakan beberapa fitur umum yang berlaku umum untuk penawaran PaaS, seperti penerapan, penskalaan, load balancing, dan 
memungkinkan pengguna mengintegrasikan solusi logging, pemantauan, dan peringatan mereka. Namun, Kubernetes tidak monolitik, dan solusi default ini bersifat opsional 
dan dapat dicolokkan. Kubernetes menyediakan blok bangunan untuk membangun platform pengembang, tetapi mempertahankan pilihan dan fleksibilitas pengguna di tempat yang penting.

Kubernetes:

Tidak membatasi jenis aplikasi yang didukung. Kubernetes bertujuan untuk mendukung beragam beban kerja yang sangat beragam, termasuk beban kerja tanpa kewarganegaraan, status negara, dan pemrosesan data. Jika sebuah aplikasi dapat berjalan di sebuah wadah, itu harus berjalan dengan baik di Kubernetes.
Tidak menerapkan kode sumber dan tidak membangun aplikasi Anda. Alur kerja Integrasi, Pengiriman, dan Penempatan (CI / CD) yang berkelanjutan ditentukan oleh budaya dan preferensi organisasi serta persyaratan teknis.
Tidak menyediakan layanan tingkat aplikasi, seperti middleware (misalnya, bus pesan), kerangka kerja pemrosesan data (misalnya, Spark), database (misalnya, MySQL), cache, atau sistem penyimpanan cluster (misalnya, Ceph) sebagai layanan bawaan. Komponen tersebut dapat berjalan di Kubernetes, dan / atau dapat diakses oleh aplikasi yang berjalan di Kubernetes melalui mekanisme portabel, seperti Open Service Broker.
Tidak menentukan solusi logging, pemantauan, atau peringatan. Ini memberikan beberapa integrasi sebagai bukti konsep, dan mekanisme untuk mengumpulkan dan mengekspor metrik.
Tidak menyediakan atau mengamanatkan bahasa / sistem konfigurasi (misalnya, Jsonnet). Ini memberikan API deklaratif yang dapat ditargetkan oleh bentuk spesifikasi deklaratif yang sewenang-wenang.
Tidak menyediakan atau mengadopsi sistem konfigurasi, pemeliharaan, manajemen, atau pemulihan otomatis mesin yang komprehensif.
Selain itu, Kubernetes bukan sekadar sistem orkestrasi. Faktanya, ini menghilangkan kebutuhan akan orkestrasi. Definisi teknis orkestrasi adalah pelaksanaan alur kerja yang ditentukan: pertama lakukan A, lalu B, lalu C. Sebaliknya, Kubernetes terdiri dari sekumpulan proses kontrol yang dapat disusun dan independen yang secara terus menerus mendorong status saat ini menuju kondisi yang diinginkan yang disediakan. Tidak masalah bagaimana Anda mendapatkan dari A ke C. Kontrol terpusat juga tidak diperlukan. Ini menghasilkan sistem yang lebih mudah digunakan dan lebih bertenaga, kuat, tangguh, dan dapat dikembangkan.

