+++
date = '2025-02-17T03:26:28Z'
draft = false
title = 'Membuat blog di Github Pages dengan bantuan Hugo dan PaperMod theme'
+++

Sebenarnya ini catatan pribadi untuk diriku sendiri, agar tidak kelupaan di masa mendatang.

Agar tidak kelabakan ketika akan menginstall ulang tema atau blog.

## Langkah 1
(Menyiapkan repo publik untuk digunakan sebagai tempat hosting blog)

A. Hal pertama yang harus dilakukan adalah login ke akun github kamu. Lalu buat repo baru tanpa disertai README.md

B. Jika sudah, lalu buka pengaturan repo di github. 

Settings => Pages

Pada bagian 'Source', pilih Github Actions sebagai sumbernya. Tidak perlu klik simpan, karena perubahan sudah otomatis tersimpan.

## Langkah 2

#### (Membuat situs baru, lewat github codespaces)

Github Codespaces biasanya sudah terinstall hugo secara default, sehingga tidak perlu lagi install hugo.

In case somehow di masa depan hugo belum terinstall secara default, atau paket hugo yang terinstall merupakan versi lawas, install hugo terlebih dahulu.

1. Buat situs baru di current directory (root repo directory)
> hugo new site . --force

2. Situs hugo yang baru akan tergenerate di current directory.

#### (Membuat situs baru lewat local repo)

1. 