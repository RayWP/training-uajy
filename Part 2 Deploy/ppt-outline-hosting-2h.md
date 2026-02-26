# Outline PPT: Dasar Hosting Web (Fokus VPS)

## Panduan Waktu
- Total: 120 menit.
- Slide 1-3: 10 menit.
- Slide 4-13: 40 menit.
- Slide 14-24: 45 menit.
- Slide 25-27: 20 menit.
- Slide 28: 5 menit.

## Slide-by-Slide

1. Sampul
Durasi: 1 menit
Tujuan: Membuka sesi dan konteks pelatihan.
Konten: Judul, nama pengajar, tanggal.

2. Tujuan Pembelajaran
Durasi: 2 menit
Tujuan: Menyelaraskan ekspektasi.
Konten: 5-6 tujuan utama sesi.

3. Agenda 2 Jam
Durasi: 2 menit
Tujuan: Memberi peta waktu.
Konten: Alur topik dan latihan.

4. Apa Itu Hosting
Durasi: 4 menit
Tujuan: Definisi dan analogi sederhana.
Konten: Hosting = menyewa server yang selalu aktif.

5. Mengapa Butuh Hosting
Durasi: 4 menit
Tujuan: Menjelaskan manfaat.
Konten: Akses 24/7, domain, resource, deployment.

6. Istilah Dasar: Server, Domain, DNS
Durasi: 5 menit
Tujuan: Memahami istilah inti.
Konten: Server, domain, DNS, IP.

7. Istilah Dasar: HTTP/HTTPS, SSL
Durasi: 4 menit
Tujuan: Memahami keamanan web.
Konten: HTTP vs HTTPS, TLS/SSL.

8. Istilah Dasar: Bandwidth, Latency, Uptime
Durasi: 4 menit
Tujuan: Memahami performa.
Konten: Bandwidth, latency, uptime.

9. Jenis Hosting: Shared
Durasi: 3 menit
Tujuan: Memahami opsi termurah.
Konten: Kelebihan/kekurangan.

10. Shared Hosting dan cPanel (Gambaran Umum)
Durasi: 4 menit
Tujuan: Memahami cara kerja shared hosting.
Konten: Resource bersama, akses cPanel, menu penting.

11. Jenis Hosting: VPS (Fokus)
Durasi: 5 menit
Tujuan: Memahami VPS.
Konten: VM, kontrol, resource.

12. PaaS vs IaaS
Durasi: 4 menit
Tujuan: Memahami level pengelolaan.
Konten: Contoh PaaS vs IaaS.

13. Contoh Provider (Indonesia)
Durasi: 4 menit
Tujuan: Memberi konteks lokal.
Konten: Shared & VPS populer.

14. Hosting “Biologi”
Durasi: 4 menit
Tujuan: Menjelaskan arsitektur.
Konten: Reverse proxy, app, DB, storage, dan contoh stack shared hosting.

15. Diagram Alur Request
Durasi: 4 menit
Tujuan: Visualisasi request.
Konten: User → DNS → proxy → app → DB.

16. Reverse Proxy
Durasi: 4 menit
Tujuan: Fungsi Nginx.
Konten: Routing dan SSL termination.

17. App Server
Durasi: 4 menit
Tujuan: Menjalankan backend.
Konten: Node.js/Python/PHP.

18. Database
Durasi: 4 menit
Tujuan: Menyimpan data.
Konten: MySQL/PostgreSQL.

19. Storage & CDN
Durasi: 3 menit
Tujuan: File statis dan percepatan.
Konten: Storage + CDN.

20. Frontend vs Backend Hosting
Durasi: 5 menit
Tujuan: Bedakan kebutuhan.
Konten: Static vs dynamic.

21. Hosting AI App (Ringkas)
Durasi: 4 menit
Tujuan: Memahami dua skenario AI hosting.
Konten: API wrapper vs inference engine, tips singkat.
Catatan: Tekankan perbedaan kebutuhan resource, biaya, dan latency. Sarankan rate limit + cache untuk API wrapper, serta GPU + queue untuk inference engine.

22. Studi Kasus: Portfolio
Durasi: 4 menit
Tujuan: Pilih hosting tepat.
Konten: Shared/PaaS frontend.

23. Studi Kasus: Web App UMKM
Durasi: 5 menit
Tujuan: Pilih hosting tepat.
Konten: VPS atau PaaS backend.

24. Latihan: Pilih Hosting
Durasi: 5 menit
Tujuan: Praktik keputusan.
Konten: 2 skenario dan diskusi.

25. Latihan: Pemetaan Istilah
Durasi: 5 menit
Tujuan: Menguatkan istilah.
Konten: Match istilah ke fungsi.

26. Recap
Durasi: 3 menit
Tujuan: Menutup materi utama.
Konten: Ringkasan 5 poin.

27. Q&A
Durasi: 5 menit
Tujuan: Menjawab pertanyaan.
Konten: Diskusi.

28. Penutup & Referensi
Durasi: 2 menit
Tujuan: Arah belajar lanjut.
Konten: Link referensi.

---

# Catatan Presentasi
- Gunakan analogi sederhana untuk DNS dan server.
- Sisipkan diagram arsitektur agar mudah dipahami.
- Fokus pada VPS sebagai target utama.

# Referensi
- https://nginx.org/en/
- https://www.cloudflare.com/learning/
- https://developer.mozilla.org/en-US/docs/Web/HTTP
