# hwz-mas-kommunikation-claude-plugin

Claude Code Plugin-Marketplace mit Skills aus dem **CAS Consulting & Communication an der HWZ Zürich**. Jeder Skill operationalisiert eine konkrete Methode aus dem Studium für die Analyse und Gestaltung von Kommunikation im Alltag — Verhandlung, Konflikt, Gewaltfreie Kommunikation, 4-Ohren-Modell, Interkulturelles, Wertequadrat/Systemisch, Rhetorik.

| | |
|---|---|
| **Marketplace** | `kommunikation-hwz-marketplace` |
| **Plugin** | `kommunikation-hwz` |
| **Repository** | `sansan88/hwz-mas-kommunikation-claude-plugin` |

## Installation

Führe die folgenden Befehle in einer Claude-Code-Session aus.

### 1. Marketplace hinzufügen

Direkt von GitHub:

```
/plugin marketplace add sansan88/hwz-mas-kommunikation-claude-plugin
```

Alternativ über die volle URL oder einen lokalen Klon-Pfad:

```
/plugin marketplace add https://github.com/sansan88/hwz-mas-kommunikation-claude-plugin
/plugin marketplace add /pfad/zum/lokalen/klon
```

### 2. Plugin installieren

```
/plugin install kommunikation-hwz@kommunikation-hwz-marketplace
```

Oder interaktiv über das Menü:

```
/plugin
```

→ *Browse marketplaces* → `kommunikation-hwz-marketplace` → `kommunikation-hwz` → **Install**.

### 3. Aktivierung prüfen

Nach der Installation stehen die Slash-Commands und Skills sofort zur Verfügung. Test:

```
/hwz-4ohren Diese Nachricht muss ich beantworten, aber ohne dass es eskaliert.
```

### Aktualisieren / Entfernen

```
/plugin marketplace update kommunikation-hwz-marketplace
/plugin uninstall kommunikation-hwz@kommunikation-hwz-marketplace
```

## Inhalt

### Skills

| Skill | Wofür |
|---|---|
| `verhandlung-harvard` | Verhandlung nach Harvard vorbereiten & reflektieren (5 Prinzipien, BATNA, 7 Phasen) |
| `konflikt-analyse` | Konfliktanalyse (Glasl-Eskalation, Teufelskreis, Dramadreieck) und Reaktionsstrategie |
| `gewaltfreie-kommunikation` | Eine Aussage / Antwort in die 4 NVC-Schritte umformen (Rosenberg) |
| `nachrichtenanalyse-4-ohren` | Eine Mail / Chat / Social-Nachricht auf 4 Ebenen analysieren (Schulz von Thun) |
| `interkulturelle-kommunikation` | Situation auf Kulturdimensionen analysieren (Uehlinger / Hofstede / Erin Meyer) |
| `wertequadrat-systemisch` | Entwicklungsblick auf Person / Verhalten (Wertequadrat + systemische Sicht) |
| `rhetorik-auftritt` | Rede / Pitch / Statement vorbereiten (Bigi, Aristoteles, 5-Satz-Methode) |

### Slash-Commands

- `/hwz-verhandlung [Anliegen]`
- `/hwz-konflikt [Anliegen]`
- `/hwz-gfk [Anliegen]`
- `/hwz-4ohren [Nachricht]`
- `/hwz-interkulturell [Anliegen]`
- `/hwz-wertequadrat [Anliegen]`
- `/hwz-rede [Anliegen]`

Die Skills feuern auch automatisch bei passenden natürlichsprachigen Anfragen — der Slash-Command ist nur die Abkürzung.

Detaillierte Beschreibung, Beispiele und Quellen: siehe [`kommunikation-hwz/README.md`](kommunikation-hwz/README.md).

## Version

0.1.0 — Initial Release (Mai 2026)
