# Signal / DAC

Windows desktop app for audio format monitoring and DAC setup.

**[Download SignalDAC.exe for Windows x64](https://github.com/kulunkilabs/SignalDAC-downloads/releases/latest/download/SignalDAC.exe)**

One portable EXE, with its runtime included. No separate .NET installation. Windows 10 version 2004+ or Windows 11, x64. This build is unsigned.

## Features

- Automatically detects source formats where players/local files expose them.
- Supports NAS/mapped-file metadata and buffered Astra playback through a read-only local-library match.
- Shows audio activity for games and other Windows apps, with a separately labelled Windows mixer format when original PCM metadata is unavailable.
- Reads the submitted format of a Windows app or game when an unambiguous playback stream is observed.
- Shows the running DAC output format from a readable driver pin or Windows audio trace. The trace reports sample rate and container width when valid bits are unavailable.
- During active shared playback without driver access, the output panel clearly says **Windows output setting** and **driver not verified**. Driver container bitrate stays unavailable.
- Shared 16/24/32-bit controls, sample-rate selection and automatic source matching.
- **Apply best Windows settings** configures supported DAC endpoint policies, checks each result, and saves a per-device restore backup.
- Resizable window with standard Windows controls, Snap and remembered placement.
- **Window > Compact monitor** opens a small floating view with input and output depth and sample rate. It has its own **Always on top** switch.
- Send to tray, optional automatic tray minimization, Always on top and an audio setup guide.
- No song titles or artist names in the window.

## Quick start

1. Download and run the EXE, then select your DAC or System default output.
2. Pause exclusive playback before applying the Windows setup preset. Review any manual checks in its result. **Restore previous** returns the saved setup.
3. In your music player, select the same DAC with WASAPI Exclusive/native output if supported. Disable resampling, EQ and normalization when you want unchanged samples.

The preset enables Windows exclusive control/priority, disables Windows system effects and spatial sound where supported, chooses a supported source format or retains the current rate, and enables shared-mode source matching. Volume and default-device routing keep their current settings. Changes can briefly interrupt playback and remain applied after exit.

Source quality can remain **Unknown** for games, browser, streaming, protected or unsupported sources. The Windows mixer fallback is its shared engine format, not original recording precision or a driver measurement; it never triggers source matching. Astra requires exactly one matching local-library entry and no API token. Some drivers/ASIO paths do not expose a readable active stream. Windows 10 spatial sound and unsupported policy controls need manual setup. Matching sample rates does not prove bit-perfect audio. Original 16/24-bit music can use 32-bit USB containers.

Open Signal / DAC before playback so it can observe stream creation. App, mixer, live driver and configured format labels identify which reading you are seeing.

## Licence and credits

Proprietary freeware — application source is privately maintained. This repository contains documentation and binary releases, not application source. See [LICENSE.txt](LICENSE.txt). Bundled third-party components retain their own licences in the EXE's About panel and [THIRD-PARTY-NOTICES.txt](THIRD-PARTY-NOTICES.txt).

Developed with AI and Half-Life HAZY IPA.

© 2026 Th0st3r & MacekW.
