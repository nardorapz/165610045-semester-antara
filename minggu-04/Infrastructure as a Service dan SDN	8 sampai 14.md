
1.nfrastructure as a service (IaaS) adalah

yanan online yang menyediakan API tingkat tinggi yang digunakan untuk melakukan dereferensi berbagai detail tingkat rendah dari infrastruktur jaringan yang mendasarinya seperti sumber daya komputasi fisik, lokasi, partisi data, penskalaan, keamanan, cadangan dll. Hypervisor, seperti Xen, Oracle VirtualBox, Oracle VM, KVM, VMware ESX / ESXi, atau Hyper-V, LXD, menjalankan mesin virtual sebagai tamu. Kelompok hypervisor dalam sistem operasional cloud dapat mendukung sejumlah besar mesin virtual dan kemampuan untuk meningkatkan skala layanan sesuai dengan kebutuhan pelanggan yang beragam.
Biasanya IaaS melibatkan penggunaan teknologi orkestrasi cloud seperti Open Stack, Apache Cloudstack atau OpenNebula. Ini mengelola pembuatan mesin virtual dan memutuskan hypervisor (mis. Host fisik) untuk memulainya, memungkinkan fitur migrasi VM antara host, mengalokasikan volume penyimpanan dan melampirkannya ke VM, informasi penggunaan untuk penagihan dan banyak lagi.

Alternatif untuk hypervisor adalah wadah Linux, yang berjalan di partisi terisolasi dari satu kernel Linux yang berjalan langsung pada perangkat keras fisik. Linux cgroups dan namespaces adalah teknologi kernel Linux yang digunakan untuk mengisolasi, mengamankan dan mengelola wadah. Containerisation menawarkan kinerja yang lebih tinggi daripada virtualisasi, karena tidak ada overhead hypervisor. Selain itu, skala wadah kapasitas otomatis secara dinamis dengan beban komputasi, yang menghilangkan masalah penyediaan berlebihan dan memungkinkan penagihan berbasis penggunaan.
aaS cloud sering menawarkan sumber daya tambahan seperti pustaka citra disk mesin-mesin virtual, penyimpanan blok mentah, penyimpanan file atau objek, firewall, penyeimbang beban, alamat IP, jaringan area lokal virtual (VLAN), dan bundel perangkat lunak

Definisi NIST tentang komputasi awan mendefinisikan infrastruktur sebagai layanan sebagai: 

Kemampuan yang diberikan kepada konsumen adalah untuk menyediakan pemrosesan, penyimpanan, jaringan, dan sumber daya komputasi mendasar lainnya di mana konsumen dapat menggunakan dan menjalankan perangkat lunak sewenang-wenang, yang dapat mencakup sistem operasi dan aplikasi. Konsumen tidak mengelola atau mengendalikan infrastruktur cloud yang mendasarinya tetapi memiliki kendali atas sistem operasi, penyimpanan, dan aplikasi yang digunakan; dan kemungkinan kontrol terbatas untuk komponen jaringan tertentu (mis., host firewall).

Menurut Internet Engineering Task Force (IETF), model layanan cloud yang paling dasar adalah penyedia yang menawarkan infrastruktur TI - mesin virtual dan sumber daya lainnya - sebagai layanan kepada pelanggan.

Penyedia IaaS-cloud memasok sumber daya ini sesuai permintaan dari kumpulan besar peralatan mereka yang dipasang di pusat data. Untuk konektivitas area luas, pelanggan dapat menggunakan Internet atau cloud operator (jaringan pribadi virtual khusus). Untuk menyebarkan aplikasi mereka, pengguna cloud menginstal gambar sistem operasi dan perangkat lunak aplikasi mereka pada infrastruktur cloud. [4] [sumber tidak dapat diandalkan?] Dalam model ini, pengguna cloud menambal dan memelihara sistem operasi dan perangkat lunak aplikasi. Penyedia cloud biasanya menagih layanan IaaS berdasarkan komputasi utilitas: biaya mencerminkan jumlah sumber daya yang dialokasikan dan dikonsumsi.

2.Infrastruktur-sebagai-a-Layanan, adalah 

bentuk komputasi awan yang memberikan sumber daya komputasi, jaringan, dan penyimpanan yang mendasar kepada konsumen sesuai permintaan, melalui internet, dan dengan pembayaran dasar you-go. IaaS memungkinkan pengguna akhir untuk skala dan menyusutkan sumber daya sesuai kebutuhan, mengurangi kebutuhan untuk pengeluaran modal yang tinggi di muka atau infrastruktur “milik” yang tidak perlu, terutama dalam hal beban kerja “runcing”. Berbeda dengan PaaS dan SaaS (bahkan model komputasi yang lebih baru seperti container dan serverless), IaaS memberikan kontrol sumber daya tingkat terendah di cloud.

IaaS muncul sebagai model komputasi yang populer di awal 2010-an, dan sejak saat itu, iaaS menjadi model abstraksi standar untuk banyak jenis beban kerja. Namun, dengan munculnya teknologi baru, seperti wadah dan serverless, dan munculnya pola aplikasi layanan mikro yang terkait, IaaS tetap mendasar tetapi berada di bidang yang lebih ramai dari sebelumnya.
Pusat data fisik: Penyedia IaaS akan mengelola pusat data besar, biasanya di seluruh dunia, yang berisi mesin fisik yang diperlukan untuk memberi daya pada berbagai lapisan abstraksi di atasnya dan yang disediakan untuk pengguna akhir melalui web. Pada sebagian besar model IaaS, pengguna akhir tidak berinteraksi langsung dengan infrastruktur fisik, tetapi disediakan sebagai layanan untuk mereka.

Komputasi: IaaS biasanya dipahami sebagai sumber daya komputasi tervirtualisasi, jadi untuk keperluan artikel ini, kami akan mendefinisikan komputasi IaaS sebagai mesin virtual. Penyedia mengelola hypervisor dan pengguna akhir kemudian dapat secara program menyediakan "instance" virtual dengan jumlah komputasi dan memori yang diinginkan (dan terkadang penyimpanan). Sebagian besar penyedia menawarkan CPU dan GPU untuk berbagai jenis beban kerja. Cloud Compute juga biasanya dipasangkan dengan layanan pendukung seperti penskalaan otomatis dan penyeimbangan beban yang memberikan skala dan karakteristik kinerja yang menjadikan cloud diinginkan.

3.IaaS dengan cepat naik turun sesuai permintaan, 

membiarkan Anda membayar hanya untuk apa yang Anda gunakan. Ini membantu Anda menghindari biaya dan kerumitan membeli dan mengelola server fisik Anda sendiri dan infrastruktur pusat data lainnya. Setiap sumber daya ditawarkan sebagai komponen layanan terpisah, dan Anda hanya perlu menyewa yang khusus selama Anda membutuhkannya. Penyedia layanan komputasi awan, seperti Azure, mengelola infrastruktur, saat Anda membeli, menginstal, mengonfigurasi, dan mengelola perangkat lunak Anda sendiri — sistem operasi, middleware, dan aplikasi.

Penyimpanan, cadangan, dan pemulihan. Organisasi menghindari pengeluaran modal untuk penyimpanan dan kompleksitas manajemen penyimpanan, yang biasanya membutuhkan staf ahli untuk mengelola data dan memenuhi persyaratan hukum dan kepatuhan. IaaS berguna untuk menangani permintaan yang tidak terduga dan terus meningkatkan kebutuhan penyimpanan. Ini juga dapat menyederhanakan perencanaan dan pengelolaan sistem cadangan dan pemulihan.

Keuntungan IaaS
Menghilangkan biaya modal dan mengurangi biaya berkelanjutan. IaaS mengesampingkan biaya dimuka untuk mendirikan dan mengelola pusat data di lokasi, menjadikannya pilihan yang ekonomis untuk para pemula dan bisnis yang menguji ide-ide baru.

Meningkatkan kesinambungan bisnis dan pemulihan bencana. Mencapai ketersediaan tinggi, kesinambungan bisnis, dan pemulihan bencana adalah mahal, karena membutuhkan sejumlah besar teknologi dan staf. Tetapi dengan perjanjian tingkat layanan yang tepat (SLA) di tempat, IaaS dapat mengurangi biaya ini dan mengakses aplikasi dan data seperti biasa selama bencana atau pemadaman.

Berinovasi dengan cepat. Segera setelah Anda memutuskan untuk meluncurkan produk atau inisiatif baru, infrastruktur komputasi yang diperlukan dapat siap dalam hitungan menit atau jam, daripada beberapa hari atau minggu — dan kadang-kadang berbulan-bulan — mungkin diperlukan untuk mengatur secara internal.

Tanggapi kondisi bisnis dengan lebih cepat. IaaS memungkinkan Anda untuk dengan cepat meningkatkan sumber daya untuk mengakomodasi lonjakan permintaan untuk aplikasi Anda — selama liburan, misalnya — kemudian menurunkan sumber daya kembali ketika aktivitas berkurang untuk menghemat uang.

Fokus pada bisnis inti Anda. IaaS membebaskan tim Anda untuk fokus pada bisnis inti organisasi Anda dan bukan pada infrastruktur TI.

Tingkatkan stabilitas, keandalan, dan dukungan. Dengan IaaS tidak perlu memelihara dan meningkatkan perangkat lunak dan perangkat keras atau memecahkan masalah peralatan. Dengan perjanjian yang sesuai, penyedia layanan memastikan bahwa infrastruktur Anda dapat diandalkan dan memenuhi SLA.

Keamanan yang lebih baik. Dengan perjanjian layanan yang sesuai, penyedia layanan cloud dapat memberikan keamanan untuk aplikasi dan data Anda yang mungkin lebih baik daripada yang bisa Anda dapatkan di rumah.

Mendapat aplikasi baru untuk pengguna lebih cepat. Karena Anda tidak perlu terlebih dahulu menyiapkan infrastruktur sebelum Anda dapat mengembangkan dan mengirimkan aplikasi, Anda dapat membuatnya lebih cepat dengan pengguna dengan IaaS.

4.Teknologi network-defined networking (SDN) adalah 

pendekatan manajemen jaringan yang memungkinkan konfigurasi jaringan yang dinamis dan efisien secara program untuk meningkatkan kinerja dan pemantauan jaringan, menjadikannya lebih seperti komputasi awan daripada manajemen jaringan tradisional. [1] SDN dimaksudkan untuk mengatasi kenyataan bahwa arsitektur statis jaringan tradisional terdesentralisasi dan kompleks sedangkan jaringan saat ini membutuhkan lebih banyak fleksibilitas dan pemecahan masalah yang mudah. SDN berupaya memusatkan kecerdasan jaringan dalam satu komponen jaringan dengan melepaskan proses penerusan paket jaringan (bidang data) dari proses perutean (bidang kendali). Bidang kontrol terdiri dari satu atau lebih pengontrol, yang dianggap sebagai otak dari jaringan SDN di mana seluruh kecerdasan dimasukkan. Namun, sentralisasi cerdas memiliki kelemahannya sendiri dalam hal keamanan, [1] skalabilitas dan elastisitas [1] dan ini adalah masalah utama SDN.

SDN umumnya dikaitkan dengan protokol OpenFlow (untuk komunikasi jarak jauh dengan elemen bidang jaringan untuk tujuan menentukan jalur paket jaringan di seluruh switch jaringan) sejak kemunculannya yang terakhir pada 2011. Namun, sejak 2012 [2] [3] OpenFlow bagi banyak perusahaan bukan lagi solusi eksklusif, mereka menambahkan teknik kepemilikan. Ini termasuk Lingkungan Jaringan Terbuka Cisco Systems dan platform virtualisasi jaringan Nicira.

SD-WAN menerapkan teknologi serupa ke jaringan area luas (WAN). [4]

Teknologi SDN saat ini tersedia untuk aplikasi kontrol industri yang memerlukan failover yang sangat cepat. Satu perusahaan menawarkan 100x Faster Failover untuk proses-proses Misi-kritis (gagal dalam waktu kurang dari 100 μs, dibandingkan dengan 10 ms untuk jaringan tradisional) bersama dengan penghapusan Kerentanan Cyber tertentu yang terkait dengan sakelar manajemen jaringan tradisional.
