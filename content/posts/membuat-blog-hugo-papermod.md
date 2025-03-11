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

### (Membuat situs baru, lewat github codespaces)

Github Codespaces biasanya sudah terinstall hugo secara default, sehingga tidak perlu lagi install hugo.

In case somehow di masa depan hugo belum terinstall secara default, atau paket hugo yang terinstall merupakan versi lawas, install hugo terlebih dahulu.

1. Buat situs baru di current directory (root repo directory)
> hugo new site . --force

2. Situs hugo yang baru akan tergenerate di current directory.

### (Membuat situs baru lewat local repo)

Dikarenakan kita akan membuat situs baru nya lewat local repo, maka dari itu kita harus install Hugo terlebih dahulu.

1. Update kemudian install wget dan curl.

> apt update && apt install wget curl -y

2. Dapatkan Hugo versi terbaru
Contoh :

(amd64)
> wget https://github.com/gohugoio/hugo/releases/download/v0.145.0/hugo_0.145.0_linux-amd64.deb

(arm64)
> wget https://github.com/gohugoio/hugo/releases/download/v0.145.0/hugo_0.145.0_linux-arm64.deb

3. Install Hugo
> apt install ./file-hugo-yang-akan-diinstall -y

4. Buat situs baru di folder baru.
> hugo new site nama-blog

5. Situs baru akan ter-generate di folder nama-blog
