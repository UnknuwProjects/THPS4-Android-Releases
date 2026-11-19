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

Menemukan bug? Laporkan di
[halaman Issues](https://github.com/UnknuwProjects/THPS4-Android-Releases/issues)
dengan model HP, versi Android, dan kejadiannya. Kalau bisa, lampirkan file
`thps4.log` dari folder `THPS4/logs` di penyimpananmu — log itu membuat
sebagian besar bug bisa diperbaiki.
