# 04 - Branching dan Checkout

Tujuan modul:
- memahami branch secara praktis
- belajar `git branch`, `git checkout`, `git switch`
- memisahkan pekerjaan per fitur

Membuat branch baru:

```bash
git branch
git checkout -b feature/<username>/04-branching
# atau
# git switch -c feature/<username>/04-branching
```

Pindah ke branch lain:

```bash
git checkout main
git checkout feature/<username>/04-branching
```

Contoh alur kerja:

```bash
git checkout main
git pull origin main
git checkout -b feature/<username>/04-branching
# edit file

git add .
git commit -m "add branch example"
git push -u origin feature/<username>/04-branching
```

Tugas latihan:
- buat file `workspace/<username>/04-branch-notes.md`
- tulis perbedaan branch utama vs branch fitur
- commit dan push ke branch baru

Tips:
- tiap fitur sebaiknya dibuat di branch sendiri
- nama branch sebaiknya singkat dan deskriptif
- branch utama biasanya `main` atau `master`

Kriteria sukses:
- bisa membuat branch baru
- bisa berpindah antar branch
- bisa push perubahan ke branch tertentu
