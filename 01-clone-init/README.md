# 01 - Clone dan Init

Tujuan modul:
- memahami cara clone repo dari remote
- memahami repo yang baru dibuat dengan `git init`
- memahami `git status` dan `git log`

Bagian A: clone repo yang sudah ada

```bash
git clone https://github.com/ucay/belajar-git.git
cd belajar-git
```

Cek status:

```bash
git status
git log --oneline --graph --decorate --all
```

Bagian B: buat repo baru dengan init

```bash
mkdir demo-repo
demo-repo

git init
```

Buat file awal:

```bash
echo "Belajar Git" > README.md
git status
git add README.md
git commit -m "initial commit"
```

Tugas latihan:
- di repo ini, buat file `workspace/<username>/01-clone-notes.md`
- isi dengan 3-5 baris mengenai pengalaman awal Anda saat melihat repo ini
- jalankan:

```bash
git add workspace/<username>/01-clone-notes.md
git commit -m "add notes for clone module"
```

Push ke branch Anda:

```bash
git checkout -b feature/<username>/01-clone-init
git push -u origin feature/<username>/01-clone-init
```

Tips:
- `git status` membantu melihat apakah file sudah diubah atau belum
- `git log` membantu melihat sejarah commit

Kriteria sukses:
- bisa clone repo
- bisa membuat repo baru dengan `git init`
- bisa melihat `git log`
- bisa commit dan push ke branch baru
