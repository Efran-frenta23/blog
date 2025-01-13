---
title: mengatasi masalah saat proses download/boot
---


Jika kamu mendapatkan pesan "Signature detected. Check secure boot policy in setup", ini biasanya berkaitan dengan fitur Secure Boot yang aktif di BIOS/UEFI komputer kamu. Secure Boot adalah fitur keamanan di UEFI yang mencegah sistem operasi yang tidak dipercaya (tidak bersertifikat) untuk dijalankan pada komputer kamu.

CachyOS atau beberapa distribusi Linux lainnya mungkin tidak memiliki sertifikat yang ditandatangani oleh Microsoft, yang sering kali menjadi penyebab Secure Boot menolak untuk memuat sistem.

Berikut adalah cara untuk mengatasi masalah ini:

1. Nonaktifkan Secure Boot di BIOS/UEFI
Cara paling umum untuk mengatasi masalah ini adalah dengan menonaktifkan Secure Boot. Berikut langkah-langkahnya:

- Restart Komputer
Saat komputer mulai menyala, tekan tombol yang sesuai untuk masuk ke BIOS/UEFI. Tombol ini biasanya F2, DEL, ESC, atau F10 (tergantung merek komputer kamu). Saat booting, biasanya ada instruksi singkat di layar yang menyebutkan tombol apa yang harus ditekan untuk masuk ke BIOS atau Setup.

- Masuk ke Pengaturan Secure Boot
Setelah masuk ke BIOS/UEFI, navigasikan ke pengaturan Boot atau Security. Di dalam menu ini, cari opsi Secure Boot.

- Nonaktifkan Secure Boot
Ubah status Secure Boot dari Enabled menjadi Disabled. Ini memungkinkan komputer untuk menjalankan sistem operasi yang tidak memiliki tanda tangan yang diperlukan oleh Secure Boot.

- Simpan Pengaturan dan Keluar
Setelah menonaktifkan Secure Boot, simpan pengaturan dengan menekan tombol yang sesuai (biasanya ada instruksi di BIOS untuk "Save and Exit"). Komputer kemudian akan restart.

- Boot dari USB atau Media Instalasi
Sekarang, coba lagi boot dari USB atau media instalasi CachyOS. Sistem seharusnya bisa boot tanpa masalah sekarang.

2. Menggunakan Shim (Opsi Alternatif)
Jika kamu ingin tetap menggunakan Secure Boot, beberapa distribusi Linux menggunakan alat bernama Shim untuk memungkinkan booting di sistem dengan Secure Boot diaktifkan. Namun, tidak semua distribusi Linux mendukung ini, jadi pastikan untuk memeriksa apakah CachyOS mendukung Secure Boot menggunakan Shim.

Langkah-langkah ini mungkin lebih kompleks, dan biasanya memerlukan distribusi Linux yang sudah diatur untuk bekerja dengan Secure Boot, seperti Ubuntu. Jika tidak ingin ribet, menonaktifkan Secure Boot adalah solusi yang paling praktis.

3. Install Key Khusus di BIOS (Advanced)
Ada opsi lain untuk menginstal kunci khusus (public key) yang digunakan oleh sistem operasi seperti CachyOS ke dalam firmware Secure Boot, namun ini adalah langkah yang lebih teknis dan jarang dilakukan oleh pengguna biasa. Untuk ini, kamu perlu menambahkan kunci UEFI ke daftar trusted keys di BIOS/UEFI.

Kesimpulan:
Cara yang paling mudah dan cepat adalah dengan menonaktifkan Secure Boot di BIOS/UEFI, karena ini akan memungkinkan kamu untuk boot ke sistem operasi yang tidak memiliki sertifikat Secure Boot yang sesuai, seperti CachyOS.

Jika ada kesulitan saat melakukan langkah-langkah di atas atau jika kamu butuh bantuan lebih lanjut, beri tahu aku!






