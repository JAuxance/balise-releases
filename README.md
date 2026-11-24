<p align="center">
  <img src="assets/banner.svg" alt="Balise" width="100%">
</p>

<p align="center">
  <img src="https://img.shields.io/github/v/release/JAuxance/balise-releases?style=flat-square&label=version&color=444" alt="Latest version">
  <img src="https://img.shields.io/badge/Windows-10%20%7C%2011-444?style=flat-square" alt="Windows 10 and 11">
</p>

<p align="center">
  A web browser for Windows that blocks ads and trackers by default,<br>
  keeps your passwords encrypted on your PC, and stays small.<br>
  No account, no admin rights.
</p>

<p align="center">
  <a href="https://github.com/JAuxance/balise-releases/releases/latest/download/Balise-Setup.exe"><b>Download Balise-Setup.exe</b></a>
  &nbsp;·&nbsp;
  <a href="https://github.com/JAuxance/balise-releases/releases">All releases</a>
  &nbsp;·&nbsp;
  <a href="#en-français">Français</a>
</p>

---

## Features

- **Ad and tracker blocking** with EasyList, EasyPrivacy and the uBlock Origin lists, updated in the background. Can be turned off per site.
- **Password vault** encrypted with Argon2 and ChaCha20-Poly1305, stored locally. CSV import.
- **Lightweight.** An 11 MB installer. Hidden tabs are put to sleep, and tabs of the same site share one process.
- **Tabs** on top or in a sidebar, pinned tabs, mute, sound only, and clean links without trackers.
- **Profiles and private windows**, each with its own data.
- **Favorites and history** stored locally, importable from Firefox or a bookmarks file.
- **A few checked extensions**, such as Bitwarden, Dark Reader and SponsorBlock.
- **Automatic updates**, installed only when you restart Balise.
- English and French.

## Privacy

- No account, no sync, no telemetry from Balise.
- Strict tracking prevention, and Global Privacy Control sent to every site.
- No SmartScreen lookups, no WebRTC local IP leak, no link pings.
- On first launch, an optional prompt to turn off the Windows advertising ID and related sharing.

Balise renders pages with Microsoft Edge WebView2, the engine built into Windows. Windows may still send its own diagnostic data, depending on your Windows privacy settings.

## Install

1. Download [`Balise-Setup.exe`](https://github.com/JAuxance/balise-releases/releases/latest/download/Balise-Setup.exe) and run it. It installs for the current user, without admin rights.
2. If WebView2 is missing, the installer offers to add it with Microsoft's official installer.

The installer is not code-signed yet. If Windows shows "Windows protected your PC", choose **More info → Run anyway**. Each release includes a `Balise-Setup.exe.sha256` checksum.

To uninstall, run `uninstall.ps1` from `%LOCALAPPDATA%\Programs\Balise`.

## FAQ

**Is Balise built on Edge?**
It uses WebView2, the web engine Windows provides to all apps, so pages render as in Chrome or Edge. The interface, blocker, vault, profiles and updates are Balise's own, written in Rust. There is no Microsoft account, Bing or Copilot.

**Where is my data?**
Only on your PC, in `%LOCALAPPDATA%\Nav`.

**How do updates work?**
Balise checks this page regularly, downloads and verifies the new installer, then shows an Update button. It installs when you click it or close Balise.

## En français

Balise est un navigateur web léger pour Windows. Il bloque les pubs et les traqueurs par défaut, garde tes mots de passe chiffrés sur ton PC, et se met à jour tout seul. Aucun compte, pas besoin de droits administrateur.

[Télécharger `Balise-Setup.exe`](https://github.com/JAuxance/balise-releases/releases/latest/download/Balise-Setup.exe). Si Windows affiche « Windows a protégé votre ordinateur », choisis **Informations complémentaires → Exécuter quand même** : l'installeur n'est pas encore signé.
