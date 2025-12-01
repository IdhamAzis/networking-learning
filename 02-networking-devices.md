# Belajar Networking Devices - Dokumentasi
    Tujuan : untuk memahami dan mendokumentasikan peran dan fungsi.

# 1 Apa si networking devices itu??
    Networking devices adaladh perangkat yang digunakan untuk membangun, menghubungkan, mengatur, dan mengamankan jaringan komputer sehingga perangkat bisa saling berkommunikasi dan bertukar data. 

    Sebelum itu, apa si perbedaan dari modem dengan router?
    Perbedaan utama modem dan router adalah fungsi: modem menghubungkan jaringan rumah ke internet dari penyedia layanan (ISP), sedangkan router membagikan koneksi internet tersebut ke berbagai perangkat di rumah melalui kabel (LAN) atau nirkabel (Wi-Fi)

# 2 Jenis dan Fungsi Dasar Perangkat
    - Switch
        Switch lebih canggih dibanding Hub karena switch dapat meneruskan data berdasarkan alamat perangkat keras. Dapat juga meningkatkan efisiensi dan keamanan pada jaringan.
        Terdapat pada Layer 2 OSI Layer

    - Router
        Router dapat memfilter dan meneruskan data menggunakan alamat logis seperti alamat IP. Router menyimpan informasi jaringan, bertindak sebagai firewall pemfilter paket, dan memainkan peran penting dalam mengendalikan dan mengoptimalkan lalu lintas jaringan.
        Terdapat pada Layer 3 OSI Layer

    - Hub
        Hub adalah konektivitas sederhana yang menghubungkan kabel - kabel, untuk membentuk suatu jaringan.
        Fungsi dari Hub yaitu sebagai pengulang data jarak jauh dan mentransmisikan ulang tanpa penyaringan.
        Terdapat pada Layer 1 OSI Layer

    - Bridges
        Bridge adalah perangkat jaringan yang menyaring dan meneruskan paket berdasarkan alamat fisik, menghubungkan berbagai segmen jaringan. Bridge mengelola aliran data antar segmen dan bermanfaat untuk membagi jaringan yang luas menjadi bagian-bagian yang lebih kecil.
        Terdapat pada Layer 2 OSI Layer

    - Acces Point
        Titik akses menghubungkan LAN nirkabel dan Ethernet, menciptakan LAN nirkabel. Titik akses ini mencakup pemancar, penerima, dan antena internal. Beberapa titik akses juga berfungsi sebagai sakelar, firewall, dan server DHCP.
        Terdapat pada Layer 2 OSI Layer

    - Modem
        Modem memungkinkan komputer mengirim atau menerima data melalui saluran telepon atau kabel. Modem mengubah sinyal digital menjadi analog selama transmisi dan sebaliknya selama penerimaan.
        Terdapat pada Layer 1 OSI Layer

    - Firewall
        Firewall (perangkat keras atau perangkat lunak) beroperasi pada berbagai lapisan Model OSI, melindungi jaringan dari akses tidak sah atau serangan berbahaya. Firewall menerapkan aturan untuk mengontrol aliran paket, memastikan keamanan jaringan melalui enkripsi, autentikasi, pencatatan, dan audit.
        Terdapat pada Layer 3 - 7 OSI Layer

    - Repeater  
        Berfungsi memperkuat atau memperluas jangkauan sinyal jaringan.
        Layer 1 OSI Layer

    - Load Balancer  
        Mengatur distribusi trafik ke beberapa server untuk menghindari overload.
        Layer 4–7 OSI Layer

    - Server
        Menyediakan layanan jaringan seperti DNS, DHCP, File Sharing, Web Service, dll.
        Layer 7 OSI Layer


# 3 Protokol yang Bekerja di Network Devices
    - DHCP, berfungsi untuk memberi IP otomatis yang dipakai oleh Router/Server
    - ARP (Address Resolution Protocol), berfungsi untuk mencari MAC address yang dipakai oleh Switch/Router
    - ICMP, berfungsi untuk ping/troubleshoot yang dipakai oleh semua device
    - DNS, berfungsi untuk resolusi domain yang dipakai oleh server/router
    - OSPF/BGP, berfungsi untuk merouting yang dipakai oleh router enterprise

# 4 Standar Keamanan Networking Devices
    - WPA3 (wifi security)
    - VLAN Segmentasi Jaringan
    - Access Control List (ACL)
    - IDS/IPS (Intrusion Prevention and Detection)

# 5 Alur Internet
    Internet
       ↓
     Modem
       ↓
Router → Firewall (opsional)
       ↓
     Switch
       ↓
 Device / Access Point

# 6 Kesimpulan
    

# 7 Next ??
    Setelah memahami networking devices, langkah berikutnya adalah belajar Subnetting, Routing, dan VLAN Configuration, lalu praktik menggunakan Cisco Packet Tracer / GNS3 / EVE-NG.