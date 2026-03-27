---
title: Install CachyOS
---

# Cara Install CachyOS - Panduan Lengkap untuk Pemula

Panduan lengkap instalasi CachyOS dari awal sampai selesai. Dokumentasi ini dibuat dengan penjelasan detail agar mudah dipahami bahkan oleh orang yang baru pertama kali mencoba Linux.

---

## Apa itu CachyOS?

**CachyOS** adalah sistem operasi berbasis Linux yang dirancang untuk performa maksimal. Ini adalah distribusi Linux yang relatif baru yang berbasis pada **Arch Linux**, salah satu distribusi Linux paling populer.

### Kenapa Memilih CachyOS?

CachyOS menawarkan beberapa keunggulan dibanding distribusi Linux lainnya:

**🚀 Performa Optimal**
- Menggunakan kernel yang sudah dioptimalkan untuk performa
- Package yang dikompilasi dengan optimasi khusus untuk prosesor modern
- Booting lebih cepat dan responsif

**🎯 Mudah Digunakan**
- Installer grafis yang user-friendly
- Sudah termasuk desktop environment yang siap pakai
- Cocok untuk pemula yang ingin mencoba Arch Linux

**📦 Package Terbaru**
- Menggunakan model **rolling release** - selalu dapat versi terbaru
- Tidak perlu upgrade versi besar seperti Windows
- Update rutin setiap hari

**🛡️ Aman**
- Berdasarkan Arch Linux yang terkenal stabil
- Update keamanan cepat
- Komunitas yang aktif

### Apa itu Arch Linux?

**Arch Linux** adalah distribusi Linux yang terkenal dengan:
- **Simplicity** - Sistem yang sederhana dan minimalis
- **Rolling Release** - Selalu update, tidak ada versi "2.0" atau "3.0"
- **Pacman** - Package manager yang cepat dan mudah
- **AUR (Arch User Repository)** - Ribuan package tambahan yang dibuat komunitas

CachyOS membuat Arch Linux lebih mudah diakses dengan menyediakan installer yang mudah dan konfigurasi yang sudah dioptimalkan.

---

## Persiapan Sebelum Install

Sebelum memulai instalasi, pastikan kamu sudah mempersiapkan hal-hal berikut:

### 1. Backup Data Penting ⚠️

**PENTING:** Proses instalasi akan menghapus data di hard drive/SSD. Pastikan kamu sudah:

- ✅ Backup file penting ke external hard drive
- ✅ Backup foto, dokumen, dan data pribadi ke cloud atau storage lain
- ✅ Catat software/aplikasi yang perlu diinstall ulang nanti

> **Kenapa harus backup?**
> Karena instalasi Linux akan memformat hard drive, semua data akan hilang permanen. Backup adalah langkah keamanan untuk menghindari kehilangan data berharga.

### 2. Cek Spesifikasi Minimum

CachyOS membutuhkan spesifikasi hardware berikut:

**Spesifikasi Minimum:**
- **Prosesor:** 64-bit (x86_64) - Intel atau AMD
- **RAM:** 4 GB (rekomendasi 8 GB atau lebih)
- **Storage:** 20 GB space kosong (rekomendasi 40 GB atau lebih)
- **USB Port:** Untuk flashdisk installer

**Spesifikasi Rekomendasi:**
- **Prosesor:** Intel Core i3 / AMD Ryzen 3 atau lebih tinggi
- **RAM:** 8 GB atau lebih
- **Storage:** SSD 120 GB atau lebih (SSD jauh lebih cepat dari HDD)
- **Internet:** Untuk update dan download package tambahan

> **Catatan:** CachyOS tidak support prosesor 32-bit. Jika komputermu sangat lama (sebelum 2010), mungkin tidak kompatibel.

### 3. Siapkan Koneksi Internet

CachyOS membutuhkan koneksi internet saat instalasi untuk:
- Download update terbaru
- Download package tambahan
- Setup sistem yang optimal

**Jenis koneksi yang didukung:**
- ✅ Kabel LAN/Ethernet (direkomendasikan - lebih stabil)
- ✅ WiFi (support sebagian besar adapter WiFi)
- ⚠️ Tethering USB dari HP (bisa digunakan jika tidak ada opsi lain)

### 4. Siapkan Flashdisk

Kamu membutuhkan flashdisk dengan spesifikasi:
- **Kapasitas:** Minimal 4 GB (rekomendasi 8 GB)
- **Kondisi:** Tidak rusak dan bisa ditulis
- **Isi:** Kosongkan atau backup isi flashdisk karena akan diformat

---

## Langkah 1: Download ISO CachyOS

### Apa itu File ISO?

**File ISO** adalah file image disk yang berisi installer lengkap CachyOS. File ini nantinya akan "dibakar" ke flashdisk untuk membuat installer bootable.

### Cara Download

1. **Buka browser** (Chrome, Firefox, Edge, dll)
2. **Kunjungi website resmi:** [cachyos.org/download](https://cachyos.org/download/)
3. **Klik tombol download** untuk versi yang kamu inginkan

### Memilih Versi CachyOS

CachyOS tersedia dalam beberapa versi desktop environment:

| Desktop Environment | Deskripsi | Rekomendasi Untuk |
|--------------------|-----------|-------------------|
| **KDE Plasma** | Tampilan modern, fitur lengkap, customizable | Pengguna Windows yang pindah ke Linux |
| **GNOME** | Tampilan sederhana, fokus pada produktivitas | Pengguna macOS atau yang suka simplicity |
| **XFCE** | Ringan, cepat, stabil | Komputer dengan spesifikasi rendah |
| **Cinnamon** | Mirip Windows, mudah digunakan | Pemula yang ingin familiaritas |
| **MATE** | Klasik, ringan, stabil | Komputer lama atau yang suka tampilan tradisional |

**Rekomendasi untuk pemula:**
- **KDE Plasma** - Paling lengkap fiturnya dan mirip Windows
- **Cinnamon** - Paling mudah untuk transisi dari Windows

### Proses Download

1. **Klik link download** untuk versi yang kamu pilih
2. **Pilih mirror** terdekat (untuk speed lebih cepat)
3. **Tunggu download selesai** (file berukuran 2-4 GB)
4. **Simpan di lokasi yang mudah ditemukan** (misal: Downloads folder)

> **Tips:** Gunakan download manager jika koneksi tidak stabil untuk bisa resume jika terputus.

### Opsi Download yang Tersedia

Saat download CachyOS, kamu akan menemukan beberapa opsi download. Berikut penjelasan lengkapnya:

#### 1. Direct Download

**Apa itu?**
Direct Download adalah link download langsung dari server utama CachyOS atau mirror partner mereka.

**Karakteristik:**
- ✅ **Kecepatan:** Biasanya paling cepat karena langsung dari server
- ✅ **Simpel:** Klik link, download langsung dimulai
- ✅ **Tanpa perantara:** Tidak perlu melalui website pihak ketiga
- ✅ **Kontrol penuh:** Kamu langsung terhubung ke server CachyOS

**Kapan memilih Direct:**
- ✅ Kamu ingin download secepat mungkin
- ✅ Koneksi internet stabil
- ✅ Tidak butuh fitur resume download
- ✅ Server CachyOS tidak diblokir di regionmu

**Cara pakai:**
1. Klik link "Direct" atau nama mirror (misal: "Germany", "USA", "Indonesia")
2. Download akan otomatis dimulai
3. Simpan file ISO

#### 2. SourceForge

**Apa itu?**
**SourceForge** adalah platform hosting file yang sudah lama ada (sejak 1999) dan sering digunakan oleh proyek open source untuk mendistribusikan software mereka.

**Karakteristik:**
- ✅ **Server mirror tersebar** di seluruh dunia - otomatis pilih yang terdekat
- ✅ **Resume support:** Bisa lanjutkan download jika terputus
- ✅ **Statistik download:** Bisa lihat berapa kali file sudah didownload
- ✅ **Reliable:** Server stabil dan jarang down
- ⚠️ **Ada iklan:** Halaman download SourceForge ada iklan (tapi tidak mengganggu)

**Kapan memilih SourceForge:**
- ✅ Koneksi internet tidak stabil (bisa resume)
- ✅ Download sering terputus di tengah
- ✅ Server Direct diblokir atau lambat di regionmu
- ✅ Ingin alternatif jika Direct gagal

**Cara pakai:**
1. Klik link "SourceForge"
2. Kamu akan diarahkan ke halaman SourceForge
3. Download akan otomatis dimulai setelah beberapa detik
4. Jika terputus, buka lagi link dan download akan resume

**Perbandingan Direct vs SourceForge:**

| Aspek | Direct | SourceForge |
|-------|--------|-------------|
| Kecepatan | ⭐⭐⭐⭐⭐ | ⭐⭐⭐⭐ |
| Resume Support | ❌ Tidak | ✅ Ya |
| Iklan | ❌ Tidak | ⚠️ Ada |
| Reliability | ⭐⭐⭐⭐ | ⭐⭐⭐⭐⭐ |
| Alternatif | ❌ Tidak | ✅ Ya |

> **Rekomendasi:** Coba **Direct** dulu untuk kecepatan maksimal. Jika gagal atau sering terputus, gunakan **SourceForge**.

#### 3. Checksum

**Apa itu?**
**Checksum** adalah file yang berisi kode hash (seperti SHA256, SHA512, atau MD5) yang berfungsi sebagai "sidik jari digital" untuk file ISO.

**Fungsi Checksum:**
- ✅ **Verifikasi integritas:** Memastikan file tidak corrupt saat download
- ✅ **Keamanan:** Memastikan file tidak dimodifikasi oleh pihak ketiga
- ✅ **Validasi:** Memastikan file yang kamu download sama persis dengan yang dirilis developer

**Kenapa perlu verifikasi checksum?**
- File ISO berukuran besar (2-4 GB) rentan corrupt saat download
- Gangguan jaringan, server error, atau masalah lain bisa merusak file
- File yang corrupt bisa menyebabkan instalasi gagal atau sistem tidak stabil
- Ada kemungkinan (walau kecil) file dimodifikasi oleh attacker (man-in-the-middle attack)

**Cara Verifikasi Checksum:**

**Di Windows:**
1. Buka PowerShell atau Command Prompt
2. Jalankan perintah:
```powershell
certutil -hashfile C:\Users\NamaKamu\Downloads\cachyos.iso SHA256
```
3. Copy hash yang dihasilkan
4. Buka file checksum dari website CachyOS (biasanya bernama `SHA256SUMS` atau `sha256sum.txt`)
5. Bandingkan hash - harus **SAMA PERSIS**

**Di Linux/macOS:**
1. Buka Terminal
2. Jalankan perintah:
```bash
sha256sum ~/Downloads/cachyos.iso
```
atau
```bash
shasum -a 256 ~/Downloads/cachyos.iso
```
3. Bandingkan dengan file checksum resmi

**Di Hash Checker (GUI Tools):**
- **Windows:** HashTab, 7-Zip (klik kanan → CRC SHA → SHA-256)
- **macOS:** QuickHash, Hash Check
- **Linux:** GtkHash, KHasher

**Apa yang harus dilakukan jika checksum TIDAK cocok?**
- ❌ **JANGAN install** file tersebut!
- ✅ Hapus file ISO yang sudah didownload
- ✅ Download ulang dari sumber resmi
- ✅ Verifikasi lagi setelah download selesai

> **Rekomendasi:** Selalu verifikasi checksum, terutama untuk file besar atau jika download dari mirror tidak resmi. Ini adalah langkah keamanan penting!

#### 4. Signature (GPG/PGP)

**Apa itu?**
**Signature** (tanda tangan digital) adalah file terpisah (biasanya berekstensi `.sig` atau `.asc`) yang ditandatangani oleh developer menggunakan kunci GPG/PGP mereka.

**Fungsi Signature:**
- ✅ **Autentikasi:** Memastikan file benar-benar dari developer resmi
- ✅ **Non-repudiation:** Developer tidak bisa menyangkal bahwa mereka yang merilis file
- ✅ **Integritas:** Memastikan file tidak diubah setelah ditandatangani
- ✅ **Trust chain:** Membangun rantai kepercayaan dari developer ke user

**Perbedaan Checksum vs Signature:**

| Aspek | Checksum | Signature |
|-------|----------|-----------|
| Fungsi | Verifikasi file tidak corrupt | Verifikasi file asli dari developer |
| Keamanan | ⭐⭐⭐ (bisa dipalsukan) | ⭐⭐⭐⭐⭐ (kriptografi asimetris) |
| Kompleksitas | Mudah | Agak teknis |
| Kebutuhan | Tidak butuh kunci | Butuh kunci publik developer |

**Cara Verifikasi Signature:**

**Langkah 1: Download file yang diperlukan**
- File ISO CachyOS
- File signature (`.sig` atau `.asc`)
- Kunci publik GPG developer

**Langkah 2: Import kunci publik developer**
```bash
gpg --import cachyos-public-key.asc
```

**Langkah 3: Verifikasi signature**
```bash
gpg --verify cachyos.iso.sig cachyos.iso
```

**Output yang diharapkan:**
```
gpg: Signature made [tanggal]
gpg:                using RSA key [KEY ID]
gpg: Good signature from "CachyOS Team <email@cachyos.org>" [unknown]
```

**"Good signature"** = File terverifikasi asli dan aman!

**Output yang WAJIB diwaspadai:**
```
gpg: BAD signature from ...
```
❌ **JANGAN GUNAKAN FILE INI!** File sudah dimodifikasi atau bukan dari developer resmi.

**Kapan perlu verifikasi signature?**
- ✅ Untuk keamanan maksimal (production server, enterprise)
- ✅ Jika download dari mirror tidak resmi
- ✅ Jika kamu paranoid tentang keamanan (dalam artian baik!)
- ⚠️ Untuk penggunaan pribadi, checksum biasanya sudah cukup

> **Catatan:** Verifikasi signature lebih teknis dan jarang dilakukan user biasa. Untuk sebagian besar user, **verifikasi checksum sudah cukup**. Tapi jika kamu ingin keamanan maksimal (misal untuk server produksi), verifikasi signature adalah best practice.

### Kesimpulan Opsi Download

| Opsi | Fungsi | Kapan Digunakan |
|------|--------|-----------------|
| **Direct** | Download cepat dari server utama | Download utama, koneksi stabil |
| **SourceForge** | Download alternatif dengan resume | Download cadangan, koneksi tidak stabil |
| **Checksum** | Verifikasi file tidak corrupt | **WAJIB** untuk semua download |
| **Signature** | Verifikasi file asli dari developer | Keamanan maksimal, production |

> **Rekomendasi untuk pemula:**
> 1. Download via **Direct** (atau SourceForge jika gagal)
> 2. Verifikasi **Checksum** untuk memastikan file utuh
> 3. Signature bisa di-skip untuk penggunaan pribadi

---

## Langkah 2: Verifikasi File ISO (Opsional tapi Direkomendasikan)

### Mengapa Verifikasi Penting?

Setelah download, sebaiknya verifikasi file untuk memastikan:
- ✅ File tidak corrupt saat download
- ✅ File asli dari sumber resmi
- ✅ Tidak ada malware atau modifikasi

### Cara Verifikasi di Windows

1. **Buka PowerShell** (klik Start → ketik "PowerShell")
2. **Jalankan perintah:**
```powershell
certutil -hashfile C:\Users\NamaKamu\Downloads\cachyos.iso SHA256
```
3. **Bandingkan hash** dengan yang ada di website CachyOS

### Cara Verifikasi di Linux/macOS

1. **Buka Terminal**
2. **Jalankan perintah:**
```bash
sha256sum ~/Downloads/cachyos.iso
```
3. **Bandingkan hash** dengan yang ada di website

> **Jika hash tidak cocok:** Download ulang file karena file corrupt atau tidak asli.

---

## Langkah 3: Membuat Bootable USB

### Apa itu Bootable USB?

**Bootable USB** adalah flashdisk yang sudah diisi file installer dan bisa digunakan untuk "booting" komputer, mirip seperti CD/DVD installer zaman dulu.

### Pilihan Aplikasi Pembuat Bootable USB

Kamu bisa menggunakan salah satu dari aplikasi berikut:

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
   - **Boot selection:** Klik "SELECT" dan pilih file ISO CachyOS
   - **Partition scheme:** GPT (untuk komputer modern UEFI)
   - **Target system:** UEFI (non CSM)
5. **Klik "START"**
6. **Tunggu proses selesai** (5-10 menit)
7. **Klik "CLOSE"** setelah selesai

> **Peringatan:** Semua data di flashdisk akan dihapus! Backup dulu jika ada data penting.

#### 2. Balena Etcher (Windows, macOS, Linux)

**Website:** [balena.io/etcher](https://www.balena.io/etcher)

**Kelebihan:**
- ✅ Interface sangat sederhana
- ✅ Cross-platform (bisa di Windows, Mac, Linux)
- ✅ Ada verifikasi otomatis
- ✅ Sulit salah pilih disk (lebih aman)

**Cara Menggunakan Balena Etcher:**

1. **Download Balena Etcher** dari [balena.io/etcher](https://www.balena.io/etcher)
2. **Install dan jalankan** Etcher
3. **Klik "Flash from file"** → pilih file ISO CachyOS
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
5. **Copy file ISO CachyOS** ke dalam flashdisk (seperti copy file biasa)
6. **Done!** Flashdisk siap digunakan

> **Kelebihan Ventoy:** Kamu bisa taruh banyak ISO (Windows, Ubuntu, dll) dalam 1 flashdisk dan pilih saat booting!

---

## Langkah 4: Boot dari USB

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

---

## Langkah 5: Memulai Instalasi CachyOS

### Tampilan Awal Boot

Setelah boot dari USB, kamu akan melihat:

1. **Menu GRUB** - Pilih opsi pertama "CachyOS"
2. **Loading screen** - Tunggu sistem loading
3. **Desktop Live** - Kamu akan masuk ke desktop CachyOS tanpa install

> **Apa itu Live Session?**
> Live session adalah mode "coba dulu" di mana kamu bisa mencoba CachyOS tanpa menginstall. Semua perubahan tidak akan tersimpan setelah restart.

### Menjalankan Installer

1. **Klik ikon "Install CachyOS"** di desktop
2. **Installer akan terbuka** dan memandu kamu melalui proses instalasi

---

## Langkah 6: Konfigurasi Instalasi

### 1. Pilih Bahasa

**Langkah:**
- Pilih bahasa yang kamu mengerti
- **Rekomendasi:** English (US) atau Indonesia (jika tersedia)

> **Tips:** Pilih English untuk kemudahan troubleshooting karena sebagian besar tutorial Linux menggunakan bahasa Inggris.

### 2. Pilih Lokasi/Timezone

**Langkah:**
- Klik pada peta atau pilih dari dropdown
- Pilih timezone kamu (misal: Jakarta, Singapore, dll)

**Fungsi:** Mengatur waktu sistem yang benar sesuai lokasimu.

### 3. Pilih Keyboard Layout

**Langkah:**
- Pilih layout keyboard
- **Rekomendasi:** English (US) - default

**Test keyboard:** Ketik di kotak test untuk memastikan keyboard berfungsi normal.

### 4. Partisi Disk (PENTING!)

Ini adalah langkah paling penting. Ada beberapa opsi:

#### Opsi A: Erase Disk (Otomatis) - ⭐ Direkomendasikan untuk Pemula

**Apa yang terjadi:**
- ✅ Seluruh hard drive akan dihapus
- ✅ Installer yang atur partisi otomatis
- ✅ Cocok jika kamu ingin install Linux saja (dual boot tidak)

**Kapan memilih ini:**
- Komputer baru/kosong
- Tidak ada data penting di hard drive
- Ingin install Linux sebagai satu-satunya sistem operasi

> **PERINGATAN:** Semua data di hard drive akan hilang! Pastikan sudah backup!

#### Opsi B: Manual Partitioning - Untuk Advanced User

**Apa yang terjadi:**
- Kamu atur sendiri partisi
- Bisa dual boot dengan Windows
- Lebih fleksibel

**Kapan memilih ini:**
- Ingin dual boot dengan Windows
- Punya kebutuhan partisi khusus
- Sudah berpengalaman dengan Linux

#### Panduan Partisi Manual (Jika Memilih Manual)

Jika memilih manual, buat partisi berikut:

| Partisi | Mount Point | Ukuran | Fungsi |
|---------|-------------|--------|--------|
| **EFI** | /boot/efi | 512 MB - 1 GB | Untuk boot UEFI |
| **Root** | / | 30-50 GB | Untuk sistem operasi dan aplikasi |
| **Home** | /home | Sisa space | Untuk data dan file pribadi |
| **Swap** | swap | 4-8 GB (opsional) | Virtual memory |

**Penjelasan Partisi:**

**1. EFI Partition (/boot/efi)**
- **Fungsi:** Tempat file boot untuk sistem UEFI
- **Ukuran:** 512 MB - 1 GB
- **Format:** FAT32
- **Wajib untuk:** Komputer modern dengan UEFI

**2. Root Partition (/)**
- **Fungsi:** Tempat install sistem operasi dan aplikasi
- **Ukuran:** Minimal 30 GB, rekomendasi 50 GB atau lebih
- **Format:** ext4 atau btrfs
- **Wajib:** Ya, ini partisi utama

**3. Home Partition (/home)**
- **Fungsi:** Tempat menyimpan file pribadi (dokumen, foto, download, dll)
- **Ukuran:** Sisa space hard drive
- **Format:** ext4 atau btrfs
- **Wajib:** Tidak, tapi sangat direkomendasikan

> **Kenapa pisahkan Root dan Home?**
> Jika suatu saat ingin reinstall Linux, data di /home tetap aman karena terpisah dari sistem.

**4. Swap Partition**
- **Fungsi:** Virtual memory (menggunakan storage sebagai RAM tambahan)
- **Ukuran:** 4-8 GB (atau 2x RAM jika RAM kecil)
- **Format:** swap
- **Wajib:** Tidak, tapi berguna untuk hibernasi dan saat RAM penuh

> **Catatan:** Di sistem modern dengan RAM besar (8GB+), swap tidak terlalu diperlukan.

### 5. Buat User Account

**Langkah:**
1. **Masukkan nama lengkap** (misal: John Doe)
2. **Masukkan username** (misal: john) - untuk login
3. **Masukkan password** - buat password yang kuat
4. **Konfirmasi password** - ketik ulang password

**Tips Password:**
- ✅ Minimal 8 karakter
- ✅ Kombinasi huruf besar, huruf kecil, angka, dan simbol
- ✅ Jangan gunakan password yang mudah ditebak
- ✅ Catat password di tempat aman

### 6. Setup SSH (Opsional)

**Apa itu SSH?**
SSH (Secure Shell) adalah protokol untuk mengakses komputer dari jarak jauh secara aman.

**Kapan enable SSH:**
- ✅ Jika ingin remote access dari komputer lain
- ✅ Untuk server
- ⚠️ Untuk PC pribadi, bisa di-skip saja

**Langkah:**
- Centang "Enable SSH" jika butuh
- Biarkan kosong jika tidak butuh

### 7. Review dan Konfirmasi

**Sebelum install:**
- Review semua pengaturan
- Pastikan partisi sudah benar
- Pastikan user sudah dibuat
- Klik "Install" untuk mulai

---

## Langkah 7: Proses Instalasi

### Yang Terjadi Saat Instalasi

Setelah klik "Install", installer akan:

1. **Format partisi** - Menyiapkan hard drive
2. **Install sistem** - Menyalin file sistem ke hard drive
3. **Install bootloader** - GRUB untuk booting
4. **Setup user** - Membuat akun yang kamu buat
5. **Install package dasar** - Sistem dasar yang diperlukan

### Durasi Instalasi

- **SSD:** 10-20 menit
- **HDD:** 20-40 menit

Tergantung kecepatan storage dan spesifikasi komputer.

### Jangan Lakukan Ini Saat Instalasi

❌ **Jangan matikan komputer** - Bisa corrupt sistem
❌ **Jangan cabut USB** - Bisa gagal install
❌ **Jangan restart** - Tunggu hingga selesai

---

## Langkah 8: Restart dan Selesai

### Setelah Instalasi Selesai

1. **Muncul pesan "Installation Complete"**
2. **Klik "Restart"** atau "Reboot"
3. **Lepaskan flashdisk USB** saat komputer mulai restart
4. **Komputer akan boot** ke CachyOS yang baru diinstall

### Bootloader GRUB

Saat boot, kamu akan melihat **GRUB Menu**:
- **CachyOS** - Opsi boot utama
- **Advanced options** - Untuk recovery atau kernel lain

Tekan Enter untuk boot ke CachyOS.

### Login Pertama

1. **Masuk ke login screen**
2. **Pilih user** kamu
3. **Masukkan password**
4. **Welcome to CachyOS!** 🎉

---

## Langkah 9: Setup Awal Setelah Install

### 1. Update Sistem

Setelah install, selalu update sistem untuk mendapatkan package terbaru:

**Cara Update:**

1. **Buka Terminal**
   - Tekan `Ctrl + Alt + T` atau
   - Cari "Terminal" di aplikasi menu

2. **Jalankan perintah update:**
```bash
sudo pacman -Syu
```

**Penjelasan perintah:**
- `sudo` - Jalankan sebagai administrator (root)
- `pacman` - Package manager Arch Linux
- `-S` - Sync package database
- `-y` - Refresh database
- `-u` - Upgrade semua package

3. **Masukkan password** saat diminta
4. **Ketik 'y'** untuk konfirmasi update
5. **Tunggu hingga selesai**

> **Kenapa harus update?**
> Untuk mendapatkan security patch terbaru, bug fixes, dan fitur terbaru.

### 2. Install Driver (Jika Perlu)

CachyOS biasanya sudah include driver yang diperlukan. Tapi untuk hardware tertentu:

**Driver NVIDIA:**
```bash
sudo pacman -S nvidia nvidia-utils
```

**Driver WiFi tertentu:**
```bash
sudo pacman -S linux-firmware
```

### 3. Install Aplikasi Tambahan

**Browser (jika belum ada):**
```bash
sudo pacman -S firefox
# atau
sudo pacman -S google-chrome
```

**Office Suite:**
```bash
sudo pacman -S libreoffice-fresh
```

**Media Player:**
```bash
sudo pacman -S vlc
```

**File Compression:**
```bash
sudo pacman -S p7zip unzip unrar
```

### 4. Setup AUR Helper (Opsional)

**Apa itu AUR?**
AUR (Arch User Repository) adalah repository komunitas dengan ribuan package tambahan.

**Install yay (AUR helper populer):**

1. **Install dependency:**
```bash
sudo pacman -S --needed git base-devel
```

2. **Clone yay:**
```bash
git clone https://aur.archlinux.org/yay.git
cd yay
```

3. **Build dan install:**
```bash
makepkg -si
```

4. **Gunakan yay seperti pacman:**
```bash
yay -S nama-package
```

---

## Troubleshooting - Masalah Umum dan Solusi

### 1. USB Tidak Terdeteksi Saat Boot

**Masalah:** Komputer tidak boot dari USB

**Solusi:**
- ✅ Pastikan USB sudah terpasang dengan benar
- ✅ Coba port USB lain (prefer USB 2.0 jika ada)
- ✅ Cek boot order di BIOS
- ✅ Disable "Secure Boot" di BIOS
- ✅ Pastikan flashdisk dibuat dengan benar (coba buat ulang)

### 2. WiFi Tidak Berfungsi

**Masalah:** WiFi tidak terdeteksi setelah install

**Solusi:**
- ✅ Install firmware tambahan:
```bash
sudo pacman -S linux-firmware
```
- ✅ Restart komputer
- ✅ Gunakan kabel LAN sementara untuk download driver
- ✅ Cek apakah WiFi adapter butuh driver proprietary

### 3. Resolusi Layar Salah

**Masalah:** Resolusi tidak sesuai atau layar kecil

**Solusi:**
- ✅ Update sistem:
```bash
sudo pacman -Syu
```
- ✅ Install driver grafis:
  - **Intel:** `sudo pacman -S mesa vulkan-intel`
  - **AMD:** `sudo pacman -S mesa vulkan-radeon`
  - **NVIDIA:** `sudo pacman -S nvidia nvidia-utils`
- ✅ Restart

### 4. Dual Boot Tidak Muncul di GRUB

**Masalah:** Windows tidak muncul di menu GRUB

**Solusi:**
- ✅ Install os-prober:
```bash
sudo pacman -S os-prober
```
- ✅ Update GRUB:
```bash
sudo grub-mkconfig -o /boot/grub/grub.cfg
```
- ✅ Restart

### 5. Suara Tidak Keluar

**Masalah:** Tidak ada suara

**Solusi:**
- ✅ Cek volume tidak mute
- ✅ Install PulseAudio/PipeWire:
```bash
sudo pacman -S pipewire pipewire-pulse pipewire-alsa
```
- ✅ Restart

### 6. Touchpad Tidak Berfungsi (Laptop)

**Masalah:** Touchpad tidak responsif

**Solusi:**
- ✅ Install driver touchpad:
```bash
sudo pacman -S xf86-input-libinput
```
- ✅ Restart
- ✅ Cek setting touchpad di System Settings

### 7. Secure Boot Mencegah Booting CachyOS

**Masalah:** Saat boot dari USB, muncul pesan error:
- "Signature detected. Check secure boot policy in setup"
- "Secure Boot Violation"
- "Invalid Signature"
- USB tidak mau boot dan langsung skip ke Windows

**Apa itu Secure Boot?**

**Secure Boot** adalah fitur keamanan di UEFI/BIOS yang dirancang untuk mencegah malware dan software tidak terpercaya dari proses booting. Fitur ini bekerja dengan cara:

- ✅ Hanya mengizinkan software yang memiliki "tanda tangan digital" resmi (biasanya dari Microsoft)
- ✅ Mencegah rootkit dan malware level boot
- ✅ Default aktif di sebagian besar laptop/komputer modern (2013-sekarang)

**Kenapa CachyOS Tidak Boot dengan Secure Boot?**

CachyOS (dan sebagian besar distribusi Linux) tidak memiliki sertifikat tanda tangan digital dari Microsoft yang diperlukan oleh Secure Boot. Akibatnya:
- ❌ USB installer ditolak untuk boot
- ❌ Sistem menganggap CachyOS sebagai "untrusted software"
- ❌ Error signature muncul

**Solusi 1: Nonaktifkan Secure Boot (Direkomendasikan)**

Ini adalah solusi paling mudah dan praktis:

**Langkah 1: Masuk BIOS/UEFI**
1. Restart komputer
2. Saat komputer menyala, tekan tombol BIOS berulang-ulang
   - **ASUS:** F2 atau DEL
   - **Acer:** F2 atau DEL
   - **Lenovo:** F1, F2, atau Fn + F2
   - **HP:** F10 atau ESC
   - **Dell:** F2 atau F12
   - **MSI:** DEL
   - **Gigabyte:** F2 atau DEL

**Langkah 2: Cari Pengaturan Secure Boot**
1. Setelah masuk BIOS, cari menu:
   - **"Security"** atau
   - **"Boot"** atau
   - **"Authentication"**
2. Gunakan tombol panah keyboard untuk navigasi (mouse mungkin tidak berfungsi)

**Langkah 3: Nonaktifkan Secure Boot**
1. Pilih opsi **"Secure Boot"**
2. Ubah dari **"Enabled"** menjadi **"Disabled"**
3. Tekan Enter untuk konfirmasi

**Langkah 4: Simpan dan Exit**
1. Tekan **F10** untuk Save & Exit
2. Pilih **"Yes"** untuk konfirmasi
3. Komputer akan restart

**Langkah 5: Boot dari USB**
1. Setelah restart, boot dari USB installer CachyOS
2. Seharusnya tidak ada error lagi

> **Apakah aman menonaktifkan Secure Boot?**
> Ya, untuk penggunaan pribadi aman. Secure Boot adalah lapisan keamanan tambahan, tapi bukan satu-satunya. Selama kamu download software dari sumber terpercaya dan pakai antivirus yang baik, sistem tetap aman.

> **Apakah Secure Boot bisa diaktifkan lagi?**
> Ya, kapan saja! Setelah CachyOS terinstall, kamu bisa aktifkan lagi Secure Boot jika mau. Tapi biasanya CachyOS tetap tidak akan boot kecuali kamu setup key khusus (advanced).

**Solusi 2: Setup Custom Key (Advanced - Tidak Direkomendasikan untuk Pemula)**

Jika kamu ingin tetap menggunakan Secure Boot, ada opsi advanced:

1. **Download key CachyOS** dari website resmi (jika tersedia)
2. **Masuk BIOS/UEFI** → Secure Boot → Key Management
3. **Enroll custom key** - Import key CachyOS
4. **Save dan restart**

> **Catatan:** Proses ini teknis dan tidak semua motherboard support. CachyOS juga mungkin tidak menyediakan key resmi. Untuk pemula, lebih baik disable Secure Boot saja.

**Solusi 3: Gunakan Shim (Jika Support)**

**Shim** adalah bootloader kecil yang ditandatangani Microsoft dan bisa mem-boot Linux dengan Secure Boot aktif. Beberapa distro (seperti Ubuntu, Fedora) support ini.

**Cek apakah CachyOS support Shim:**
- Lihat di website resmi CachyOS
- Cek dokumentasi
- Tanya di forum komunitas

Jika support, install package shim:
```bash
sudo pacman -S shim
```

> **Catatan:** Sampai saat ini, CachyOS belum secara resmi support Secure Boot via Shim. Disable Secure Boot adalah solusi terbaik.

**Video Tutorial:**

Untuk panduan visual cara disable Secure Boot, tonton video ini:
- [Cara Disable Secure Boot di YouTube](https://youtu.be/fhOodF4QfAU?si=6A2N5Cqjdg1fIo1v)

**Kesimpulan:**

| Opsi | Kelebihan | Kekurangan | Rekomendasi |
|------|-----------|------------|-------------|
| **Disable Secure Boot** | Mudah, cepat, praktis | Keamanan sedikit berkurang | ⭐⭐⭐⭐⭐ (Untuk semua user) |
| **Custom Key** | Secure Boot tetap aktif | Teknis, ribet, tidak semua motherboard support | ⭐⭐ (Advanced user saja) |
| **Shim** | Secure Boot tetap aktif | Belum support di CachyOS | ⭐ (Tidak tersedia) |

> **Rekomendasi:** Disable Secure Boot adalah solusi terbaik untuk 99% user CachyOS.

---

## FAQ - Pertanyaan yang Sering Ditanyakan

### Q: Apakah CachyOS gratis?

**A:** Ya, 100% gratis! CachyOS adalah open source dan bisa digunakan tanpa biaya.

### Q: Apakah CachyOS aman untuk pemula?

**A:** Ya! CachyOS didesain untuk membuat Arch Linux lebih mudah digunakan. Installer-nya user-friendly dan sudah dikonfigurasi dengan baik.

### Q: Apa bedanya CachyOS dengan Arch Linux biasa?

**A:**
| CachyOS | Arch Linux |
|---------|------------|
| Installer grafis | Install manual via command line |
| Sudah dioptimalkan | Konfigurasi manual |
| Desktop ready | Minimal install |
| Kernel optimized | Kernel standar |

### Q: Apakah saya bisa dual boot dengan Windows?

**A:** Ya! CachyOS support dual boot. Pilih "Manual Partitioning" saat install dan jangan format partisi Windows.

### Q: Berapa lama umur baterai di laptop?

**A:** Tergantung laptop dan usage. CachyOS cukup efisien. Untuk hemat baterai, install TLP:
```bash
sudo pacman -S tlp tlp-rdw
sudo systemctl enable tlp
```

### Q: Apakah CachyOS support aplikasi Windows (.exe)?

**A:** Tidak native, tapi bisa pakai Wine atau Proton:
```bash
sudo pacman -S wine
```
Atau gunakan Steam dengan Proton untuk gaming.

### Q: Apakah perlu antivirus di Linux?

**A:** Umumnya tidak perlu. Linux lebih aman dari virus. Tapi tetap berhati-hati saat download file dari sumber tidak terpercaya.

### Q: Bagaimana cara backup sistem?

**A:** Gunakan Timeshift:
```bash
sudo pacman -S timeshift
```
Timeshift akan membuat snapshot sistem yang bisa di-restore jika ada masalah.

### Q: Apakah CachyOS cocok untuk gaming?

**A:** Ya! CachyOS bagus untuk gaming karena:
- Kernel optimized untuk performa
- Support Steam dan Proton
- Driver NVIDIA/AMD mudah diinstall

### Q: Apa itu Rolling Release?

**A:** Rolling release berarti sistem selalu update. Tidak ada versi "2.0" atau "3.0". Kamu selalu dapat versi terbaru dengan update rutin.

---

## Tips dan Best Practices

### 1. Selalu Update Rutin

Update sistem minimal seminggu sekali:
```bash
sudo pacman -Syu
```

### 2. Buat Snapshot dengan Timeshift

Install Timeshift untuk backup sistem:
```bash
sudo pacman -S timeshift
```
Buat snapshot sebelum install package besar atau update mayor.

### 3. Jangan Hapus Package Sistem

Hindari menghapus package yang tidak kamu kenal. Bisa bikin sistem tidak stabil.

### 4. Baca Output Command

Saat jalankan command, baca outputnya. Jika ada error, cari solusinya.

### 5. Backup Data Penting

Selalu backup data ke cloud atau external drive. Jangan taruh semua data penting di satu tempat.

### 6. Gunakan AUR dengan Bijak

Package di AUR dibuat komunitas, bukan official. Pilih package yang populer dan well-maintained.

### 7. Dokumentasikan Perubahan

Catat perubahan konfigurasi yang kamu buat. Berguna untuk troubleshooting nanti.

---

## Referensi dan Link Penting

- [CachyOS Official Website](https://cachyos.org/) - Website resmi
- [CachyOS Download](https://cachyos.org/download/) - Download ISO
- [CachyOS Documentation](https://wiki.cachyos.org/) - Dokumentasi lengkap
- [CachyOS Forum](https://forum.cachyos.org/) - Forum komunitas
- [Arch Wiki](https://wiki.archlinux.org/) - Dokumentasi Arch Linux (berlaku untuk CachyOS)
- [AUR (Arch User Repository)](https://aur.archlinux.org/) - Repository komunitas

---

## Kesimpulan

Selamat! Kamu sudah mempelajari cara install CachyOS dari awal sampai selesai. Ringkasan langkah:

1. ✅ **Download ISO** dari website resmi
2. ✅ **Buat bootable USB** dengan Rufus/Etcher/Ventoy
3. ✅ **Boot dari USB** via BIOS/UEFI
4. ✅ **Ikuti instalasi** dengan konfigurasi yang sesuai
5. ✅ **Update sistem** setelah install
6. ✅ **Install aplikasi** yang diperlukan

CachyOS adalah distribusi Linux yang powerful dengan performa optimal. Dengan panduan ini, diharapkan instalasi berjalan lancar bahkan untuk pemula.

**Selamat menggunakan CachyOS!** 🎉

Jika ada masalah, jangan ragu untuk bertanya di forum CachyOS atau komunitas Linux Indonesia.
