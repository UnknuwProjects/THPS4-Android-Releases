# THPS4 — Port Android Tidak Resmi

[English](README.md) · **Bahasa Indonesia** · [Español](README.es.md) · [Português](README.pt.md)

Port Android tidak resmi dari **Tony Hawk's Pro Skater 4** (Xbox),
dikompilasi ulang agar berjalan native di HP ARM64.

**Repo ini hanya saluran rilis publik** — isinya README ini dan rilis-rilis
stabil. Tidak ada kode sumber di sini, dan **game tidak disertakan**: port ini
membaca data game asli atau file ISO milikmu sendiri dari folder `THPS4`
(`/storage/emulated/0/THPS4/`).

Fitur singkat: game penuh (Karier, Free Skate, Create-A-Skater, Park Editor,
2 pemain split-screen), bahasa Inggris / **Indonesia penuh**, Pengaturan Port
di dalam menu Options game, opsi grafis lengkap + ultrawide, meter performa
(FPS, GPU, CPU, RAM, baterai), dukungan mod (paket tekstur/deck/suara/model/
level, skater kustom), musik kustom (WMA) + pemutar My Music (MP3/OGG/FLAC),
System Link via LAN, dan launcher dengan pengelola mod & musik serta
pemeriksa pembaruan.

Syarat: Android 10+, perangkat ARM64, dan salinan game milikmu sendiri.
Cara pasang: unduh APK dari [Releases](../../releases), pasang, taruh data
game/ISO di folder `THPS4`, lalu **Launch Game**.

**Apakah salinanmu resmi?** Port ini hanya dirilis di halaman ini. Semua
build resmi ditandatangani dengan sertifikat yang sama, sidik jari
SHA-256: `12474f52e9b6a461bceb2af6882a0543d8dc6e49fc8fcb06ac25de83489885bb`.
Mulai 1.0.4, game memeriksanya sendiri saat menyala dan berhenti kalau
salinannya ditandatangani ulang. Salinan dari situs lain bisa berisi kode
tambahan yang diselipkan di dalamnya — itu bukan dari kami, dan apa pun
yang dilakukan salinan seperti itu bukan bagian dari proyek ini.

**Main online:** satu Wi-Fi — System Link (sampai 8 pemain) dan 2P Online
(2 pemain) langsung jalan di jaringan lokal: satu HP jadi host, HP lain
bergabung dengan kode host dari halaman Multipemain di panel. Beda jaringan
— HP di balik NAT operator tidak bisa saling menjangkau langsung. Dua jalan
keluarnya: (1) aplikasi VPN seperti Tailscale (gratis untuk pemakaian
pribadi) di kedua HP, masuk ke akun yang sama, lalu pakai alamat
`100.x.x.x` host sebagai target gabung di panel, persis seperti alamat LAN
— System Link lewat VPN bisa menampung sampai 8 pemain, sama seperti di
LAN; (2) room online, hadir di 1.0.4 — panel dapat Multiplayer Port: room
publik di server komunitas, buat room atau gabung dari daftarnya, tanpa
aplikasi tambahan dan tanpa tukar kode. Satu room isinya 2 pemain (itu
mode 2 pemain lokal game ini, dimainkan lewat internet), dan banyak room
bisa jalan bersamaan. Daftar yang sama juga memuat room link: sesi System
Link lewat internet sampai 8 pemain, bertanda LINK di daftar. Apa pun
jalurnya, kedua HP harus memakai **versi
yang sama dengan mod yang sama** dan memilih **level yang sama** — 2P Online
hanya bertukar input tombol dan tiap HP menjalankan salinan game-nya
sendiri, jadi data game yang berbeda tidak bisa tetap sinkron. Room di
daftar bertanda kalau set mod-nya berbeda dengan milikmu, dan panel bisa
mengunduhkan paket milik host untukmu — setelah satu kali mulai ulang,
set mod milikmu sama dengan room.

Menemukan bug? Laporkan di
[halaman Issues](https://github.com/UnknuwProjects/THPS4-Android-Releases/issues)
dengan model HP, versi Android, dan kejadiannya. Kalau bisa, lampirkan file
`thps4.log` dari folder `THPS4/logs` di penyimpananmu — log itu membuat
sebagian besar bug bisa diperbaiki.
