# 07 - Tag, Release, Revert, Reset, Stash

Tujuan modul:
- memahami tag untuk release
- mengetahui cara membatalkan perubahan dengan revert dan reset
- memahami stash untuk sementara menyimpan perubahan

Tag:

```bash
git tag -a v0.1.0 -m "release v0.1.0"
git push origin v0.1.0
```

Revert commit terakhir:

```bash
git revert HEAD
```

Reset (hati-hati):

```bash
git reset --soft HEAD~1
git reset --mixed HEAD~1
git reset --hard HEAD~1
```

Stash:

```bash
git stash push -m "kerja sementara"
git stash list
git stash pop
```

Tugas latihan:
- buat tag untuk state tertentu
- buat perubahan yang salah lalu gunakan `git revert`
- buat perubahan yang belum selesai lalu simpan dengan `git stash`

Tips:
- `git revert` aman untuk perubahan yang sudah dipush ke remote
- `git reset --hard` menghapus perubahan secara permanen dari working directory
- gunakan stash jika Anda ingin meninggalkan pekerjaan sementara

Kriteria sukses:
- bisa membuat tag
- bisa membatalkan perubahan aman dengan revert
- bisa menyimpan kerja sementara dengan stash
