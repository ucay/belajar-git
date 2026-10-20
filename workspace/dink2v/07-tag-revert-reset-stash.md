# Modul 07 - Tag, Revert, Reset, dan Stash

## Tag
Tag menandai commit tertentu, misalnya untuk versi rilis.

Contoh:
git tag -a v0.5.0 -m "release v0.5.0"
git tag
git show --no-patch v0.5.0

Tag v0.5.0 dibuat pada latihan lokal dan belum di-push ke GitHub.

## Revert
Revert membatalkan perubahan dengan membuat commit baru.

Contoh:
git revert HEAD

## Reset Soft
git reset --soft HEAD~1

Memundurkan posisi commit, tetapi perubahan tetap berada di staging.

## Reset Mixed
git reset --mixed HEAD~1

Memundurkan posisi commit, tetapi perubahan tetap di folder kerja dan tidak berada di staging.

## Reset Hard
git reset --hard HEAD~1

Mengembalikan HEAD, staging, dan folder kerja ke commit tujuan. Perubahan yang tidak ada pada commit tujuan dapat hilang.

Latihan hard reset dilakukan pada branch sementara dengan file khusus.

## Stash
Stash menyimpan sementara perubahan yang belum di-commit.

Contoh:
git stash push -m "kerja sementara"
git stash list
git stash pop

## Ringkasan
- Tag: menandai commit.
- Revert: membatalkan perubahan melalui commit baru.
- Reset soft: perubahan tetap di staging.
- Reset mixed: perubahan tetap di folder kerja.
- Reset hard: perubahan yang tidak ada pada commit tujuan dapat hilang.
- Stash: menyimpan sementara perubahan yang belum di-commit.
