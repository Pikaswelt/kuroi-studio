# Kuroi Studio

**AI Anime Video Studio für Windows und Linux.** Kuroi Studio ist eine Desktop-App für Anime-Edits, AMVs und Kurzvideos.
Herzstück ist **Kuroi Cut**, ein Schnitt-Editor im Stil von CapCut, in dem KI-Agents (z. B. Claude Code) live mitschneiden
können, während du zuschaust und selbst weiterarbeitest.

## Features
- **Kuroi Cut Editor:** Mehrspur-Timeline, Player, Inspector und Bibliothek
- **Agents schneiden live mit:** Ein Geister-Cursor zeigt, wo der Agent arbeitet. Clips teilen und verschieben sich animiert, Notizen erscheinen als Sprechblasen.
- **Verlauf mit Autor:** Jede Änderung steht im Verlauf, mit Vorschau und Zurücksetzen auf jede Version
- **Beat-Erkennung und Beat-Cuts**, Texte, Effekte, Übergänge, Keyframes, Untertitel
- **Export als MP4** über FFmpeg, mit Fortschritt im Rendering-Tab
- **Dashboard:** laufende Jobs, Live-Protokoll, fertige Videos und Systemauslastung
- **Automatische Einrichtung:** Node.js, FFmpeg, yt-dlp und Python werden beim ersten Start installiert, der KI-Agent wird automatisch verbunden

## Download
Unter **[Releases](../../releases)**:
- **Windows:** `Kuroi Studio_x.y.z_x64-setup.exe`
- **Linux:** `Kuroi Studio_x.y.z_amd64.deb` (Ubuntu, Debian, Mint …) oder `Kuroi Studio_x.y.z_amd64.AppImage` (alle Distributionen)

## Voraussetzungen
- Windows 10 oder 11 (64 Bit) mit winget (App-Installer, ist bei aktuellen Versionen dabei)
- oder Linux x86_64 mit apt, dnf, pacman oder zypper
- Optional: [Claude Code](https://claude.com/claude-code) oder Claude Desktop für den KI-Agent

Alles andere richtet die App selbst ein.

## Installation
**Windows:** Installer herunterladen und ausführen.

**Linux:**
```bash
sudo apt install "./Kuroi Studio_1.1.0_amd64.deb"
```
oder das AppImage ausführbar machen (`chmod +x`) und starten.

Beim ersten Start richtet sich Kuroi Studio selbst ein:
1. Fehlende Tools (Node.js, FFmpeg, yt-dlp, Python) werden installiert. Windows fragt dabei evtl. nach Admin-Rechten, Linux nach deinem Passwort.
2. Der MCP-Server `kuroi-studio` und der Live-Hook werden bei Claude Code (und Claude Desktop, falls installiert) eingetragen.
3. Der Editor-Server startet.

Danach Claude einmal neu starten. Projekte und Exporte liegen in `%USERPROFILE%\KuroiStudio` bzw. `~/KuroiStudio`.
Die Einrichtung lässt sich jederzeit im Dashboard unter *System Status → Fehlendes automatisch einrichten* wiederholen.

## Lizenz
Kuroi Studio ist **proprietäre Software**. Der Quellcode ist nicht öffentlich.
Du darfst die offiziellen Releases kostenlos für **private, nicht-kommerzielle Zwecke** nutzen.
Verändern, Reverse Engineering, Weitergeben, erneutes Hochladen, Verkaufen und kommerzielle Nutzung sind ohne
schriftliche Erlaubnis verboten. Details stehen in der [LICENSE](LICENSE).

© 2026 Pikaswelt. Alle Rechte vorbehalten.
