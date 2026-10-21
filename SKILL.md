---
name: aufgabenblatt
description: >
  Erstellt druckfertige Übungs- und Aufgabenblätter als PDF für den MINT-Unterricht (Physik, Mathe, Chemie, Bio, Informatik), Klasse 5–10, orientiert am Rahmenplan MV. Dieser Skill erzeugt reine Aufgabensammlungen OHNE neuen Stoff oder Erklärungen, OHNE Formelkasten (Schüler haben das Merkheft) und immer schwarz/weiß. Verwende diesen Skill wenn der User explizit ein Übungsblatt, Aufgabenblatt, Übungszettel oder eine Aufgabensammlung möchte — also wenn es nur um Üben geht, nicht um neuen Stoff lernen. Triggern bei: "Übungsblatt", "Aufgabenblatt", "Übungszettel", "Aufgaben zu…", "Übungen für die Klassenarbeit", "Aufgabensammlung", "nur Aufgaben", oder wenn klar ist dass Schüler bereits den Stoff kennen und nur üben sollen.
---

# aufgabenblatt – Reine Übungsblätter ohne Erklärungen

## Was dieser Skill macht

Dieser Skill erstellt **reine Aufgaben- und Übungsblätter** als druckfertige PDF-Dokumente für MINT-Fächer (Physik, Mathematik, Chemie, Biologie, Informatik) der Klassen 5–10. Anders als der `lernplan`-Skill (der kombinierte Lernpläne mit Erklärungen + Aufgaben erzeugt) fokussiert dieser Skill **ausschließlich auf das Üben**:

- Kein neuer Lernstoff, keine Erklärungen, keine Zusammenfassungen
- **Kein Formelkasten** — Schüler haben das Merkheft, dort stehen alle Formeln bereits
- **8–12 Aufgaben** nach Schwierigkeit sortiert (AFB I–III), mit verschiedenen Aufgabentypen
- Ein **Lösungsblatt** mit vollständigen Lösungswegen
- Immer **schwarz/weiß** — keine Farben, keine farbigen Boxen, keine `\rowcolor`

**Einsatzszenarien**: Übungszettel vor Klassenarbeiten, Vertiefungsmaterial nach einer Unterrichtseinheit, schnelle Hausaufgabenpakete, Differenzierung für unterschiedliche Leistungsniveaus.

---

## Bevor du loslegst

### Rahmenplan MV recherchieren

Genau wie beim `lernplan`-Skill:

1. **Fach + Klasse + Thema** identifizieren (z.B. "Physik · Klasse 8 · Energieumwandlungen")
2. **Rahmenplan Mecklenburg-Vorpommern** für diese Klassenstufe und das Thema konsultieren
3. **Kompetenzanforderungen** und **Inhalte** aus dem Rahmenplan herauslesen
4. Sicherstellen, dass **alle benutzten Formeln und Konzepte** im Curriculum vorgesehen sind
5. **Kontexte/Anwendungsbeispiele** wählen, die zum Rahmenplan passen

Falls kein expliziter Rahmenplan vorliegt, auf häufige deutsche Lehrpläne (KMK-Standards) und übliche Schulbücher (Duden Physik, Lambacher Schweizer, etc.) zurückgreifen.

---

## Inhaltliche Gestaltung

### 1. Aufgaben: Struktur und Umfang

**Anzahl**: 8–12 Aufgaben (mehr als beim Lernplan, weil es keine langen Erklärungen gibt)

**Verteilung nach Anforderungsbereich (AFB)**:
- **AFB I (Reproduktion)**: 1–4 Aufgaben → einfache Berechnungen, direktes Anwenden einer Formel
- **AFB II (Transfer)**: 5–8 Aufgaben → Kombination mehrerer Formeln, einfache Fallunterscheidungen, Alltagskontexte
- **AFB III (Reflexion)**: 9–10 Aufgaben → Problemlösen, Reflexion, ggf. Begründung oder kleine Projekte

**Aufgabentypen variieren**:
- Reine **Berechnungsaufgaben** (mit Zahlen)
- **Tabellen ausfüllen** (Schüler rechnen mehrere Fälle durch)
- **Multiple Choice** (1–2 Aufgaben zur schnellen Überprüfung)
- **Graph lesen/zeichnen** (mit vorgedrucktem Koordinatensystem oder leerem Feld zum Eintragen)
- **Kurze Textantworten** (Begründungen, "Erkläre..." oder "Nenne...")
- **Mischaufgaben** (Formel-Umstellung, Textaufgaben mit Kontext)

**Progressive Schwierigkeit — kein Stagnieren auf gleichem Niveau**:

**REGEL**: Mehrere Aufgaben, die buchstäblich dasselbe üben, zusammenführen. Lieber eine Aufgabe mit 4 Unteraufgaben (a–d, von leicht nach schwer) als vier separate Aufgaben auf gleichem Schwierigkeitsniveau.

Schwierigkeit steigern durch:
- Einfache, kleine ganze Zahlen → größere Zahlen → negative Zahlen → Dezimalzahlen → Brüche
- Einschrittige Rechnung → mehrschrittige Rechnung → Rechnung mit Umstellung
- Ohne Klammern → mit Klammern → verschachtelte Klammern
- Eine Variable → mehrere Variablen

**Nach 2–3 Unteraufgaben auf gleichem Niveau: AFB erhöhen**, nicht mehr vom gleichen. Das ist der häufigste Fehler — zu lange auf AFB I verweilen.

Diese Progression gilt **pro Aufgabenblock** — nicht nur global über das ganze Blatt.

**Formulierung: ABSOLUTES NO-GO — keine Fragen, keine W-Wörter**

Jede Aufgabe beginnt mit einem Imperativ. Fragen sind verboten — auch verkleidete Fragen wie "Für welchen x-Wert gilt...?" oder "Bestimme, ob...?".

- ✓ "Berechne...", "Bestimme...", "Lies ab...", "Zeichne...", "Konstruiere...", "Vergleiche...", "Fülle aus...", "Prüfe...", "Zeige..."
- ✗ "Was ist...?", "Wie groß ist...?", "Für welchen Wert gilt...?", "Welcher Wert...?", "Liegt der Punkt...?"

**Vor der PDF-Erzeugung: Jeden Aufgabentext prüfen.** Enthält er ein Fragezeichen oder ein W-Wort am Satzanfang → umschreiben.

### 3. Lösungsblatt

**Immer enthalten, als eigene Datei** - nie im AB-PDF. Die Lösung erreichen die Schüler nur über den QR-Code oben rechts auf dem AB, und der führt zum selbrTutor, nicht in die Dropbox (siehe Schritt 4 im technischen Workflow).

- **Vollständige Lösungswege** für alle 8–12 Aufgaben
- Schrittweise Rechnung mit **Zwischenschritten**
- Ggf. **Skizzen/Diagramme** in den Lösungen (z.B. freier Fall-Diagramm)
- **Kurze Erklärungssätze** nur wo nötig (z.B. "Wir wählen die Hubarbeit-Formel, weil…")
- Eigene Datei: `<Einheit>/Lösungen/[EE][NN] [Name] - Lösung.pdf`, Quelle in `Lösungen/_Quellen/`

---

## Design-Regeln

**Alle Arbeitsblätter werden mit LaTeX erstellt** — kein HTML, kein Playwright, kein KaTeX.

- **Schrift**: `\renewcommand{\familydefault}{\sfdefault}` (CM Sans-Serif)
- **Seitenlayout**: `geometry` mit `left=2cm, right=2cm, top=2cm, bottom=2.5cm`
- **Farben**: KEINE — immer schwarz/weiß. Kein `\colorbox`, kein `\rowcolor`, keine `\definecolor`, kein `\textcolor`. Schüler drucken schwarz/weiß.
- **Header oben**: NUR der Thementitel als zentrierte Überschrift — kein „FACH · KLASSE · ÜBUNGSBLATT" darüber. Fach, Klasse und Dokumenttyp stehen ausschließlich im Footer.
- **Abschnittsheader**: Fettgedruckter Text + `\rule{\linewidth}{0.5pt}` — keine farbige Box
- **Antwortzeilen**: `\rule{\linewidth}{0.3pt}` mit 5mm Abstand, via `\antwortbereich{n}`
- **Tabellen**: Einfache `tabular`-Tabellen mit `|`-Spalten — kein `\rowcolor`
- **Koordinatensystem**: TikZ mit `arrows.meta` und Stealth-Pfeilspitzen (schwarz)
- **Fußzeile**: `fancyhdr` mit Fach · Jahrgang · Dokumenttyp

---

## Struktur des Arbeitsblatts

```
┌─────────────────────────────────────────────────────────────┐
│  KOPFZEILE (Header)                                         │
│  Nur der Thementitel — z.B. „Lage von Geraden und LGS"      │
│  KEIN „FACH · KLASSE X · ÜBUNGSBLATT" oben (steht im Footer)│
└─────────────────────────────────────────────────────────────┘

┌─────────────────────────────────────────────────────────────┐
│  AUFGABEN (nach Schwierigkeit sortiert)                    │
│                                                             │
│  1–4: AFB I (Reproduktion)                                 │
│       - Einfache Berechnungen                              │
│       - Direkte Formelanwendung                            │
│                                                             │
│  5–8: AFB II (Transfer)                                    │
│       - Mehrschrittiges Rechnen                            │
│       - Alltagskontexte                                    │
│       - Kleine Formel-Umstellungen                         │
│                                                             │
│  9–10: AFB III (Reflexion)                                 │
│        - Problemlösen                                       │
│        - Begründungen                                       │
│        - Ggf. Bonusaufgaben                                │
│                                                             │
│  BONUS (optional)                                          │
│        - Knifflige Aufgabe                                 │
│        - Fächerübergreifend (optional)                     │
└─────────────────────────────────────────────────────────────┘

[Seitenumbruch – neue Seite]

┌─────────────────────────────────────────────────────────────┐
│  LÖSUNGEN                                                   │
│  [Vollständige Lösungswege zu allen Aufgaben]              │
│  (Ggf. hinter Lochung / für Lehrer separat)               │
└─────────────────────────────────────────────────────────────┘
```

---

## LaTeX — Mathematische Notation

**Alle Arbeitsblätter werden mit LaTeX erstellt** — kein HTML, kein KaTeX, kein Playwright.

### Inline-Mathe
```latex
Die Steigung ist $m = \dfrac{y_2 - y_1}{x_2 - x_1}$.
```

### Abgesetzte Formel
```latex
\[ P = \frac{W}{t} \]
```

### Häufige Befehle

| Befehl | Output |
|--------|--------|
| `\cdot` | · |
| `\dfrac{a}{b}` | Bruch (display-Größe) |
| `\approx` | ≈ |
| `\sqrt{x}` | Wurzel |
| `^2`, `_i` | hoch-/tiefgestellt |
| `\Rightarrow` | ⇒ |
| `\checkmark` | ✓ |
| `\alpha, \beta` | Griechische Buchstaben |

### Dezimalnotation (Deutsch)
`$0{,}5$` → 0,5 (Komma als Dezimaltrennzeichen)

---

## TikZ — Koordinatensysteme und Diagramme

TikZ direkt in LaTeX — kein TikZJax, kein JavaScript.

### Standardvorlage Koordinatensystem

```latex
\usepackage{tikz}
\usetikzlibrary{arrows.meta}

\begin{tikzpicture}[scale=0.65]
  \draw[very thin,gray!30] (-4.5,-4.5) grid (5.5,5.5);
  \draw[-{Stealth[length=6pt]},thick]
    (-4.8,0) -- (5.8,0) node[right,font=\small] {$x$};
  \draw[-{Stealth[length=6pt]},thick]
    (0,-4.8) -- (0,5.8) node[above,font=\small] {$y$};
  \foreach \x in {-4,...,5} {
    \draw[thin] (\x,0.08) -- (\x,-0.08);
    \node[below,font=\scriptsize] at (\x,-0.15) {\x};
  }
  \foreach \y in {-4,...,5} {
    \draw[thin] (0.08,\y) -- (-0.08,\y);
    \node[left,font=\scriptsize] at (-0.15,\y) {\y};
  }
\end{tikzpicture}
```

---

## Technischer Workflow: LaTeX → PDF

Ausgangspunkt ist `references/template.tex`. Die Datei kompiliert unverändert mit `pdflatex` und enthält Präambel, Fußzeile, Antwortzeilen-Makro, ein TikZ-Koordinatensystem und einen Lösungsteil. Kopieren, Inhalt ersetzen, kompilieren.

### 1. .tex-Datei erstellen

**Dateiname:** Schema `[EE][NN] AB [Name]` (z.B. `0405 AB Nullstellen.tex`)

- `EE` = zweistellige Einheitsnummer des Jahres (z.B. `04`)
- `NN` = laufende Nummer quer durch ALLE Materialtypen (MH, AB, Test, KA, TÜ) dieser Einheit — alle PDFs im Einheitsordner zählen, dann +1
- `[Name]` = kurzer beschreibender Name — kein Datum, keine Klasse
- Dokument-ID klein im Footer: z.B. `· 0405 ·` zwischen den übrigen Footer-Infos
- **Keine klassenspezifischen Kopien** — dasselbe AB gilt für alle Klassen, mehrfach hochladen

Pflicht-Pakete:
```latex
\usepackage[T1]{fontenc}
\usepackage[utf8]{inputenc}
\usepackage[ngerman]{babel}
\usepackage[left=2cm,right=2cm,top=2cm,bottom=2.5cm]{geometry}
\usepackage{amsmath,amssymb}
\usepackage{tikz}
\usetikzlibrary{arrows.meta}
\usepackage{array,booktabs}
\usepackage{fancyhdr}
\renewcommand{\familydefault}{\sfdefault}
```

Antwortzeilen-Makro (zuverlässig, kein Loop-Problem):
```latex
\newcommand{\AL}{\noindent\rule{\linewidth}{0.3pt}\par\vspace{5mm}}
\newcommand{\antwortbereich}[1]{\vspace{3mm}\ifcase#1\or\AL\or\AL\AL\or\AL\AL\AL%
\or\AL\AL\AL\AL\or\AL\AL\AL\AL\AL\or\AL\AL\AL\AL\AL\AL\or\AL\AL\AL\AL\AL\AL\AL%
\or\AL\AL\AL\AL\AL\AL\AL\AL\or\AL\AL\AL\AL\AL\AL\AL\AL\AL\fi\vspace{1mm}}
```

### 2. Kompilieren

```bash
cd /pfad/zum/ordner
pdflatex -interaction=nonstopmode dateiname.tex
```

Erfolg: `Output written on dateiname.pdf (N pages, ...)`

Fehlersuche: `.log`-Datei prüfen, Zeile mit `!` suchen.

### 3. Aufräumen

```bash
rm dateiname.aux dateiname.log
```

### 4. QR-Code zum selbrTutor

Jedes AB bekommt oben rechts einen QR-Code mit der Beschriftung "Hilfe & Lösung". Er führt zu `https://selbr.app/blatt/<klasse>-<nr>`: dort wählt das Kind eine Aufgabe, holt sich einen Einstieg oder lässt eine fotografierte Rechnung prüfen, und als letzte Stufe öffnet es die Lösung. **Kein QR-Code führt direkt in die Dropbox.**

1. Tutor-Entwurf schreiben (JSON, ins Scratchpad): `titel`, `hinweis` (zwei bis drei Sätze an das Kind, ohne Lösung) und `aufgaben` mit je `nr` (wie auf dem Blatt), `titel` (zwei bis vier Wörter), `text` (Aufgabe vollständig, Formeln in `$...$`, Teilaufgaben je Zeile mit `\n`, Tabellen zeilenweise) und `loesung` (reiner Text ohne `$`, Teilaufgaben a), b) ... hintereinander). Vorbild: `~/Projekte/selbr/public/blaetter/8-0146.json`.
2. Aufrufen:
   ```bash
   ~/scripte/ab-tutor.py --blatt <entwurf.json> ".../Arbeitsblätter/_Quellen/[EE][NN] AB [Name].tex"
   ```
   Das Skript teilt die Lösung, legt das Blatt in selbr an und pusht es, rendert den QR, baut `\tutorqr` ins TeX, kompiliert zweimal, legt die PDF nach `Arbeitsblätter/` und prüft den Code mit `ab-share.sh verify`. Erst bei "Fertig: https://selbr.app/blatt/..." ist das AB druckbar.

### 5. Qualitätsprüfung

PDF öffnen und prüfen: Formeln korrekt? Tabellen vollständig? Koordinatensystem sauber? Keine Textabschneidungen? QR oben rechts mit "Hilfe & Lösung"?

---

## Hinweise (für Lehrer und Skill-Nutzer)

1. **Für Lehrer**:
   - Das Aufgabenblatt ist **sofort druckbar** (schwarz/weiß, schülernah)
   - Lösung liegt als eigene Datei vor und wird nicht ausgeteilt - die Schüler kommen über den QR-Code im selbrTutor an sie heran
   - Zeitrahmen: Je nach Klassenstufe und Aufgabentyp 30–60 Min.

2. **Kontextwahl**:
   - Aufgaben sollten aus dem **Alltag** oder **typischen Textaufgaben** sein
   - Zahlenbeispiele realistisch halten (keine absurden Werte)
   - Aufbau von AFB I → AFB III schafft Motivation ("Das kann ich!")

3. **Formelnwahl**:
   - Nur Formeln verwenden, die im entsprechenden **Rahmenplan** vorgesehen sind
   - Bei Formelumstellung: nur einstufig (max. zwei Schritte), sonst wird es zu schwer für reine Übung

4. **Bonus-Aufgaben**:
   - Optional, für stärkere Schüler
   - Kann fächerübergreifend sein oder eine größere Reflexion einfordern

5. **Differenzierung**:
   - Der Skill kann verschiedene Blätter für verschiedene Leistungsniveaus erzeugen:
     - **Basis-Blatt**: 6–8 Aufgaben, nur AFB I–II
     - **Standard-Blatt**: 10–12 Aufgaben, AFB I–III
     - **Erweiterung**: +2 Bonus mit Projektcharakter

6. **Zusammenhang mit `lernplan`**:
   - Ein `lernplan` könnten zunächst Erklärung + erste Übungsaufgaben enthalten
   - Danach folgt ein `aufgabenblatt` zur Vertiefung
   - Oder: `aufgabenblatt` allein, wenn Schüler den Stoff bereits beherrschen

---

## Checkliste vor Ausgabe

- [ ] Dateiname nach Schema `[EE][NN] AB [Name]` (z.B. `0405 AB Nullstellen`)?
- [ ] Dokument-ID im Footer (z.B. `· 0405 ·`)?
- [ ] **Kein Datum- und kein Namensfeld** im Header?
- [ ] **Header oben enthält NUR den Thementitel** — kein „FACH · KLASSE · ÜBUNGSBLATT" (das gehört in den Footer)?
- [ ] **Keine klassenspezifische Kopie** — ein AB für alle Klassen?
- [ ] Fach, Klasse und Thema korrekt?
- [ ] **KEIN Formelkasten** — Schüler haben das Merkheft?
- [ ] **KEINE Farben** — kein `\colorbox`, kein `\rowcolor`, kein `\textcolor`, kein `\definecolor`?
- [ ] 8–12 Aufgaben vorhanden, AFB I–III verteilt?
- [ ] **AFB-Progression schnell genug** — nicht mehr als 2–3 Unteraufgaben auf gleichem Niveau, bevor AFB steigt?
- [ ] **PFLICHT: Jeder Aufgabentext beginnt mit Imperativ — kein einziges Fragezeichen, kein W-Wort am Satzanfang?**
- [ ] Lösungsblatt vollständig mit Zwischenschritten?
- [ ] `ab-tutor.py` mit "Fertig" durchgelaufen, QR führt zu selbr?
- [ ] LaTeX fehlerfrei kompiliert (kein `!` im Log)?
- [ ] PDF-Layout: Kein Text abgeschnitten, alle Seiten sichtbar?
- [ ] TikZ-Koordinatensysteme korrekt gerendert?
- [ ] Deutsche Dezimalnotation (`{,}`) konsistent?
