# kommunikation-hwz

Skills, die das CAS Consulting & Communication an der HWZ Zürich in tagestaugliche Werkzeuge übersetzen. Jeder Skill operationalisiert eine konkrete Methode aus deinem Studium und wendet sie auf reale Situationen an: E-Mails, Chats, Verhandlungen, Konflikte, Reden.

## Skills

| Skill | Wofür |
|---|---|
| `verhandlung-harvard` | Vorbereitung & Reflexion einer Verhandlung nach Harvard (5 Prinzipien, BATNA, 7 Phasen) |
| `konflikt-analyse` | Konfliktanalyse (Glasl-Eskalation, Teufelskreis, Dramadreieck) und Reaktionsstrategie |
| `gewaltfreie-kommunikation` | Eine Aussage / Antwort in die 4 NVC-Schritte umformen (Rosenberg) |
| `nachrichtenanalyse-4-ohren` | Eine Mail / Chat / Social-Nachricht auf 4 Ebenen analysieren (Schulz von Thun) |
| `interkulturelle-kommunikation` | Situation auf Kulturdimensionen analysieren (Uehlinger / Hofstede / Erin Meyer) |
| `wertequadrat-systemisch` | Entwicklungsblick auf Person / Verhalten (Wertequadrat + systemische Sicht) |
| `rhetorik-auftritt` | Rede / Pitch / Statement vorbereiten (Bigi, Aristoteles, 5-Satz-Methode) |

## Slash-Commands

- `/hwz-verhandlung [Anliegen]`
- `/hwz-konflikt [Anliegen]`
- `/hwz-gfk [Anliegen]`
- `/hwz-4ohren [Nachricht]`
- `/hwz-interkulturell [Anliegen]`
- `/hwz-wertequadrat [Anliegen]`
- `/hwz-rede [Anliegen]`

Die Skills feuern auch automatisch bei passenden natürlichsprachigen Anfragen — der Slash-Command ist nur die Abkürzung.

## Verwendung — typische Beispiele

- *"Ich habe morgen ein Gespräch mit dem Chef über Gehalt — kannst du mir helfen, das vorzubereiten?"* → `verhandlung-harvard`
- *"Mein Kollege schreibt mir nur noch ganz knapp und mit CC an alle. Was ist da los?"* → `nachrichtenanalyse-4-ohren`, evtl. `konflikt-analyse`
- *"Diese Nachricht muss ich beantworten, aber ohne dass es eskaliert."* → `gewaltfreie-kommunikation`
- *"Ich finde meine Schwester einfach zu chaotisch."* → `wertequadrat-systemisch`
- *"Wir haben ein Meeting mit dem indischen Partner und ich verstehe nicht, warum nichts vorwärts geht."* → `interkulturelle-kommunikation`
- *"Hochzeitsrede in 3 Wochen."* → `rhetorik-auftritt`
- *"Im Team kracht es seit Monaten zwischen X und Y."* → `konflikt-analyse`

## Installation (Claude Code / Cowork)

### Variante A — Plugin lokal installieren

Wenn du Claude Code mit Plugin-Unterstützung nutzt:

```bash
# Im Claude Code:
/plugin marketplace add /Users/sandro/SynologyDrive/Studium/Master/HWZ/01_Fächer/02_Communication_Consulting/plugin
/plugin install kommunikation-hwz
```

### Variante B — Skills direkt benutzen

Du musst nicht installieren. Wenn du in einer Cowork-Session arbeitest und den Ordner mit den Skills gemounted hast, kannst du Claude auch direkt sagen:

> *Lies `kommunikation-hwz/skills/nachrichtenanalyse-4-ohren/SKILL.md` und wende es auf die folgende Nachricht an: …*

Claude wird die Skill-Datei lesen und dem Vorgehen folgen.

## Aufbau eines Skills

```
skills/<skill-name>/
├── SKILL.md           # Hauptdatei: wann verwenden, Workflow, Methode
├── references/        # Tiefere Inhalte (Modelle, Listen, Tipps)
└── templates/         # Ausfüllbare Vorlagen
```

Das `SKILL.md` ist die Pflichtdatei. Die Frontmatter (`name`, `description`) entscheidet, *wann* Claude den Skill triggert.

## Quellen

Alle Skills basieren auf den Originalskripten und Handouts deines CAS Consulting & Communication an der HWZ Zürich:

- **Skript Kommunikation** (Dr. Bettina Hoffmann)
- **Skript Verhandeln** (Dr. Bettina Hoffmann)
- **Skript Systemtheorie und Konstruktivismus** (Hoffmann)
- **Skript Teamentwicklung und systemische Beratung** (Hoffmann)
- **Handouts Wertequadrat, Systemische Beratung** (Hoffmann)
- **Handouts und Checklisten zur Interkulturellen Kommunikation** (Dr. Christa Uehlinger)
- **Handouts Rhetorische Auftrittskompetenz** (Dr. phil. Hugo Bigi)

Ergänzt um die Standard-Literatur (Rosenberg, Watzlawick, Fisher/Ury/Patton, Schulz von Thun, Glasl, Hofstede, Trompenaars, Erin Meyer, Bateson, Schlippe, Aristoteles).

## Version

0.1.0 — Initial Release (Mai 2026)
