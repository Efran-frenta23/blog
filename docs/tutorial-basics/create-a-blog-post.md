---
sidebar_position: 3
---

# Tutorial: Deploy Aplikasi Pertama Kamu di Dalang.io

Panduan lengkap step-by-step untuk deploy aplikasi web pertama kamu menggunakan VPS dari Dalang.io. Tutorial ini dirancang untuk pemula yang baru pertama kali deploy aplikasi ke server.

---

## Apa yang Akan Kita Pelajari?

Dalam tutorial ini, kamu akan belajar:

1. ✅ Cara order dan setup VPS di Dalang.io
2. ✅ Cara connect ke VPS via Dalang CLI (cara modern & mudah!)
3. ✅ Cara install software yang diperlukan (Node.js, Python, atau PHP)
4. ✅ Cara deploy aplikasi web sederhana
5. ✅ Cara setup domain dan SSL
6. ✅ Cara maintain dan monitor server

**Estimasi waktu:** 30-60 menit

**Level:** Pemula

---

## Prerequisites (Persiapan Awal)

Sebelum memulai, pastikan kamu sudah punya:

### 1. Akun Dalang.io

- Daftar di [dalang.io](https://dalang.io)
- Verifikasi email dan akun kamu

### 2. Aplikasi Web Sederhana

Untuk tutorial ini, kita akan deploy salah satu dari:

**Node.js App:**
```javascript
// app.js
const http = require('http');

const server = http.createServer((req, res) => {
  res.statusCode = 200;
  res.setHeader('Content-Type', 'text/plain');
  res.end('Hello from Dalang.io VPS!\n');
});

server.listen(3000, '0.0.0.0', () => {
  console.log('Server running on port 3000');
});
```

**Python Flask App:**
```python
# app.py
from flask import Flask

app = Flask(__name__)

@app.route('/')
def hello():
    return 'Hello from Dalang.io VPS!'

if __name__ == '__main__':
    app.run(host='0.0.0.0', port=3000)
```

**PHP App:**
```php
<?php
// index.php
echo "Hello from Dalang.io VPS!";
?>
```

> **Pilih salah satu** sesuai dengan bahasa programming yang kamu kuasai.

### 3. Software di Lokal

- **Terminal** (Linux/macOS) atau **PowerShell** (Windows)
- **Text Editor** (VS Code, Sublime, dll)
- **Git** (opsional, untuk upload code)
- **Dalang CLI** - Akan diinstall di Langkah 2!

---

## Langkah 1: Order dan Setup VPS

### 1.1 Pilih Paket VPS

1. **Login ke Dalang.io**
2. **Klik "Create VPS"** atau "Order Now"
3. **Pilih paket** yang sesuai:

| Paket | CPU | RAM | Storage | Harga/Bulan | Cocok Untuk |
|-------|-----|-----|---------|-------------|-------------|
| **Starter** | 1 Core | 1 GB | 15 GB | Rp 40.000 | Testing, belajar |
| **Basic** | 1 Core | 2 GB | 20 GB | Rp 60.000 | Website kecil |
| **Standard** | 2 Core | 4 GB | 40 GB | Rp 120.000 | Production kecil ⭐ |

> **Rekomendasi:** Pilih **Standard** untuk production. Tapi untuk belajar, **Starter** sudah cukup!

### 1.2 Pilih Sistem Operasi

Pilih OS sesuai aplikasi kamu:

| Aplikasi | OS Rekomendasi |
|----------|----------------|
| Node.js | Ubuntu 24.04 LTS |
| Python | Ubuntu 24.04 LTS |
| PHP | Ubuntu 24.04 LTS |
| .NET | Ubuntu 24.04 LTS |

> **Tips:** Ubuntu 24.04 LTS adalah pilihan paling aman dengan dokumentasi terbanyak.

### 1.3 Pilih Region

Pilih data center terdekat dengan target user:

- **User Indonesia:** Jakarta atau Surabaya
- **User Southeast Asia:** Singapore
- **User Global:** Multi-region deployment

### 1.4 Konfigurasi Tambahan

- **SSH Key:** Upload public key SSH kamu (direkomendasikan)
- **Backup:** Enable automatic backup (Rp 20.000/bln)
- **Monitoring:** Enable free monitoring

### 1.5 Payment dan Deploy

1. Pilih metode pembayaran
2. Lakukan payment
3. Tunggu 2-5 menit, VPS akan deployed!
4. Kamu akan dapat email dengan detail VPS:
   - **IP Address:** `xxx.xxx.xxx.xxx`
   - **Username:** `root` atau user yang kamu buat
   - **Password:** (jika tidak pakai SSH key)

---

## Langkah 2: Install dan Setup Dalang CLI

### 2.1 Apa itu Dalang CLI?

**Dalang CLI** adalah command-line interface modern untuk mengelola infrastruktur Dalang.io langsung dari terminal kamu.

**Keunggulan Dalang CLI:**
- ✅ **Tanpa konfigurasi SSH** - Tidak perlu setup SSH key atau firewall
- ✅ **Direct shell access** - Connect ke VPS dengan satu command
- ✅ **Fast & lightweight** - Binary ~6MB, no dependencies
- ✅ **Cross-platform** - Support Linux, macOS, Windows (Intel & ARM)
- ✅ **Secure auth** - OAuth device flow, token tersimpan aman
- ✅ **AI-ready** - Dibangun untuk autonomous AI agents

> **🎯 Dalang CLI adalah cara TERMUDAH untuk connect ke VPS!** Tidak perlu ribet dengan SSH keys, IP addresses, atau firewall configuration!

### 2.2 Install Dalang CLI

**Linux / macOS:**
```bash
curl -fsSL https://dalang.io/install.sh | bash
```

**Windows (PowerShell):**
```powershell
irm https://dalang.io/install.ps1 | iex
```

**Manual Install (jika curl tidak tersedia):**

1. Download binary dari [dalang.io/cli](https://dalang.io/cli)
2. Extract dan pindahkan ke PATH:
```bash
chmod +x dalang-*
sudo mv dalang-* /usr/local/bin/dalang
```

**Verify installation:**
```bash
dalang --version
```

Output:
```
dalang version 1.0.0
```

### 2.3 Authenticate (Login)

Setelah install, login ke akun Dalang.io:

```bash
dalang auth
```

**Proses login:**
1. Command akan menampilkan URL dan code
2. Buka URL di browser
3. Masukkan code yang ditampilkan
4. Approve akses
5. Terminal akan otomatis logged in

Output setelah sukses:
```
✓ Authentication successful!
✓ Welcome back, [your-name]!
```

### 2.4 Command Dasar Dalang CLI

Berikut command-command yang sering digunakan:

| Command | Fungsi |
|---------|--------|
| `dalang auth` | Login ke akun Dalang |
| `dalang service list` | Lihat semua VPS/layanan |
| `dalang service info <name>` | Lihat detail VPS |
| `dalang shell <name>` | Connect ke VPS (seperti SSH) |
| `dalang start <name>` | Start VPS |
| `dalang stop <name>` | Stop VPS |
| `dalang delete <name>` | Delete VPS |
| `dalang credit` | Cek saldo kredit |
| `dalang credit add <amount>` | Top up kredit |
| `dalang domain add <vps> <domain>` | Add domain |
| `dalang help` | Lihat semua command |

### 2.5 Lihat Daftar VPS Kamu

Setelah login, lihat VPS yang kamu punya:

```bash
dalang service list
```

Output:
```
NAME            TYPE    STATUS      EXPIRED       CPU   RAM    STORAGE
my-webapp       VPS     RUNNING     2024-02-15    2     4GB    40GB
test-server     VPS     RUNNING     2024-02-20    1     2GB    20GB
```

> **💡 Tips:** Gunakan `dalang service list --json` untuk output dalam format JSON (cocok untuk scripting/automation).

### 2.6 Connect ke VPS dengan Dalang CLI

Ini adalah bagian terbaik! Connect ke VPS sangat mudah:

```bash
dalang shell my-webapp
```

Output:
```
→ Connecting to my-webapp (shell mode)...
✓ Connected!

Welcome to Ubuntu 24.04 LTS (GNU/Linux 6.8.0-31-generic x86_64)

 * Documentation:  https://help.ubuntu.com
 * Management:     https://landscape.canonical.com
 * Support:        https://ubuntu.com/advantage

Last login: Mon Jan 15 10:30:00 2024 from 10.0.0.1
root@my-webapp:~#
```

**Selamat! Kamu sekarang terhubung ke VPS!** 🎉

> **🎯 Keuntungan Dalang CLI vs SSH Tradisional:**
> - ❌ **SSH:** Perlu IP address, SSH key, firewall config
> - ✅ **Dalang CLI:** Cukup `dalang shell <name>` - selesai!

### 2.7 Disconnect dari VPS

Untuk disconnect dari VPS:

```bash
exit
```

Kamu akan kembali ke terminal lokal.

---

## Langkah 3: Setup Awal Server

### 3.1 Update Sistem

Selalu update sistem setelah pertama kali connect:

```bash
apt update && apt upgrade -y
```

Ini akan:
- Update database package
- Install security patches terbaru
- Memastikan semua package up-to-date

### 3.2 Buat User Baru (Security Best Practice)

Jangan gunakan `root` untuk daily use! Buat user biasa:

```bash
# Buat user baru
adduser dalanguser

# Masukkan password yang kuat
# Isi informasi user (opsional, tekan Enter untuk skip)

# Berikan akses sudo
usermod -aG sudo dalanguser
```

### 3.3 Setup SSH Key untuk User Baru

```bash
# Switch ke user baru
su - dalanguser

# Buat folder .ssh
mkdir -p ~/.ssh

# Set permission yang benar
chmod 700 ~/.ssh

# Edit authorized_keys
nano ~/.ssh/authorized_keys
```

Paste public key kamu (`~/.ssh/id_rsa.pub` dari komputer lokal) ke file ini.

```bash
# Set permission file
chmod 600 ~/.ssh/authorized_keys

# Exit
exit
```

### 3.4 Disable Root Login (Optional tapi Direkomendasikan)

Edit SSH configuration:

```bash
sudo nano /etc/ssh/sshd_config
```

Ubah baris berikut:

```bash
PermitRootLogin no
PasswordAuthentication no
```

Save (Ctrl+O, Enter) dan Exit (Ctrl+X), lalu restart SSH:

```bash
sudo systemctl restart sshd
```

> **⚠️ PENTING:** Pastikan SSH key sudah setup sebelum disable password!

### 3.5 Setup Firewall (UFW)

```bash
# Enable firewall
sudo ufw enable

# Allow SSH
sudo ufw allow 22/tcp

# Allow HTTP (untuk web server)
sudo ufw allow 80/tcp

# Allow HTTPS (untuk SSL)
sudo ufw allow 443/tcp

# Check status
sudo ufw status
```

Output:
```
Status: active

To                         Action      From
--                         ------      ----
22/tcp                     ALLOW       Anywhere
80/tcp                     ALLOW       Anywhere
443/tcp                    ALLOW       Anywhere
```

---

## Langkah 4: Install Software yang Diperlukan

Pilih salah satu sesuai aplikasi kamu:

### 4.1 Install Node.js (Untuk Aplikasi Node.js)

```bash
# Install NodeSource repository (Node.js 20.x)
curl -fsSL https://deb.nodesource.com/setup_20.x | sudo -E bash -

# Install Node.js
sudo apt install -y nodejs

# Verify installation
node --version
npm --version
```

Output:
```
v20.10.0
10.2.3
```

### 4.2 Install Python (Untuk Aplikasi Python)

```bash
# Install Python dan pip
sudo apt install -y python3 python3-pip python3-venv

# Verify installation
python3 --version
pip3 --version
```

Output:
```
Python 3.12.3
pip 24.0
```

### 4.3 Install PHP (Untuk Aplikasi PHP)

```bash
# Install PHP dan extensions
sudo apt install -y php php-fpm php-mysql php-curl php-gd php-mbstring php-xml php-zip

# Verify installation
php --version
```

Output:
```
PHP 8.3.4 (cli) (built: Mar  1 2024 15:23:45) (NTS)
```

### 4.4 Install Git (Opsional, untuk Clone Repository)

```bash
sudo apt install -y git
git --version
```

### 4.5 Install Text Editor (Nano/Vim)

```bash
# Nano sudah terinstall, install vim jika prefer
sudo apt install -y vim
```

---

## Langkah 5: Deploy Aplikasi

Pilih salah satu sesuai aplikasi kamu:

### 5.1 Deploy Node.js App

**Opsi A: Upload Manual**

1. Buat folder aplikasi:
```bash
mkdir -p /var/www/myapp
cd /var/www/myapp
```

2. Buat file `app.js`:
```bash
nano app.js
```

3. Paste code Node.js dari persiapan, save dan exit.

4. Install dependencies (jika ada):
```bash
npm install
```

**Opsi B: Clone dari Git**

```bash
cd /var/www
git clone https://github.com/username/repo.git myapp
cd myapp
npm install
```

**Setup PM2 (Process Manager)**

PM2 akan menjaga aplikasi tetap running:

```bash
# Install PM2 global
sudo npm install -g pm2

# Start aplikasi
pm2 start app.js --name myapp

# Setup PM2 startup
pm2 startup systemd

# Jalankan command yang muncul (copy-paste)
# Contoh: sudo env PATH=$PATH:/usr/bin pm2 startup systemd -u dalanguser

# Save PM2 configuration
pm2 save

# Monitor aplikasi
pm2 status
pm2 logs
```

### 5.2 Deploy Python Flask App

**Opsi A: Upload Manual**

1. Buat folder aplikasi:
```bash
mkdir -p /var/www/myapp
cd /var/www/myapp
```

2. Buat virtual environment:
```bash
python3 -m venv venv
source venv/bin/activate
```

3. Install Flask:
```bash
pip install flask gunicorn
```

4. Buat file `app.py`:
```bash
nano app.py
```

5. Paste code Flask dari persiapan, save dan exit.

**Opsi B: Clone dari Git**

```bash
cd /var/www
git clone https://github.com/username/repo.git myapp
cd myapp
python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt
```

**Setup Gunicorn + Systemd**

1. Buat file service systemd:
```bash
sudo nano /etc/systemd/system/myapp.service
```

2. Paste konfigurasi berikut:
```ini
[Unit]
Description=Gunicorn instance to serve Flask app
After=network.target

[Service]
User=dalanguser
Group=www-data
WorkingDirectory=/var/www/myapp
ExecStart=/var/www/myapp/venv/bin/gunicorn -w 3 -b 0.0.0.0:3000 app:app

[Install]
WantedBy=multi-user.target
```

3. Enable dan start service:
```bash
sudo systemctl daemon-reload
sudo systemctl enable myapp
sudo systemctl start myapp
sudo systemctl status myapp
```

### 5.3 Deploy PHP App

**Opsi A: Upload Manual**

1. Buat folder aplikasi:
```bash
sudo mkdir -p /var/www/myapp
sudo chown -R www-data:www-data /var/www/myapp
cd /var/www/myapp
```

2. Buat file `index.php`:
```bash
sudo nano index.php
```

3. Paste code PHP dari persiapan, save dan exit.

**Setup Nginx untuk PHP**

1. Install Nginx:
```bash
sudo apt install -y nginx
```

2. Buat konfigurasi Nginx:
```bash
sudo nano /etc/nginx/sites-available/myapp
```

3. Paste konfigurasi:
```nginx
server {
    listen 80;
    server_name your-domain.com;
    root /var/www/myapp;
    index index.php index.html;

    location / {
        try_files $uri $uri/ =404;
    }

    location ~ \.php$ {
        include snippets/fastcgi-php.conf;
        fastcgi_pass unix:/run/php/php8.3-fpm.sock;
    }
}
```

4. Enable site:
```bash
sudo ln -s /etc/nginx/sites-available/myapp /etc/nginx/sites-enabled/
sudo nginx -t
sudo systemctl reload nginx
```

---

## Langkah 6: Setup Reverse Proxy (Untuk Node.js/Python)

Jika deploy Node.js atau Python app, setup reverse proxy dengan Nginx:

### 6.1 Install Nginx

```bash
sudo apt install -y nginx
```

### 6.2 Buat Konfigurasi Nginx

```bash
sudo nano /etc/nginx/sites-available/myapp
```

Paste konfigurasi berikut:

**Untuk Node.js:**
```nginx
server {
    listen 80;
    server_name your-domain.com;

    location / {
        proxy_pass http://localhost:3000;
        proxy_http_version 1.1;
        proxy_set_header Upgrade $http_upgrade;
        proxy_set_header Connection 'upgrade';
        proxy_set_header Host $host;
        proxy_cache_bypass $http_upgrade;
        proxy_set_header X-Real-IP $remote_addr;
        proxy_set_header X-Forwarded-For $proxy_add_x_forwarded_for;
        proxy_set_header X-Forwarded-Proto $scheme;
    }
}
```

**Untuk Python (Gunicorn):**
```nginx
server {
    listen 80;
    server_name your-domain.com;

    location / {
        proxy_pass http://localhost:3000;
        proxy_set_header Host $host;
        proxy_set_header X-Real-IP $remote_addr;
        proxy_set_header X-Forwarded-For $proxy_add_x_forwarded_for;
        proxy_set_header X-Forwarded-Proto $scheme;
    }
}
```

### 6.3 Enable Site

```bash
# Create symlink
sudo ln -s /etc/nginx/sites-available/myapp /etc/nginx/sites-enabled/

# Test configuration
sudo nginx -t

# Reload Nginx
sudo systemctl reload nginx
```

### 6.4 Check Status

```bash
# Check Nginx status
sudo systemctl status nginx

# Check jika aplikasi sudah accessible
curl http://localhost
```

---

## Langkah 7: Setup Domain dan SSL

### 7.1 Setup DNS

1. **Login ke domain provider** (Niagahoster, Domainesia, Namecheap, dll)
2. **Tambahkan A Record:**
   - **Name/Host:** `@` atau `your-domain.com`
   - **Value/Points to:** `xxx.xxx.xxx.xxx` (IP VPS kamu)
   - **TTL:** 3600 atau auto

3. **Tambahkan CNAME untuk www:**
   - **Name/Host:** `www`
   - **Value/Points to:** `your-domain.com`
   - **TTL:** 3600

> **Catatan:** DNS propagation bisa memakan waktu 5 menit - 48 jam.

### 7.2 Update Nginx Configuration

Edit konfigurasi Nginx:

```bash
sudo nano /etc/nginx/sites-available/myapp
```

Update `server_name`:

```nginx
server_name your-domain.com www.your-domain.com;
```

Reload Nginx:

```bash
sudo nginx -t && sudo systemctl reload nginx
```

### 7.3 Install SSL dengan Let's Encrypt

```bash
# Install Certbot
sudo apt install -y certbot python3-certbot-nginx

# Request SSL certificate
sudo certbot --nginx -d your-domain.com -d www.your-domain.com

# Ikuti instruksi:
# 1. Masukkan email
# 2. Setuju terms
# 3. Pilih redirect HTTP → HTTPS (pilih 2)
```

### 7.4 Auto-Renewal SSL

SSL Let's Encrypt expired setelah 90 hari. Setup auto-renewal:

```bash
# Test auto-renewal
sudo certbot renew --dry-run

# Certbot sudah setup automatic renewal via systemd timer
# Check timer status
sudo systemctl list-timers | grep certbot
```

### 7.5 Verify SSL

Buka browser dan akses:
- `https://your-domain.com`
- Klik icon gembok untuk verify SSL

---

## Langkah 8: Monitoring dan Maintenance

### 8.1 Monitor Resource

**Check CPU & RAM:**
```bash
htop
```

**Check Disk Usage:**
```bash
df -h
```

**Check Memory:**
```bash
free -h
```

### 8.2 Monitor Aplikasi

**Untuk Node.js (PM2):**
```bash
pm2 status
pm2 logs
pm2 monit
```

**Untuk Python (Systemd):**
```bash
sudo systemctl status myapp
sudo journalctl -u myapp -f
```

**Untuk Nginx:**
```bash
sudo systemctl status nginx
sudo tail -f /var/log/nginx/access.log
sudo tail -f /var/log/nginx/error.log
```

### 8.3 Setup Monitoring Dashboard (Opsional)

Install Netdata untuk real-time monitoring:

```bash
# Install Netdata
bash <(curl -Ss https://my-netdata.io/kickstart.sh)

# Akses dashboard
# http://your-domain.com:19999
```

### 8.4 Backup Data

**Manual Backup:**
```bash
# Backup aplikasi
tar -czf myapp-backup-$(date +%Y%m%d).tar.gz /var/www/myapp

# Download ke lokal
scp dalanguser@your-ip:/path/to/backup.tar.gz ~/backups/
```

**Setup Automatic Backup:**
```bash
# Install rsync
sudo apt install -y rsync

# Buat backup script
nano ~/backup.sh
```

Paste script:
```bash
#!/bin/bash
DATE=$(date +%Y%m%d)
BACKUP_DIR="/home/dalanguser/backups"
APP_DIR="/var/www/myapp"

mkdir -p $BACKUP_DIR
tar -czf $BACKUP_DIR/myapp-$DATE.tar.gz $APP_DIR

# Keep only last 7 backups
find $BACKUP_DIR -name "myapp-*.tar.gz" -mtime +7 -delete
```

Make executable dan add to crontab:
```bash
chmod +x ~/backup.sh
crontab -e
```

Add line:
```
0 2 * * * /home/dalanguser/backup.sh
```

### 8.5 Security Updates

Setup automatic security updates:

```bash
# Install unattended-upgrades
sudo apt install -y unattended-upgrades

# Enable
sudo dpkg-reconfigure --priority=low unattended-upgrades
```

---

## Troubleshooting - Masalah Umum

### 1. Cannot Connect via Dalang CLI

**Masalah:** Connection timeout, error, atau tidak bisa connect

**Solusi:**

**Check authentication:**
```bash
# Verify sudah login
dalang auth

# Jika perlu re-authenticate
dalang auth --refresh
```

**Check VPS status:**
```bash
# Lihat semua VPS
dalang service list

# Check detail VPS
dalang service info my-webapp
```

**Restart VPS dari CLI:**
```bash
# Stop VPS
dalang stop my-webapp

# Start ulang
dalang start my-webapp

# Connect lagi
dalang shell my-webapp
```

**Check kredensial:**
```bash
# Verify credit/saldo
dalang credit

# Jika credit habis, top up
dalang credit add 100
```

### 2. Dalang CLI Tidak Terinstall/Not Found

**Masalah:** Command `dalang` tidak ditemukan

**Solusi:**

**Linux/macOS:**
```bash
# Reinstall
curl -fsSL https://dalang.io/install.sh | bash

# Verify PATH
export PATH=$PATH:/usr/local/bin

# Test
dalang --version
```

**Windows:**
```powershell
# Reinstall
irm https://dalang.io/install.ps1 | iex

# Restart PowerShell
```

**Manual:**
```bash
# Download dari https://dalang.io/cli
# Extract dan copy ke PATH
chmod +x dalang-*
sudo mv dalang-* /usr/local/bin/dalang
```

### 3. Website tidak accessible

**Masalah:** Browser tidak bisa akses website

**Solusi:**
```bash
# Connect ke VPS
dalang shell my-webapp

# Check Nginx status
sudo systemctl status nginx

# Check firewall
sudo ufw status

# Allow port 80/443 jika belum
sudo ufw allow 80/tcp
sudo ufw allow 443/tcp

# Check Nginx config
sudo nginx -t

# Check logs
sudo tail -f /var/log/nginx/error.log
```

### 4. Aplikasi crash atau tidak running

**Masalah:** Aplikasi berhenti tiba-tiba

**Untuk Node.js (PM2):**
```bash
# Connect ke VPS
dalang shell my-webapp

# Check status
pm2 status

# Check logs
pm2 logs

# Restart aplikasi
pm2 restart myapp
```

**Untuk Python (Systemd):**
```bash
# Connect ke VPS
dalang shell my-webapp

# Check status
sudo systemctl status myapp

# Check logs
sudo journalctl -u myapp -f

# Restart service
sudo systemctl restart myapp
```

### 5. SSL tidak bekerja

**Masalah:** Browser warning "Not Secure"

**Solusi:**
```bash
# Connect ke VPS
dalang shell my-webapp

# Check SSL certificate
sudo certbot certificates

# Renew jika expired
sudo certbot renew

# Force renew
sudo certbot renew --force-renewal

# Check Nginx config
sudo nginx -t
```

### 6. Disk penuh

**Masalah:** No space left on device

**Solusi:**
```bash
# Connect ke VPS
dalang shell my-webapp

# Check disk usage
df -h

# Find large files
sudo du -ah / | sort -rh | head -20

# Clean apt cache
sudo apt clean
sudo apt autoremove

# Clean logs
sudo journalctl --vacuum-time=1d

# Remove old kernels
sudo apt autoremove --purge
```

### 7. Out of Memory

**Masalah:** Server lemot atau aplikasi crash

**Solusi:**
```bash
# Connect ke VPS
dalang shell my-webapp

# Check memory
free -h
htop

# Add swap file (jika belum ada)
sudo fallocate -l 2G /swapfile
sudo chmod 600 /swapfile
sudo mkswap /swapfile
sudo swapon /swapfile

# Make permanent
echo '/swapfile none swap sw 0 0' | sudo tee -a /etc/fstab
```

### 8. Dalang CLI Error/Permission Denied

**Masalah:** Permission denied saat run command

**Solusi:**

**Check file permissions:**
```bash
chmod +x /usr/local/bin/dalang
```

**Run dengan sudo (jika perlu):**
```bash
sudo dalang service list
```

**Reinstall dengan permissions benar:**
```bash
# Linux/macOS
curl -fsSL https://dalang.io/install.sh | bash

# Verify
ls -l /usr/local/bin/dalang
```

### 9. Disk Penuh

**Masalah:** No space left on device

**Solusi:**
```bash
# Connect ke VPS
dalang shell my-webapp

# Check disk usage
df -h

# Find large files
sudo du -ah / | sort -rh | head -20

# Clean apt cache
sudo apt clean
sudo apt autoremove

# Clean logs
sudo journalctl --vacuum-time=1d

# Remove old kernels
sudo apt autoremove --purge
```

### 10. Out of Memory

**Masalah:** Server lemot atau aplikasi crash

**Solusi:**
```bash
# Connect ke VPS
dalang shell my-webapp

# Check memory
free -h
htop

# Add swap file (jika belum ada)
sudo fallocate -l 2G /swapfile
sudo chmod 600 /swapfile
sudo mkswap /swapfile
sudo swapon /swapfile

# Make permanent
echo '/swapfile none swap sw 0 0' | sudo tee -a /etc/fstab
```

---

## Best Practices

### 1. Security

- ✅ Gunakan **Dalang CLI** untuk akses - lebih aman dan mudah
- ✅ Setup firewall (UFW) dengan benar
- ✅ Update sistem rutin
- ✅ Gunakan SSL/TLS untuk semua website
- ✅ Backup data secara teratur
- ✅ Monitor logs untuk suspicious activity
- ✅ Disable root login untuk SSH tradisional

### 2. Performance

- ✅ Gunakan caching (Redis, Memcached)
- ✅ Enable Gzip compression di Nginx
- ✅ Gunakan CDN untuk static assets
- ✅ Monitor resource usage via `dalang service info`
- ✅ Optimize database queries

### 3. Reliability

- ✅ Enable automatic backup
- ✅ Setup monitoring dan alerting
- ✅ Gunakan process manager (PM2, systemd)
- ✅ Setup log rotation
- ✅ Document semua konfigurasi
- ✅ Gunakan Dalang CLI untuk automation

### 4. Dalang CLI Tips

**Automation dengan JSON output:**
```bash
# Get VPS info dalam JSON
dalang service list --json

# Parse dengan jq
dalang service list --json | jq '.[] | select(.status=="RUNNING")'
```

**Scripting contoh:**
```bash
#!/bin/bash
# Check semua VPS status
for vps in $(dalang service list --json | jq -r '.[].name'); do
  echo "Checking $vps..."
  dalang service info $vps
done
```

**Quick commands:**
```bash
# Connect cepat
alias dshell='dalang shell'

# Check credit
alias dcredit='dalang credit'

# List semua VPS
alias dvps='dalang service list'
```

### 5. Maintenance

- ✅ Update sistem mingguan via `dalang shell`
- ✅ Review logs secara berkala
- ✅ Clean unused files dan packages
- ✅ Test backup restore secara berkala
- ✅ Document perubahan konfigurasi
- ✅ Gunakan Dalang CLI untuk semua operasi

---

## Next Steps

Selamat! Aplikasi kamu sudah deployed di Dalang.io VPS! Berikut beberapa hal yang bisa dipelajari selanjutnya:

### 1. Scale Up dengan Dalang CLI

```bash
# Upgrade VPS
dalang upgrade my-webapp --cpu 4 --ram 8

# Add more VPS
dalang create vps --name my-app-2 --plan standard

# Setup load balancer
dalang create lb --name my-lb --targets my-webapp,my-app-2
```

### 2. Improve Security

- Setup fail2ban untuk protect dari brute force
- Setup intrusion detection system
- Monitor security logs via Dalang CLI

### 3. Optimize Performance

- Setup caching layer (Redis, Varnish)
- Configure CDN untuk static assets
- Optimize database dengan indexing

### 4. Automate Deployment dengan Dalang CLI

**CI/CD integration:**
```bash
# GitHub Actions example
- name: Deploy to Dalang.io
  run: |
    curl -fsSL https://dalang.io/install.sh | bash
    dalang auth --token ${{ secrets.DALANG_TOKEN }}
    dalang shell my-app --command "cd /var/www && git pull && npm restart"
```

**Automation scripts:**
```bash
#!/bin/bash
# Auto-deploy script
dalang shell my-app --command "cd /var/www && git pull && npm install && pm2 restart all"
```

### 5. Monitoring & Alerting

```bash
# Monitor via Dalang CLI
dalang service info my-webapp --json

# Setup alerting
dalang alert create --service my-webapp --type cpu --threshold 90
```

### 6. Learn Dalang CLI Advanced Features

- **AI Agents** - Autonomous infrastructure management
- **JSON Output** - For scripting and automation
- **Batch Operations** - Manage multiple VPS at once
- **API Integration** - Integrate dengan tools lain

---

## Referensi & Resources

### Dalang.io Resources
- [Dalang.io Documentation](https://dalang.io/docs)
- [Dalang.io CLI Documentation](https://dalang.io/cli)
- [Dalang.io Support](https://dalang.io/support)
- [Dalang.io Status](https://status.dalang.io)
- [Dalang.io API Docs](https://dalang.io/api)

### External Resources
- [Ubuntu Documentation](https://ubuntu.com/server/docs)
- [Nginx Documentation](https://nginx.org/en/docs/)
- [PM2 Documentation](https://pm2.keymetrics.io/docs/)
- [Let's Encrypt Documentation](https://letsencrypt.org/docs/)
- [DigitalOcean Community Tutorials](https://www.digitalocean.com/community/tutorials)

### Komunitas
- [Dalang.io Community Forum](https://forum.dalang.io)
- [Dalang.io Discord](https://dalang.io/discord)
- [Ubuntu Forum](https://ubuntuforums.org)
- [Stack Overflow](https://stackoverflow.com)
- [Reddit r/webdev](https://reddit.com/r/webdev)

---

## Kesimpulan

Dalam tutorial ini, kamu sudah belajar:

1. ✅ Cara order dan setup VPS di Dalang.io
2. ✅ Cara install dan setup **Dalang CLI**
3. ✅ Cara connect ke VPS via **Dalang CLI** (mudah & cepat!)
4. ✅ Cara install software yang diperlukan
5. ✅ Cara deploy aplikasi (Node.js, Python, atau PHP)
6. ✅ Cara setup reverse proxy dengan Nginx
7. ✅ Cara setup domain dan SSL
8. ✅ Cara monitor dan maintain server dengan Dalang CLI

**Selamat!** Kamu sekarang sudah bisa deploy aplikasi web ke VPS Dalang.io dengan mudah menggunakan **Dalang CLI**! 🎉

### Quick Reference - Dalang CLI Commands

```bash
# Install
curl -fsSL https://dalang.io/install.sh | bash

# Login
dalang auth

# List VPS
dalang service list

# Connect ke VPS
dalang shell <nama-vps>

# Check info
dalang service info <nama-vps>

# Start/Stop VPS
dalang start <nama-vps>
dalang stop <nama-vps>

# Check credit
dalang credit

# Domain management
dalang domain add <vps> <domain>
```

Jika ada pertanyaan atau masalah, jangan ragu untuk:
- Contact Dalang.io support (24/7)
- Check dokumentasi lengkap di [dalang.io/docs](https://dalang.io/docs)
- Bergabung dengan komunitas Dalang.io
- Baca [Dalang CLI documentation](https://dalang.io/cli)

**Happy Deploying dengan Dalang CLI!** 🚀
