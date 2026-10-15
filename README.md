# Belajar Git

Repo ini dibuat untuk belajar Git secara bertahap dan praktis dalam tim.

Tujuan:
- memahami konsep Git dasar
- latihan perintah Git secara nyata
- belajar kolaborasi tim: branch, merge, conflict, pull, push, tag, release
- mempunyai workspace untuk tiap peserta yang bisa dipakai dari awal hingga final project

Struktur repo:

- `00-prasyarat/` — setup awal, install, konfigurasi user, konsep dasar
- `01-clone-init/` — clone repo baru, init, status, log
- `02-commit-staging/` — add, diff, commit, amend
- `03-remote-fetch-pull-push/` — remote, fetch, pull, push, upstream
- `04-branching-checkout/` — branch, checkout, switch, merge dasar
- `05-merge-conflict/` — konflik merge, resolusi, review
- `06-rebase-cherry-pick/` — rebase, interactive rebase, cherry-pick
- `07-tag-release-revert-reset/` — tag, release, revert, reset, stash
- `08-final-project/` — gabungan semua materi untuk project mini
- `workspace/` — folder kerja peserta, format standar: `workspace/<username>`
- `shared/` — folder latihan kolaboratif, dipakai untuk merge/conflict
- `solutions/` — solusi referensi untuk instruktur (opsional)

Aturan umum:
- semua peserta kerja di branch sendiri
- untuk latihan kolaboratif, semua orang akan mengedit file yang sama di `shared/`
- gunakan branch naming standar: `feature/<username>/<modul>`
- commit message dibuat singkat dan jelas
- jangan force push ke branch shared tanpa koordinasi

Contoh branch:
- `feature/ucay/01-clone-init`
- `feature/member-1/05-merge-conflict`

Cara kerja belajar:
1. Clone repo ini
2. Masuk ke folder modul yang sesuai
3. Baca README di modul tersebut
4. Ikuti langkah latihan
5. Buat branch sesuai format
6. Commit hasil kerja
7. Push ke remote
8. Lakukan review dan merge seperti tim

Catatan:
- Repo ini dibuat agar bisa digunakan oleh orang lain di luar tim juga.
- Untuk peserta baru, cukup buat folder `workspace/<nama-pengguna>` lalu ikuti petunjuk pada modul.

Semoga repo ini membantu proses belajar Git secara bertahap dan menyenangkan.
