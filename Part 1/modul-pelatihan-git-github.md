# Modul Pelatihan: Git dan GitLab

## Ringkasan
Modul ini membahas dasar Git dan GitLab untuk peserta pemula hingga menengah. Fokus utama adalah memahami konsep, alur kerja, dan praktik kolaborasi dasar yang relevan untuk individu maupun tim kecil.

## Tujuan Pembelajaran
Setelah pelatihan, peserta mampu:
- Menjelaskan konsep version control dan manfaatnya.
- Menggunakan Git untuk membuat repo, melacak perubahan, dan mengelola riwayat.
- Menerapkan workflow Git sederhana dengan branch, merge, dan resolusi konflik.
- Menggunakan fitur inti GitLab: repository, issues, merge request, dan kolaborasi.
- Memahami perbedaan Git vs GitLab serta opsi hosting Git lain.
- Memilih pendekatan merge (merge commit, squash, rebase) sesuai kebutuhan.
- Menulis dokumentasi dan komunikasi teknis dasar dengan Markdown.

## Target Peserta
- Mahasiswa, junior developer, atau anggota tim non-teknis yang perlu memahami Git/GitLab.

## Durasi Rekomendasi
- 2 jam (120 menit).

## Agenda 2 Jam (Ringkas)
- 0-10: Pembukaan, tujuan, dan konsep version control.
- 10-30: Git dasar dan Git sebagai dokumentasi.
- 30-50: Perintah inti + demo `git log`.
- 50-65: Branching dan konflik (demo cepat).
- 65-85: GitLab dasar (repo, issue, MR).
- 85-100: Merge strategy, Actions (intro), dan Markdown.
- 100-120: Latihan cepat, recap, dan kuis singkat.

## Prasyarat
- Mampu menggunakan komputer dasar.
- Pernah menggunakan terminal/command prompt (minimal). Jika belum, sediakan waktu 15-20 menit pengenalan.

## Perlengkapan
- Git terinstal.
- Akun GitLab.
- VS Code atau IDE lain.

---

# A. Git

## 1. Apa itu Version Control dan Pentingnya
- Definisi: sistem untuk melacak perubahan pada kode atau dokumen dari waktu ke waktu.
- Manfaat: histori perubahan, kolaborasi, rollback, dan mengurangi risiko konflik serta kehilangan data.
- Analogi: dokumentasi otomatis berbasis perubahan, bukan folder manual.

**Latihan singkat**
- Diskusikan 3 masalah yang muncul bila bekerja tanpa version control.

## 2. Apa itu Git dan Alternatifnya
- Git adalah sistem version control terdistribusi (DVCS).
- Alternatif umum: Subversion (SVN), Mercurial, Perforce.
- Kapan memilih Git: mayoritas proyek modern, kolaborasi lintas tim, histori lengkap lokal.

## 3. Git sebagai Dokumentasi Kode
- Commit adalah snapshot perubahan pada repo.
- Commit yang konsisten membentuk cerita evolusi proyek.
- Riwayat commit menjadi dokumentasi perubahan dibanding folder versi manual.

**Contoh praktik**
- Bandingkan: Folder `v1`, `v2`, `v3` vs histori commit yang bisa ditelusuri.

## 4. Konsep Dasar Git
- Repository: tempat menyimpan histori.
- Commit: snapshot perubahan dengan metadata.
- Branch: jalur pengembangan terpisah.
- Merge: menggabungkan perubahan dari branch lain.
- Remote: repo jarak jauh untuk kolaborasi.
- .gitignore: daftar file yang diabaikan Git (misal build, cache, env).

## 5. Git Workflow dan Dampaknya pada Cara Kerja
- Alur umum: buat branch -> ubah -> commit -> push -> pull request -> review -> merge.
- Dampak: perubahan terisolasi, review lebih mudah, dan integrasi lebih aman.

## 6. Perintah Git Paling Sering Dipakai (Individu/Tim Kecil)
- `git init`: membuat repo baru.
- `git clone`: menyalin repo.
- `git status`: mengecek status perubahan.
- `git add`: menaruh perubahan ke staging.
- `git commit`: menyimpan snapshot.
- `git log`: melihat histori commit.
- `git branch` / `git switch`: membuat atau berpindah branch.
- `git checkout`: cara lama yang masih sering ditemui untuk berpindah branch.
- `git merge`: menggabungkan branch.
- `git pull`: mengambil perubahan dari remote.
- `git push`: mengirim perubahan ke remote.
- `git remote -v`: melihat remote.

**Latihan singkat**
- Buat repo lokal, lakukan 2-3 commit kecil, tampilkan `git log`.

## 7. Git di Terminal/Bash vs GUI
- Terminal memberikan akses penuh ke fitur Git.
- GUI memudahkan visualisasi dan staging.
- Contoh GUI: GitKraken, Sourcetree, VS Code Source Control.

**Latihan singkat**
- Lakukan commit di terminal, lalu lihat hasilnya di GUI.

## 8. Konvensi Commit
- Commit harus singkat, deskriptif, dan mewakili satu unit perubahan.
- Gunakan gaya kalimat perintah (imperatif) dan fokus pada tujuan perubahan.
- Hindari commit terlalu besar atau mencampur banyak hal.

**Contoh**
- `add login page layout`
- `fix null check on user profile`

## 9. Branching dan Conflict
- Branch dipakai untuk memisahkan fitur/perbaikan.
- Conflict terjadi saat perubahan pada baris yang sama.
- Resolusi konflik: edit file, pilih perubahan yang benar, `git add`, lalu `git merge --continue`.

**Latihan singkat**
- Buat dua branch yang mengubah baris sama dan lakukan merge untuk memunculkan konflik.

## 10. Git Log
- `git log` menampilkan histori commit.
- Gunakan untuk menelusuri perubahan dan memahami evolusi proyek.

## 11. Git Blame
- `git blame` menandai setiap baris dengan commit terakhir yang mengubahnya.
- Berguna untuk audit perubahan dan konteks diskusi.

## 12. Git di VS Code atau IDE
- VS Code memiliki Source Control bawaan: staging, commit, branch, diff, dan conflict resolver.
- Visualisasi membantu review perubahan dan histori.

---

# B. GitLab

## 1. Perbedaan Git dan GitLab
- Git: tool version control.
- GitLab: platform hosting repo Git dan kolaborasi berbasis cloud.

## 2. Alternatif GitLab
- GitHub, Bitbucket, Azure Repos.
- Pilih sesuai kebutuhan organisasi, integrasi, dan kontrol akses.

## 3. Fitur Dasar GitLab
- Repository management.
- Issues untuk pencatatan tugas/bug.
- Boards untuk papan perencanaan kerja berbasis issue/MR.
- Branch, commit, dan merge request.
- CI/CD (pipelines) untuk otomatisasi build/test/deploy.
- Kolaborasi dan notifikasi.

## 4. Konsep Local vs Remote dan Git GUI
- Repo lokal berada di komputer pengguna.
- Remote repo berada di server (GitLab).
- GUI seperti GitKraken/Sourcetree/VS Code membantu operasi Git umum (clone, commit, push, MR).

## 5. GitLab Issues
- Digunakan untuk mencatat ide, tugas, bug, atau diskusi.
- Mendukung label, assignee, dan keterkaitan dengan MR.

## 6. GitLab Merge Request
- MR adalah proposal untuk menggabungkan perubahan dari branch ke branch lain.
- Dapat di-review, dikomentari, dan direvisi sebelum merge.

## 7. GitLab CI/CD (Pengantar)
- Otomatisasi workflow seperti build, test, dan deploy langsung di repo.
- Pipeline didefinisikan dalam file `.gitlab-ci.yml`.

## 8. GitLab Forking
- Fork adalah salinan repo ke akun lain.
- Memungkinkan kontribusi tanpa akses langsung ke repo utama.

## 9. Panduan Branching, Issue, dan MR (Ringkas)
- Buat issue untuk mendefinisikan pekerjaan.
- Buat branch dari issue.
- Commit perubahan kecil dan fokus.
- Buka MR, lakukan review, dan merge.

## 10. Squash vs Merge vs Rebase
- Merge commit: mempertahankan histori lengkap dari branch.
- Squash merge: menggabungkan banyak commit menjadi satu.
- Rebase merge: menyusun ulang commit agar histori linear.
- Pilih sesuai kebutuhan: audit detail vs histori ringkas.

## 11. Bonus: Markdown
- Markdown dipakai untuk README, issue, MR, dan dokumentasi.
- Syntax dasar: heading, list, code block, link, task list.

---

# Latihan Praktik (Versi 2 Jam)

## Latihan A: Git Lokal Cepat (15 menit)
1. `git init` repo baru.
2. Buat file `README.md`.
3. `git add` dan `git commit`.
4. Ubah file, commit lagi.
5. Lihat `git log`.

## Latihan B: GitLab Flow Ringkas (25 menit)
1. Push repo ke GitLab.
2. Buat issue.
3. Buat branch dan commit.
4. Push branch, buka MR.
5. Lakukan review dan merge.

## Opsional (Jika Waktu Cukup)
- Demo konflik singkat di satu file.
- Buat README sederhana dengan Markdown.

---

# Evaluasi
- Kuis singkat 5-10 menit: konsep Git, GitLab, workflow.
- Tugas lanjutan (opsional): kolaborasi dengan 1 rekan menggunakan branch dan MR.

---

# Referensi
- https://git-scm.com/docs/git-log
- https://git-scm.com/docs/git-blame
- https://git-scm.com/docs/git-branch
- https://git-scm.com/docs/git-merge
- https://git-scm.com/docs/git-rebase
- https://code.visualstudio.com/docs/sourcecontrol/overview
- https://docs.gitlab.com/ee/
- https://docs.gitlab.com/ee/user/project/
- https://docs.gitlab.com/ee/user/project/issues/
- https://docs.gitlab.com/ee/user/project/merge_requests/
- https://docs.gitlab.com/ee/ci/
- https://docs.gitlab.com/ee/user/project/repository/
- https://docs.gitlab.com/ee/user/project/issues/issue_board.html
- https://docs.gitlab.com/ee/user/ssh.html
- https://docs.gitlab.com/ee/user/profile/personal_access_tokens.html
- https://www.atlassian.com/software/bitbucket/guides/getting-started/overview
- https://learn.microsoft.com/en-us/azure/devops/repos/
- https://azure.microsoft.com/products/devops/repos/
