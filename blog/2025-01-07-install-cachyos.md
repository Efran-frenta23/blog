---
title: install cachyos
---

## ini adalah tutorial tentang cara installasi cachyos
**berikut adalah cara caranya** 
1. pertama kamu harus mendownload iso cachyos [download cachyos disini](https://cachyos.org/download/)
2. Membuat Bootable USB
Setelah mendownload ISO, kamu perlu membuat bootable USB untuk menginstall CachyOS. Kamu bisa menggunakan aplikasi seperti:

Rufus (untuk Windows)
Balena Etcher (untuk Windows, macOS, dan Linux)

Pilih file ISO yang sudah kamu download dan ikuti langkah-langkah di aplikasi tersebut untuk membuat USB bootable.

3. Setelah membuat bootable USB, masukkan USB ke dalam komputer dan restart. Masuk ke BIOS (biasanya dengan menekan tombol F2, DEL, atau ESC saat booting) dan ubah urutan boot untuk memprioritaskan USB. Simpan pengaturan BIOS dan boot dari USB.

4. Mulai Instalasi CachyOS
Setelah booting dari USB, kamu akan melihat layar welcome dari CachyOS. Pilih opsi untuk memulai instalasi. Proses instalasi akan memandu kamu melalui beberapa langkah seperti:

Memilih bahasa dan zona waktu
Memilih tata letak keyboard
Membuat partisi hard drive atau memilih partisi otomatis

5. Membuat Partisi
Jika kamu memilih untuk membuat partisi manual, pastikan untuk membuat setidaknya tiga partisi:

Root (/) – sebagai tempat sistem operasi diinstal.
Swap – sebagai virtual memory jika diperlukan.
Home (/home) – untuk menyimpan file dan data pribadi.

6. Proses Instalasi Dimulai
Setelah konfigurasi partisi selesai, klik tombol "Install" untuk memulai proses instalasi. Tunggu beberapa saat hingga instalasi selesai. CachyOS akan menyalin semua file dan menginstal sistem pada partisi yang dipilih.

7. Restart dan Selesai
Setelah proses instalasi selesai, kamu akan diminta untuk me-restart komputer. Lepaskan USB bootable dan biarkan komputer melakukan booting ke sistem operasi CachyOS yang baru terinstal.

8. Setelah masuk ke sistem, jangan lupa untuk memperbarui sistem agar mendapatkan pembaruan terbaru. Buka terminal dan jalankan perintah berikut:

bash
Copy code
sudo pacman -Syu
Selamat, kamu telah berhasil menginstal CachyOS!




