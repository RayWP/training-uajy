# Panduan Pengajar: Git dan GitHub

## Tujuan Pengajar
- Menyampaikan konsep Git/GitHub secara bertahap dan praktis.
- Menjamin peserta mampu melakukan workflow dasar dengan percaya diri.
- Mendorong kolaborasi sehat melalui issue dan pull request.

## Profil Peserta
- Pemula hingga menengah.
- Bisa berbeda latar: mahasiswa, staf non-teknis, atau developer junior.

## Persiapan Teknis
- Pastikan Git terinstal dan berjalan (`git --version`).
- Pastikan setiap peserta memiliki akun GitHub.
- Siapkan repo latihan (public) dan materi contoh.
- Pastikan koneksi internet stabil.

## Struktur Sesi (Versi 2 Jam)
- 0-10: Pembukaan, tujuan, dan konsep version control.
- 10-30: Git dasar + Git sebagai dokumentasi.
- 30-50: Perintah inti + demo `git log`.
- 50-65: Branching dan konflik (demo cepat).
- 65-85: GitHub dasar (repo, issue, PR).
- 85-100: Merge strategy, Actions (intro), dan Markdown.
- 100-120: Latihan cepat, recap, dan kuis singkat.

## Strategi Mengajar
- Mulai dari masalah nyata: file versi manual vs histori Git.
- Demo singkat (5-7 menit), lalu praktik mandiri.
- Gunakan contoh konflik sederhana untuk menunjukkan nilai Git.
- Tekankan alasan, bukan hanya perintah.

## Rencana Detail Mengajar

### A. Git
1. Version control dan pentingnya
- Cerita awal: 3 folder versi file yang membingungkan.
- Hubungkan ke histori commit.

2. Apa itu Git dan alternatifnya
- Jelaskan Git sebagai DVCS.
- Beri contoh alternatif (SVN, Mercurial, Perforce) agar peserta paham ekosistem.

3. Git sebagai dokumentasi
- Tunjukkan `git log` sebagai audit trail.

4. Konsep dasar Git
- Repo, commit, branch, merge, remote.
- Visualisasi sederhana di papan.

5. Workflow Git
- Diagram: branch -> commit -> push -> PR -> merge.
- Hubungkan dengan kebiasaan kerja tim.

6. Perintah umum
- Fokus pada 10-12 perintah inti.
- Jangan overload dengan perintah langka.

7. Terminal vs GUI
- Demo commit di terminal, tampilkan hasil di GitHub Desktop atau VS Code.

8. Konvensi commit
- Tekankan commit kecil, deskriptif.

9. Branching dan conflict
- Buat konflik terencana.
- Latih cara menyelesaikan konflik.

10. Git log dan git blame
- Jelaskan kapan dipakai untuk audit.

11. Git di VS Code/IDE
- Perlihatkan staging, diff, dan merge tool.

### B. GitHub
1. Git vs GitHub
- Tekankan Git = alat, GitHub = platform.

2. Alternatif GitHub
- Sebutkan GitLab, Bitbucket, Azure Repos.

3. Fitur dasar GitHub
- Repo, issue, PR, review.

4. Local vs remote dan GitHub Desktop
- Jelaskan arah data: push dan pull.

5. Issues
- Biasakan membuat issue sebelum coding.

6. Pull request
- Simulasikan review sederhana.

7. GitHub Actions (intro)
- Tunjukkan contoh workflow sederhana (build/test).

8. Forking
- Jelaskan konsep kontribusi open source.

9. Panduan branch-issue-PR
- Beri contoh langkah dan naming branch.

10. Squash vs merge vs rebase
- Jelaskan dampak histori.
- Diskusikan kapan masing-masing dipakai.

11. Markdown
- Ajak peserta membuat README sederhana.

## Aktivitas Kelas (2 Jam)
- Latihan cepat Git lokal (15 menit).
- GitHub flow ringkas (25 menit).
- Quiz 5-10 menit: konsep Git, GitHub, workflow.

## Rubrik Penilaian (Ringkas, 2 Jam)
- Git lokal: repo, commit, log (40%).
- GitHub flow: issue, branch, PR, merge (50%).
- Markdown README (10%).

## Pertanyaan Pemantik
- Mengapa menyimpan banyak folder versi itu berisiko?
- Kapan kita butuh `git blame`?
- Mengapa PR penting walau tim kecil?

## Kesalahan Umum dan Cara Mengatasinya
- Lupa staging (`git add`) sebelum commit.
- Commit terlalu besar dan tidak fokus.
- Menyelesaikan konflik tanpa memahami konteks.
- Membuat PR tanpa issue atau deskripsi.

## Checklist Akhir Sesi
- Peserta mampu membuat repo lokal dan melakukan commit.
- Peserta paham branch dan merge.
- Peserta bisa membuat PR di GitHub.
- Peserta memahami perbedaan Git vs GitHub.
- Peserta mampu menulis README sederhana dengan Markdown.

## Catatan untuk PPT
- Buat visual sederhana: alur workflow, diagram local vs remote.
- Gunakan contoh kecil dan nyata untuk memudahkan pemahaman.

---

# Referensi
- https://github.com/git-guides
- https://github.com/resources/articles/what-is-version-control
- https://learn.microsoft.com/en-us/training/paths/github-foundations/
- https://learn.microsoft.com/en-us/training/paths/github-foundations-2/
- https://learn.microsoft.com/en-us/training/modules/introduction-to-github/
- https://learn.microsoft.com/en-us/training/modules/intro-to-git/
- https://learn.microsoft.com/en-us/training/modules/manage-changes-pull-requests-github/
- https://docs.github.com/en/issues/tracking-your-work-with-issues/learning-about-issues/about-issues
- https://docs.github.com/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/about-pull-requests
- https://docs.github.com/articles/about-forks
- https://docs.github.com/en/actions
- https://docs.github.com/articles/about-merge-methods-on-github/
- https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax
- https://git-scm.com/docs/git-log
- https://git-scm.com/docs/git-blame
- https://git-scm.com/docs/git-branch
- https://git-scm.com/docs/git-merge
- https://git-scm.com/docs/git-rebase
- https://docs.github.com/en/desktop
- https://code.visualstudio.com/docs/sourcecontrol/overview
- https://docs.gitlab.com/ee/user/project/repository/
- https://www.atlassian.com/software/bitbucket/guides/getting-started/overview
- https://learn.microsoft.com/en-us/azure/devops/repos/
- https://azure.microsoft.com/products/devops/repos/
