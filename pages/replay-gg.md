---
id: replay-gg.overview
product: replay-gg
title: Replay.GG
status: Released
review: draft
updated: 2026-10-23
sources:
  - https://replay-gg-site.shadylabs.workers.dev/
  - https://nova-legal.shadylabs.workers.dev/
---

# Replay.GG

Replay.GG records gameplay and makes clips. It currently ships as a Windows installer (Windows 10 and 11). Its site notes that the
code includes macOS and Linux capture paths, but those platforms do not have supported release builds yet.

## What it does

- **Instant Replay:** keeps a rolling replay buffer running and saves what just happened with a hotkey.
- **Full recording:** records whole sessions with adjustable resolution, frame rate and encoder.
- **Local library:** browse recordings and clips in one place, play them back, and trim moments out of recordings.
- **Global hotkeys:** start recording, toggle the replay buffer and save clips while a game has focus.
- **Video, audio and webcam options:** choose the display, resolution, FPS, quality and encoder; set the microphone and
  system-audio devices, including separate tracks; add a webcam overlay.

## Where your files go

Clips and recordings are stored locally on your computer. A Nova Account is optional and does not upload recordings.

## Installing

FFmpeg is included in the installer. The installer is not yet code-signed, so Windows SmartScreen may show a warning; the site
explains how to continue. Current version and downloads are on the Replay.GG site.
