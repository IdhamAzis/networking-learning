# Belajar Jaringan - Dokumentasi
    Tujuan : mempelajari network agar menjadi dasar/pondasi yang kuat untuk belajar cyber security ke depannya.

# 1	Macam - macam jaringan
    Macam - macam jaringan :
    1. LAN (Local Area Network), yang dimana LAN ini memiliki jangkauan kecil dibanding ke 2 jaringan lainnya,
    contohnya : pada ruangan gedung, ruangan lab kampus, namun LAN memiliki kecepatan antara 100 Mbps hinggan mencapai 10Gbps.

    2. MAN (Metropolitan Area Network), MAN memiliki jangkauan yang cukup lumayan luas,
    contohnya : jaringan kampus antar gedung dengan menghubungkan beberapa LAN.
    
    3. WAN (Wide Area Network), WAN ini memiliki jangkauan terluas dari kedua jaringan sebelumnya, ia menghubungkan MAN dan LAN antar wilayah negara, dan memiliki koneksi yang kompleks, namun membutuhkan biaya yang lebih mahal.

# 2	OSI Model (Open System Interconnect)
    Tujuan dari OSI model yaitu agar sistem yang berbeda - beda dapat berkomunikasi
    OSI model ini juga berguna untuk memahami bagaimana komunikasi antar sistem bekerja dan merancang atau mengimplementasikan software dan hardware untuk komunikasi antar sistem.

    OSI model memiliki 7 layer :
    7 : Application
    6 : Presentation
    5 : Session
    4 : Transport
    3 : Network
    2 : Data Link
    1 : Physical

    layer 7 - 3 merupakan bagian software
    layer 2 dan 1 merupakan bagian Hardware

    Tujuan dari layers : untuk memecahkan persoalan/masalah menjadi bagian - bagian yang lebih mudah

    Tugas - tugas dari layer :
    a. Layer 1 Physical memiliki tugas untuk mengirimkan bit secara fisik melalui kabel, sinyal listrik, radio, fiber, dll. Dan unit komunikasi pada layer ini adalah
       bit.
    b. Layer 2 Data Link memiliki tugas untuk mengatur akses ke media fisik, error detection, framing, dan komunikasi antar perangkat dalam 1 jaringan (LAN). Dan unit
       komunikasi pada layer ini adalah frame.
    c. Layer 3 Network memiliki tugas untuk melakukan routing antar jaringan, menentukan jalur terbaik, dan menambahkan alamat IP (source dan destination) dan unit
       komunikasi pada layer ini adalah packet.
    d. Layer 4 Transport memiliki tugas untuk Mengatur komunikasi end-to-end (process to process), sequencing, error control, flow control (TCP/UDP) dan unit komunikasi
       pada layer ini adalah segment.
    e. Layer 5 Session memiliki tugas untuk Mengatur sesi komunikasi: membuka, memelihara, dan menutup koneksi antara perangkat. Dan unit komunikasi
       pada layer ini adalah data.
    f. Layer 6 Presentation memiliki tugas untuk Mengatur format data (enkripsi, dekripsi, kompresi, encoding/decoding), memastikan data dapat dipahami aplikasi dan
       unit komunikasi pada layer ini adalah data.
    g. Layer 7 Application memiliki tugas sebagai Berinteraksi langsung dengan pengguna dan aplikasi (HTTP, FTP, DNS, SSH). dan
       unit komunikasi pada layer ini adalah data.

    Pada transport layer (layer ke 4) Flow control adalah mengatur laju kecepatan pengirim agar dapat diterima oleh penerima dengan baik.

# 3 TCP IP (Transmission Control Protocol)
    Frame adalah kumpulan bit.
    Link : jaringan komputer yang menghubungkan perangkat agar bisa berkomunikasi.

    Model TCP/IP terdiri dari 4 - 5 layer :
    a. Network Acces memiliki fungsi untuk menangani detail fisik dan koneksi ke media jaringan (kabel, Wi-Fi), seperti pengalamatan fisik (MAC Address). Unit
       Data (PDU) nya yaitu frame, contoh protokol ethernet, wi-fi.
    b. Network memiliki fungsi untuk bertanggung jawab untuk pengalamatan logis (IP Address) dan perutean (routing) paket data antar jaringan, Unit Data (PDU) nya yaitu 
       packet (paket), contoh protokol IP, ICMP, ARP.
    c. Transport memiliki fungsi mengatur komunikasi end-to-end (ujung ke ujung), mengontrol aliran data, dan penanganan kesalahan, Unit Data (PDU) nya yaitu segmen
       (segmen), contoh protokol TCP, UDP.
    d. Application memilikl fungsi untuk menyediakan antarmuka untuk aplikasi pengguna, menangani detail presentasi dan sesi, Unit Data (PDU) nya yaitu Data/Pesan,
       contoh protokol HTTP, HTTPS, FTP, SMTP, POP3, DNS.

# 4 Perbedaan antara OSI model dengan TCP IP
    **OSI Model**                                 
    - Memiliki 7 layer :
      OSI model memiliki 7 layer :
      7 : Application
      6 : Presentation
      5 : Session
      4 : Transport
      3 : Network
      2 : Data Link
      1 : Physical  
    - Berfungsi untuk model teoritis untuk standarisasi komunikasi
    - Digunakan untuk konsep dan troubleshooting
    - Lebih detail, kompleks

    
    **TCP/IP Model**                                           
    - Memiliki 4 kadang 5 layer
      TCP IP memiliki 4 - 5 layer :
      4 : Application (gabungan antara Session, Presentation dan Application)
      3 : Transport
      2 : Internet
      1 : Network Acces (gabungan antara Physical dan Data Link) 
    - Berfungsi untuk model yang benar-benar digunakan di dunia nyata (Internet)
    - Digunakan untuk operasi internet dan networking modern
    - Lebih sederhana, praktis

    Jadi dapat di ilustrasikan bahwa :
    OSI model   : Blueprint detail rumah sebelum dibangun
    TCP IP      : Rumah yang benar-benar dibangun dan dipakai orang

    Dan intinya 
    OSI         : teori dan konsep struktur komunikasi
    TCP/IP      : penerapan nyata pada jaringan modern dan internet

# 5 LATIHAN SOAL
    1. Sebutkan 3 contoh protokol yang bekerja di Transport Layer                       
    = TCP dan UDP
    
    2. Perbedaan utama antara TCP dan UDP dalam 1 kalimat.                              
    = CP lebih handal (reliable) karena ada mekanisme acknowledgment, sequence number, retransmission. UDP tidak memiliki mekanisme tersebut.
    
    3. Pada OSI model, perangkat router bekerja di layer berapa?                        
    = Transport layer
    
    4. Pada TCP/IP model, layer manakah yang berhubungan dengan Ethernet dan Wi-Fi?     
    = Layer 5 Session, karena layer ini yang mengatur enkripsi/dekripsi sesi komunikasi (walau kadang enkripsi juga dikatakan bagian dari Presentation).
    
    5. Apa nama unit data di OSI Layer 2?                                               
    = Physical layer (Layer 1) tidak ada data unit, biasanya disebut bits.

    6. Model OSI memiliki berapa layer dan apa tujuan utama dari model tersebut?
    = Model OSI memiliki 7 layer

    7. Pada OSI model, layer manakah yang bertanggung jawab terhadap enkripsi, kompresi, dan format data?
    = Layer 6: Presentation

    8. Protokol TCP dan UDP bekerja pada layer berapa di OSI model?
    = Layer 4: Transport Layer

    9. Apa nama unit data pada layer Transport OSI untuk TCP dan UDP?
    = Untuk TCP → Segment
      Untuk UDP → Datagram

    10. Layer mana yang berfungsi untuk pengalamatan IP dan routing paket ke jaringan tujuan?
    = Layer 3: Network Layer

    11. Dalam TCP/IP model, layer apakah yang menggabungkan fungsi Session, Presentation, dan Application dari OSI?
    = Application Layer

    12. Jelaskan perbedaan fungsi antara Network Layer pada OSI dan Internet Layer pada TCP/IP — apakah sama atau ada perbedaan?
    = keduanya hampir sama, yaitu menangani IP addressing, routing, dan forwarding paket.
      Bedanya, Internet Layer TCP/IP lebih sederhana, sedangkan OSI Network Layer lebih konseptual dan lengkap sebagai model referensi.


    13. Protokol seperti HTTP, DNS, dan FTP berada pada layer mana dalam TCP/IP model?
    = Application Layer

    14. Jelaskan peran Physical Layer pada OSI model dengan contoh nyata pada dunia jaringan.
    = Physical Layer bertanggung jawab untuk mengirimkan bit (0 dan 1) melalui media fisik jaringan.
      Contoh nyata: kabel LAN (RJ45), fiber optic, Wi-Fi signal, hub, connector RJ45, voltase sinyal.

    15. Pada TCP/IP model, layer mana yang bertanggung jawab pada komunikasi end-to-end, termasuk flow control, error control, dan reliability?
    = Transport Layer