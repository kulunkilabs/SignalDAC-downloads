# Signal / DAC

Windows audio-format monitor and DAC setup widget.

**[Download SignalDAC.exe for Windows x64](https://github.com/kulunkilabs/SignalDAC-downloads/releases/latest/download/SignalDAC.exe)**

One portable EXE, with its runtime included. No separate .NET installation. Windows 10 version 2004+ or Windows 11, x64. This build is unsigned.

## Features

- Automatically detects source formats where players/local files expose them.
- Shows readable live DAC driver format separately from source precision and the Windows shared setting.
- Shared 16/24/32-bit controls, sample-rate selection and automatic source matching.
- **Apply best Windows settings** configures supported DAC endpoint policies, checks each result, and saves a per-device restore backup.
- Tray minimization, explicit Quit, always-on-top and an audio setup guide.
- No song titles or artist names in the widget.

## Quick start

1. Download and run the EXE, then select your DAC or System default output.
2. Pause exclusive playback before applying the Windows setup preset. Review any manual checks in its result. **Restore previous** returns the saved setup.
3. In your music player, select the same DAC with WASAPI Exclusive/native output if supported. Disable resampling, EQ and normalization when you want unchanged samples.

The preset enables Windows exclusive control/priority, disables Windows system effects and spatial sound where supported, chooses a supported source format or retains the current rate, and enables shared-mode source matching. Volume and default-device routing keep their current settings. Changes can briefly interrupt playback and remain applied after exit.

Source quality can remain **Unknown** for browser, streaming, protected or unsupported sources. Some drivers/ASIO paths do not expose a readable active stream. Windows 10 spatial sound and unsupported policy controls need manual setup. Matching sample rates does not prove bit-perfect audio. Original 16/24-bit music can use 32-bit USB containers.

## Licence and credits

Proprietary freeware — application source is privately maintained. This repository contains documentation and binary releases, not application source. See [LICENSE.txt](LICENSE.txt). Bundled third-party components retain their own licences in the EXE's About panel and [THIRD-PARTY-NOTICES.txt](THIRD-PARTY-NOTICES.txt).

Developed with AI and Half-Life HAZY IPA.

© 2026 Th0st3r & MacekW.
