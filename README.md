Ardhitya Belajar Branch

!lorem

Pakai yang setelah # sebagai penjelasan

git branch
# lihat daftar branch yang ada
# tanda * artinya branch yang sedang aktif

git branch fitur-3
# buat branch baru bernama fitur-3
# tapi belum pindah ke branch itu

git checkout fitur-3
# pindah ke branch fitur-3

git checkout -b fitur-3
# buat branch fitur-3 lalu langsung pindah ke sana
# ini versi singkat dari:
# git branch fitur-3
# git checkout fitur-3

git status
# cek kondisi file
# lihat apakah ada file yang berubah, belum di-add, atau belum di-commit

git add .
# masukkan semua file yang berubah ke staging area
# siap untuk di-commit

git commit -m "kerja di fitur-3"
# simpan perubahan ke branch yang sedang aktif

git checkout main
# pindah kembali ke branch utama yaitu main

git merge fitur-3
# gabungkan isi branch fitur-3 ke branch yang sedang aktif
# kalau sekarang posisi kamu di main, berarti fitur-3 masuk ke main

git push origin fitur-3
# kirim branch fitur-3 ke GitHub

git push origin main
# kirim branch main ke GitHub

git branch -d fitur-3
# hapus branch fitur-3 di lokal
# biasanya dilakukan setelah branch selesai dan sudah di-merge

git push origin --delete fitur-3
# hapus branch fitur-3 di GitHub
Urutan yang paling sering dipakai
git checkout -b fitur-3
# buat branch baru dan langsung pindah ke branch fitur-3

git add .
# siapkan semua perubahan

git commit -m "menambahkan perubahan di fitur-3"
# simpan perubahan ke branch fitur-3

git push origin fitur-3
# upload branch fitur-3 ke GitHub

git checkout main
# balik ke branch utama

git merge fitur-3
# gabungkan isi fitur-3 ke main

git push origin main
# kirim hasil merge ke GitHub

git branch -d fitur-3
# hapus branch fitur-3 di lokal karena sudah selesai
Versi super singkat buat dihafal
git checkout -b fitur-3   # buat branch baru + pindah
git add .                 # siapkan perubahan
git commit -m "pesan"     # simpan perubahan
git push origin fitur-3   # push branch fitur
git checkout main         # balik ke main
git merge fitur-3         # gabungkan ke main
git push origin main      # push main
git branch -d fitur-3     # hapus branch lokal
Catatan penting
git status
# selalu cek ini sebelum pindah branch
# kalau masih ada modified, sebaiknya commit dulu