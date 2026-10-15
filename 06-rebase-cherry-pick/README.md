# 06 - Rebase dan Cherry Pick

Tujuan modul:
- memahami rebase
- memahami cherry-pick
- belajar cara menyusun history commit agar lebih rapi

Rebase dasar:

```bash
git checkout feature/<username>/06-rebase
git rebase main
```

Jika conflict terjadi, selesaikan seperti merge conflict, lalu:

```bash
git add <file>
git rebase --continue
```

Interactive rebase (opsional):

```bash
git rebase -i HEAD~3
```

Pilih `pick`/`squash` sesuai kebutuhan.

Cherry-pick commit tertentu:

```bash
git log --oneline
git cherry-pick <commit-sha>
```

Tugas latihan:
- buat beberapa commit kecil di branch Anda
- lalu pakai `git rebase -i HEAD~3` untuk squash commit
- kalau ada commit yang bagus dari branch lain, lakukan `git cherry-pick <sha>`

Tips:
- rebase mengubah history commit, jadi hindari rebase pada branch yang sudah dibagikan ke banyak orang
- jika branch masih local dan belum dipush bersama, rebase aman dipakai

Kriteria sukses:
- memahami rebase
- bisa resolve konflik saat rebase
- bisa menyalin commit dengan cherry-pick
