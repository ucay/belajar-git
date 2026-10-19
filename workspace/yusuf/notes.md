 1. Setup Awal
- `git config`: Pasang nama dan email pembuat kode.
- `git --version`: Cek apakah Git sudah terpasang.

 2. Memulai Proyek
- `git init`: Ubah folder biasa jadi folder proyek Git.
- `git clone`: Download proyek dari internet (GitHub) ke laptop.
- `git status`: Cek file apa saja yang baru diubah atau belum disimpan.
- `git log`: Buku harian untuk melihat riwayat perubahan dari awal.

 3. Menyimpan Perubahan
- `git add`: Masukkan file editan ke kantong persiapan (-staging-).
- `git diff`: Intip beda ketikan kodingan lama vs kodingan baru.
- `git commit -m`: Titik penyimpanan resmi (-save point-) beserta pesan perubahannya.
- `git commit --amend`: Edit pesan atau selipkan file kelupaan ke commit terakhir.

 4. Sinkronisasi Internet
- `git remote`: Sambungkan folder laptop dengan server online (GitHub/GitLab).
- `git fetch`: Cek dan intip update terbaru dari internet tanpa mengubah file lokal.
- `git pull`: Download dan langsung gabungkan update terbaru ke file laptop.
- `git push`: Upload hasil commit laptop ke internet.

 5. Cabang Kerja (Branch)
- `git branch`: Buat cabang kerja terpisah agar kode utama tidak berantakan.
- `git switch` / `git checkout`: Berpindah ruangan antar-cabang kerja.
- `git merge`: Satukan kembali hasil kerja cabang fitur ke cabang utama.

 6. Tabrakan Kode (Conflict)
- Penyebab: Dua orang mengedit baris yang sama di file yang sama.
- Solusi: Buka file, pilih kode yang mau dipakai, hapus penanda bentrok Git, lalu commit ulang.

 7. Rapikan & Ambil Pilihan
- `git rebase`: Geser pangkal cabang fitur ke ujung terbaru cabang utama biar jalurnya lurus rapi.
- `git cherry-pick`: Comot hanya satu commit tertentu saja dari cabang lain.

 8. Tombol Darurat & Trik Cepat
- `git tag`: Tempel stiker versi rilis resmi (contoh: `v1.0.0`).
- `git reset`: Putar balik waktu dan hapus commit terakhir.
- `git revert`: Buat commit baru untuk membatalkan kesalahan (aman untuk branch publik).
- `git stash` / `stash pop`: Selipkan kerjaan belum selesai ke kantong sementara, lalu ambil lagi nanti.



MODUL YANG PALING SULIT :
Tidak ada

Cara Resolve Konflik yang paling membantu :

1. Git Revert
2. Git Stash
3. Git pull

Daftar Git Yang Sering Di Pakai

1. Git config
2. Git init
3. Git clone
4. Git push
5. Git pull
6. Git merge
7. Git log
8. Git stash
9. Git revert
