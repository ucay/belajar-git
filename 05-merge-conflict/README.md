# 05 - Merge Conflict

Tujuan modul:
- memahami cara kerja merge
- belajar cara menanggulangi konflik saat merge
- memahami pentingnya resolve konflik dengan hati-hati

Skenario latihan:
- semua peserta akan mengedit file yang sama di `shared/team-notes.md`
- file ini berisi beberapa baris teks yang akan diubah oleh setiap peserta
- saat branch di-merge, kemungkinan akan muncul conflict

Langkah 1: masuk ke shared folder

```bash
cd shared
```

Buat file `team-notes.md` jika belum ada:

```bash
cat > team-notes.md <<'EOF'
Catatan Tim Git
1. Setup repo
2. Commit perubahan
3. Review dan merge
EOF
```

Langkah 2: tiap peserta buat branch

```bash
git checkout -b feature/<username>/05-merge-conflict
```

Edit file `shared/team-notes.md` dengan cara berbeda, misalnya:

- ucay menulis: "ucay menambahkan catatan pengalaman awal"
- peserta lain menulis: "peserta lain menambahkan catatan proses belajar"

Commit perubahan masing-masing:

```bash
git add shared/team-notes.md
git commit -m "update team notes"
```

Push branch masing-masing:

```bash
git push -u origin feature/<username>/05-merge-conflict
```

Langkah 3: merge branch ke main

- salah satu peserta membuat PR dan merge ke `main`
- peserta lain pull `main` lalu merge branch masing-masing

```bash
git checkout main
git pull origin main
git checkout feature/<username>/05-merge-conflict
git merge main
```

Jika ada conflict, buka file:

```bash
cat shared/team-notes.md
```

Cari marker konflik seperti:

```text
<<<<<<< HEAD
...
=======
...
>>>>>>> feature/...
```

Edit file sehingga isinya final dan benar. Setelah itu:

```bash
git add shared/team-notes.md
git commit -m "resolve merge conflict in team notes"
git push
```

Tips:
- baca seluruh konflik dengan hati-hati
- jangan hapus bagian yang benar hanya karena masih konflik
- gunakan `git status` untuk melihat file yang masih bermasalah

Kriteria sukses:
- memahami kondisi konflik
- bisa membaca marker konflik
- bisa resolve file yang konflik
- bisa lanjutkan commit dan push
