# 03 - Remote, Fetch, Pull, Push

Tujuan modul:
- memahami remote repository
- bisa fetch, pull, dan push perubahan
- memahami tracking branch dan upstream

Cek remote:

```bash
git remote -v
```

Fetch perubahan dari remote tanpa mengubah workspace:

```bash
git fetch origin
```

Pull perubahan dari branch tertentu:

```bash
git pull origin main
```

Push branch ke remote:

```bash
git checkout -b feature/<username>/03-remote
# buat file perubahan

git add .
git commit -m "add remote practice notes"
git push -u origin feature/<username>/03-remote
```

Tugas latihan:
- buat folder `workspace/<username>/remote-practice/`
- buat file `notes.txt` di dalamnya
- tulis ringkasan cara kerja fetch, pull, dan push
- commit dan push ke branch Anda

Praktik kolaborasi:
- salah satu peserta buat perubahan di main
- peserta lain lakukan `git fetch origin` dan `git status`
- lakukan `git pull --rebase origin main` atau `git pull origin main` lalu bandingkan hasilnya

Tips:
- `git fetch` biasanya lebih aman sebelum `git merge` atau `git rebase`
- `git pull` adalah gabungan `fetch + merge`
- `git push -u origin <branch>` membuat tracking upstream

Kriteria sukses:
- bisa melihat remote
- bisa fetch
- bisa pull
- bisa push branch baru
