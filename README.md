# Pflegegutachten prüfen – Skill für Claude

Ein Skill für [Claude](https://claude.ai), der Pflegegutachten des Medizinischen Dienstes (MD) oder von Medicproof nach dem Neuen Begutachtungsassessment (NBA) prüft. Er rechnet die Punkte nach, findet typische Fehler und erstellt einen begründeten Widerspruch, eine Stellungnahme oder einen Höherstufungsantrag als Word-Datei.

> **Wichtiger Hinweis:** Dieser Skill ist eine Hilfe zur Selbsthilfe und **keine Rechtsberatung**. Er ersetzt nicht die Beratung durch einen Pflegestützpunkt, einen Sozialverband (z. B. VdK, SoVD) oder eine Fachanwältin bzw. einen Fachanwalt für Sozialrecht. Alle Ergebnisse sind vor der Verwendung selbst zu prüfen. Es wird keine Haftung für die Richtigkeit übernommen.

## Für wen?

- Pflegende Angehörige und gesetzliche Betreuer
- Pflegeeltern und Eltern pflegebedürftiger Kinder
- Pflegeberaterinnen und Pflegeberater, Sozialdienste, Pflegedienste

## Was der Skill macht

1. **Gutachten einlesen:** Eckdaten, Verfahrensart, Bewertungen und Befundtexte aller Kriterien erfassen
2. **Punkte nachrechnen:** Einzelpunkte je Modul, gewichtete Punkte nach Anlage 2 zu § 15 SGB XI, Gesamtpunkte und Pflegegrad
3. **Gutachten prüfen:** Widersprüche zwischen Befund und Bewertung, Widersprüche zwischen Modulen, nicht berücksichtigte Diagnosen, fehlende Befragung der Pflegeperson, Verfahrensmängel, Herabstufung ohne Begründung
4. **Ehrlich einschätzen:** realistisch erreichbarer Pflegegrad, mit vorsichtiger und realistischer Rechnung
5. **Schreiben erstellen:** Widerspruch mit Vergleichstabelle, neuer Punkteberechnung, Platzhaltern für das Pflegetagebuch und Anlagenverzeichnis
6. **Fristen berechnen:** Widerspruchsfrist, Bekanntgabe per Post, fehlende Rechtsbehelfsbelehrung; Hinweise für privat Versicherte

Enthalten sind alle Kriterien der Module 1 bis 6, die Bewertungsskalen, die vollständige Umrechnung für Modul 5 und die Schwellenwerte der Pflegegrade.

## Installation

**Claude (Web, Desktop, App):**
1. Den Ordner `pflegegutachten-pruefung` als ZIP-Datei herunterladen (oder die Datei `SKILL.md` in einen Ordner dieses Namens legen und den Ordner zippen).
2. In Claude in den Einstellungen den Bereich für Skills öffnen und die ZIP-Datei als eigenen Skill hochladen.

**Claude Code:**
```
mkdir -p ~/.claude/skills/pflegegutachten-pruefung
cp SKILL.md ~/.claude/skills/pflegegutachten-pruefung/
```

## Verwendung

Das Gutachten (meist als PDF) und wenn möglich den Bescheid hochladen und kurz dazuschreiben, worum es geht, zum Beispiel:

> Prüf bitte dieses Gutachten. Widerspruch gegen Pflegegrad 2, Ziel Pflegegrad 3, Bescheid vom 10.11., Pflegeperson ist die Tochter. Nachts steht meine Mutter drei- bis viermal auf.

Claude liefert zuerst ein Kurzfazit mit Punkten, Angriffspunkten und Frist und erstellt danach auf Wunsch das Schreiben.

## Datenschutz

Pflegegutachten enthalten Gesundheitsdaten. Laden Sie nur Unterlagen hoch, zu denen Sie berechtigt sind, und teilen Sie Ergebnisse nicht öffentlich.

## Rechtsstand

Bewertungssystematik nach Anlagen 1 und 2 zu § 15 SGB XI, Stand November 2026. Bei Gesetzesänderungen bitte die aktuelle Fassung prüfen.

## Autor

Andreas Rennhack, Buchholz i. d. Nordheide

Rückmeldungen und Verbesserungsvorschläge gern über die Issues dieses Repositorys.

## Lizenz

Siehe Datei `LICENSE`.
