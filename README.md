# aufgabenblatt - Claude-Skill für Übungsblätter

Ein Skill für [Claude Code](https://claude.com/claude-code) und die Claude-App, der aus einer kurzen
Ansage ein druckfertiges Übungsblatt macht: LaTeX-Quelle, PDF, Lösungsblatt.

Eingabe ist ein Satz wie "Übungsblatt lineare Funktionen, Klasse 8". Heraus kommt eine
`.tex`-Datei mit 8 bis 12 Aufgaben, sortiert nach Anforderungsbereich I bis III, dahinter die
Lösungen mit Zwischenschritten. Schwarz-weiß, weil Schulen schwarz-weiß drucken.

## Was der Skill festlegt

- **Nur Aufgaben.** Kein neuer Stoff, keine Erklärtexte, kein Formelkasten. Die Annahme dahinter:
  die Klasse hat ein Merkheft, dort stehen die Formeln.
- **Imperative statt Fragen.** "Berechne die Nullstelle", nicht "Wie groß ist die Nullstelle?".
  Der Skill prüft jeden Aufgabentext vor der PDF-Erzeugung auf Fragezeichen und W-Wörter.
- **Progression innerhalb jedes Aufgabenblocks.** Nach zwei bis drei Teilaufgaben auf gleichem
  Niveau steigt der Anforderungsbereich. Der häufigste Fehler beim Aufgabenschreiben ist, zu lange
  auf AFB I zu bleiben.
- **Keine Farben.** Kein `\textcolor`, kein `\rowcolor`, keine farbigen Boxen.
- **Teilaufgaben brechen nicht um.** `\Needspace` hält zusammen, was zusammengehört.

## Installation

**Claude Code**

```bash
git clone https://github.com/johanneshohls/claude-skill-aufgabenblatt.git ~/.claude/skills/aufgabenblatt
```

Danach `claude` neu starten. Der Skill meldet sich selbst, sobald von einem Übungsblatt die Rede ist.

**Claude-App / claude.ai**

Ordner als ZIP packen und unter Einstellungen als Skill hochladen.

## Voraussetzung

Eine LaTeX-Installation mit `pdflatex`. Unter macOS reicht
[BasicTeX](https://tug.org/mactex/morepackages.html), unter Linux `texlive-latex-recommended`
plus `texlive-pictures` für TikZ.

Ob alles da ist, zeigt ein Testlauf:

```bash
cd references && pdflatex -interaction=nonstopmode template.tex
```

Das erzeugt ein dreiseitiges Beispielblatt zu linearen Funktionen.

## Inhalt

| Datei | Zweck |
|---|---|
| `SKILL.md` | Die eigentlichen Anweisungen an Claude: Aufgabenmischung, Formulierungsregeln, Layout, Checkliste vor der Ausgabe |
| `references/template.tex` | Vorlage mit Präambel, Fußzeile, Antwortzeilen-Makro, TikZ-Koordinatensystem und Lösungsteil |
| `references/template.pdf` | Das kompilierte Beispiel |

## Was ihr wahrscheinlich anpassen wollt

Der Skill ist aus meinem eigenen Unterricht entstanden, ein paar Stellen sind entsprechend gefärbt:

- **Rahmenplan Mecklenburg-Vorpommern.** Steht als Bezugsrahmen in `SKILL.md`. Für andere
  Bundesländer die Stelle im Abschnitt "Bevor du loslegst" austauschen.
- **Dateinamen-Schema `[EE][NN] AB [Name]`**, also Einheitsnummer plus laufende Nummer über alle
  Materialien einer Einheit. Praktisch, wenn man Merkhefteinträge, Arbeitsblätter und Tests in einem
  Ordner hält. Wenn ihr anders sortiert: Abschnitt "1. .tex-Datei erstellen" ändern.
- **Fußzeile** in `template.tex` steht auf "Mathematik, Klasse 8, Übungsblatt".
- **Merkheft-Annahme.** Wenn eure Klassen keins führen, gehört ein Formelkasten aufs Blatt, und
  die entsprechende Regel in `SKILL.md` muss weg.

Der Skill verweist an zwei Stellen auf verwandte Skills `lernplan` und `merkheft`. Die sind hier
nicht dabei; die Verweise stören nicht, führen aber ins Leere.

## Lizenz

MIT, siehe [LICENSE](LICENSE). Nehmt ihn, ändert ihn, gebt ihn weiter.
