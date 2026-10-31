# Kuroi Studio

**AI Anime Video Studio für Windows.** Kuroi Studio ist eine Desktop-App für Anime-Edits, AMVs und Kurzvideos.
Herzstück ist **Kuroi Cut**, ein Schnitt-Editor im Stil von CapCut, in dem KI-Agents (z. B. Claude Code) live mitschneiden
können, während du zuschaust und selbst weiterarbeitest.

## Features
- **Kuroi Cut Editor:** Mehrspur-Timeline, Player, Inspector und Bibliothek
- **Agents schneiden live mit:** Ein Geister-Cursor zeigt, wo der Agent arbeitet. Clips teilen und verschieben sich animiert, Notizen erscheinen als Sprechblasen.
- **Verlauf mit Autor:** Jede Änderung steht im Verlauf, mit Vorschau und Zurücksetzen auf jede Version
- **Beat-Erkennung und Beat-Cuts**, Texte, Effekte, Übergänge, Keyframes, Untertitel
- **Export als MP4** über FFmpeg, mit Fortschritt im Rendering-Tab
- **Dashboard:** laufende Jobs, Live-Protokoll, fertige Videos und Systemauslastung

## Download
Den Installer (`Kuroi Studio_x.y.z_x64-setup.exe`) gibt es unter **[Releases](../../releases)**.

## Voraussetzungen
- Windows 10 oder 11 (64 Bit)
- [Node.js](https://nodejs.org) 20 oder neuer
- [FFmpeg](https://ffmpeg.org) im `PATH` (`ffmpeg` und `ffprobe`)
- Optional: [yt-dlp](https://github.com/yt-dlp/yt-dlp) für Downloads, [Claude Code](https://claude.com/claude-code) für den KI-Agent

## Installation
1. Installer aus den Releases herunterladen und ausführen
2. Kuroi Studio starten. Beim ersten Start legt die App den Ordner `%USERPROFILE%\KuroiStudio` an, dort liegen deine Projekte und Exporte.

### KI-Agent verbinden (optional)
Damit Claude Code im Editor mitschneiden kann, registrierst du den mitgelieferten MCP-Server einmalig:

```bash
claude mcp add --scope user kuroi-studio -- node "%USERPROFILE%\KuroiStudio\studio\server.mjs"
```

## Lizenz
Kuroi Studio ist **proprietäre Software**. Der Quellcode ist nicht öffentlich.
Du darfst die offiziellen Releases kostenlos für **private, nicht-kommerzielle Zwecke** nutzen.
Verändern, Reverse Engineering, Weitergeben, erneutes Hochladen, Verkaufen und kommerzielle Nutzung sind ohne
schriftliche Erlaubnis verboten. Details stehen in der [LICENSE](LICENSE).

© 2026 Pikaswelt. Alle Rechte vorbehalten.
