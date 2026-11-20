 CATATAN HARIAN CYBER SECURITY - MINGGU 1 HARI 2
Tanggal: Sabtu, 21 November 2026  
Topik: Arsitektur Jaringan Dasar (IP Address, MAC Address, Default Gateway, dan Packet)

 1. Konsep Dasar Jaringan
IP Address itu alamat perangkat dalam jaringan yang bisa berubah ketika perangkat berpindah jaringan. Sementara itu, MAC Address itu sendiri kode identitas pada kartu jaringan yang biasanya tetap dan digunakan untuk mengenali perangkat dalam komunikasi jaringan lokal.

Default Gateway berfungsi sebagai pintu keluar atau penghubung dari jaringan lokal menuju jaringan lain, seperti internet. Contohnya, ketika laptop ingin mengakses Google, laptop mengirimkan data melalui router sebagai Default Gateway agar data bisa diteruskan ke jaringan luar.

2. Identitas Jaringan Lokal (Hasil ipconfig /all)
- Adapter Aktif: Wireless LAN adapter Wi-Fi
- IPv4 Address (Private IP): 192.168.x.x (Preferred)
- Default Gateway: fe80::1%7 / 192.168.1.1
- Physical Address (MAC Address): 6C-94-xx-xx-xx-xx

 3. Pengujian Koneksi & Pelacakan Rute
A. Hasil Ping ke Default Gateway
- Perintah: `ping 192.168.1.1`
- Paket Hilang (Loss): Lost = 0 (0% loss)
- Waktu Respons Rata-rata: 47ms
- Arti Hasil: Munculnya status Reply dan Lost = 0 (0% loss) menandakan bahwa koneksi antara laptop saya dan router (192.168.1.1) dalam keadaan terhubung dengan kecepatan respons rata-rata 47 ms.

B. Hasil Pelacakan Rute (Tracert)
- Perintah: `tracert 1.1.1.1`
- Total Hop: 9 hop
```text
  1    10 ms     1 ms     1 ms  192.168.x.x
  2    27 ms     7 ms    17 ms  10.82.0.x
  3     *       11 ms     6 ms  180.250.252.x
  4    22 ms    17 ms    17 ms  180.240.196.x
  5    40 ms    11 ms    10 ms  180.240.196.x
  6     *        *        *     Request timed out.
  7    29 ms    26 ms    26 ms  172.69.117.x
  8    52 ms    42 ms    34 ms  172.69.117.x
  9    30 ms    28 ms    26 ms  one.one.one.one [1.1.1.1]

Trace complete.
