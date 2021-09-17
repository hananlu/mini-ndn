# mini-ndn
Installasi Mini-ndn yang akan dilakukan dengan menggunakan source

1. Untuk menginstall mini-ndn langkah pertama menginstall dependency yang dibutuhkan.
```
sudo apt install libpcap-dev libsystemd-dev g++ pkg-config python3-minimal libboost-all-dev libssl-dev libsqlite3-dev doxygen graphviz python3-pip sphinx sphinxcontrib-doxylink
```
2. Selanjutnya menginsatall dependecy dari NDN yaitu NFD, NLSR, serta ndn-tools

 - Instalasi NFD
 
   Download NFD dan ndn-cxx
   ```
   git clone https://github.com/named-data/ndn-cxx.git
   git clone https://github.com/named-data/NFD.git
   ```
   Setelah berhasil didownload masuk ke setiap folder dan lakukan build
   ```
   ./waf configure
   ./waf
   sudo ./waf install
   ```
 - Instalasi NLSR

   Download PSnyc dan NLSR
   ```
   git clone https://github.com/named-data/PSync
   git clone https://github.com/named-data/NLSR
   ```
   Lakukan build ke setiap folder tersebut
   ```
   ./waf configure
   ./waf
   sudo ./waf install
   ```
  
