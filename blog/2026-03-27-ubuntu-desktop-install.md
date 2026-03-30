---
title: Install Ubuntu Desktop
---

# Cara Install Ubuntu Desktop - Panduan Lengkap untuk Pemula

Panduan lengkap instalasi Ubuntu Desktop dari awal sampai selesai. Dokumentasi ini dibuat dengan penjelasan detail agar mudah dipahami bahkan oleh orang yang baru pertama kali mencoba Linux.

---

## Apa itu Ubuntu Desktop?

**Ubuntu Desktop** adalah sistem operasi berbasis Linux yang dirancang untuk penggunaan pribadi di komputer desktop dan laptop. Ubuntu adalah salah satu distribusi Linux paling populer di dunia, digunakan oleh jutaan orang dari berbagai kalangan.

### Kenapa Memilih Ubuntu Desktop?

Ubuntu Desktop menawarkan banyak keunggulan dibanding sistem operasi lain:

**🆓 Gratis dan Open Source**
- 100% gratis - tidak perlu bayar lisensi
- Open source - bisa dimodifikasi sesuai kebutuhan
- Komunitas besar - mudah cari bantuan dan tutorial

**🎨 User-Friendly**
- Interface modern dan intuitif (GNOME Desktop)
- Mirip dengan macOS/Windows - mudah untuk pemula
- Banyak aplikasi pre-installed

**🔒 Aman**
- Virus dan malware sangat jarang di Linux
- Update keamanan rutin
- Permission system yang ketat

**📦 Software Center**
- Ribuan aplikasi gratis tersedia
- Install dengan satu klik
- Tidak perlu cari installer di internet

**🔄 Update Rutin**
- Update fitur setiap 6 bulan
- Versi LTS (Long Term Support) setiap 2 tahun
- Dukungan 5 tahun untuk versi LTS

**💻 Kompatibel**
- Support hardware luas
- Bisa dual boot dengan Windows
- Bisa jalan di virtual machine

### Apa itu Linux?

**Linux** adalah sistem operasi seperti Windows atau macOS, tapi:
- ✅ **Gratis** - Tidak perlu bayar lisensi
- ✅ **Open Source** - Kode sumber terbuka untuk umum
- ✅ **Aman** - Lebih kebal terhadap virus/malware
- ✅ **Ringan** - Bisa jalan di hardware lama
- ✅ **Customizable** - Bisa dimodifikasi sesuai selera

Ubuntu adalah salah satu "distribusi" (versi) Linux yang paling mudah digunakan.

---

## Persiapan Sebelum Install

Sebelum memulai instalasi, pastikan kamu sudah mempersiapkan hal-hal berikut:

### 1. Backup Data Penting ⚠️

**PENTING:** Proses instalasi bisa menghapus data di hard drive. Pastikan kamu sudah:

- ✅ Backup file penting ke external hard drive
- ✅ Backup foto, dokumen, dan data pribadi ke cloud (Google Drive, OneDrive, dll)
- ✅ Catat software/aplikasi yang perlu diinstall ulang nanti
- ✅ Backup bookmark browser
- ✅ Export password dari browser jika perlu

> **Kenapa harus backup?**
> Karena instalasi Linux akan memformat hard drive, semua data akan hilang permanen. Backup adalah langkah keamanan untuk menghindari kehilangan data berharga.

### 2. Cek Spesifikasi Minimum

Ubuntu Desktop membutuhkan spesifikasi hardware berikut:

**Spesifikasi Minimum:**
- **Prosesor:** 64-bit (x86_64) - Intel atau AMD, 2 GHz dual-core
- **RAM:** 4 GB (rekomendasi 8 GB atau lebih)
- **Storage:** 25 GB space kosong (rekomendasi 50 GB atau lebih)
- **Display:** 1024x768 resolution
- **USB Port:** Untuk flashdisk installer
- **Internet:** Untuk download update dan aplikasi (opsional tapi direkomendasikan)

**Spesifikasi Rekomendasi:**
- **Prosesor:** Intel Core i3 / AMD Ryzen 3 atau lebih tinggi
- **RAM:** 8 GB atau lebih
- **Storage:** SSD 120 GB atau lebih (SSD jauh lebih cepat dari HDD)
- **Internet:** WiFi atau kabel LAN

> **Catatan:** 
> - Ubuntu tidak support prosesor 32-bit sejak Ubuntu 19.04
> - Jika komputermu sangat lama (sebelum 2010), pertimbangkan Ubuntu MATE atau Xubuntu yang lebih ringan

### 3. Pilih Metode Instalasi

Ada beberapa cara untuk menggunakan Ubuntu:

#### Opsi A: Install di Komputer/Laptop (Native)

**Kelebihan:**
- ✅ Performa maksimal
- ✅ Semua hardware terutilisasi penuh
- ✅ Pengalaman terbaik

**Kekurangan:**
- ⚠️ Menghapus Windows (jika tidak dual boot)
- ⚠️ Butuh backup data dulu

**Kapan memilih ini:**
- Kamu ingin pindah sepenuhnya ke Ubuntu
- Komputer/laptop dedicated untuk Ubuntu
- Tidak butuh Windows lagi

#### Opsi B: Dual Boot dengan Windows

**Kelebihan:**
- ✅ Bisa pilih Ubuntu atau Windows saat boot
- ✅ Data Windows tetap aman
- ✅ Backup plan jika ada masalah

**Kekurangan:**
- ⚠️ Setup lebih kompleks
- ⚠️ Butuh space kosong di hard drive
- ⚠️ Ada risiko (kecil) data Windows terganggu

**Kapan memilih ini:**
- Masih butuh Windows untuk aplikasi tertentu
- Ingin coba Ubuntu tanpa commit penuh
- Butuh Windows untuk gaming atau software khusus

#### Opsi C: Virtual Machine (VM)

**Kelebihan:**
- ✅ Aman - tidak affect sistem utama
- ✅ Mudah setup dan hapus
- ✅ Bisa jalan bersamaan dengan Windows/macOS
- ✅ Bisa snapshot dan restore

**Kekurangan:**
- ⚠️ Performa tidak maksimal
- ⚠️ Butuh RAM dan storage lebih
- ⚠️ Tidak semua fitur hardware accessible

**Kapan memilih ini:**
- Ingin coba Ubuntu dulu sebelum install native
- Butuh Ubuntu untuk development/testing
- Tidak mau ambil risiko install native

**Software VM Populer:**
- **VirtualBox** - Gratis, open source (direkomendasikan)
- **VMware Player** - Gratis untuk personal use
- **Hyper-V** - Built-in di Windows Pro
- **Parallels** - Untuk Mac (berbayar)

#### Opsi D: Live USB (Try Without Installing)

**Kelebihan:**
- ✅ Coba Ubuntu tanpa install
- ✅ Tidak ada perubahan ke sistem
- ✅ Bisa test hardware compatibility

**Kekurangan:**
- ⚠️ Perubahan tidak tersimpan (kecuali pakai persistence)
- ⚠️ Performa lebih lambat dari USB
- ⚠️ Tidak untuk penggunaan jangka panjang

**Kapan memilih ini:**
- Ingin test Ubuntu dulu
- Ingin cek hardware compatibility
- Demo atau presentasi

> **Rekomendasi untuk pemula:**
> 1. **Coba dulu di Virtual Machine** - Untuk familiarisasi
> 2. **Dual Boot** - Jika masih butuh Windows
> 3. **Install Native** - Jika sudah yakin dan siap

---

## Langkah 1: Download ISO Ubuntu Desktop

### Apa itu File ISO?

**File ISO** adalah file image disk yang berisi installer lengkap Ubuntu Desktop. File ini nantinya akan "dibakar" ke flashdisk untuk membuat installer bootable.

### Cara Download

1. **Buka browser** (Chrome, Firefox, Edge, dll)
2. **Kunjungi website resmi:** [ubuntu.com/download/desktop](https://ubuntu.com/download/desktop)
3. **Pilih versi yang ingin didownload**

### Memilih Versi Ubuntu Desktop

Ubuntu tersedia dalam beberapa versi:

#### Versi LTS (Long Term Support) - ⭐ Direkomendasikan

**LTS** adalah singkatan dari **Long Term Support**. Ini adalah versi Ubuntu yang mendapatkan dukungan jangka panjang.

**Karakteristik versi LTS:**
- ✅ **Dukungan 5 tahun** - Update keamanan dan bug fix selama 5 tahun
- ✅ **Stabil** - Sudah melalui testing matang
- ✅ **Direkomendasikan untuk kebanyakan user**
- ✅ **Update fitur minimal** - Fokus pada stabilitas

**Versi LTS Terbaru:**
- **Ubuntu 24.04 LTS (Noble Numbat)** - Rilis April 2024, didukung sampai 2029 ⭐
- **Ubuntu 22.04 LTS (Jammy Jellyfish)** - Rilis April 2022, didukung sampai 2027
- **Ubuntu 20.04 LTS (Focal Fossa)** - Rilis April 2020, didukung sampai 2025

> **Rekomendasi:** Pilih **Ubuntu 24.04 LTS** untuk kebanyakan user. Stabil dan didukung sampai 2029!

#### Versi Interim (Short Term Support)

Versi **Interim** adalah versi Ubuntu yang dirilis di antara versi LTS.

**Karakteristik versi Interim:**
- ⚠️ **Dukungan hanya 9 bulan** - Harus upgrade setelah 9 bulan
- ⚠️ **Fitur lebih baru** - Mendapatkan fitur terbaru lebih dulu
- ⚠️ **Untuk enthusiast dan developer**

**Versi Interim Terbaru:**
- Ubuntu 24.10 (Oracular Oriole) - Rilis Oktober 2024
- Ubuntu 23.10 (Mantic Minotaur) - Sudah EOL
- Ubuntu 23.04 (Lunar Lobster) - Sudah EOL

> **Kapan memilih Interim?**
> - Kamu developer yang butuh fitur terbaru
> - Kamu enthusiast yang suka coba hal baru
> - Kamu tidak masalah upgrade setiap 6-9 bulan

### Proses Download

1. **Klik tombol "Download"** untuk versi yang kamu pilih
2. **Download akan otomatis dimulai** (file berukuran 5-6 GB)
3. **Tunggu hingga selesai** - Bisa 30 menit - 2 jam tergantung koneksi
4. **Simpan di lokasi yang mudah ditemukan** (misal: Downloads folder)

> **Tips Download:**
> - Gunakan koneksi WiFi atau kabel LAN yang stabil
> - Download bisa di-pause dan resume jika terputus
> - File ISO Ubuntu berukuran 5-6 GB, pastikan ada space cukup

### Opsi Download yang Tersedia

Saat download Ubuntu, kamu akan menemukan beberapa opsi:

#### 1. Direct Download

**Apa itu?** Download langsung dari server Ubuntu.

**Karakteristik:**
- ✅ Cepat dan langsung
- ✅ Server resmi Ubuntu
- ⚠️ Bisa lambat saat rilis baru (banyak yang download)

#### 2. Torrent Download

**Apa itu?** Download peer-to-peer dari user lain.

**Karakteristik:**
- ✅ Bisa lebih cepat jika banyak seeder
- ✅ Tidak membebani server Ubuntu
- ✅ Resume support
- ⚠️ Butuh torrent client (qBittorrent, Transmission)

**Kapan memilih Torrent:**
- Server Ubuntu lambat
- Koneksi tidak stabil (bisa resume)
- Support komunitas Ubuntu

**Cara pakai:**
1. Download file `.torrent` dari website Ubuntu
2. Buka dengan torrent client
3. Tunggu download selesai

#### 3. Mirror Server

**Apa itu?** Server replika di berbagai lokasi geografis.

**Mirror Populer:**
- **Indonesia:** `kartolo.sby.datautama.net.id`, `mirror.telkomnet.id.id`
- **Singapore:** `mirror.nus.edu.sg`
- **Malaysia:** `mirror.seas.upenn.edu.my`

**Kapan memilih Mirror:**
- Server utama Ubuntu lambat dari lokasimu
- Ingin download lebih cepat

### Verifikasi File ISO (Opsional tapi Direkomendasikan)

**Mengapa verifikasi?**
- ✅ Pastikan file tidak corrupt saat download
- ✅ Pastikan file asli dari Ubuntu
- ✅ Hindari masalah saat instalasi

**Cara Verifikasi di Windows:**
```powershell
certutil -hashfile C:\Users\NamaKamu\Downloads\ubuntu-24.04-desktop-amd64.iso SHA256
```

**Cara Verifikasi di Linux/macOS:**
```bash
sha256sum ~/Downloads/ubuntu-24.04-desktop-amd64.iso
```

**Bandingkan hash** dengan yang ada di website Ubuntu (`SHA256SUMS` file).

> **Untuk pemula:** Verifikasi opsional. Jika download dari website resmi dan selesai 100%, biasanya aman.

---

## Langkah 2: Membuat Bootable USB

### Apa itu Bootable USB?

**Bootable USB** adalah flashdisk yang sudah diisi file installer Ubuntu dan bisa digunakan untuk "booting" komputer, mirip seperti CD/DVD installer zaman dulu.

### Persiapan Flashdisk

- **Kapasitas:** Minimal 8 GB (file ISO 5-6 GB)
- **Kondisi:** Tidak rusak
- **Isi:** Kosongkan atau backup isi flashdisk (akan diformat)

### Pilihan Aplikasi Pembuat Bootable USB

#### 1. Rufus (Windows) - ⭐ Paling Direkomendasikan

**Website:** [rufus.ie](https://rufus.ie)

**Kelebihan:**
- ✅ Gratis dan open source
- ✅ Sangat cepat
- ✅ Ringan (tidak perlu install)
- ✅ Support banyak opsi

**Cara Menggunakan Rufus:**

1. **Download Rufus** dari [rufus.ie](https://rufus.ie)
2. **Jalankan Rufus** (klik dua kali file .exe)
3. **Colokkan flashdisk** ke komputer
4. **Di Rufus, pilih:**
   - **Device:** Pilih flashdiskmu
   - **Boot selection:** Klik "SELECT" dan pilih file ISO Ubuntu
   - **Partition scheme:** GPT (untuk komputer modern UEFI)
   - **Target system:** UEFI (non CSM)
5. **Klik "START"**
6. **Pilih mode:** "Write in ISO Image mode (Recommended)"
7. **Tunggu proses selesai** (10-20 menit)
8. **Klik "CLOSE"** setelah selesai

> **Peringatan:** Semua data di flashdisk akan dihapus! Backup dulu jika ada data penting.

#### 2. Balena Etcher (Windows, macOS, Linux)

**Website:** [balena.io/etcher](https://www.balena.io/etcher)

**Kelebihan:**
- ✅ Interface sangat sederhana
- ✅ Cross-platform (bisa di Windows, Mac, Linux)
- ✅ Ada verifikasi otomatis
- ✅ Aman (sulit salah pilih disk)

**Cara Menggunakan Balena Etcher:**

1. **Download Balena Etcher** dari [balena.io/etcher](https://www.balena.io/etcher)
2. **Install dan jalankan** Etcher
3. **Klik "Flash from file"** → pilih file ISO Ubuntu
4. **Klik "Select target"** → pilih flashdiskmu
5. **Klik "Flash!"**
6. **Tunggu hingga selesai** (ada proses verifikasi otomatis)
7. **Done!** Flashdisk siap digunakan

#### 3. Ventoy (Windows, Linux) - Paling Fleksibel

**Website:** [ventoy.net](https://www.ventoy.net)

**Kelebihan:**
- ✅ Bisa taruh MULTIPLE ISO dalam 1 flashdisk
- ✅ Tidak perlu format ulang setiap ganti ISO
- ✅ Cukup copy-paste file ISO
- ✅ Bisa boot banyak distribusi Linux

**Cara Menggunakan Ventoy:**

1. **Download Ventoy** dari [ventoy.net](https://www.ventoy.net)
2. **Extract dan jalankan** Ventoy2Disk.exe
3. **Pilih flashdisk** dan klik "Install"
4. **Setelah selesai,** flashdisk akan muncul di File Explorer
5. **Copy file ISO Ubuntu** ke dalam flashdisk (seperti copy file biasa)
6. **Done!** Flashdisk siap digunakan

> **Kelebihan Ventoy:** Kamu bisa taruh banyak ISO (Windows, Ubuntu, dll) dalam 1 flashdisk dan pilih saat booting!

#### 4. Startup Disk Creator (Ubuntu)

Jika kamu sudah punya Ubuntu dan ingin buat bootable USB:

1. **Buka "Startup Disk Creator"** dari aplikasi menu
2. **Pilih file ISO** Ubuntu
3. **Pilih flashdisk** target
4. **Klik "Make Startup Disk"**

---

## Langkah 3: Boot dari USB

### Apa itu Booting?

**Booting** adalah proses menyalakan komputer dan memuat sistem operasi. Normalnya komputer boot dari hard drive (Windows/Linux yang sudah terinstall). Kita akan mengubahnya untuk boot dari USB installer.

### Cara Masuk BIOS/UEFI

**BIOS/UEFI** adalah sistem dasar yang mengontrol hardware komputer sebelum sistem operasi berjalan.

**Langkah masuk BIOS/UEFI:**

1. **Matikan komputer** sepenuhnya (shutdown)
2. **Colokkan flashdisk** installer ke port USB
3. **Nyalakan komputer**
4. **Segera tekan tombol BIOS berulang-ulang** sebelum logo Windows/Linux muncul

**Tombol BIOS berdasarkan merk:**

| Merk Laptop/Motherboard | Tombol BIOS |
|------------------------|-------------|
| ASUS | F2 atau DEL |
| Acer | F2 atau DEL |
| Lenovo | F1, F2, atau Fn + F2 |
| HP | F10 atau ESC |
| Dell | F2 atau F12 |
| MSI | DEL |
| Gigabyte | F2 atau DEL |
| Toshiba | F2 atau F12 |
| Samsung | F2 atau F10 |

> **Tips:** Jika tidak berhasil, coba restart dan tekan tombol lebih cepat. Beberapa laptop butuh tombol Fn ditekan bersamaan (misal: Fn + F2).

### Mengubah Boot Order

Setelah masuk BIOS/UEFI:

1. **Cari menu "Boot"** atau "Boot Priority" atau "Boot Order"
   - Gunakan tombol panah keyboard untuk navigasi
   - Mouse mungkin tidak berfungsi di BIOS lama

2. **Pindahkan USB ke posisi paling atas**
   - Biasanya menggunakan tombol F5/F6 atau +/-
   - Cari yang bernama "USB", "Removable Device", atau nama flashdiskmu

3. **Simpan pengaturan dan exit**
   - Biasanya tekan **F10** untuk Save & Exit
   - Atau pilih "Save Changes and Reset"

4. **Komputer akan restart** dan boot dari USB

### Boot Menu (Cara Alternatif)

Beberapa komputer punya **Boot Menu** yang lebih cepat tanpa masuk BIOS:

**Cara pakai Boot Menu:**
1. Restart komputer
2. Tekan tombol Boot Menu berulang-ulang (biasanya **F12**, **F11**, **F8**, atau **ESC**)
3. Pilih flashdisk dari list
4. Enter dan komputer akan boot dari USB

**Tombol Boot Menu berdasarkan merk:**
- ASUS: F8 atau ESC
- Acer: F12
- Lenovo: F12 atau Fn + F12
- HP: F9 atau ESC
- Dell: F12
- MSI: F11

### Disable Secure Boot (Jika Diperlukan)

**Apa itu Secure Boot?**
Secure Boot adalah fitur keamanan di UEFI yang hanya mengizinkan software dengan tanda tangan digital resmi untuk boot.

**Kenapa disable Secure Boot?**
Ubuntu seharusnya bisa boot dengan Secure Boot aktif, tapi beberapa komputer punya masalah.

**Cara disable Secure Boot:**
1. Masuk BIOS/UEFI
2. Cari menu **"Security"** atau **"Boot"**
3. Cari opsi **"Secure Boot"**
4. Ubah dari **"Enabled"** ke **"Disabled"**
5. Save dan Exit (F10)

> **Catatan:** Ubuntu modern support Secure Boot. Disable hanya jika ada masalah booting.

---

## Langkah 4: Memulai Instalasi Ubuntu Desktop

### Tampilan Awal Boot

Setelah boot dari USB, kamu akan melihat:

1. **Menu GRUB** - Pilih opsi pertama "Try or Install Ubuntu"
2. **Loading screen** - Tunggu sistem loading
3. **Desktop Live** - Kamu akan masuk ke desktop Ubuntu tanpa install

> **Apa itu Live Session?**
> Live session adalah mode "coba dulu" di mana kamu bisa mencoba Ubuntu Desktop tanpa menginstall. Semua perubahan tidak akan tersimpan setelah restart. Ini bagus untuk test hardware compatibility!

### Test Ubuntu Dulu (Opsional tapi Direkomendasikan)

Sebelum install, coba dulu Ubuntu di live session:

**Yang bisa dicoba:**
- ✅ Browse internet
- ✅ Test WiFi
- ✅ Test audio/suara
- ✅ Test display resolution
- ✅ Test touchpad/mouse
- ✅ Buka aplikasi pre-installed

**Jika semua berfungsi:** Lanjut install!
**Jika ada masalah:** Cari solusi dulu sebelum install.

### Menjalankan Installer

1. **Klik ikon "Install Ubuntu"** di desktop
2. **Installer akan terbuka** dan memandu kamu melalui proses instalasi

---

## Langkah 5: Konfigurasi Instalasi

### 1. Pilih Bahasa

**Langkah:**
- Pilih bahasa yang kamu mengerti
- **Rekomendasi:** English (US) atau Indonesia (jika tersedia)

> **Tips:** Pilih English untuk kemudahan troubleshooting karena sebagian besar tutorial Ubuntu menggunakan bahasa Inggris.

### 2. Pilih Keyboard Layout

**Langkah:**
1. Pilih bahasa keyboard
2. **Rekomendasi:** "English (US)" atau "English (UK)"
3. **Test keyboard:** Ketik di kotak test untuk memastikan keyboard berfungsi normal

**Deteksi Otomatis:**
Ubuntu biasanya auto-detect keyboard layout. Test dengan mengetik beberapa karakter khusus seperti `@`, `#`, `$`, `&`.

### 3. Pilih Updates dan Software

**Opsi yang tersedia:**

#### Normal Installation

**Includes:**
- ✅ Web browser (Firefox)
- ✅ Office suite (LibreOffice)
- ✅ Media players
- ✅ Games
- ✅ Utilities

**Kapan memilih ini:**
- ✅ Untuk penggunaan sehari-hari
- ✅ Kamu ingin sistem yang siap pakai
- ✅ Tidak mau ribet install aplikasi nanti

#### Minimal Installation

**Includes:**
- ✅ Web browser (Firefox)
- ✅ Basic utilities

**Kapan memilih ini:**
- ✅ Kamu suka custom sendiri
- ✅ Storage terbatas
- ✅ Hanya butuh aplikasi tertentu

#### Download updates while installing Ubuntu

**Kelebihan:**
- ✅ Sistem langsung up-to-date setelah install
- ✅ Tidak perlu update manual setelah install

**Kekurangan:**
- ⚠️ Instalasi lebih lama
- ⚠️ Butuh koneksi internet

**Kapan memilih ini:**
- ✅ Koneksi internet cepat
- ✅ Tidak masalah tunggu lebih lama

#### Install third-party software for graphics and Wi-Fi hardware

**Apa ini?**
Driver proprietary untuk hardware tertentu (NVIDIA, WiFi adapters, dll).

**Kelebihan:**
- ✅ Hardware berfungsi optimal
- ✅ WiFi dan graphics berfungsi penuh

**Kekurangan:**
- ⚠️ Software proprietary (bukan open source)

**Kapan memilih ini:**
- ✅ **CHECK!** Sangat direkomendasikan untuk hardware compatibility

> **Rekomendasi untuk pemula:**
> - **Normal Installation**
> - **✓ Download updates while installing** (jika internet cepat)
> - **✓ Install third-party software** (PENTING!)

### 4. Tipe Instalasi (PENTING!)

Ini adalah langkah paling penting. Ada beberapa opsi:

#### Opsi A: Erase Disk and Install Ubuntu (Otomatis) - ⭐ Untuk Install Bersih

**Apa yang terjadi:**
- ✅ Seluruh hard drive akan dihapus
- ✅ Installer yang atur partisi otomatis
- ✅ Ubuntu akan jadi satu-satunya sistem operasi

**Kapan memilih ini:**
- Komputer/laptop baru/kosong
- Tidak ada data penting di hard drive
- Ingin install Ubuntu sebagai satu-satunya OS
- Sudah backup semua data

> **⚠️ PERINGATAN:** Semua data di hard drive akan hilang! Pastikan sudah backup!

#### Opsi B: Install Ubuntu Alongside Windows Boot Manager (Dual Boot)

**Apa yang terjadi:**
- ✅ Ubuntu dan Windows akan co-exist
- ✅ Kamu bisa pilih Ubuntu atau Windows saat boot
- ✅ Installer akan resize partisi Windows otomatis

**Kapan memilih ini:**
- Masih butuh Windows untuk aplikasi tertentu
- Ingin coba Ubuntu tanpa commit penuh
- Ada space kosong di hard drive

**Requirement:**
- Minimal 50 GB space kosong di Windows
- Backup data Windows dulu (untuk jaga-jaga)

> **Tips:** Dual boot adalah pilihan aman untuk pemula yang masih butuh Windows.

#### Opsi C: Something Else (Manual Partitioning) - Untuk Advanced User

**Apa yang terjadi:**
- Kamu atur sendiri partisi secara manual
- Kontrol penuh atas layout partisi
- Bisa custom sesuai kebutuhan

**Kapan memilih ini:**
- Sudah berpengalaman dengan Linux
- Punya kebutuhan partisi khusus
- Ingin kontrol penuh

#### Panduan Partisi Manual (Jika Memilih Manual)

Jika memilih manual, buat partisi berikut:

| Partisi | Mount Point | Ukuran | Tipe | Fungsi |
|---------|-------------|--------|------|--------|
| **EFI** | /boot/efi | 512 MB | EFI System | Untuk boot UEFI |
| **Root** | / | 50-100 GB | ext4 | Untuk sistem operasi dan aplikasi |
| **Home** | /home | Sisa space | ext4 | Untuk data dan file pribadi |
| **Swap** | swap | 4-8 GB | swap | Virtual memory (opsional) |

**Penjelasan Partisi:**

**1. EFI Partition (/boot/efi)**
- **Fungsi:** Tempat file boot untuk sistem UEFI
- **Ukuran:** 512 MB
- **Format:** EFI System Partition
- **Wajib untuk:** Komputer modern dengan UEFI
- **Catatan:** Jika sudah ada Windows, biasanya sudah ada EFI partition - reuse saja!

**2. Root Partition (/)**
- **Fungsi:** Tempat install sistem operasi dan aplikasi
- **Ukuran:** Minimal 50 GB, rekomendasi 100 GB atau lebih
- **Format:** ext4
- **Wajib:** Ya, ini partisi utama

**3. Home Partition (/home)**
- **Fungsi:** Tempat menyimpan file pribadi (dokumen, foto, download, dll)
- **Ukuran:** Sisa space hard drive
- **Format:** ext4
- **Wajib:** Tidak, tapi sangat direkomendasikan

> **Kenapa pisahkan Root dan Home?**
> Jika suatu saat ingin reinstall Ubuntu, data di /home tetap aman karena terpisah dari sistem.

**4. Swap Partition**
- **Fungsi:** Virtual memory (menggunakan storage sebagai RAM tambahan)
- **Ukuran:** 4-8 GB (atau sama dengan RAM jika RAM < 8GB)
- **Format:** swap
- **Wajib:** Tidak, Ubuntu modern bisa pakai swap file

> **Catatan:** Di sistem modern dengan RAM besar (8GB+), swap tidak terlalu diperlukan. Ubuntu akan membuat swap file otomatis jika perlu.

### 5. Pilih Lokasi/Timezone

**Langkah:**
1. Klik pada peta atau pilih dari dropdown
2. Pilih timezone kamu (misal: Jakarta, Singapore, dll)

**Fungsi:** Mengatur waktu sistem yang benar sesuai lokasimu.

### 6. Buat User Account

**Langkah:**
1. **Masukkan nama lengkap** (misal: John Doe)
2. **Masukkan nama komputer** (hostname) - otomatis terisi, bisa diubah
3. **Masukkan username** - untuk login (huruf kecil, tanpa spasi)
4. **Masukkan password** - buat password yang kuat
5. **Konfirmasi password** - ketik ulang password

**Tips Password:**
- ✅ Minimal 8 karakter
- ✅ Kombinasi huruf besar, huruf kecil, angka, dan simbol
- ✅ Jangan gunakan password yang mudah ditebak
- ✅ Catat password di tempat aman

**Opsi Login:**
- **Log in automatically** - Login otomatis tanpa password (tidak direkomendasikan)
- **Require my password to log in** - Butuh password saat login (direkomendasikan)
- **Encrypt my home folder** - Encrypt folder home untuk keamanan (opsional)

> **Rekomendasi:** Pilih "Require my password to log in" untuk keamanan.

### 7. Review dan Konfirmasi

**Sebelum install:**
- Review semua pengaturan
- Pastikan partisi sudah benar (terutama jika dual boot!)
- Pastikan user sudah dibuat
- Klik "Install Now" untuk mulai

**Konfirmasi:**
- Akan muncul popup konfirmasi partisi
- Baca dengan teliti (terutama untuk dual boot)
- Klik "Continue" jika sudah yakin

---

## Langkah 6: Proses Instalasi

### Yang Terjadi Saat Instalasi

Setelah klik "Install Now", installer akan:

1. **Format partisi** - Menyiapkan hard drive
2. **Install sistem** - Menyalin file sistem ke hard drive
3. **Install bootloader** - GRUB untuk booting
4. **Setup user** - Membuat akun yang kamu buat
5. **Install package dasar** - Sistem dasar dan aplikasi
6. **Download updates** - Jika dipilih tadi
7. **Install third-party software** - Driver dan codec

### Durasi Instalasi

- **SSD:** 15-30 menit
- **HDD:** 30-60 menit

Tergantung:
- Kecepatan storage (SSD vs HDD)
- Spesifikasi komputer
- Apakah download updates
- Jumlah aplikasi yang diinstall

### Jangan Lakukan Ini Saat Instalasi

❌ **Jangan matikan komputer** - Bisa corrupt sistem
❌ **Jangan cabut USB** - Bisa gagal install
❌ **Jangan restart** - Tunggu hingga selesai
❌ **Jangan tutup laptop** - Bisa sleep/hibernate

---

## Langkah 7: Restart dan Selesai

### Setelah Instalasi Selesai

1. **Muncul pesan "Installation Complete"**
2. **Klik "Restart Now"**
3. **Lepaskan flashdisk USB** saat diminta (atau saat layar blank)
4. **Komputer akan boot** ke Ubuntu Desktop yang baru diinstall

### Bootloader GRUB (Untuk Dual Boot)

Jika dual boot dengan Windows, saat boot kamu akan melihat **GRUB Menu**:

```
Ubuntu
Advanced options for Ubuntu
Windows Boot Manager (pada /dev/sda)
```

**Cara pakai:**
- Gunakan tombol panah ↑↓ untuk pilih
- Tekan Enter untuk boot
- Tunggu beberapa detik akan boot ke default (Ubuntu)

**Timeout:**
- Default boot setelah 10 detik
- Bisa diubah di Ubuntu: `sudo nano /etc/default/grub`

### Login Pertama

1. **Masuk ke login screen**
2. **Pilih user** kamu
3. **Masukkan password**
4. **Welcome to Ubuntu Desktop!** 🎉

---

## Langkah 8: Setup Awal Setelah Install

### 1. Update Sistem

Setelah install, selalu update sistem untuk mendapatkan package terbaru:

**Cara Update:**

1. **Buka Terminal**
   - Tekan `Ctrl + Alt + T` atau
   - Cari "Terminal" di aplikasi menu (tekan Super/Windows key, ketik "Terminal")

2. **Jalankan perintah update:**
```bash
sudo apt update && sudo apt upgrade -y
```

**Penjelasan perintah:**
- `sudo` - Jalankan sebagai administrator (root)
- `apt` - Package manager Ubuntu
- `update` - Refresh database package
- `upgrade` - Upgrade semua package yang ada update
- `-y` - Otomatis jawab "yes" untuk konfirmasi

3. **Masukkan password** saat diminta (password tidak akan terlihat saat diketik - ini normal!)
4. **Tunggu hingga selesai** - Bisa 5-30 menit tergantung jumlah update

> **Kenapa harus update?**
> Untuk mendapatkan security patch terbaru, bug fixes, dan fitur terbaru.

### 2. Install Driver Tambahan (Jika Perlu)

Ubuntu biasanya sudah include driver yang diperlukan. Tapi untuk hardware tertentu:

**Cara Install Driver:**

1. **Buka "Software & Updates"**
2. **Tab "Additional Drivers"**
3. **Tunggu scan selesai**
4. **Pilih driver** yang direkomendasikan (misal: NVIDIA driver)
5. **Klik "Apply Changes"**
6. **Restart** setelah selesai

**Driver NVIDIA (Manual):**
```bash
sudo apt install nvidia-driver-535
sudo reboot
```

### 3. Install Codec Multimedia

Untuk play video dan audio format tertentu:

```bash
sudo apt install ubuntu-restricted-extras
```

**Includes:**
- MP3, DVD, MP4 playback
- Microsoft fonts
- Flash plugin
- Codecs berbagai format

> **Catatan:** Saat install, akan muncul popup EULA. Pilih "OK" atau tekan Tab + Enter.

### 4. Install Aplikasi Esensial

Berikut aplikasi yang berguna untuk install:

**Web Browser:**
```bash
# Google Chrome
wget https://dl.google.com/linux/direct/google-chrome-stable_current_amd64.deb
sudo dpkg -i google-chrome-stable_current_amd64.deb

# Atau Microsoft Edge
sudo curl https://packages.microsoft.com/keys/microsoft.asc | gpg --dearmor > microsoft.gpg
sudo install -o root -g root -m 644 microsoft.gpg /etc/apt/trusted.gpg.d/
sudo sh -c 'echo "deb [arch=amd64] https://packages.microsoft.com/repos/edge stable main" > /etc/apt/sources.list.d/microsoft-edge-dev.list'
sudo apt update && sudo apt install microsoft-edge-stable
```

**Media Player:**
```bash
sudo apt install vlc
```

**Office Suite:**
```bash
# LibreOffice (sudah terinstall)
# Atau install WPS Office
```

**Compression:**
```bash
sudo apt install p7zip-full p7zip-rar unrar
```

**Git (untuk developer):**
```bash
sudo apt install git
```

**GIMP (image editor):**
```bash
sudo apt install gimp
```

**Steam (gaming):**
```bash
sudo apt install steam
```

### 5. Customize Desktop

**Install GNOME Tweaks:**
```bash
sudo apt install gnome-tweaks
```

**Buka "Tweaks"** dari aplikasi menu untuk:
- Ubah tema
- Ubah icon
- Ubah font
- Customize desktop behavior

**Install Extensions:**
1. Buka browser, kunjungi [extensions.gnome.org](https://extensions.gnome.org)
2. Install GNOME Shell integration extension di browser
3. Browse dan install extensions yang kamu suka

**Extensions Populer:**
- **Dash to Dock** - Dock seperti macOS
- **User Themes** - Custom shell theme
- **Clipboard Indicator** - Clipboard history
- **Weather O'Clock** - Weather di clock
- **GSConnect** - Integrate dengan Android phone

### 6. Setup Backup (Timeshift)

**Install Timeshift:**
```bash
sudo apt install timeshift
```

**Setup Timeshift:**
1. Buka Timeshift dari aplikasi menu
2. Pilih tipe snapshot: **RSYNC**
3. Pilih lokasi backup (external drive direkomendasikan)
4. Setup schedule: **Daily, Weekly, Monthly**
5. Klik **Finish**

> **Kenapa Timeshift?**
> Timeshift akan membuat snapshot sistem. Jika ada masalah, bisa restore ke kondisi sebelumnya!

### 7. Enable Firewall

**Enable UFW (Uncomplicated Firewall):**
```bash
sudo ufw enable
sudo ufw status
```

> **Catatan:** Untuk desktop usage, firewall biasanya tidak terlalu critical, tapi good to have!

---

## Troubleshooting - Masalah Umum dan Solusi

### 1. USB Tidak Terdeteksi Saat Boot

**Masalah:** Komputer tidak boot dari USB

**Solusi:**
- ✅ Pastikan USB sudah terpasang dengan benar
- ✅ Coba port USB lain (prefer USB 2.0 jika ada)
- ✅ Cek boot order di BIOS
- ✅ Disable "Secure Boot" di BIOS
- ✅ Pastikan flashdisk dibuat dengan benar (coba buat ulang dengan Rufus/Etcher)

### 2. WiFi Tidak Berfungsi

**Masalah:** WiFi tidak terdeteksi setelah install

**Solusi:**
- ✅ Connect ke LAN cable sementara
- ✅ Update sistem:
```bash
sudo apt update && sudo apt upgrade
```
- ✅ Install firmware tambahan:
```bash
sudo apt install linux-firmware
```
- ✅ Install driver WiFi spesifik (cari model WiFi adapter dulu):
```bash
lspci | grep -i network
```
- ✅ Restart

### 3. Resolusi Layar Salah

**Masalah:** Resolusi tidak sesuai atau layar kecil

**Solusi:**
- ✅ Buka **Settings** → **Displays**
- ✅ Pilih resolution yang sesuai
- ✅ Apply dan Keep Changes
- ✅ Jika tidak ada pilihan yang sesuai, install driver:
```bash
# NVIDIA
sudo apt install nvidia-driver-535

# AMD/Intel (biasanya sudah include)
sudo apt install xserver-xorg-video-amdgpu
```
- ✅ Restart

### 4. Audio Tidak Keluar

**Masalah:** Tidak ada suara

**Solusi:**
- ✅ Cek volume tidak mute (klik icon speaker di top bar)
- ✅ Buka **Settings** → **Sound**
- ✅ Pilih output device yang benar
- ✅ Install PulseAudio controls:
```bash
sudo apt install pavucontrol
pavucontrol
```
- ✅ Restart audio service:
```bash
systemctl --user restart pulseaudio
```

### 5. Touchpad Tidak Berfungsi (Laptop)

**Masalah:** Touchpad tidak responsif

**Solusi:**
- ✅ Buka **Settings** → **Mouse & Touchpad**
- ✅ Pastikan touchpad enabled
- ✅ Install driver:
```bash
sudo apt install xserver-xorg-input-libinput
```
- ✅ Restart

### 6. GRUB Tidak Muncul (Dual Boot)

**Masalah:** Langsung boot ke Windows, GRUB tidak muncul

**Solusi:**
- ✅ Restart dan masuk BIOS
- ✅ Ubah boot order, pindah Ubuntu/GRUB ke atas
- ✅ Disable "Fast Boot" di BIOS
- ✅ Jika masih tidak muncul, boot dari USB Ubuntu dan repair GRUB:
```bash
sudo add-apt-repository ppa:yannubuntu/boot-repair
sudo apt update
sudo apt install boot-repair
boot-repair
```

### 7. Windows Tidak Muncul di GRUB

**Masalah:** Dual boot tapi Windows tidak ada di menu GRUB

**Solusi:**
```bash
sudo os-prober
sudo update-grub
```

Jika os-prober tidak detect Windows:
```bash
sudo nano /etc/default/grub
# Tambahkan atau ubah:
GRUB_DISABLE_OS_PROBER=false
# Save (Ctrl+O, Enter) dan Exit (Ctrl+X)
sudo update-grub
```

### 8. Laptop Cepat Panas/Baterai Cepat Habis

**Masalah:** Laptop cepat panas atau baterai cepat habis

**Solusi:**
- ✅ Install TLP untuk power management:
```bash
sudo apt install tlp tlp-rdw
sudo tlp start
```
- ✅ Install thermald:
```bash
sudo apt install thermald
sudo systemctl enable thermald
```
- ✅ Gunakan integrated graphics (jika ada dedicated GPU):
```bash
sudo apt install prime-select
prime-select intel  # atau nvidia
```

### 9. Aplikasi Tidak Bisa Dibuka/Crash

**Masalah:** Aplikasi tertentu crash atau tidak bisa dibuka

**Solusi:**
- ✅ Update sistem:
```bash
sudo apt update && sudo apt upgrade
```
- ✅ Reinstall aplikasi:
```bash
sudo apt install --reinstall nama-aplikasi
```
- ✅ Cek log error:
```bash
journalctl -xe
```

### 10. Storage Penuh

**Masalah:** Storage cepat penuh

**Solusi:**
- ✅ Bersihkan cache apt:
```bash
sudo apt clean
sudo apt autoremove
```
- ✅ Hapus kernel lama:
```bash
sudo apt install byobu
byobu-select-backend
sudo apt autoremove --purge
```
- ✅ Cek penggunaan storage:
```bash
df -h
du -sh ~/*
```
- ✅ Install Stacer (system optimizer):
```bash
sudo apt install stacer
```

---

## FAQ - Pertanyaan yang Sering Ditanyakan

### Q: Apakah Ubuntu gratis?

**A:** Ya, 100% gratis! Ubuntu adalah open source dan bisa digunakan tanpa biaya.

### Q: Apakah Ubuntu aman untuk pemula?

**A:** Ya! Ubuntu adalah salah satu distribusi Linux paling ramah untuk pemula dengan komunitas besar dan dokumentasi lengkap.

### Q: Apa bedanya Ubuntu dan Windows?

**A:**
| Ubuntu | Windows |
|--------|---------|
| Gratis | Berbayar (lisensi) |
| Open Source | Closed Source |
| Lebih aman dari virus | Target empuk virus |
| Package manager untuk install app | Install dari installer/exe |
| Customizable | Terbatas |
| Ringan | Lebih berat |

### Q: Apakah saya bisa dual boot dengan Windows?

**A:** Ya! Ubuntu support dual boot dengan Windows. Pilih "Install Ubuntu alongside Windows" saat instalasi.

### Q: Berapa RAM minimal untuk Ubuntu?

**A:**
- **Minimal:** 4 GB RAM
- **Rekomendasi:** 8 GB RAM atau lebih
- **Untuk heavy usage:** 16 GB RAM atau lebih

### Q: Berapa storage minimal untuk Ubuntu?

**A:**
- **Minimal:** 25 GB
- **Rekomendasi:** 50 GB atau lebih
- **Untuk长期使用:** 100 GB atau lebih

### Q: Apakah Ubuntu punya Microsoft Office?

**A:** Tidak native, tapi ada alternatif:
- **LibreOffice** (sudah terinstall) - Compatible dengan MS Office
- **WPS Office** - Bisa download terpisah
- **Office 365 Online** - Via browser

### Q: Apakah perlu antivirus di Ubuntu?

**A:** Umumnya tidak perlu. Ubuntu/Linux lebih aman dari virus. Tapi tetap berhati-hati saat download file dari sumber tidak terpercaya.

### Q: Bagaimana cara backup sistem?

**A:** Gunakan Timeshift:
```bash
sudo apt install timeshift
```
Timeshift akan membuat snapshot sistem yang bisa di-restore jika ada masalah.

### Q: Apakah Ubuntu cocok untuk gaming?

**A:** Semakin baik! Steam Proton membuat banyak game Windows bisa jalan di Ubuntu. Tapi tidak semua game compatible.

### Q: Apa itu LTS?

**A:** LTS = Long Term Support. Versi LTS mendapatkan update keamanan selama 5 tahun. Direkomendasikan untuk kebanyakan user.

### Q: Bisakah upgrade dari versi lama ke versi baru?

**A:** Ya! Ubuntu mendukung upgrade. Contoh: 22.04 → 24.04. Tapi selalu backup dulu sebelum upgrade!

### Q: Apakah Ubuntu support printer dan scanner?

**A:** Ya, sebagian besar printer dan scanner support out-of-the-box. Cek compatibility di [openprinting.org](https://www.openprinting.org/printers)

### Q: Bagaimana cara install aplikasi?

**A:** Ada beberapa cara:
1. **Ubuntu Software** - App store (paling mudah)
2. **APT** - Command line: `sudo apt install nama-aplikasi`
3. **Snap** - `sudo snap install nama-aplikasi`
4. **Download .deb** - Dari website, install dengan `sudo dpkg -i file.deb`

### Q: Apa itu Snap dan Flatpak?

**A:**
- **Snap** - Package format dari Canonical (pembuat Ubuntu)
- **Flatpak** - Package format universal Linux

Keduanya adalah cara install aplikasi yang terisolasi dan mudah.

### Q: Apakah saya bisa run aplikasi Windows (.exe) di Ubuntu?

**A:** Tidak native, tapi bisa pakai:
- **Wine** - Compatibility layer untuk run .exe
- **PlayOnLinux** - GUI untuk Wine
- **Virtual Machine** - Install Windows di VM

### Q: Bagaimana cara contact support?

**A:**
- **Forum Ubuntu:** [ubuntuforums.org](https://ubuntuforums.org)
- **Ask Ubuntu:** [askubuntu.com](https://askubuntu.com)
- **Reddit:** r/ubuntu
- **Komunitas Indonesia:** Ubuntu Indonesia (Telegram/Facebook)

---

## Tips dan Best Practices

### 1. Selalu Update Rutin

Update sistem minimal seminggu sekali:
```bash
sudo apt update && sudo apt upgrade
```

Atau enable automatic updates:
- Buka **Software & Updates**
- Tab **Updates**
- Pilih **Automatically check for updates**

### 2. Buat Snapshot dengan Timeshift

Install Timeshift untuk backup sistem:
```bash
sudo apt install timeshift
```
Buat snapshot sebelum install aplikasi besar atau update mayor.

### 3. Jangan Hapus Package Sistem

Hindari menghapus package yang tidak kamu kenal. Bisa bikin sistem tidak stabil.

### 4. Install Aplikasi dari Sumber Terpercaya

- ✅ Ubuntu Software Center
- ✅ Official repository (`sudo apt install`)
- ✅ Website resmi developer
- ❌ Hindari download dari sumber tidak jelas

### 5. Backup Data Penting

Selalu backup data ke cloud atau external drive. Jangan taruh semua data penting di satu tempat.

### 6. Belajar Command Line Dasar

Command line sangat powerful di Linux. Pelajari dasar-dasar:
```bash
ls          # List files
cd          # Change directory
cp          # Copy
mv          # Move
rm          # Remove
mkdir       # Make directory
cat         # View file
sudo        # Run as admin
```

### 7. Customize Sesuai Kebutuhan

Ubuntu sangat customizable. Install GNOME Tweaks, extensions, themes, icons untuk make it yours!

### 8. Bergabung dengan Komunitas

Bergabung dengan forum atau grup Ubuntu untuk:
- Bertanya jika ada masalah
- Belajar tips dan trik baru
- Berbagi pengalaman

---

## Referensi dan Link Penting

- [Ubuntu Official Website](https://ubuntu.com/) - Website resmi Ubuntu
- [Ubuntu Desktop Download](https://ubuntu.com/download/desktop) - Download Ubuntu Desktop
- [Ubuntu Documentation](https://help.ubuntu.com/) - Dokumentasi lengkap
- [Ubuntu Forum](https://ubuntuforums.org/) - Forum komunitas
- [Ask Ubuntu](https://askubuntu.com/) - Tanya jawab Ubuntu
- [Ubuntu Indonesia](https://ubuntu.id/) - Komunitas Ubuntu Indonesia
- [OMG! Ubuntu!](https://www.omgubuntu.co.uk/) - News dan tips Ubuntu

---

## Kesimpulan

Selamat! Kamu sudah mempelajari cara install Ubuntu Desktop dari awal sampai selesai. Ringkasan langkah:

1. ✅ **Backup data** penting
2. ✅ **Download ISO** dari website resmi
3. ✅ **Buat bootable USB** dengan Rufus/Etcher/Ventoy
4. ✅ **Boot dari USB** via BIOS/UEFI
5. ✅ **Ikuti instalasi** dengan konfigurasi yang sesuai
6. ✅ **Update sistem** setelah install
7. ✅ **Install aplikasi** yang diperlukan
8. ✅ **Customize** desktop sesuai selera

Ubuntu Desktop adalah sistem operasi yang powerful, user-friendly, dan gratis. Dengan panduan ini, diharapkan instalasi berjalan lancar bahkan untuk pemula.

**Selamat menggunakan Ubuntu Desktop!** 🎉🐧

Jika ada masalah, jangan ragu untuk bertanya di forum Ubuntu atau komunitas Linux Indonesia.

> **"Linux is for everyone!"** - Mark Shuttleworth (Founder of Ubuntu)
