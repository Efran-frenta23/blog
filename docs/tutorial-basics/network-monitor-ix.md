---
sidebar_position: 5
---

# Network Monitor — ix.dalang.io

**[ix.dalang.io](https://ix.dalang.io/)** adalah dashboard pemantau traffic jaringan (network traffic monitor) Dalang. Halaman ini menjelaskan apa itu, apa yang ditampilkan, dan kapan dipakai.

---

## Fungsi utama

Dashboard ini menampilkan **statistik traffic jaringan secara real-time** dari device-device yang terhubung ke jaringan Dalang.

Singkatnya: kalau kamu mau tahu "sekarang lagi sibuk nggak jaringan Dalang?" — bukanya di `ix.dalang.io`.

---

## Apa saja yang ditampilkan?

### 1. Live Traffic Metrics

Kecepatan traffic yang sedang terjadi **saat itu juga**, dalam satuan **bits per second**:

- **Download rate** — berapa cepat data masuk.
- **Upload rate** — berapa cepat data keluar.

### 2. Cumulative Data

Total data yang sudah pernah ditransfer (sepanjang waktu):

- Total download (all-time).
- Total upload (all-time).

### 3. Device Monitoring

Agregat traffic dari **banyak device sekaligus**, jadi kamu bisa lihat gambaran umumnya.

### 4. Per-Device Details

Kalau mau detail, bisa di-klik tiap device untuk lihat breakdown traffic-nya sendiri-sendiri.

---

## Analogi Sederhana

Bayangkan `ix.dalang.io` sebagai **speedometer** di jaringan kantor:

- Jarum speedometer = live traffic.
- Odometer = cumulative data.
- Dashboard = agregat semua kendaraan.
- Klik satu device = lihat speedometer per kendaraan.

---

## Teknologi di balik layar

Dashboard ini dibangun dengan:

- **Go** (bahasa pemrograman backend)
- **HTMX** (untuk interaksi ringan di browser)
- **DaisyUI** (komponen UI di atas Tailwind CSS)

Kombinasi ini dipilih supaya dashboard-nya ringan dan cepat — cocok untuk monitor real-time.

---

## Kapan kamu perlu membuka ini?

- **Saat troubleshooting** — kalau ada pelanggan komplain koneksi lemot, cek dulu apakah jaringan memang lagi sibuk.
- **Saat laporan** — kalau perlu data konsumsi bandwidth.
- **Saat rutin monitoring** — untuk memastikan tidak ada anomali traffic.

---

## Hubungan dengan dashboard lain

Dalang punya dua dashboard publik yang sering disalahpahami:

| Dashboard | URL | Fungsi |
|-----------|-----|--------|
| **Network Monitor** | [ix.dalang.io](https://ix.dalang.io/) | Traffic jaringan real-time |
| **Uptime Monitor** | [uptime.dalang.io](https://uptime.dalang.io/) | Status "hidup/mati"-nya tiap layanan |

Jangan tertukar — `ix` untuk traffic, `uptime` untuk status layanan.

Baca selengkapnya di **[Status & Uptime](./status-uptime)**.
