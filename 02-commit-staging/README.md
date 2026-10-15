# 02 - Commit dan Staging

Tujuan modul:
- memahami perbedaan working tree, staging area, dan commit
- belajar `git add`, `git diff`, `git commit`, `git commit --amend`

Konsep penting:

1. File dibuat atau diubah di working directory
2. File dijadikan siap commit dengan `git add`
3. File masuk ke commit dengan `git commit`

Contoh:

```bash
echo "baris pertama" >> workspace/<username>/commit-demo.txt
git status
git diff
```

Setelah yakin:

```bash
git add workspace/<username>/commit-demo.txt
git diff --cached
git commit -m "add commit demo file"
```

Latihan amend:

```bash
echo "baris tambahan" >> workspace/<username>/commit-demo.txt
git add workspace/<username>/commit-demo.txt
git commit --amend -m "add commit demo file with extra line"
```

Tugas latihan:
- buat file `workspace/<username>/02-commit-practice.md`
- buat minimal 3 paragraf singkat tentang manfaat commit yang rapi
- lakukan `git add` dan `git commit`
- buat satu commit tambahan untuk revisi kecil lalu gunakan `git commit --amend`

Tips:
- `git diff` melihat perubahan yang belum di-stage
- `git diff --cached` melihat perubahan yang sudah di-stage
- `git commit --amend` biasa dipakai untuk memperbaiki isi commit atau pesan commit

Kriteria sukses:
- memahami stage vs commit
- bisa membuat commit yang jelas
- bisa memperbaiki commit terakhir dengan amend
