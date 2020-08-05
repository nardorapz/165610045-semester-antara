1. Basis data cloud adalah basis data yang biasanya berjalan pada platform komputasi awan, dan akses ke basis data disediakan sebagai layanan.

Layanan basis data menjaga skalabilitas dan ketersediaan tinggi basis data. Layanan basis data membuat tumpukan perangkat lunak yang mendasarinya transparan 
bagi pengguna
Gambar mesin virtual
Platform cloud memungkinkan pengguna untuk membeli mesin virtual untuk waktu yang terbatas, dan seseorang dapat menjalankan basis data pada mesin virtual tersebut. Pengguna dapat mengunggah gambar mesin mereka sendiri dengan database yang diinstal di atasnya, atau menggunakan gambar mesin yang sudah jadi yang sudah termasuk instalasi optimalisasi database.
Database-as-a-service (DBaaS)
Dengan database sebagai model layanan, pemilik aplikasi tidak harus menginstal dan memelihara sendiri database tersebut. Sebagai gantinya, penyedia layanan basis data bertanggung jawab untuk menginstal dan memelihara basis data, dan pemilik aplikasi dikenai biaya sesuai dengan penggunaan layanan tersebut. Ini adalah jenis Saas - Perangkat Lunak sebagai Layanan.
Arsitektur dan karakteristik umum
Sebagian besar layanan database menawarkan konsol berbasis web, yang dapat digunakan pengguna akhir untuk menyediakan dan mengkonfigurasi instance database.
Layanan database terdiri dari komponen database-manager, yang mengontrol instance database yang mendasarinya menggunakan API layanan. API layanan terpapar ke pengguna akhir, dan memungkinkan pengguna untuk melakukan operasi pemeliharaan dan penskalaan pada instance basis data mereka.
Perangkat lunak stack-stack yang mendasarinya biasanya mencakup sistem operasi, database, dan perangkat lunak pihak ketiga yang digunakan untuk mengelola database. Penyedia layanan bertanggung jawab untuk menginstal, menambal, dan memperbarui tumpukan perangkat lunak yang mendasarinya dan memastikan kesehatan dan kinerja keseluruhan basis data.
Fitur skalabilitas berbeda antara vendor - beberapa menawarkan penskalaan otomatis, yang lain memungkinkan pengguna untuk meningkatkan menggunakan API, tetapi tidak skala secara otomatis.
Biasanya ada komitmen untuk tingkat ketersediaan tinggi tertentu (mis. 99,9% atau 99,99%). Ini dicapai dengan mereplikasi data dan gagal contoh ke contoh database lain.
Model data
Desain dan pengembangan sistem tipikal menggunakan manajemen data dan database relasional sebagai blok bangunan utama mereka. Kueri lanjutan yang diungkapkan dalam SQL berfungsi baik dengan hubungan ketat yang dibebankan pada informasi oleh basis data relasional. Namun, teknologi basis data relasional pada awalnya tidak dirancang atau dikembangkan untuk digunakan pada sistem terdistribusi. Masalah ini telah diatasi dengan penambahan peningkatan pengelompokan ke database relasional, meskipun beberapa tugas dasar membutuhkan protokol yang kompleks dan mahal, seperti dengan sinkronisasi data. [1]

Database relasional modern menunjukkan kinerja yang buruk pada sistem intensif data, oleh karena itu, gagasan NoSQL telah digunakan dalam sistem manajemen basis data untuk sistem berbasis cloud. [2] Di dalam penyimpanan yang diterapkan NoSQL, tidak ada persyaratan untuk skema tabel tetap, dan penggunaan operasi gabungan dihindari. "Basis data NoSQL telah terbukti memberikan skalabilitas horizontal yang efisien, kinerja yang baik, dan kemudahan perakitan ke dalam aplikasi cloud." [4]

Penting juga untuk membedakan antara basis data cloud yang bersifat relasional dan bukan non-relasional atau NoSQL: [5]

Database SQL
adalah salah satu jenis database yang dapat berjalan di cloud, baik di mesin virtual atau sebagai layanan, tergantung pada vendor. Sementara database SQL mudah skalabel secara vertikal, skalabilitas horizontal menjadi tantangan, bahwa layanan basis data cloud berbasis SQL sudah mulai diatasi.[perlu kutip untuk memverifikasi]
Database NoSQL
adalah tipe lain dari basis data yang dapat berjalan di cloud. Basis data NoSQL dibangun untuk melayani banyak baca / tulis dan dapat meningkatkan dan menurunkan dengan mudah, [7] dan karenanya mereka lebih cocok untuk berjalan di cloud. Namun, sebagian besar aplikasi kontemporer dibangun di sekitar model data SQL, sehingga bekerja dengan basis data NoSQL seringkali membutuhkan penulisan ulang kode aplikasi yang lengkap. [8]
Beberapa basis data SQL telah mengembangkan kemampuan NoSQL termasuk JSON, JSON biner (mis. BSON atau varian serupa), dan tipe data penyimpanan nilai kunci.
Database multi-model dengan kemampuan relasional dan non-relasional menyediakan antarmuka SQL standar untuk pengguna dan aplikasi dan dengan demikian memfasilitasi penggunaan database tersebut untuk aplikasi kontemporer yang dibangun di sekitar model data SQL. Basis data multi-model asli mendukung beberapa model data dengan satu inti dan bahasa permintaan terpadu untuk mengakses semua model data.

2. 
Dalam komputasi, data sebagai layanan, atau DaaS, diaktifkan oleh perangkat lunak sebagai layanan (SaaS). [1] Seperti semua teknologi "sebagai layanan" (aaS), DaaS membangun konsep bahwa produk datanya dapat diberikan kepada pengguna berdasarkan permintaan, [2] terlepas dari pemisahan geografis atau organisasi antara penyedia dan konsumen. Arsitektur berorientasi layanan (SOA), dan meluasnya penggunaan API, telah menjadikan platform tempat data berada sebagai tidak relevan. [3]

DaaS dimulai terutama dalam mashup Web dan, sejak 2015, telah semakin dipekerjakan baik secara komersial, maupun di dalam organisasi seperti PBB. [4]

Secara tradisional, sebagian besar organisasi telah menggunakan data yang disimpan dalam repositori mandiri, yang untuknya perangkat lunak dikembangkan secara khusus untuk mengakses dan menyajikan data dalam bentuk yang dapat dibaca manusia. Salah satu hasil dari paradigma ini adalah penggabungan data dan perangkat lunak yang diperlukan untuk menafsirkannya menjadi satu paket, dijual sebagai produk konsumen. Karena jumlah perangkat lunak yang dibundel dengan paket data berkembang biak, dan diperlukan interaksi antara satu sama lain, lapisan antarmuka lain diperlukan. Antarmuka ini, secara kolektif dikenal sebagai integrasi aplikasi perusahaan (EAI), sering cenderung mendorong vendor lock-in, karena umumnya mudah untuk mengintegrasikan aplikasi yang dibangun di atas teknologi pondasi yang sama. [5]

Hasil dari paket perangkat lunak / data konsumen gabungan dan middleware EAI yang dibutuhkan telah meningkatkan jumlah perangkat lunak untuk dikelola dan dikelola organisasi, hanya untuk penggunaan data tertentu. Selain biaya perawatan rutin, sejumlah pembaruan perangkat lunak yang mengalir diperlukan karena format data berubah. Keberadaan situasi ini berkontribusi pada daya tarik DaaS kepada konsumen data, karena memungkinkan pemisahan biaya data dan penggunaan data dari biaya lingkungan atau platform perangkat lunak tertentu. Sensing as a Service [6] [7] (S2aaS) adalah model bisnis yang mengintegrasikan data Internet of Things untuk membuat pasar perdagangan data.

Vendor, seperti MuleSoft, Oracle Cloud dan Microsoft Azure, melakukan pengembangan DaaS yang lebih cepat menghitung volume data yang besar; mengintegrasikan dan menganalisis data itu; dan menerbitkannya secara real-time, menggunakan API layanan Web yang mematuhi batasan arsitektur REST-nya (RESTful API).


Model penetapan harga
Ada ratusan vendor DaaS di Web, dan model penetapan harga yang digunakan untuk menagih pelanggan mereka terutama ke dalam dua kategori utama. [8]

Model berbasis volume yang memiliki dua pendekatan:
penetapan harga berbasis kuantitas adalah model paling sederhana untuk diterapkan. Vendor membebankan biaya kepada pelanggan berdasarkan jumlah data yang ingin mereka gunakan. Langganan untuk jumlah data yang tidak terbatas disebut sebagai "pendekatan selang api".
layanan bayar per panggilan, di mana vendor mengenakan biaya untuk setiap panggilan dari pelanggan ke API.
model berbasis tipe data disusun oleh vendor untuk menagih pengguna berdasarkan pada tipe atau atribut data yang mereka butuhkan. Data geografis, keuangan, dan historis yang diperlukan untuk bisnis pelanggan adalah contoh tipe data yang menjadi dasar penetapan harga. Beberapa vendor, seperti Microsoft Azure, menyimpan data dalam tiga jenis berbeda - gumpalan, antrian, dan tabel.
