# 00 - Prasyarat

Tujuan modul:
- memastikan Git terinstall
- memahami konfigurasi dasar
- memahami konsep repository, working tree, staging area, commit, branch, remote

Langkah 1: cek Git

```bash
git --version
```

Jika belum terinstall, install dulu sesuai OS:
- Windows: https://git-scm.com/download/win
- macOS: `brew install git`
- Ubuntu/Debian: `sudo apt install git`

Langkah 2: set konfigurasi user

```bash
git config --global user.name "Nama Anda"
git config --global user.email "email@example.com"
```

Cek konfigurasi:

```bash
git config --global --list
```

Langkah 3: buat folder kerja

```bash
mkdir latihan-git
cd latihan-git
```

Jika repo ini sudah diclone, lanjutkan ke langkah 4. Jika belum, clone repo:

```bash
git clone https://github.com/ucay/belajar-git.git
cd belajar-git
```

Langkah 4: cek status

```bash
git status
```

Langkah 5: pahami konsep dasar

- repository = folder project yang dilacak Git
- working directory = file yang sedang Anda edit
- staging area = area persiapan sebelum commit
- commit = snapshot permanen dari perubahan
- branch = jalur pengembangan terpisah
- remote = repo lain yang tersambung (misalnya GitHub)

Tugas latihan:
- buat folder `workspace/<username>` jika belum ada
- buat file kecil seperti `workspace/<username>/notes.txt`
- isi 3 baris tentang apa yang Anda pahami tentang Git
- git add, git commit, lalu push ke branch Anda

Tips:
- gunakan `git status` sebelum dan sesudah operasi Git
- commit yang baik biasanya berisi satu tujuan perubahan

Kriteria sukses:
- konfigurasi user sudah benar
- status repo bersih atau siap untuk perubahan
- memahami perbedaan repo lokal vs repo remote
