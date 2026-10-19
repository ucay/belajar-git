warning: in the working copy of 'latihan-module-06/README.md', LF will be replaced by CRLF the next time Git touches it
[1mdiff --git a/latihan-module-06/README.md b/latihan-module-06/README.md[m
[1mindex 4b045be..c99baef 100644[m
[1m--- a/latihan-module-06/README.md[m
[1m+++ b/latihan-module-06/README.md[m
[36m@@ -1,49 +1 @@[m
[31m-﻿# 06 - Rebase dan Cherry Pick[m
[31m-[m
[31m-Tujuan modul:[m
[31m-- memahami rebase[m
[31m-- memahami cherry-pick[m
[31m-- belajar cara menyusun history commit agar lebih rapi[m
[31m-[m
[31m-Rebase dasar:[m
[31m-[m
[31m-```bash[m
[31m-git checkout feature/<username>/06-rebase[m
[31m-git rebase main[m
[31m-```[m
[31m-[m
[31m-Jika conflict terjadi, selesaikan seperti merge conflict, lalu:[m
[31m-[m
[31m-```bash[m
[31m-git add <file>[m
[31m-git rebase --continue[m
[31m-```[m
[31m-[m
[31m-Interactive rebase (opsional):[m
[31m-[m
[31m-```bash[m
[31m-git rebase -i HEAD~3[m
[31m-```[m
[31m-[m
[31m-Pilih `pick`/`squash` sesuai kebutuhan.[m
[31m-[m
[31m-Cherry-pick commit tertentu:[m
[31m-[m
[31m-```bash[m
[31m-git log --oneline[m
[31m-git cherry-pick <commit-sha>[m
[31m-```[m
[31m-[m
[31m-Tugas latihan:[m
[31m-- buat beberapa commit kecil di branch Anda[m
[31m-- lalu pakai `git rebase -i HEAD~3` untuk squash commit[m
[31m-- kalau ada commit yang bagus dari branch lain, lakukan `git cherry-pick <sha>`[m
[31m-[m
[31m-Tips:[m
[31m-- rebase mengubah history commit, jadi hindari rebase pada branch yang sudah dibagikan ke banyak orang[m
[31m-- jika branch masih local dan belum dipush bersama, rebase aman dipakai[m
[31m-[m
[31m-Kriteria sukses:[m
[31m-- memahami rebase[m
[31m-- bisa resolve konflik saat rebase[m
[31m-- bisa menyalin commit dengan cherry-pick[m
[32m+[m[32m﻿TEST 0666[m
