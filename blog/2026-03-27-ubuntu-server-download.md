---
title: Download Ubuntu Server
---

## Cara Download Semua Versi Ubuntu Server - Panduan Lengkap

Dokumentasi ini menjelaskan secara detail cara download semua versi Ubuntu Server beserta link download resmi dari Ubuntu. Panduan ini dibuat untuk transfer knowledge agar kamu paham setiap langkah dan istilah yang ada.

---

## Apa itu Ubuntu Server?

**Ubuntu Server** adalah sistem operasi berbasis Linux yang dirancang khusus untuk menjalankan server. Berbeda dengan Ubuntu Desktop yang memiliki tampilan grafis (GUI), Ubuntu Server menggunakan antarmuka command line (CLI) saja. Ini membuat Ubuntu Server lebih ringan dan cocok untuk:

- Web server (menjalankan website)
- Database server (menyimpan dan mengelola database)
- Cloud server (server di cloud seperti AWS, Google Cloud, Azure)
- File server (penyimpanan file jaringan)
- Mail server (server email)
- Dan berbagai kebutuhan server lainnya

---

## Langkah 1: Kunjungi Situs Resmi Ubuntu

Untuk mendownload Ubuntu Server, **selalu gunakan sumber resmi** untuk menghindari file yang sudah dimodifikasi atau mengandung malware.

**Link resmi:** [ubuntu.com/download/server](https://ubuntu.com/download/server)

> **Mengapa harus situs resmi?**
> - File dijamin asli dan aman
> - Mendapatkan versi terbaru
> - Mendapatkan checksum untuk verifikasi file
> - Mendukung pengembangan Ubuntu

---

## Langkah 2: Memahami Versi Ubuntu Server

Ubuntu Server tersedia dalam beberapa versi. Ini bagian penting yang harus kamu pahami sebelum memilih versi mana yang akan didownload.

### Apa itu Versi LTS (Long Term Support)?

**LTS** adalah singkatan dari **Long Term Support**. Ini adalah versi Ubuntu yang mendapatkan dukungan jangka panjang dari Canonical (perusahaan di balik Ubuntu).

**Karakteristik versi LTS:**
- ✅ **Dukungan keamanan selama 5 tahun** - Kamu akan mendapatkan update keamanan dan bug fix selama 5 tahun setelah rilis
- ✅ **Stabil** - Versi LTS sudah melalui testing yang matang
- ✅ **Direkomendasikan untuk produksi** - Cocok untuk server yang akan digunakan di lingkungan produksi
- ✅ **Update fitur minimal** - Fokus pada stabilitas, bukan fitur baru

**Kapan harus memilih LTS?**
- Untuk server produksi di perusahaan
- Untuk server yang tidak ingin sering diupgrade
- Untuk lingkungan yang mengutamakan stabilitas

### Apa itu Versi Interim (Short Term Support)?

Versi **Interim** (atau disebut juga versi non-LTS) adalah versi Ubuntu yang dirilis di antara versi LTS. Versi ini mendapatkan dukungan lebih singkat.

**Karakteristik versi Interim:**
- ⚠️ **Dukungan hanya 9 bulan** - Setelah 9 bulan, kamu harus upgrade ke versi berikutnya
- ⚠️ **Fitur lebih baru** - Mendapatkan fitur dan teknologi terbaru yang belum ada di LTS
- ⚠️ **Cocok untuk testing** - Bagus untuk developer yang ingin mencoba fitur baru
- ⚠️ **Tidak direkomendasikan untuk produksi** - Karena dukungan singkat dan harus sering upgrade

**Kapan harus memilih Interim?**
- Untuk development dan testing
- Untuk belajar fitur-fitur terbaru
- Untuk lingkungan yang tidak kritis

---

## Daftar Lengkap Versi Ubuntu Server

### Versi LTS (Long Term Support) - Direkomendasikan untuk Produksi

| Versi | Nama Kode | Tanggal Rilis | Status | Download Link |
|-------|-----------|---------------|--------|---------------|
| Ubuntu Server 24.04 LTS | Noble Numbat | April 2024 | ✅ Aktif (sampai 2029) | [Download](https://releases.ubuntu.com/noble/) |
| Ubuntu Server 22.04 LTS | Jammy Jellyfish | April 2022 | ✅ Aktif (sampai 2027) | [Download](https://releases.ubuntu.com/jammy/) |
| Ubuntu Server 20.04 LTS | Focal Fossa | April 2020 | ✅ Aktif (sampai 2025) | [Download](https://releases.ubuntu.com/focal/) |
| Ubuntu Server 18.04 LTS | Bionic Beaver | April 2018 | ⚠️ ESM* (sampai 2028) | [Download](https://releases.ubuntu.com/bionic/) |
| Ubuntu Server 16.04 LTS | Xenial Xerus | April 2016 | ❌ End of Life | [Download](https://releases.ubuntu.com/xenial/) |

> **ESM (Extended Security Maintenance):** Dukungan keamanan extended yang memerlukan subscription Ubuntu Pro (gratis untuk personal use hingga 5 mesin)

### Versi Interim (Short Term Support) - Untuk Testing/Development

| Versi | Nama Kode | Tanggal Rilis | Status Support | Download Link |
|-------|-----------|---------------|----------------|---------------|
| Ubuntu Server 24.10 | Oracular Oriole | Oktober 2024 | ✅ Aktif (sampai Juli 2025) | [Download](https://releases.ubuntu.com/oracular/) |
| Ubuntu Server 23.10 | Mantic Minotaur | Oktober 2023 | ❌ End of Life | [Download](https://releases.ubuntu.com/mantic/) |
| Ubuntu Server 23.04 | Lunar Lobster | April 2023 | ❌ End of Life | [Download](https://releases.ubuntu.com/lunar/) |
| Ubuntu Server 22.10 | Kinetic Kudu | Oktober 2022 | ❌ End of Life | [Download](https://releases.ubuntu.com/kinetic/) |
| Ubuntu Server 21.10 | Impish Indri | Oktober 2021 | ❌ End of Life | [Download](https://releases.ubuntu.com/impish/) |
| Ubuntu Server 21.04 | Hirsute Hippo | April 2021 | ❌ End of Life | [Download](https://releases.ubuntu.com/hirsute/) |
| Ubuntu Server 20.10 | Groovy Gorilla | Oktober 2020 | ❌ End of Life | [Download](https://releases.ubuntu.com/groovy/) |
| Ubuntu Server 19.10 | Eoan Ermine | Oktober 2019 | ❌ End of Life | [Download](https://releases.ubuntu.com/eoan/) |

> **Catatan:** Versi interim yang sudah End of Life tidak lagi mendapatkan update keamanan. Jangan gunakan untuk produksi!

---

## Langkah 3: Memahami Tipe File Download

Setiap versi Ubuntu Server tersedia dalam beberapa format file. Berikut penjelasannya:

### 1. ISO Image (Live Server Installer)

**Apa itu?** File `.iso` adalah image disk yang berisi installer Ubuntu Server lengkap.

**Untuk apa?** Digunakan untuk:
- Instalasi manual di komputer/server fisik
- Instalasi di virtual machine (VirtualBox, VMware, Proxmox, dll)
- Membuat bootable USB

**Kapan memilih ini?** 
- ✅ Kamu ingin install Ubuntu Server di komputer/server lokal
- ✅ Kamu ingin install di virtual machine untuk testing
- ✅ Kamu pemula yang baru belajar Ubuntu Server

### 2. Cloud Images

**Apa itu?** Image Ubuntu Server yang sudah dioptimalkan untuk platform cloud.

**Untuk apa?** Digunakan untuk deploy server virtual di:
- Amazon Web Services (AWS) EC2
- Microsoft Azure
- Google Cloud Platform (GCP)
- OpenStack
- LXD containers

**Format yang tersedia:**
- `QCOW2` - Untuk KVM/QEMU dan OpenStack
- `IMG` - Raw disk image
- `VHDX` - Untuk Microsoft Hyper-V
- `VMDK` - Untuk VMware

**Kapan memilih ini?**
- ✅ Kamu deploy server di cloud (AWS, Azure, GCP)
- ✅ Kamu menggunakan virtualisasi enterprise
- ✅ Kamu butuh image yang sudah pre-configured untuk cloud

### 3. Netboot Images

**Apa itu?** Image booting kecil (sekitar 50-100 MB) yang mendownload paket instalasi dari internet saat instalasi.

**Untuk apa?** Digunakan untuk:
- Instalasi via network/PXE boot
- Instalasi massal di banyak server sekaligus
- Datacenter dengan infrastruktur network boot

**Kapan memilih ini?**
- ✅ Kamu admin IT yang install Ubuntu di banyak server
- ✅ Kamu punya infrastruktur PXE boot
- ✅ Kamu ingin custom instalasi minimal

---

## Langkah 4: Memilih Arsitektur Prosesor

Setelah memilih versi, kamu akan melihat beberapa pilihan arsitektur. Ini penting karena harus sesuai dengan prosesor komputermu.

### AMD64 (x86_64) - Paling Umum

**Apa itu?** Arsitektur 64-bit untuk prosesor Intel dan AMD.

**Untuk prosesor:**
- Intel Core i3, i5, i7, i9
- Intel Xeon
- AMD Ryzen
- AMD EPYC

**Kapan memilih ini?**
- ✅ Hampir semua komputer/laptop modern (2010-sekarang)
- ✅ Server dengan prosesor Intel/AMD
- ✅ Virtual machine di VirtualBox/VMware

**Nama file:** `ubuntu-XX.XX-live-server-amd64.iso`

### ARM64 (AArch64)

**Apa itu?** Arsitektur 64-bit untuk prosesor ARM.

**Untuk prosesor:**
- Raspberry Pi 3/4/5 (model 64-bit)
- Apple Silicon (M1, M2, M3) - di VM
- AWS Graviton
- NVIDIA Jetson
- Board development ARM lainnya

**Kapan memilih ini?**
- ✅ Kamu menggunakan Raspberry Pi
- ✅ Kamu deploy di AWS Graviton
- ✅ Kamu menggunakan Mac M1/M2/M3 untuk development

**Nama file:** `ubuntu-XX.XX-live-server-arm64.iso`

### I386 (32-bit) - Sudah Tidak Didukung

**Catatan:** Ubuntu Server sudah tidak mendukung arsitektur 32-bit sejak Ubuntu 18.04. Jika kamu punya hardware lama 32-bit, pertimbangkan menggunakan:
- Ubuntu 18.04 (versi terakhir yang support 32-bit)
- Distribusi lain seperti Debian

---

## Langkah 5: Download File ISO

Berikut langkah-langkah download:

1. **Klik link download** pada tabel versi di atas
2. **Scroll ke bagian "Server"** atau cari file dengan nama `live-server`
3. **Pilih arsitektur** yang sesuai (biasanya `amd64`)
4. **Klik file ISO** untuk mulai download
5. **Tunggu hingga selesai** (file berukuran 2-3 GB)

### Contoh Nama File

```
ubuntu-24.04-live-server-amd64.iso
ubuntu-22.04-live-server-amd64.iso
ubuntu-24.04-live-server-arm64.iso
```

**Penjelasan nama file:**
- `ubuntu` = Nama sistem operasi
- `24.04` = Versi Ubuntu (tahun.bulan rilis)
- `live-server` = Tipe installer (live server installer)
- `amd64` = Arsitektur prosesor
- `.iso` = Extension file image disk

### Opsi Download yang Tersedia

Saat download Ubuntu Server, kamu akan menemukan beberapa opsi download. Berikut penjelasan lengkapnya:

#### 1. Direct Download (Torrent/HTTP)

**Apa itu?**
Direct Download adalah link download langsung dari server resmi Ubuntu (`releases.ubuntu.com`).

**Karakteristik:**
- ✅ **Kecepatan:** Cepat jika server Ubuntu tidak overload
- ✅ **Simpel:** Klik link, download langsung dimulai
- ✅ **Tanpa perantara:** Langsung dari server Canonical/Ubuntu
- ✅ **Resmi:** Sumber paling terpercaya
- ⚠️ **Server overload:** Bisa lambat saat rilis versi baru (banyak yang download)

**Kapan memilih Direct:**
- ✅ Kamu ingin download dari sumber resmi langsung
- ✅ Koneksi internet stabil
- ✅ Server Ubuntu tidak sedang overload
- ✅ File yang kamu cari ada di server utama

**Cara pakai:**
1. Buka halaman release (misal: `releases.ubuntu.com/noble/`)
2. Klik file ISO yang kamu inginkan
3. Download akan otomatis dimulai
4. Simpan file ISO

#### 2. Torrent Download

**Apa itu?**
**Torrent** adalah metode download peer-to-peer (P2P) di mana file didownload dari banyak user (seeder) sekaligus, bukan dari satu server.

**Karakteristik:**
- ✅ **Kecepatan tinggi:** Bisa lebih cepat dari HTTP jika banyak seeder
- ✅ **Tidak membebani server:** Download dari user lain, bukan server Ubuntu
- ✅ **Resume support:** Bisa pause dan lanjut download kapan saja
- ✅ **Stabil:** Tidak terpengaruh server overload
- ⚠️ **Butuh client torrent:** Perlu install software torrent (qBittorrent, Transmission, dll)
- ⚠️ **Tergantung seeder:** Jika sedikit seeder, download bisa lambat

**Kapan memilih Torrent:**
- ✅ Server Ubuntu sedang overload (saat rilis versi baru)
- ✅ Download versi lama yang sudah jarang di server
- ✅ Koneksi internet tidak stabil (bisa resume)
- ✅ Kamu sudah punya torrent client

**Cara pakai:**
1. Download file `.torrent` dari halaman release Ubuntu
2. Buka file `.torrent` dengan torrent client
3. Pilih lokasi save file ISO
4. Tunggu download selesai

**Rekomendasi Torrent Client:**
- **Windows:** qBittorrent (gratis, open source, no ads)
- **macOS:** Transmission (gratis, ringan)
- **Linux:** qBittorrent, Transmission, Deluge

#### 3. Mirror Server

**Apa itu?**
**Mirror** adalah server replika yang menyimpan copy file Ubuntu di berbagai lokasi geografis. Ubuntu punya ratusan mirror di seluruh dunia.

**Karakteristik:**
- ✅ **Lokasi terdekat:** Pilih mirror di negaramu untuk speed lebih cepat
- ✅ **Load balancing:** Mengurangi beban server utama Ubuntu
- ✅ **Alternatif:** Jika server utama down atau lambat
- ⚠️ **Kualitas bervariasi:** Mirror dikelola pihak ketiga, kecepatan berbeda-beda

**Kapan memilih Mirror:**
- ✅ Server utama Ubuntu lambat dari lokasimu
- ✅ Ingin support mirror lokal (negara sendiri)
- ✅ Server utama down atau maintenance
- ✅ Download ukuran besar (butuh speed maksimal)

**Daftar Mirror Populer:**
- **Indonesia:** `kartolo.sby.datautama.net.id` (Surabaya), `mirror.telkomnet.id.id` (Jakarta)
- **Singapore:** `mirror.nus.edu.sg` (National University of Singapore)
- **Malaysia:** `mirror.seas.upenn.edu.my`
- **Thailand:** `mirror.kku.ac.th` (Khon Kaen University)
- **Australia:** `mirror.aarnet.edu.au` (AARNet)

**Cara pakai Mirror:**
1. Buka halaman mirror (misal: `mirror.nus.edu.sg/ubuntu-releases/`)
2. Navigasi ke versi yang kamu cari (misal: `noble/`)
3. Download file ISO seperti biasa

#### 4. Checksum

**Apa itu?**
**Checksum** adalah file yang berisi kode hash (SHA256, SHA512, MD5) yang berfungsi sebagai "sidik jari digital" untuk file ISO.

**Fungsi Checksum:**
- ✅ **Verifikasi integritas:** Memastikan file tidak corrupt saat download
- ✅ **Keamanan:** Memastikan file tidak dimodifikasi oleh pihak ketiga
- ✅ **Validasi:** Memastikan file yang kamu download sama persis dengan yang dirilis Canonical

**Kenapa perlu verifikasi checksum?**
- File ISO berukuran besar (2-5 GB) rentan corrupt saat download
- Gangguan jaringan, server error, atau masalah lain bisa merusak file
- File yang corrupt bisa menyebabkan instalasi gagal atau sistem tidak stabil
- Ada kemungkinan (walau kecil) file dimodifikasi oleh attacker (man-in-the-middle attack)

**File Checksum Ubuntu:**
Ubuntu menyediakan beberapa file checksum:
- `SHA256SUMS` - Hash SHA256 (direkomendasikan)
- `SHA512SUMS` - Hash SHA512 (lebih aman)
- `MD5SUMS` - Hash MD5 (sudah deprecated, tidak direkomendasikan)

**Cara Verifikasi Checksum:**

**Di Windows:**
1. Buka PowerShell atau Command Prompt
2. Jalankan perintah:
```powershell
certutil -hashfile C:\Users\NamaKamu\Downloads\ubuntu-24.04-live-server-amd64.iso SHA256
```
3. Copy hash yang dihasilkan
4. Buka file `SHA256SUMS` dari halaman download Ubuntu
5. Bandingkan hash - harus **SAMA PERSIS**

**Di Linux/macOS:**
1. Buka Terminal
2. Jalankan perintah:
```bash
sha256sum ~/Downloads/ubuntu-24.04-live-server-amd64.iso
```
atau
```bash
shasum -a 256 ~/Downloads/ubuntu-24.04-live-server-amd64.iso
```
3. Bandingkan dengan file `SHA256SUMS` resmi

**Di Hash Checker (GUI Tools):**
- **Windows:** HashTab (klik kanan file → Properties → File Hashes), 7-Zip (klik kanan → CRC SHA → SHA-256)
- **macOS:** QuickHash, Hash Check
- **Linux:** GtkHash, KHasher, `nautilus-hash-checker` (extension untuk Nautilus)

**Apa yang harus dilakukan jika checksum TIDAK cocok?**
- ❌ **JANGAN install** file tersebut!
- ✅ Hapus file ISO yang sudah didownload
- ✅ Download ulang dari sumber resmi
- ✅ Verifikasi lagi setelah download selesai

> **Rekomendasi:** Selalu verifikasi checksum, terutama untuk file besar atau jika download dari mirror tidak resmi. Ini adalah langkah keamanan penting!

#### 5. Signature (GPG)

**Apa itu?**
**Signature** (tanda tangan digital) adalah file terpisah (`.gpg`) yang ditandatangani oleh developer Ubuntu menggunakan kunci GPG mereka.

**Fungsi Signature:**
- ✅ **Autentikasi:** Memastikan file benar-benar dari Canonical/Ubuntu resmi
- ✅ **Non-repudiation:** Canonical tidak bisa menyangkal bahwa mereka yang merilis file
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
- File ISO Ubuntu Server
- File signature (`.gpg`)
- Kunci publik GPG Ubuntu

**Langkah 2: Import kunci publik Ubuntu**
```bash
gpg --recv-keys 0x46181433FBB75451 0xD56571B88A8BACF3
```
Atau download dari keyserver:
```bash
gpg --keyserver keyserver.ubuntu.com --recv-keys 0x46181433FBB75451
```

**Langkah 3: Download file signature**
```bash
wget https://releases.ubuntu.com/noble/SHA256SUMS.gpg
```

**Langkah 4: Verifikasi signature**
```bash
gpg --verify SHA256SUMS.gpg SHA256SUMS
```

**Output yang diharapkan:**
```
gpg: Signature made [tanggal]
gpg:                using RSA key [KEY ID]
gpg: Good signature from "Ubuntu CD Image Automatic Signing Key <cdimage@ubuntu.com>" [unknown]
```

**"Good signature"** = File terverifikasi asli dan aman!

**Output yang WAJIB diwaspadai:**
```
gpg: BAD signature from ...
```
❌ **JANGAN GUNAKAN FILE INI!** File sudah dimodifikasi atau bukan dari Canonical.

**Kapan perlu verifikasi signature?**
- ✅ Untuk keamanan maksimal (production server, enterprise)
- ✅ Jika download dari mirror tidak resmi
- ✅ Untuk compliance/audit requirement
- ⚠️ Untuk penggunaan pribadi/lab, checksum biasanya sudah cukup

> **Catatan:** Verifikasi signature lebih teknis dan jarang dilakukan user biasa. Untuk sebagian besar user, **verifikasi checksum sudah cukup**. Tapi jika kamu ingin keamanan maksimal (misal untuk server produksi), verifikasi signature adalah best practice.

### Kesimpulan Opsi Download

| Opsi | Fungsi | Kapan Digunakan |
|------|--------|-----------------|
| **Direct (HTTP)** | Download dari server utama Ubuntu | Download utama, server tidak overload |
| **Torrent** | Download P2P dari user lain | Server overload, butuh resume, download besar |
| **Mirror** | Download dari server lokal | Speed lebih cepat, support lokal |
| **Checksum** | Verifikasi file tidak corrupt | **WAJIB** untuk semua download |
| **Signature** | Verifikasi file asli dari Canonical | Keamanan maksimal, production, compliance |

> **Rekomendasi untuk pemula:**
> 1. Download via **Direct** atau **Torrent** (jika server lambat)
> 2. Gunakan **Mirror lokal** jika tersedia di negaramu
> 3. Verifikasi **Checksum** untuk memastikan file utuh
> 4. Signature bisa di-skip untuk penggunaan pribadi/lab

---

## Langkah 6: Verifikasi File Download (PENTING!)

**Mengapa perlu verifikasi?**
Setelah download file ISO, sangat penting untuk memverifikasi bahwa file yang kamu download:
- ✅ **Asli** - Bukan file palsu yang dimodifikasi
- ✅ **Utuh** - Tidak corrupt saat download
- ✅ **Aman** - Tidak mengandung malware

### Cara Verifikasi dengan SHA256 Checksum

**Apa itu SHA256 Checksum?**
SHA256 adalah hash unik yang dihasilkan dari file. Jika file berubah sedikit saja (bahkan 1 bit), hash akan berubah total. Ini seperti "sidik jari" digital untuk file.

**Langkah verifikasi di Windows:**

1. Buka PowerShell atau Command Prompt
2. Jalankan perintah:
```powershell
certutil -hashfile ubuntu-24.04-live-server-amd64.iso SHA256
```

**Langkah verifikasi di macOS/Linux:**

1. Buka Terminal
2. Jalankan perintah:
```bash
sha256sum ubuntu-24.04-live-server-amd64.iso
```

**Setelah dapat hash:**
1. Buka halaman download Ubuntu
2. Cari file `SHA256SUMS`
3. Bandingkan hash yang kamu dapat dengan hash di file SHA256SUMS
4. ✅ **Jika SAMA** = File asli dan aman
5. ❌ **Jika BEDA** = File corrupt atau palsu, download ulang!

### Contoh Output Verifikasi

```bash
$ sha256sum ubuntu-24.04-live-server-amd64.iso
a1b2c3d4e5f6...  ubuntu-24.04-live-server-amd64.iso
```

Bandingkan dengan isi file `SHA256SUMS`:
```
a1b2c3d4e5f6...  ubuntu-24.04-live-server-amd64.iso
```

---

## Langkah 7: Membuat Bootable USB

Setelah download dan verifikasi, langkah selanjutnya adalah membuat bootable USB. Ini diperlukan untuk menginstall Ubuntu Server ke komputer/server.

### Apa itu Bootable USB?

**Bootable USB** adalah flashdisk yang berisi file installer Ubuntu Server dan bisa digunakan untuk booting komputer. Mirip seperti CD/DVD installer zaman dulu, tapi menggunakan flashdisk.

### Pilihan Aplikasi Pembuat Bootable USB

#### 1. Rufus (Windows) - ⭐ Direkomendasikan

**Website:** [rufus.ie](https://rufus.ie)

**Kelebihan:**
- ✅ Gratis dan open source
- ✅ Cepat dan ringan
- ✅ Support banyak format
- ✅ Bisa bypass requirement Windows 11 (bonus)

**Cara pakai:**
1. Download dan jalankan Rufus
2. Pilih flashdisk di "Device"
3. Klik "SELECT" dan pilih file ISO Ubuntu
4. Klik "START"
5. Tunggu hingga selesai

#### 2. Balena Etcher (Windows, macOS, Linux)

**Website:** [balena.io/etcher](https://www.balena.io/etcher)

**Kelebihan:**
- ✅ Interface sangat sederhana
- ✅ Cross-platform (bisa di Windows, Mac, Linux)
- ✅ Ada verifikasi otomatis setelah write
- ✅ Aman (sulit salah pilih disk)

**Cara pakai:**
1. Download dan install Balena Etcher
2. Klik "Flash from file" → pilih ISO Ubuntu
3. Klik "Select target" → pilih flashdisk
4. Klik "Flash!"
5. Tunggu hingga selesai

#### 3. Ventoy (Windows, Linux) - ⭐ Paling Fleksibel

**Website:** [ventoy.net](https://www.ventoy.net)

**Kelebihan:**
- ✅ Bisa taruh MULTIPLE ISO dalam 1 flashdisk
- ✅ Tidak perlu format ulang setiap ganti ISO
- ✅ Cukup copy-paste file ISO ke flashdisk
- ✅ Support banyak distribusi Linux

**Cara pakai:**
1. Download dan install Ventoy ke flashdisk
2. Setelah selesai, flashdisk akan muncul di file explorer
3. Copy file ISO Ubuntu ke dalam flashdisk
4. Selesai! Boot dari flashdisk dan pilih ISO yang mau dipakai

---

## Langkah 8: Boot dari USB dan Install

Setelah punya bootable USB, saatnya install Ubuntu Server:

### 1. Masukkan USB ke Server/Komputer

Colokkan flashdisk bootable ke port USB server atau komputer yang akan diinstall.

### 2. Masuk ke BIOS/UEFI

**Apa itu BIOS/UEFI?**
BIOS/UEFI adalah firmware yang mengontrol hardware komputer sebelum sistem operasi berjalan. Di sini kamu bisa mengatur urutan booting.

**Cara masuk BIOS/UEFI:**
1. Restart komputer
2. Saat komputer menyala, tekan tombol BIOS berulang-ulang
3. Tombol BIOS biasanya: **F2**, **DEL**, **F10**, **F12**, atau **ESC**
4. Tergantung merk motherboard/laptop:
   - **ASUS** = F2 atau DEL
   - **MSI** = DEL
   - **Gigabyte** = F2 atau DEL
   - **Dell** = F2 atau F12
   - **HP** = F10 atau ESC
   - **Lenovo** = F1 atau F2

### 3. Ubah Boot Order

Setelah masuk BIOS:
1. Cari menu **"Boot"** atau **"Boot Order"**
2. Pindahkan **USB** ke posisi paling atas (prioritas pertama)
3. Simpan pengaturan (biasanya tekan **F10**)
4. Komputer akan restart

### 4. Mulai Instalasi

Setelah boot dari USB:
1. Kamu akan melihat menu GRUB Ubuntu
2. Pilih **"Try or Install Ubuntu Server"**
3. Installer akan mulai loading
4. Ikuti langkah-langkah instalasi yang muncul

### 5. Langkah-Langkah Instalasi

Installer akan memandu kamu melalui:

**a. Pemilihan Bahasa**
- Pilih bahasa yang kamu mengerti (English direkomendasikan)

**b. Konfigurasi Keyboard**
- Pilih layout keyboard (biasanya "English (US)" atau "English (UK)")

**c. Konfigurasi Jaringan**
- Setup IP address (DHCP otomatis atau static IP)
- Setup hostname (nama server)
- Setup proxy (jika perlu)

**d. Partisi Disk**
- **Guided (Otomatis)** - Installer yang atur partisi untukmu
- **Custom (Manual)** - Kamu atur sendiri partisi

**e. Setup User**
- Buat username untuk login
- Buat password
- Setup SSH key (opsional tapi direkomendasikan)

**f. Setup SSH**
- Centang "Install OpenSSH Server" untuk remote access
- Ini penting untuk server agar bisa diakses dari jarak jauh

**g. Install Packages Tambahan (Opsional)**
- Web server (Apache, Nginx)
- Database (MySQL, PostgreSQL)
- Dan lainnya

**h. Konfirmasi dan Install**
- Review semua pengaturan
- Klik "Install" untuk mulai instalasi
- Tunggu hingga selesai (10-30 menit tergantung hardware)

**i. Restart**
- Setelah instalasi selesai, pilih "Reboot"
- Lepaskan flashdisk USB
- Server akan boot ke Ubuntu Server yang baru diinstall

---

## Tips Memilih Versi Ubuntu Server

### Untuk Server Produksi (Perusahaan/Production)

**Rekomendasi:** Ubuntu Server 24.04 LTS atau 22.04 LTS

**Alasan:**
- ✅ Dukungan 5 tahun (sampai 2029/2027)
- ✅ Sudah stabil dan teruji
- ✅ Tidak perlu sering upgrade
- ✅ Cocok untuk server kritis yang harus uptime 24/7

### Untuk Belajar/Home Lab

**Rekomendasi:** Ubuntu Server 24.04 LTS

**Alasan:**
- ✅ Versi terbaru dengan dukungan panjang
- ✅ Bisa belajar fitur terbaru
- ✅ Tidak perlu upgrade dalam waktu lama
- ✅ Komunitas besar, mudah cari tutorial

### Untuk Development/Testing

**Rekomendasi:** Ubuntu Server 24.10 (Interim)

**Alasan:**
- ✅ Fitur dan package terbaru
- ✅ Cocok untuk test kompatibilitas aplikasi
- ✅ Bisa evaluasi fitur baru sebelum masuk LTS berikutnya

### Untuk Hardware Lama

**Rekomendasi:** Ubuntu Server 22.04 LTS atau 20.04 LTS

**Alasan:**
- ✅ Lebih ringan dari versi terbaru
- ✅ Masih dapat update keamanan
- ✅ Kompatibel dengan hardware lama

---

## FAQ - Pertanyaan yang Sering Ditanyakan

### Q: Apakah Ubuntu Server gratis?

**A:** Ya, 100% gratis! Ubuntu Server adalah open source dan bisa didownload, digunakan, dan didistribusikan secara gratis.

### Q: Apakah saya perlu lisensi untuk Ubuntu Server?

**A:** Tidak perlu lisensi untuk penggunaan dasar. Namun, jika kamu butuh support enterprise, ada Ubuntu Pro (gratis untuk personal use hingga 5 mesin).

### Q: Berapa ukuran file ISO Ubuntu Server?

**A:** Sekitar 2-3 GB untuk versi terbaru. Pastikan kamu punya koneksi internet yang cukup cepat dan stabil.

### Q: Berapa RAM minimal untuk Ubuntu Server?

**A:** 
- **Minimal:** 512 MB RAM
- **Rekomendasi:** 2 GB RAM atau lebih
- **Untuk produksi:** 4 GB RAM atau lebih tergantung workload

### Q: Berapa storage minimal untuk Ubuntu Server?

**A:**
- **Minimal:** 5 GB
- **Rekomendasi:** 25 GB atau lebih
- **Untuk produksi:** 50 GB atau lebih tergantung kebutuhan

### Q: Apakah Ubuntu Server punya tampilan grafis (GUI)?

**A:** Tidak, Ubuntu Server default-nya command line (CLI) saja. Tapi kamu bisa install desktop environment jika butuh GUI (tidak direkomendasikan untuk server produksi).

### Q: Apa bedanya Ubuntu Server dan Ubuntu Desktop?

**A:**
| Ubuntu Server | Ubuntu Desktop |
|---------------|----------------|
| Tanpa GUI (CLI only) | Ada tampilan grafis |
| Lebih ringan | Lebih berat |
| Untuk server | Untuk PC/laptop |
| Package minimal | Package lengkap |

### Q: Bisakah upgrade dari versi LTS ke LTS berikutnya?

**A:** Ya, Ubuntu mendukung upgrade langsung dari satu LTS ke LTS berikutnya. Contoh: 22.04 LTS → 24.04 LTS.

### Q: Apa itu SSH dan kenapa harus diinstall?

**A:** SSH (Secure Shell) adalah protokol untuk mengakses server dari jarak jauh secara aman. Dengan SSH, kamu bisa manage server tanpa perlu monitor/keyboard fisik.

### Q: Kenapa download saya sangat lambat?

**A:** Beberapa kemungkinan:
- Server Ubuntu sedang overload (terutama saat rilis versi baru)
- Mirror yang kamu pilih jauh dari lokasimu
- Koneksi internet kamu sedang bermasalah

**Solusi:**
- Gunakan **Torrent** untuk download lebih cepat
- Pilih **Mirror lokal** di negaramu
- Download di jam sepi (malam/pagi)

### Q: Apakah saya bisa install Ubuntu Server di Raspberry Pi?

**A:** Ya! Ubuntu Server support Raspberry Pi. Download versi **ARM64** (`arm64.iso`) untuk Raspberry Pi 3/4/5.

### Q: Apakah Ubuntu Server bisa dual boot dengan Windows?

**A:** Ya, bisa! Tapi butuh konfigurasi manual saat partisi. Pastikan backup data Windows dulu dan pelajari cara partisi dual boot.

### Q: Berapa lama dukungan Ubuntu Server LTS?

**A:** Versi LTS mendapatkan dukungan keamanan dan update selama **5 tahun** dari tanggal rilis. Contoh: 24.04 LTS didukung sampai April 2029.

### Q: Apakah Ubuntu Server bisa dijadikan desktop?

**A:** Bisa! Install desktop environment seperti GNOME atau XFCE:
```bash
sudo apt install ubuntu-desktop  # GNOME
sudo apt install xubuntu-desktop  # XFCE
```
Tapi tidak direkomendasikan untuk server produksi.

### Q: Apa itu Ubuntu Pro?

**A:** **Ubuntu Pro** adalah subscription gratis (untuk personal use hingga 5 mesin) yang memberikan:
- Extended Security Maintenance (ESM) sampai 10 tahun
- Security coverage untuk 30,000+ package tambahan
- Compliance untuk enterprise (FIPS, HIPAA, etc.)
- Livepatch (update kernel tanpa reboot)

---

## Troubleshooting - Masalah Umum dan Solusi

### 1. Download Sangat Lambat atau Gagal

**Masalah:** Download ISO sangat lambat, sering terputus, atau gagal di tengah.

**Solusi:**

**Opsi A: Gunakan Torrent**
1. Download file `.torrent` dari halaman release Ubuntu
2. Install torrent client (qBittorrent untuk Windows, Transmission untuk Mac/Linux)
3. Buka file `.torrent` di client
4. Download akan lebih cepat dan bisa di-resume jika terputus

**Opsi B: Gunakan Mirror Lokal**
1. Cari mirror Ubuntu di negaramu
2. Untuk Indonesia:
   - `kartolo.sby.datautama.net.id` (Surabaya)
   - `mirror.telkomnet.id.id` (Jakarta)
3. Download dari mirror tersebut

**Opsi C: Gunakan Download Manager**
- **Windows:** Internet Download Manager (IDM), Free Download Manager (FDM)
- **macOS:** Folx, Downie
- **Linux:** uGet, XDM

Download manager bisa:
- Resume download jika terputus
- Split file jadi beberapa bagian untuk speed lebih cepat
- Schedule download di jam tertentu

### 2. Checksum Tidak Cocok

**Masalah:** Setelah verifikasi, hash checksum tidak sama dengan yang di website Ubuntu.

**Kemungkinan Penyebab:**
- File corrupt saat download (download tidak sempurna)
- File dimodifikasi (jarang, tapi bisa terjadi)
- Error saat menulis hash (salah copy)

**Solusi:**
1. ✅ **Download ulang** file ISO dari sumber resmi
2. ✅ Pastikan download selesai 100% sebelum verifikasi
3. ✅ Copy hash dari file `SHA256SUMS` dengan teliti
4. ✅ Gunakan command yang benar untuk verifikasi
5. ✅ Jika masih tidak cocok setelah beberapa kali, coba download dari mirror lain

> **PENTING:** Jangan install file yang checksum-nya tidak cocok! Bisa corrupt atau mengandung malware.

### 3. USB Tidak Terbaca Saat Boot

**Masalah:** Komputer tidak boot dari USB installer, langsung ke Windows/hard drive.

**Solusi:**

**Cek BIOS/UEFI:**
1. Restart komputer dan masuk BIOS (tekan F2/DEL/F10 saat boot)
2. Cari menu **Boot** atau **Boot Order**
3. Pindahkan **USB** ke posisi paling atas
4. Save dan Exit (biasanya F10)

**Disable Secure Boot:**
1. Masuk BIOS → menu **Security** atau **Boot**
2. Cari opsi **Secure Boot**
3. Ubah dari **Enabled** ke **Disabled**
4. Save dan Exit

**Coba Port USB Lain:**
- Gunakan port **USB 2.0** (biasanya warna hitam, bukan biru)
- Hindari USB hub, colok langsung ke motherboard
- Coba port USB belakang (langsung ke motherboard, bukan front panel)

**Buat Ulang Bootable USB:**
1. Coba aplikasi lain (jika pakai Rufus, coba Etcher atau Ventoy)
2. Gunakan flashdisk berbeda
3. Pastikan file ISO tidak corrupt (verifikasi checksum dulu)

### 4. Secure Boot Mencegah Booting Ubuntu

**Masalah:** Muncul error:
- "Secure Boot Violation"
- "Invalid Signature"
- "Security Violation"

**Apa itu Secure Boot?**
Secure Boot adalah fitur keamanan di UEFI yang hanya mengizinkan software dengan tanda tangan digital resmi (biasanya Microsoft) untuk boot.

**Solusi: Disable Secure Boot**

1. **Masuk BIOS/UEFI:**
   - Restart komputer
   - Tekan tombol BIOS (F2/DEL/F10/F12) berulang-ulang saat boot

2. **Cari Pengaturan Secure Boot:**
   - Menu **Security** atau **Boot**
   - Atau **Authentication**

3. **Disable Secure Boot:**
   - Pilih **Secure Boot**
   - Ubah dari **Enabled** ke **Disabled**

4. **Save dan Exit:**
   - Tekan F10 untuk Save & Exit
   - Komputer restart

5. **Boot dari USB:**
   - Sekarang seharusnya bisa boot dari USB Ubuntu

> **Apakah aman disable Secure Boot?** Ya, untuk penggunaan pribadi aman. Secure Boot adalah lapisan keamanan tambahan, tapi bukan satu-satunya.

### 5. Installer Tidak Mendeteksi Hard Drive/SSD

**Masalah:** Saat instalasi, hard drive/SSD tidak terdeteksi oleh installer Ubuntu.

**Kemungkinan Penyebab:**
- Driver storage controller tidak ada
- Mode SATA di BIOS salah setting
- Hardware tidak kompatibel

**Solusi:**

**Cek Mode SATA di BIOS:**
1. Masuk BIOS
2. Cari **SATA Mode** atau **Storage Configuration**
3. Ubah ke **AHCI** (bukan RAID atau IDE)
4. Save dan Exit

> **Perhatian:** Jika ada Windows di komputer yang sama, mengubah SATA mode bisa membuat Windows tidak boot. Backup data dulu!

**Load Driver Tambahan:**
1. Download driver storage controller dari website motherboard
2. Extract ke flashdisk
3. Saat instalasi, pilih "Load Driver"

**Coba Kernel Versi Lain:**
1. Di menu GRUB, pilih **Advanced Options**
2. Pilih kernel versi lain (misal: recovery mode)

### 6. Tidak Ada Koneksi Jaringan Saat Instalasi

**Masalah:** Installer tidak mendeteksi jaringan/internet.

**Untuk Kabel LAN:**
- ✅ Pastikan kabel terhubung dengan benar (ada lampu indikator)
- ✅ Coba port LAN lain di router/switch
- ✅ Cek apakah DHCP server aktif (biasanya otomatis)

**Untuk WiFi:**
- ⚠️ Ubuntu Server tidak selalu include driver WiFi proprietary
- ✅ Gunakan kabel LAN sementara untuk instalasi
- ✅ Install driver WiFi setelah instalasi selesai:
```bash
sudo apt install linux-firmware
sudo apt install firmware-iwlwifi  # Untuk Intel WiFi
```

**Solusi Alternatif:**
- Skip konfigurasi jaringan saat instalasi
- Install dulu, lalu setup jaringan setelah reboot
- Gunakan USB tethering dari HP (biasanya langsung terdeteksi)

### 7. Error Saat Download Package/Update

**Masalah:** Muncul error saat update atau install package:
- "Unable to locate package"
- "404 Not Found"
- "Connection timed out"

**Solusi:**

**Update Repository:**
```bash
sudo apt update
```

**Ganti Mirror:**
1. Edit file sources.list:
```bash
sudo nano /etc/apt/sources.list
```
2. Ganti `archive.ubuntu.com` dengan mirror lokal:
   - Indonesia: `kartolo.sby.datautama.net.id/ubuntu`
   - Singapore: `mirror.nus.edu.sg/ubuntu`
3. Save (Ctrl+O) dan Exit (Ctrl+X)
4. Update lagi:
```bash
sudo apt update
```

**Cek Koneksi Internet:**
```bash
ping 8.8.8.8
ping google.com
```

**Clear Cache:**
```bash
sudo apt clean
sudo apt update
```

---

## Referensi dan Link Penting

- [Ubuntu Server Official Website](https://ubuntu.com/server) - Website resmi Ubuntu Server
- [Ubuntu Release Notes](https://wiki.ubuntu.com/ReleaseNotes) - Catatan rilis setiap versi
- [Ubuntu Server Documentation](https://ubuntu.com/server/docs) - Dokumentasi lengkap Ubuntu Server
- [Ubuntu ISO Releases](https://releases.ubuntu.com/) - Download semua versi Ubuntu
- [Ubuntu Pro](https://ubuntu.com/pro) - Extended security dan support
- [Ask Ubuntu](https://askubuntu.com/) - Forum tanya jawab Ubuntu

---

## Kesimpulan

Download Ubuntu Server itu mudah, yang penting adalah:

1. ✅ **Pilih versi yang tepat** - LTS untuk produksi, Interim untuk testing
2. ✅ **Download dari sumber resmi** - Hindari file palsu/malware
3. ✅ **Verifikasi checksum** - Pastikan file asli dan utuh
4. ✅ **Pilih arsitektur yang sesuai** - amd64 untuk Intel/AMD, arm64 untuk ARM
5. ✅ **Buat bootable USB dengan benar** - Gunakan Rufus, Etcher, atau Ventoy
6. ✅ **Ikuti instalasi dengan teliti** - especially di bagian partisi dan SSH

Selamat mendownload dan menginstall Ubuntu Server! 🎉
