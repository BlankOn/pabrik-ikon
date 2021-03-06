# Pabrik-ikon
Membangun Ikon untuk destop GNU/Linux 

## Kebutuhan
- [inkscape](https://inkscape.org/en/)
- [svgcleaner](https://sourceforge.net/projects/svgcleaner/)

untuk memasang aplikasi diatas silahkan ikuti dokumentasi distribusi linux yang anda pakai.

## Struktur folder
Didalam folder kerja anda setidaknya membutuhkan salah satu folder dari daftar berikut:

- actions/scalable/
- animations/scalable/
- apps/scalable/
- categories/scalable/
- devices/scalable/
- emblems/scalable/
- io/scalable/
- mimetypes/scalable/
- places/scalable/
- status/scalable/
- stock/scalable/


Jika ini pertama kalinya anda membuat ikon untuk GNU/Linux, ketikan pada terminal perintah berikut:
```
$ cd ke/folder/kerja/anda
$ mkdir -p {actions,animations,apps,categories,devices,emblems,io,mimetypes,places,status,stock}/scalable

```
Berkas-berkas `*.svg` disimpan di folder `scalable`

## Pemasangan
- Unduh berkas mutakhir [disini](https://github.com/winardiaris/pabrik-ikon/archive/master.zip) dan ekstrak berkas tersebut.
- Selanjutnya salin berkas `pabrik.sh`, `index.theme` dan folder `data` _(ini contoh berkas untuk membuat symlink)_ ke folder kerja anda.
- Ubah berkas `index.theme` sesuai keinginan anda pada bagian berikut:
```
[Icon Theme]
Name=nama-ikon
Inherits=gnome,hicolor
Comment=komentar
```  


## Pemasangan cepat
```
wget https://raw.githubusercontent.com/winardiaris/pabrik-ikon/master/install.sh && bash ./install.sh "nama-ikon" "Deskripsi"
```
- ubah "`nama-ikon`" sesuai keinginan anda pastikan tidak menggunakan spasi
- ubah "`Deskripsi`" sesuai deskripsi dari ikon yang anda buat



## Penggunaan
```
$ cd ke/folder/kerja/anda
$ bash pabrik.sh

==============================================
Nama:Pabrik-ikon
Versi:0.2
==============================================
1 Buat berkas png
2 Buat berkas symlink
3 Buat berkas png + symlink
4 Vacuum SVG
5 Minizer SVG (Belum tersedia)
C Bersihkan area kerja
Q Keluar
==============================================

```

