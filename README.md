# THPS4 — Unofficial Android Port

An unofficial Android port of **Tony Hawk's Pro Skater 4** (Xbox), statically
recompiled to run natively on ARM64 phones.

> **This repository is the public release channel only.** Development happens
> in a private repository; what lives here is this README and the stable
> releases — no source code, and **no game data**.

## The game is not included

This port contains no game assets. To play, you supply **your own original
game data or ISO file** and place it in the `THPS4` folder on your phone's
shared storage:

```
/storage/emulated/0/THPS4/
```

The launcher checks the folder for you and shows what it found.

## Features

- The full game: Career, Free Skate, Create-A-Skater, Park Editor, 2-Player split-screen
- English / **full Indonesian translation**, switchable in the launcher and in-game
- Port Settings inside the game's own Options menu (graphics, language, credits)
- Graphics options: render scale, FPS cap, VSync, anti-aliasing, screen filters, ultrawide, bloom, fog
- Performance meter overlay: FPS, GPU name, GPU load & temperature, CPU, RAM, battery
- Mod support: mod packs (textures, decks, sounds, models, levels), custom skaters, texture packs
- Your own music: the game's custom-soundtrack system (WMA) plus a My Music player (MP3/OGG/FLAC/…)
- System Link multiplayer over LAN, gamepad / keyboard / mouse / touch controls
- A pre-game launcher: game-folder status, mod manager, music manager, update checks

## Requirements

- Android 10 or newer (API 29+), ARM64 device
- Your own copy of the game (see above)

## Install

1. Download the newest APK from [Releases](../../releases).
2. Install it (every build is signed with the same key, so updates install over the previous version).
3. Put your game data or ISO in the `THPS4` folder.
4. Open **THPS4** and press **Launch Game**.

The launcher also checks this repository for updates and can download the
next version for you.

## Playing online

**Same Wi-Fi** — System Link (up to 8 players) and 2P Online (2 players)
work on your local network with nothing to set up: one phone hosts, the
other joins with the host code from the panel's Multiplayer page.

**Different networks** — phones behind carrier NAT cannot reach each other
directly. Two ways around that:

- **VPN app (works today):** install Tailscale (free for personal use) on
  both phones and sign both into the same account. Each phone gets a
  `100.x.x.x` address — use the host's as the join target in the panel,
  exactly like a LAN address. System Link over the VPN holds up to
  8 players, same as on a LAN.
- **Relay rooms (coming in 1.0.4):** the panel gains Multiplayer Port —
  public rooms on a relay server. Create a room or join one from the
  list; no extra app, no codes to trade. A room seats 2 players (it is
  the game's local 2-player mode, played over the internet), and many
  rooms can run at the same time. The same list also carries link
  rooms: System Link sessions over the internet for up to 8 players,
  marked LINK in the list.

Whichever route you use, both phones must run the **same version with the
same mods** and pick the **same level** — 2P Online exchanges controller
inputs only and each phone runs its own copy of the game, so different
game data cannot stay in sync.

## Versions

Releases here use stable semantic versioning — `MAJOR.MINOR.PATCH`
(first public release: **1.0.0**). Each release's notes list what changed.
Development builds (the `beta` track) are tested privately and are not
published here; a build is published once it is considered stable.

## Bug reports

Found a bug? Please report it on the
[Issues page](https://github.com/UnknuwProjects/THPS4-Android-Releases/issues)
with your phone model, your Android version, and what happened. If you can,
attach the file `thps4.log` from the `THPS4/logs` folder on your storage —
that log makes most bugs fixable.

## Credits & support

Port by **UNKNUW** — [github.com/UnknuwProjects](https://github.com/UnknuwProjects)

Support the project:
[Sociabuzz](https://sociabuzz.com/unknuw/tribe) ·
[Saweria](https://saweria.co/Unknuw)

*Unofficial fan project. Not affiliated with Activision or Neversoft.
Tony Hawk's Pro Skater 4 is a trademark of its respective owners.*

---

## Bahasa Indonesia

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

**Main online:** satu Wi-Fi — System Link (sampai 8 pemain) dan 2P Online
(2 pemain) langsung jalan di jaringan lokal: satu HP jadi host, HP lain
bergabung dengan kode host dari halaman Multipemain di panel. Beda jaringan
— HP di balik NAT operator tidak bisa saling menjangkau langsung. Dua jalan
keluarnya: (1) aplikasi VPN seperti Tailscale (gratis untuk pemakaian
pribadi) di kedua HP, masuk ke akun yang sama, lalu pakai alamat
`100.x.x.x` host sebagai target gabung di panel, persis seperti alamat LAN
— System Link lewat VPN bisa menampung sampai 8 pemain, sama seperti di
LAN; (2) room relay, hadir di 1.0.4 — panel dapat Multiplayer Port: room
publik di server relay, buat room atau gabung dari daftarnya, tanpa
aplikasi tambahan dan tanpa tukar kode. Satu room isinya 2 pemain (itu
mode 2 pemain lokal game ini, dimainkan lewat internet), dan banyak room
bisa jalan bersamaan. Daftar yang sama juga memuat room link: sesi System
Link lewat internet sampai 8 pemain, bertanda LINK di daftar. Apa pun
jalurnya, kedua HP harus memakai **versi
yang sama dengan mod yang sama** dan memilih **level yang sama** — 2P Online
hanya bertukar input tombol dan tiap HP menjalankan salinan game-nya
sendiri, jadi data game yang berbeda tidak bisa tetap sinkron.

Menemukan bug? Laporkan di
[halaman Issues](https://github.com/UnknuwProjects/THPS4-Android-Releases/issues)
dengan model HP, versi Android, dan kejadiannya. Kalau bisa, lampirkan file
`thps4.log` dari folder `THPS4/logs` di penyimpananmu — log itu membuat
sebagian besar bug bisa diperbaiki.
