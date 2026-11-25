# THPS4 — Port Android Tidak Resmi

[English](README.md) · **Bahasa Indonesia** · [Español](README.es.md) · [Português](README.pt.md)

Port Android tidak resmi dari **Tony Hawk's Pro Skater 4** (Xbox),
dikompilasi ulang secara statis agar berjalan native di HP ARM64.

> **Repo ini hanya saluran rilis publik.** Pengembangan berlangsung di repo
> privat; yang ada di sini hanya README ini dan rilis-rilis stabil — tidak
> ada kode sumber, dan **tidak ada data game**.

## Game tidak disertakan

Port ini tidak memuat aset game apa pun. Untuk bermain, kamu menyediakan
**data game asli atau file ISO milikmu sendiri** dan menaruhnya di folder
`THPS4` pada penyimpanan bersama HP-mu:

```
/storage/emulated/0/THPS4/
```

Launcher akan memeriksa folder itu untukmu dan menunjukkan apa yang ia temukan.

## Apakah salinanmu resmi?

Port ini hanya dirilis di halaman ini. Semua build resmi ditandatangani
dengan sertifikat yang sama, sidik jari SHA-256:

```
12474f52e9b6a461bceb2af6882a0543d8dc6e49fc8fcb06ac25de83489885bb
```

Mulai 1.0.4, game memeriksanya sendiri saat menyala dan berhenti kalau
salinannya ditandatangani ulang. Salinan dari situs lain bisa berisi kode
tambahan yang diselipkan di dalamnya — itu bukan dari kami, dan apa pun
yang dilakukan salinan seperti itu bukan bagian dari proyek ini.

## Fitur

- Game penuh: Karier, Free Skate, Create-A-Skater, Park Editor, 2 pemain split-screen
- Bahasa Inggris / **terjemahan Indonesia penuh**, bisa diganti di launcher dan di dalam game
- Pengaturan Port di dalam menu Options bawaan game (grafis, bahasa, credit)
- Opsi grafis: skala render, batas FPS, VSync, anti-aliasing, filter layar, ultrawide, bloom, fog
- Meter performa di layar: FPS, nama GPU, beban & suhu GPU, CPU, RAM, baterai
- Dukungan mod: paket mod (tekstur, deck, suara, model, level), skater kustom, paket tekstur
- Musikmu sendiri: sistem soundtrack kustom bawaan game (WMA) plus pemutar My Music (MP3/OGG/FLAC/…)
- Multiplayer System Link lewat LAN, kontrol gamepad / keyboard / mouse / sentuh
- Launcher sebelum game: status folder game, pengelola mod, pengelola musik, pemeriksa pembaruan

## Syarat

- Android 10 atau lebih baru (API 29+), perangkat ARM64
- Salinan game milikmu sendiri (lihat di atas)

## Cara pasang

1. Unduh APK terbaru dari [Releases](../../releases).
2. Pasang (semua build ditandatangani dengan kunci yang sama, jadi pembaruan terpasang menimpa versi sebelumnya).
3. Taruh data game atau ISO milikmu di folder `THPS4`.
4. Buka **THPS4** lalu tekan **Launch Game**.

Launcher juga memeriksa repo ini untuk pembaruan dan bisa mengunduhkan
versi berikutnya untukmu.

## Main online

**Satu Wi-Fi** — System Link (sampai 8 pemain) dan 2P Online (2 pemain)
langsung jalan di jaringan lokalmu tanpa perlu diatur: satu HP jadi host,
HP lain bergabung dengan kode host dari halaman Multipemain di panel.

**Beda jaringan** — HP di balik NAT operator tidak bisa saling menjangkau
langsung. Dua jalan keluarnya:

- **Aplikasi VPN (bisa dipakai sekarang):** pasang Tailscale (gratis untuk
  pemakaian pribadi) di kedua HP dan masuk ke akun yang sama. Tiap HP
  mendapat alamat `100.x.x.x` — pakai alamat host sebagai target gabung di
  panel, persis seperti alamat LAN. System Link lewat VPN bisa menampung
  sampai 8 pemain, sama seperti di LAN.
- **Room online (hadir di 1.0.4):** panel mendapat Multiplayer Port — room
  publik di server komunitas. Buat room atau gabung dari daftarnya, tanpa
  aplikasi tambahan dan tanpa tukar kode. Satu room isinya 2 pemain (itu
  mode 2 pemain lokal game ini, dimainkan lewat internet), dan banyak room
  bisa jalan bersamaan. Daftar yang sama juga memuat room link: sesi System
  Link lewat internet sampai 8 pemain, bertanda LINK di daftar.

Apa pun jalurnya, kedua HP harus memakai **versi yang sama dengan mod yang
sama** dan memilih **level yang sama** — 2P Online hanya bertukar input
tombol dan tiap HP menjalankan salinan game-nya sendiri, jadi data game
yang berbeda tidak bisa tetap sinkron. Room di daftar bertanda kalau set
mod-nya berbeda dengan milikmu, dan panel bisa mengunduhkan paket milik
host untukmu — setelah satu kali mulai ulang, set mod milikmu sama dengan
room.

## Versi

Rilis di sini memakai versi semantik yang stabil — `MAJOR.MINOR.PATCH`
(rilis publik pertama: **1.0.0**). Catatan tiap rilis merinci apa yang
berubah. Build pengembangan (jalur `beta`) dites secara privat dan tidak
diterbitkan di sini; sebuah build diterbitkan setelah dianggap stabil.

## Laporan bug

Menemukan bug? Laporkan di
[halaman Issues](https://github.com/UnknuwProjects/THPS4-Android-Releases/issues)
dengan model HP, versi Android, dan kejadiannya. Kalau bisa, lampirkan file
`thps4.log` dari folder `THPS4/logs` di penyimpananmu — log itu membuat
sebagian besar bug bisa diperbaiki.

## Credit & dukungan

Port oleh **UNKNUW** — [github.com/UnknuwProjects](https://github.com/UnknuwProjects)

Dukung proyek ini:
[Sociabuzz](https://sociabuzz.com/unknuw/tribe) ·
[Saweria](https://saweria.co/Unknuw)

*Proyek fan tidak resmi. Tidak berafiliasi dengan Activision atau Neversoft.
Tony Hawk's Pro Skater 4 adalah merek dagang pemiliknya masing-masing.*
