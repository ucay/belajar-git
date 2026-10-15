# 08 - Final Project

Tujuan modul:
- menggabungkan seluruh konsep Git yang sudah dipelajari
- membuat project mini dengan workflow tim yang realistis

Langkah umum:

1. Buat branch baru:

```bash
git checkout -b feature/<username>/08-final-project
```

2. Di folder `workspace/<username>/`, buat file project mini seperti:
- `project-summary.md`
- `notes.md`
- `timeline.md`

3. Tulis ringkasan:
- apa yang Anda pelajari
- modul paling sulit
- cara resolve konflik yang Anda rasa paling membantu
- daftar perintah Git yang paling sering dipakai

4. Commit dan push:

```bash
git add workspace/<username>/
git commit -m "final project summary"
git push -u origin feature/<username>/08-final-project
```

5. Buat PR ke `main` dan lakukan review bersama tim

6. Setelah review, merge ke main

Tugas akhir:
- semua peserta menulis ringkasan belajar mereka
- buat PR masing-masing
- lakukan review antar peserta
- merge ke branch utama

Kriteria sukses:
- semua materi dasar sudah dipraktikkan
- punya pengalaman bekerja di branch dan review PR
- memahami alur kerja Git dalam tim
