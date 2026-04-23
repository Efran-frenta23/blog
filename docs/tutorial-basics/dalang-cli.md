---
sidebar_position: 4
---

# Dalang CLI

**Dalang CLI** adalah tool command-line (terminal) untuk mengelola layanan cloud Dalang langsung dari terminal. Referensinya dari [dalang.io/cli](https://dalang.io/cli).

---

## Apa itu Dalang CLI?

> *"Manage your cloud infrastructure from the terminal. Fast, scriptable, and developer-friendly."*
>
> Kelola infrastruktur cloud kamu dari terminal. Cepat, bisa di-script, dan developer-friendly.

Singkatnya: kalau pelanggan tipe developer dan tidak mau klik-klik di dashboard, mereka pakai Dalang CLI supaya bisa:

- Manage VPS langsung dari terminal.
- Otomatisasi pekerjaan lewat script.
- Terintegrasi dengan tools lain di workflow mereka.

---

## Kenapa CLI-nya spesial?

Ada lima hal yang jadi keunggulan Dalang CLI:

### 1. 🔑 Direct Shell Access

Masuk ke Virtual Machine **tanpa perlu setup SSH key atau firewall**. Satu command, langsung connect.

### 2. 📦 JSON Output

Hampir semua command mendukung flag `--json`. Output-nya rapi dalam format JSON — cocok untuk automation, scripting, atau integrasi dengan tools lain.

### 3. 🪶 Lightweight

Hanya satu binary, ukurannya sekitar **6 MB**, **tanpa dependency**. Tinggal download, taruh, jalan.

### 4. 🖥️ Cross-Platform

Dalang CLI jalan di banyak platform:

- Linux (x86_64 & ARM64)
- macOS (Intel & Apple Silicon)
- Windows (x86_64)
- Android (lewat Termux, ARM64)

### 5. 🔐 Secure Authentication

Login pakai **OAuth device flow**. Token tersimpan dengan permission khusus user — lebih aman daripada password di file.

---

## Cara Install

### Linux / macOS

```bash
curl -fsSL https://dalang.io/install.sh | bash
```

### Windows (PowerShell)

```powershell
irm https://dalang.io/install.ps1 | iex
```

### Manual

Kalau kamu atau pelanggan tidak bisa pakai installer:

1. Download binary dari [dalang.io/cli](https://dalang.io/cli).
2. Buat file jadi executable, lalu pindahkan ke PATH:

```bash
chmod +x dalang-*
sudo mv dalang-* /usr/local/bin/dalang
```

### Verifikasi

Setelah install selesai, cek dengan:

```bash
dalang --version
```

Kalau muncul versinya, berarti install berhasil.

---

## Login Pertama Kali

Langkah login pakai OAuth device flow. Sangat mudah:

```bash
dalang auth
```

Alurnya:

1. CLI menampilkan URL dan sebuah kode unik.
2. Buka URL itu di browser.
3. Masukkan kode tersebut.
4. Approve akses di browser.
5. Terminal otomatis logged in — tidak perlu ketik password.

---

## Command Dasar yang Wajib Tahu

| Command | Fungsi |
|---------|--------|
| `dalang auth` | Login |
| `dalang service list` | Lihat daftar semua layanan (VPS, dll) |
| `dalang service info <nama>` | Lihat detail satu layanan |
| `dalang shell <nama>` | Connect ke VM (langsung masuk shell) |
| `dalang start <nama>` | Nyalakan VM |
| `dalang stop <nama>` | Matikan VM |
| `dalang delete <nama>` | Hapus VM |
| `dalang credit` | Cek sisa saldo/kredit |
| `dalang domain add <vps> <domain>` | Tambahkan domain custom ke VPS |

---

## Contoh Penggunaan

### Lihat semua layananmu

```bash
dalang service list
```

### Masuk ke satu VM

```bash
dalang shell my-webserver
```

Setelah ini, kamu langsung di dalam VM itu — persis kayak habis SSH.

### Cek info detail satu service

```bash
dalang service info my-webserver
```

### Automation pakai JSON

```bash
dalang service list --json
```

Output-nya JSON — bisa langsung di-parse pakai `jq` atau script Python/Node.

Contoh: ambil semua service yang statusnya RUNNING:

```bash
dalang service list --json | jq '.[] | select(.status == "RUNNING")'
```

---

## Untuk apa ini penting buat karyawan baru?

Kalau nanti kamu:

- **Support pelanggan** — banyak pelanggan kita tipe developer. Kamu perlu paham dasar CLI supaya bisa bantu troubleshoot.
- **Internal engineer** — CLI ini juga dipakai tim internal untuk manage infrastruktur.
- **Dokumentasi / content** — kalau bikin tutorial ke publik, command di atas yang jadi referensi utama.

---

## Referensi Cepat

- Halaman resmi: [dalang.io/cli](https://dalang.io/cli)
- Script install Linux/macOS: `curl -fsSL https://dalang.io/install.sh | bash`
- Script install Windows: `irm https://dalang.io/install.ps1 | iex`

---

Selanjutnya: baca **[Network Monitor (ix.dalang.io)](./network-monitor-ix)** untuk kenalan dengan salah satu dashboard internal kami.
