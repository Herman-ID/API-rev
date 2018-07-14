# Perencanaan API OnBox
***

## Daftar Isi

1. [Latar Belakang](#latar-belakang)
2. [Tujuan Dokumen](#tujuan)
3. [Manfaat Dokumen](#manfaat)
4. [Penjelasan Dokumen](#penjelasan)
  - [Penjelasan Singkat](#overview)
  - [Struktur Berkas](#berkas)
  - [Alat](#Alat)

## 1. Latar Belakang

**OnBox** adalah platform social networking yang berusaha di bangun oleh beberapa mahasiswa Universitas Siliwangi, agar memberi manfaat untuk orang banyak.Dalam membangun **OnBox** diperlukan sebuah sistem yang kompleks, aman dan cepat sehingga kinerja aplikasi akan berjalan dengan baik.

Dalam membangun sistemnya, **OnBox** akan menggunakan sistem [***web service***](#) dengan memanfaatkan tekhnologi [***Application Program Interface (API)***](#) sehingga sistem dapat digunakan di [***platform***](#) mana saja baik itu di [***web***](#), [***mobile***](#), maupun [***desktop***](#).

API yang dibangun harus dapat memenuhi banyak kriteria, untuk itu harus dilakukan perencanaan yang matang dan pendokumentasian yang benar dalam membangun API.


## 2. Tujuan Dokumen

Dokumen ini bertujuan sebagai [***Dokumentasi***](#) atas perencanaan pembuatan Application Program Interface (API) OnBox, Baik API yang bersifat [***private***](#) maupun [***public***](#). Dokumen ini hanya boleh digunakan dalam internal team dan tidak boleh digunakan oleh orang - orang diluar tim.


## 3. Manfaat Dokumen

Dokumen ini dapat dimanfaatkan untuk :

1. Sebagai [***blue print***](#) dalam membangun API OnBox.
2. Sebagai dokumentasi terhadap API yang sudah dibangun.
3. Sebagai [***software design documentation***](#) tahap pertama

## 4. Penjelasan Dokumen

Pada bagian ini akan dijelaskan penjelasan mengenai API OnBox yang akan dibangun, berkas, alat dan lain sebagainya.

### 4.1 Penjelasan singkat

OnBox API adalah API berbasis [JSON](#), yang akan memberikan data yang dibutuhkan untuk pengembangan aplikasi.

### 4.2 Struktur Berkas

Dokumentasi ini memiliki struktur berkas seperti berikut:

    \
    --Build\
    --Documentation\
    --Plan\
    ----Private\
    ------profil-page-all.json
    ----Public\
    --Author.md
    --README.md

- `Build` adalah folder penyimpanan contoh result API yang sudah jadi dan sudah mengalami tahap pengujian, folder ini berisi file ber-ekstensi `.json` saja.

- `Documentation` adalah folder penyimpanan dokumentasi, baik yang sudah di release maupun yang masih dalam tahap perancangan, folder ini hanya berisi file ber-ekstensi `.md` saja.

- `Plan` adalah folder penyimpanan contoh result API yang akan dibuat atau masih berupa rancangan, folder ini memiliki folder `Private` untuk API private dan folder `Public` untuk API public.

- `Author.md` adalah dokumentasi developer yang terlibat dalam pembuatan dokumentasi ini.

- `README.md` adalah dokumentasi utama, tujuannya dapat dilihat pada poin ke-2 dokumen ini.

### 4.3 Alat

Dalam pembuatan API, OnBox akan menggunakan :

1. Ruby Programming Language 2.3.1p112 (2016-04-26) [x86_64-linux-gnu]
2. Ruby On Rails Framework 5.2.0
3. MySQL Database Ver 14.14 Distrib 5.7.22, for Linux (x86_64)
4. Atom v 1.7.3

Dalam pengujian API, OnBox akan menggunakan :

1. Postman
2. Curl Linux Command

---
