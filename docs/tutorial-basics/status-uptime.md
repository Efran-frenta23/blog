---
sidebar_position: 6
---

# Status & Uptime — uptime.dalang.io

**[uptime.dalang.io](https://uptime.dalang.io/)** adalah dashboard status resmi Dalang. Kalau pelanggan (atau kamu sendiri) penasaran "layanan Dalang lagi hidup nggak?" — ini tempatnya.

---

## Fungsi utama

Dashboard ini memantau **ketersediaan dan performa** seluruh layanan inti Dalang **secara real-time**.

Cara kerjanya: sistem melakukan pengecekan otomatis **setiap 5 detik** ke tiap layanan, lalu menampilkan hasilnya di halaman ini.

---

## Apa saja yang dipantau?

Saat ini ada **9 layanan** yang dipantau, dibagi jadi dua kelompok:

### Web Services (4 layanan)

Layanan yang berbentuk website atau endpoint HTTP:

| Layanan | Fungsinya |
|---------|-----------|
| `dalang.io` | Website utama Dalang |
| `api.dalang.io` | Endpoint API untuk CLI & integrasi |
| `ix.dalang.io` | Dashboard network monitor (lihat [di sini](./network-monitor-ix)) |
| `uptime.dalang.io` | Dashboard uptime ini sendiri |

### Infrastructure Nodes (5 layanan)

Node-node backend yang menopang cluster Dalang:

- **Cluster Node 1**
- **Cluster Node 2**
- **Cluster Node 3**
- **Cluster Node 4**
- **Cluster Node 5**

Lima node ini adalah server di belakang layar yang menjalankan workload pelanggan.

---

## Cara membaca halaman uptime

Setiap layanan menampilkan dua metrik utama:

### 1. Uptime Percentage

Persentase waktu layanan dalam kondisi **hidup** selama 1 tahun terakhir. Makin tinggi, makin baik.

### 2. Response Time

Berapa lama layanan merespons pengecekan (dalam milidetik). Makin rendah, makin cepat.

### Status Operational

Di sebelah tiap layanan ada label status. Kalau semuanya **Operational**, berarti semua sehat.

---

## Kenapa dashboard ini penting?

### Untuk pelanggan
- Transparansi — pelanggan bisa cek sendiri kondisi layanan, tidak perlu nunggu kita kasih kabar.
- Bisa jadi referensi saat ada laporan masalah.

### Untuk tim internal
- Early warning — ada gangguan kelihatan di sini duluan.
- Jadi "source of truth" saat ada pertanyaan "beneran down, atau cuma di sisi pelanggan?".

---

## Apa yang harus kamu lakukan kalau ada yang tidak operational?

1. **Cek ulang dari device lain.** Pastikan bukan masalah lokal kamu.
2. **Lapor ke tim yang bertanggung jawab** (biasanya tim infra/ops) — gunakan channel internal yang berlaku di tim kamu.
3. **Jangan panik dulu ke pelanggan.** Kumpulkan dulu info: layanan apa yang bermasalah, sejak kapan, respons time berapa.

---

## Hubungan dengan dashboard lain

Sudah disebut di halaman [Network Monitor](./network-monitor-ix), tapi diulang supaya jelas:

| Kalau kamu mau tahu… | Buka |
|----------------------|------|
| "Layanan Dalang hidup nggak?" | [uptime.dalang.io](https://uptime.dalang.io/) |
| "Jaringan Dalang lagi sibuk nggak?" | [ix.dalang.io](https://ix.dalang.io/) |

---

## Ringkasan

- **uptime.dalang.io** = dashboard kesehatan layanan.
- Pengecekan berjalan tiap 5 detik.
- Ada 9 layanan yang dipantau: 4 web services + 5 cluster nodes.
- Hijau semua = aman. Ada yang tidak operational = segera laporkan.
