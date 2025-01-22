**Nama : Nadia Recilia Dahmi**

**NIM  : 20220801041**
___

**Studi Kasus**
--

Buatlah Topologi dan Konfigurasi ruang lab praktikum Universitas Esa Unggul untuk masing masing kampus (CR, KHI, KJ) bagaimana agar mereka bisa terhubung dan terkoneksi dengan memanfaatkan routing statik, routing dinamik (BGP, RIP, OSPF), Kumpulkan semua ke github masing-masing.


**Deskripsi**
--
Sistem jaringan menghubungkan tiga kampus (KJ, KHI, CR) menggunakan layanan ISP dengan IP Publik dan VPN Tunnel. ISP menyediakan konektivitas internet, sedangkan VPN Tunnel menjamin keamanan data melalui jalur terenkripsi. Konfigurasi jaringan meliputi pengaturan router dasar, NAT, DHCP, dan Routing statis untuk efisiensi komunikasi antar-lokasi. 

**Analisis**
--
Tiga kampus membutuhkan konektivitas yang aman dan stabil melalui jaringan publik. ISP berperan menyediakan IP Publik yang menjadi jalur utama koneksi antar-kampus. VPN Tunnel digunakan untuk menjamin komunikasi aman melalui jalur terenksripsi, melindungi data dari penyadapan atau manipulasi. Router di setiap lokasi menangani konfigurasi dasar, NAT, Routing Statis, dan pembuatan Tunnel untuk mengelola lalu lintas data. Keamanan data menjadi prioritas, sementara efisiensi tercapai melalui routing sttais yang memastikan pengiriman data mengikuti jalur optimal tanpa konfigurasi tambahan pada perangkat lain. 

**Implementasi ISP dan VPN Tunnel untuk Koneksi Jaringan Tiga Kampus** 
--
1. Melakukan identifikasi perangkat yang dibutuhkan di setiap kampus (KJ,KHI,CR) serta pengaturan IP publik yang diberikan oleh ISP untuk masing-masing lokasi. Setelah perangkat seperti router,langkah berikutnya adalah memastikan jaringan lokal di setiap kampus siap digunakan. Tahap ini juga mencakup perencanaan untuk pengaturan koneksi antar-lokasi yang memanfaatkan jaringan ISP.
2. Pengaturan IP lokal dan IP publik pada setiap router yang terpasang di kampus-kampus tersebut. IP lokal digunakan untuk perangkat yang terhubung dalam jaringan internal, sementara IP publik disediakan oleh ISP untuk komunikasi antar-lokasi melalui internet. Setiap router dikonfigurasi dengan DHCP server untuk mendistribusikan IP lokal secara otomatis ke perangkat di jaringan kampus. Selain itu, fitur Network Address Translation (NAT) diaktifkan pada setiap router agar perangkat di jaringan lokal dapat mengakses internet menggunakan IP publik secara aman dan efisien.
3. Konfigurasi tunnel antara router yang berada di lokasi KJ, CR, dan KHI. Setiap router akan membangun tunnel ke IP publik router di lokasi lainnya untuk memastikan koneksi antar-kampus terjalin dengan aman. Tunnel ini akan mengenkripsi data yang dikirimkan antar lokasi, memastikan data terlindungi selama perjalanan melalui jaringan publik. Setelah tunnel terkonfigurasi, dilakukan pengujian untuk memverifikasi koneksi dan memastikan bahwa jalur komunikasi antar-kampus aman dan stabil.
4. Konfigurasi routing statis di setiap router untuk mengarahkan lalu lintas data menuju tujuan yang benar. Rute ini memastikan paket data yang dikirim dari satu kampus menuju kampus lainnya melewati tunnel yang sudah dibuat sebelumnya. Konfigurasi routing ini memungkinkan komunikasi langsung antar-kampus tanpa memerlukan pengaturan tambahan pada perangkat lain dalam jaringan lokal. Setelah rute statis ditetapkan, dilakukan pengujian untuk memastikan data dapat mengalir ke tujuan dengan lancar dan tanpa masalah.

**Kesimpulan**
--
Alur koneksi melibatkan penyediaan IP publik oleh ISP sebagai jalur utama komunikasi antar-lokasi. Router bertugas membangun jalur VPN Tunnel untuk memastikan keamanan data. Routing statis digunakan untuk mengatur arah lalu lintas data secara efisien, memungkinkan komunikasi langsung antar-kampus melalui jaringan internet yang aman dan stabil.

