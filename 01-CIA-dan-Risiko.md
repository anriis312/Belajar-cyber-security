Catatan Belajar: CIA Triad dan Analisis Risiko (Day 1)

1. Paham Dasar CIA Triad
Inti dari keamanan informasi itu berporos ke tiga hal utama ini:

 - Confidentiality (Kerahasiaan): Intinya data penting nggak boleh bocor atau diintip orang yang nggak punya hak. Contoh gampangnya ya kayak saldo rekening atau data pribadi lu, jangan sampe ketahuan orang lain.

 - Integrity (Integritas): Data harus dipastikan tetap akurat dan nggak boleh diubah-ubah sembarangan tanpa izin yang sah. Contohnya, saldo di rekening lu nggak boleh tiba-tiba berubah kalau nggak ada transaksi yang valid.

 - Availability (Ketersediaan): Sistem atau data harus selalu siap diakses kapan pun kita butuh. Contohnya, pas lu mau ngecek saldo atau transfer, aplikasinya harus lagi nggak down atau bisa diakses.

2. Bedah Kasus Pelanggaran CIA Triad
Kasus 1: Serangan ke Sistem Rumah Sakit
Ada kasus sistem RS diserang gara-gara keamanan mereka amsyar—password-nya gampang ditebak dan nggak punya backup data sama sekali. Pelaku masuk, nyolong data pasien, ngubah sebagian datanya, terus di-lock pake enkripsi (ransomware) sambil minta tebusan. Otomatis pihak RS nggak bisa ngapa-ngapain.

 - Confidentiality (C): Jebol, karena data pasien berhasil dibaca dan dicuri pelaku.

 - Integrity (I): Jebol juga, karena ada data yang diubah seenaknya sama si pelaku.

 - Availability (A): Ikut lumpuh, karena datanya dikunci jadi pihak RS nggak bisa akses apa-apa.

Kasus 2: Enkripsi Server Bank (Tanpa Nyolong Data)
Ada hacker nyusup ke server bank, datanya langsung di-lock atau di-enkripsi di tempat tanpa disalin atau dibawa keluar, terus minta tebusan.

Pilar yang kena: Availability. Kenapa? Karena datanya nggak dicuri atau diubah isinya, tapi cuma ditahan atau nggak bisa diakses sama pihak bank.

Kasus 3: Jebol Akun Bank (Saldo Berubah)
Akun bank si Andi diretas, terus saldonya yang tadinya 500 juta rupiah mendadak disunat jadi 1 juta rupiah doang.

Pilar yang kena: Integrity. Jelas banget ini gara-gara data nominal saldo diubah secara ilegal tanpa izin pemilik aslinya.

Kasus 4: Kebocoran Data Perusahaan
Database penting milik suatu perusahaan berhasil dijebol hacker, terus datanya disebar begitu aja ke internet atau publik.

Pilar yang kena: Confidentiality. Karena informasi rahasia perusahaan yang harusnya privat malah bocor ke tangan publik.

3. Analisis: Threat, Vulnerability, dan Risk
Contoh Kasus: Ransomware di Rumah Sakit

Vulnerability (Celah Keamanan): Lemahnya password admin sistem RS dan absennya backup data secara berkala.

Threat (Ancaman): Aksi serangan dari hacker atau pihak luar yang mau ngerusak sistem.

Risk (Risiko Dampak): Data penting pasien berisiko tinggi kena enkripsi, lumpuh total, atau bocor ke publik gara-gara pelaku sempat baca dan nyalin datanya.