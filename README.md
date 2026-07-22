#
<p align="center">
  <img src="https://raw.githubusercontent.com/SSOROZCO/files/refs/heads/main/Strawberry-Roon.svg" width="220" alt="Strawberry-Roon">
</p>

<h1 align="center">Strawberry-Roon</h1>

<p align="center">
A Minimalist Visual Refresh for Strawberry Music Player
</p>

<p align="center"></p>

[![Build Status](https://github.com/SSOROZCO/Strawberry-Roon/actions/workflows/build.yaml/badge.svg?branch=desarrollo-roon)](https://github.com/SSOROZCO/Strawberry-Roon/actions)

[![Sponsor](https://img.shields.io/badge/-Sponsor-green?logo=github)]( https://github.com/sponsors/SSOROZCO)
[![Patreon](https://img.shields.io/badge/patreon-donate-green.svg)](https://www.patreon.com/cw/SergioSebastianOrozco)
[![PayPal](https://img.shields.io/badge/Donate-PayPal-green.svg)](https://paypal.me/cineflix)

Strawberry-Roon: A Minimalist Visual Refresh for Strawberry Music Player

Inspired by minimalist desktop interfaces and refined design principles, this project modernises Strawberry’s appearance while preserving its lightweight architecture, high performance, and powerful music management features valued by audiophiles and collectors.

Originally forked from Clementine in 2018, Strawberry is developed in C++ using the Qt framework. Strawberry-Roon is not intended to introduce new playback features or imitate other players; instead, it focuses on delivering a cleaner, more contemporary visual identity while respecting the philosophy of the original project.

![Screenshot of Strawberry Music Player](https://github.com/SSOROZCO/files/blob/68594632391939344c254fda29aba3706cd02310/Screenshot_20260721_215115.png)

---
Project Vision

The initiative began with a simple idea: to refresh Strawberry’s interface without altering the qualities that make it exceptional. While early inspiration came from Roon’s clean layout, the final design direction was guided by the minimalist environment and restrained colour palette of Astra Linux Special Edition, which shaped many of the decisions.
Objectives

    Modernise the interface while maintaining simplicity.

    Preserve lightweight performance and stability.

    Ensure functional consistency across all elements.

    Refine visual coherence with updated icons and layouts.

    Respect the original project and its development philosophy.

Design Philosophy

Strawberry-Roon follows a clear and concise philosophy:

    Keep Strawberry fast and lightweight.

    Modernise the visual experience without unnecessary complexity.

    Improve consistency across icons and interface elements.

    Blend naturally with modern desktop environments.

    Honour the principles of the original Strawberry project.

Community Collaboration

This redesign is conceived as a community-driven project. Anyone is welcome to build upon, adapt, and improve the work, ensuring Strawberry continues to evolve while remaining true to its core identity.

## :white_check_mark: Features

- Play and organize your music collection
- Support for WAV, FLAC, Ogg FLAC, WavPack, Ogg Vorbis, Opus, Ogg Speex, MPC, TrueAudio, AIFF, MP4/AAC, ALAC, MP3, ASF, Monkey’s Audio, and DSD (DSF/DSDIFF)
- Bit-perfect playback on Linux
- MPRIS2 / D-Bus remote control on Linux
- Native desktop notifications
- Advanced playlist management
- Smart and dynamic playlists
- Audio analyzer, equalizer, moodbar, and waveform seek bar
- Volume normalization with ReplayGain and EBU R128 loudness analysis
- Editing tags, and fetching missing tags via acoustic fingerprinting using [AcoustID](https://acoustid.org/) and [MusicBrainz](https://musicbrainz.org/)
- Album cover art from: [Last.fm](https://www.last.fm/), [MusicBrainz](https://musicbrainz.org/), [Discogs](https://www.discogs.com/), [Musixmatch](https://www.musixmatch.com/), [Deezer](https://www.deezer.com/), [Tidal](https://www.tidal.com/), [Qobuz](https://www.qobuz.com/), [Spotify](https://www.spotify.com/)
- Lyrics from: [Genius](https://genius.com/), [Musixmatch](https://www.musixmatch.com/), [lyrics.ovh](https://lyrics.ovh/), [songlyrics](https://www.songlyrics.com/), [azlyrics](https://www.azlyrics.com/), [elyrics](https://www.elyrics.net/), [letras](https://www.letras.mus.br) and [lrclib.net](https://lrclib.net/)
- Audio format conversion (transcoding) to MP3, AAC, FLAC, Ogg Vorbis, Opus, Speex, WavPack, and ASF
- Music transfer to USB, MTP and iPod devices
- Scrobbling to [Last.fm](https://www.last.fm/), [ListenBrainz](https://listenbrainz.org/), and Subsonic
- Global keyboard shortcuts (Linux, macOS, and Windows)
- Discord Rich Presence
- Audio CD playback
- Internet radio from [Radio Paradise](https://radioparadise.com/), [SomaFM](https://somafm.com/), [Radio Browser](https://www.radio-browser.info/), and custom streams
- Streaming from Subsonic-compatible servers
- Unofficial Tidal, Spotify, and Qobuz integration

---

:white_check_mark: Tested on **Linux**.

---

## :gear: Requirements

To build Strawberry from source, you’ll need:

**Dependencies:**
- [CMake 3.13 or higher](https://cmake.org/)
- C/C++ compiler ([GCC](https://gcc.gnu.org/), [Clang](https://clang.llvm.org/), or [MSVC](https://visualstudio.microsoft.com/vs/features/cplusplus/))
- [pkg-config](https://www.freedesktop.org/wiki/Software/pkg-config/) or [pkgconf](https://github.com/pkgconf/pkgconf)
- [Boost](https://www.boost.org/)
- [GLib](https://developer.gnome.org/glib/)
- [Qt 6.4 or higher](https://www.qt.io/) (Core, Concurrent, Gui, Widgets, Network, SQL, D-Bus)
- [SQLite 3.9 or higher](https://www.sqlite.org)
- [ALSA (Linux only)](https://www.alsa-project.org/)
- [GStreamer](https://gstreamer.freedesktop.org/)
- [TagLib 1.12 or higher](https://www.taglib.org/)
- [ICU](https://unicode-org.github.io/icu/)
- [KDSingleApplication 1.1.0 or higher](https://github.com/KDAB/KDSingleApplication)

**Dependencies for optional features:**
- Fingerprinting & tagging: [Chromaprint](https://acoustid.org/chromaprint)
- Fast Spectrum Moodbar: [FFTW3](http://www.fftw.org/)
- PulseAudio integration: [PulseAudio](https://www.freedesktop.org/wiki/Software/PulseAudio/)
- Audio CD support: [libcdio](https://www.gnu.org/software/libcdio/)
- MTP devices: [libmtp](http://libmtp.sourceforge.net/)
- iPod Classic: [libgpod](http://www.gtkpod.org/libgpod/)
- EBU R128 normalization: [libebur128](https://github.com/jiixyj/libebur128)

Also install GStreamer plugins **base**, **good**, and optionally **bad**, **ugly** and **libav** for full codec support.

---

## 🔧 Build from Source

Clone the repository:

```bash
git clone --recursive https://github.com/SSOROZCO/Strawberry-Roon.git
cd Strawberry-Roon
```

Build and install:

```bash
cmake -S . -B build
cmake --build build --parallel $(nproc)
sudo cmake --install build
```

---
Versioning

Strawberry-Roon follows the official Strawberry release cycle.

Visual redesign releases append the suffix "-r1", "-r2", etc.

Examples:

9b6d4a7a-r1

## :package: Packaging status

[![Packaging status](https://repology.org/badge/vertical-allrepos/strawberry.svg?columns=3&header=Strawberry&exclude_unsupported=1)](https://repology.org/metapackage/strawberry/versions)
