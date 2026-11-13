# Galactic Desk

*Formerly Fleet Command Compendium.*

An **unofficial, fan-made** progress companion for **Star Trek Fleet Command** on Windows, by Hughes Digital LLC.
It reads your own account from the game's PC client and tells you, in plain language, what you've done, what you can
do now, and exactly how to do it.

> Not affiliated with, endorsed by, or sponsored by Paramount, CBS Studios or Scopely. No official game artwork or
> logos are included.

## Download

**[Download the latest installer](https://github.com/jhughes2466/galactic-desk/releases/latest/download/GalacticDesk-Setup.exe)**
(Windows 10 or 11, about 16 MB). Already have Fleet Command Compendium? Install over it: your data and settings carry over. All versions are on the [Releases page](https://github.com/jhughes2466/galactic-desk/releases).

Website: **[galacticdesk.com](https://galacticdesk.com)**

This repository holds the installer downloads only. The app's source code isn't published.

## Installing

1. Run `GalacticDesk-Setup.exe`. It installs for your Windows user only and doesn't need admin rights.
2. Windows may show **"Windows protected your PC"**, because the installer isn't code-signed yet. Click
   **More info**, then **Run anyway**.
3. Click **Open Galactic Desk and start setup** on the last page. The setup wizard then:
   - finds your game folder (it reads the folder Scopely's launcher recorded for your Windows user, so a custom
     install folder or another drive is fine);
   - installs the free [STFC Community Mod](https://github.com/STFC-Mod/mod) next to the game (`version.dll`
     beside `prime.exe`), with the game closed;
   - connects the mod to the app and downloads the game data.
4. Start the game. Your account syncs to the app on your PC while you play.

Your data stays on your PC. The app never asks for your Scopely password.

## Check the download (optional)

In PowerShell, in the folder you downloaded to:

```powershell
Get-FileHash .\GalacticDesk-Setup.exe -Algorithm SHA256
```

Compare the result with the SHA-256 listed in the release notes.

## Uninstalling

Settings → Apps → Installed apps → Galactic Desk → Uninstall. To remove the Community Mod as well, delete
`version.dll` and `community_patch_settings.toml` from the game folder.

## License

Copyright © 2026 Hughes Digital LLC. All rights reserved. You may download and use the installer for free for your
own play. See [LICENSE](LICENSE).
