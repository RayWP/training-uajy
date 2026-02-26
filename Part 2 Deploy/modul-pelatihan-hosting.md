# Modul Pelatihan: Dasar Hosting Web (Fokus VPS)

## Ringkasan
Modul ini membahas konsep hosting web dari nol: apa itu hosting, mengapa dibutuhkan, istilah-istilah dasar jaringan, jenis hosting (IaaS vs PaaS) dengan fokus pada VPS, hingga gambaran arsitektur layanan web dan perbedaan hosting frontend vs backend.

## Tujuan Pembelajaran
Setelah pelatihan, peserta mampu:
- Menjelaskan apa itu hosting dan mengapa dibutuhkan.
- Memahami istilah dasar: server, domain, DNS, IP, HTTP/HTTPS, SSL, bandwidth, latency.
- Membandingkan tipe hosting: shared, VPS, dan PaaS.
- Memahami komponen arsitektur hosting (reverse proxy, app server, database, storage).
- Membedakan kebutuhan hosting frontend dan backend.
- Menentukan pilihan hosting sederhana untuk kebutuhan kecil.

## Target Peserta
- Pemula yang ingin memahami dasar hosting web.

## Durasi Rekomendasi
- 2-3 jam.

## Prasyarat
- Pemahaman dasar internet dan website.

## Perlengkapan
- Laptop/PC.
- Koneksi internet.

---

# A. Konsep Dasar Hosting

## 1. Apa Itu Hosting
Hosting adalah layanan untuk menempatkan aplikasi/website agar bisa diakses publik melalui internet. Secara sederhana, hosting adalah "menyewa komputer server" yang selalu menyala.

## 2. Mengapa Kita Butuh Hosting
- Agar website bisa diakses 24/7.
- Memberikan alamat yang konsisten (domain) untuk diakses pengguna.
- Menyediakan resource (CPU, RAM, storage, bandwidth).
- Mempermudah kolaborasi dan deployment.

## 3. Istilah Dasar dalam Hosting
- **Server**: komputer yang melayani request.
- **Domain**: nama unik untuk mengakses website (contoh: `contoh.com`).
- **DNS**: sistem yang menerjemahkan domain ke IP.
- **IP Address**: alamat numerik server di internet.
- **HTTP/HTTPS**: protokol komunikasi web.
- **SSL/TLS**: enkripsi untuk HTTPS.
- **Bandwidth**: kapasitas transfer data.
- **Latency**: waktu tunda respons.
- **Uptime**: persentase waktu server aktif.

**Latihan singkat**
- Jelaskan perbedaan domain dan DNS dengan kata-kata sendiri.

---

# B. Jenis Hosting

## 4. Shared Hosting
- Banyak website berada di satu server.
- Paling murah, cocok untuk website kecil.
- Keterbatasan resource dan kontrol.

### Cara Kerja Shared Hosting (Ringkas)
- Resource server dibagi ke banyak akun.
- Provider mengelola server dan keamanan dasar.
- Pengguna fokus pada upload file dan konfigurasi aplikasi.

### cPanel (Gambaran Umum)
- **File Manager** untuk upload/edit file.
- **MySQL Databases** untuk membuat database dan user.
- **Domains/Subdomains** untuk mengatur domain.
- **SSL/TLS** untuk aktifkan HTTPS.
- **Email Accounts** untuk email hosting.

## 5. VPS (Virtual Private Server) – Fokus Utama
- Satu server fisik dibagi menjadi beberapa server virtual.
- Resource lebih terjamin dibanding shared hosting.
- Lebih fleksibel untuk setup aplikasi.
- Cocok untuk aplikasi yang berkembang.

## 6. PaaS vs IaaS (Ringkas)
- **IaaS**: Anda mengelola server sendiri (OS, security, aplikasi). VPS termasuk IaaS.
- **PaaS**: platform siap pakai untuk deploy tanpa mengelola server (lebih praktis, lebih mahal).

**Contoh PaaS**: Vercel, Render, Heroku.

## 7. Contoh Layanan Hosting (Umum di Indonesia)
**Shared Hosting**
- Niagahoster
- Rumahweb
- Dewaweb
- Qwords
- DomaiNesia

**VPS Hosting**
- IDCloudHost
- Biznet Gio
- Dewaweb VPS
- Rumahweb VPS
- Niagahoster VPS

**Global (juga populer di Indonesia)**
- DigitalOcean
- Linode
- Vultr
- AWS Lightsail

---

# C. Hosting “Biologi” (Arsitektur Dasar)

## 8. Komponen Umum dalam Hosting Web
- **Reverse Proxy** (contoh: Nginx): menerima request dan meneruskan ke app.
- **App Server**: menjalankan backend (Node.js, Python, PHP, dll).
- **Database**: menyimpan data (PostgreSQL, MySQL).
- **Storage**: menyimpan file statis (gambar, dokumen).
- **CDN** (opsional): mempercepat akses file statis.
- **Shared hosting stack**: satu server melayani banyak akun, web server bersama, database terpisah logis, dan control panel seperti cPanel.

**Ilustrasi sederhana**
Pengguna → DNS → Server → Reverse Proxy → App Server → Database

## 9. Frontend Hosting vs Backend Hosting
- **Frontend**: file statis (HTML, CSS, JS). Bisa di-host di CDN/PaaS.
- **Backend**: server aplikasi (API, logic, auth). Butuh runtime dan database.
- **Kebutuhan berbeda**: frontend fokus speed dan caching; backend fokus kestabilan dan security.

---

# D. Studi Kasus Sederhana

## 10. Studi Kasus: Website Portofolio
- Kebutuhan: halaman statis, traffic kecil.
- Rekomendasi: shared hosting atau PaaS frontend.

## 11. Studi Kasus: Web App UMKM
- Kebutuhan: login, data produk, database.
- Rekomendasi: VPS kecil (IaaS) atau PaaS backend.

---

# E. Latihan Praktik (Tanpa Deploy)

## Latihan 1: Pemetaan Istilah
- Pasangkan istilah dengan fungsinya (domain, DNS, IP, server, SSL).

## Latihan 2: Pilih Hosting
- Berikan 2 skenario dan minta peserta memilih hosting yang cocok.

---

# Evaluasi
- Kuis singkat: istilah dasar dan perbedaan jenis hosting.
- Diskusi: kapan memilih VPS vs PaaS.

---

# Referensi
- https://gitlab.com/gitlab-org/gitlab
- https://nginx.org/en/
- https://www.cloudflare.com/learning/
- https://developer.mozilla.org/en-US/docs/Web/HTTP
