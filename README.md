# Benny Visualizer — Diatonisches Akkordeon (Castagnari Benny)

Kurzbeschreibung
----------------
Benny Visualizer ist eine kleine, rein browserbasierte Visualisierung für das diatonische Akkordeon Modell "Castagnari Benny". Die Implementation besteht aus einer einzigen HTML-Datei (index.html) mit eingebettetem CSS und JavaScript.

Quick Start
-----------
1. Repository klonen:
   git clone https://github.com/wdeu/benny-visualizer.git
2. Ins Verzeichnis wechseln und die Datei index.html im Browser öffnen:
   - Direkt durch Doppelklick auf index.html oder
   - Empfohlen: lokalen Webserver starten, z. B. mit Python 3:
     python -m http.server 8000
     und im Browser öffnen: http://localhost:8000

Hinweis zur Lizenz
------------------
Dieses Projekt steht unter der MIT License (LICENSE-Datei ist bereits im Repository vorhanden).

Steuerungslogik — exakt aus dem Quellcode
-----------------------------------------
Die README wurde automatisch an die tatsächliche Steuerungslogik in index.html angepasst. Die folgenden Punkte beschreiben das exakte Verhalten der UI und die verfügbaren Interaktionen, wie sie im JavaScript-Code implementiert sind.

Globale Zustände
- Balgrichtung (dir): 'pull' (standard) oder 'push'.
- Modus (mode): 'normal' (standard) oder 'chord' (Akkordmodus).
- activeNotes: Set, das aktive (sichtbare) Noten speichert.
- chordRoot: aktuell gewählter Grundton im Akkordmodus (oder null).
- chordType: aktuell gewählter Akkordtyp (Standard: 'maj').
- scaleType: aktuell gewählte modale Skala oder null.

UI-Elemente und Verhalten
- Balgrichtung (Segmented control): Zwei Buttons ziehen ← Pull und Push →. Umschalten ändert die sichtbare Layout-Section (pull-layout / push-layout) und lädt ggf. das jeweils für die Richtung definierte Notenset eines gewählten Stücks.

- Modus-Pills: Zwei Modi "Normal" und "Akkorde". Beim Wechsel werden aktive Noten, der gewählte Grundton und die Stücksauswahl zurückgesetzt.
  - Normal: Stück-Auswahl (Select) ist sichtbar; Info-Panel für das ausgewählte Stück wird genutzt.
  - Akkord: Chord-Panel (Akkordtypen, Skalen, Grundton-Buttons) und Legende werden sichtbar; Stück-Auswahl wird ausgeblendet.

- Chord-Panel (nur im Akkordmodus):
  - Akkordtyp (Dur, Moll, 7, Maj7, dim, aug): Auswahl legt chordType fest (bei Auswahl einer Akkordtype wird scaleType zurückgesetzt).
  - Modale Skalen (Dorisch, Mixolydisch, Phrygisch, Lydisch): Auswahl setzt scaleType; die Auswahl ist eine Umschaltfunktion (erneutes Klicken hebt die Auswahl auf). Wenn eine Skala gewählt ist, wird chordType visuell deaktiviert.
  - Grundton-Buttons: ROOTS = [C, D, E, F, G, A, Bb, Ab, Eb] werden dynamisch in der UI befüllt. Klick auf einen Grundton setzt chordRoot und aktualisiert Hervorhebungen.
  - Visuelles Ergebnis im Akkordmodus:
    - Gewählter Grundton: Klassen 'root' + 'active' (dunkles Grau, markiert).
    - Weitere Akkordtöne: Klasse 'active' (helles Grau).
    - Wenn eine Skala gewählt wurde (scaleType), erscheinen diese Töne zusätzlich mit der Klasse 'scale-tone' (leichter Rand) — aber nur, wenn sie nicht bereits als Grundton markiert sind.
  - Wichtig: In Akkordmodus sind Diskant- und Bass-Buttons nicht manuell togglebar (Klicks haben keine Wirkung auf den Zustand der Noten).

- Stück-Auswahl (nur Normal-Modus):
  - Select enthält vordefinierte Stücke (z. B. "Bourrée d'Avignon", "Chapelloise" etc.).
  - Beim Laden eines Stücks werden die im Objekt pieces definierten Noten für die aktuell gewählte Balgrichtung in activeNotes gesetzt (jeweils treble- und bass-lists) und das Info-Panel mit Metadaten (Tonart, Hauptreihe, Helferreihe, Balg-Hinweis) gefüllt.

- Diskant-Buttons (Perlmutt-Tasten):
  - Generiert aus layout[d].treble für jede Richtung (pull/push). Reihen: 'Heim', 'C', 'G' mit jeweils konkreten Beschriftungen.
  - Klick im Normal-Modus toggelt die einzelne Note (aktiv / nicht aktiv). Der Schlüssel im activeNotes-Set lautet z.B. 'pull-treble-E 9'.
  - Klick im Akkordmodus ist deaktiviert (ignoriert).

- Bass-Buttons:
  - Generiert aus layout[d].bass für jede Richtung, zwei Spalten (col1, col2).
  - Verhalten im Normal-Modus:
    - Ein Klick löscht vorherige Hervorhebungen und markiert die angeklickte Bass-Taste.
    - Großbuchstabe (z. B. 'G') interpretiert der Code als Dur, Kleinbuchstabe (z. B. 'g') als Moll.
    - Ausgehend vom Grundton der Bass-Taste wird die entsprechende Dur- oder Moll-Triade berechnet (Formeln CHORD.maj / CHORD.min) und alle passenden Diskant-Tasten in activeNotes gesetzt.
  - Verhalten im Akkordmodus: Bass-Tasten bleiben passiv (Klicks werden ignoriert).

- Info-Panel (nur sichtbar im Normal-Modus, wenn ein Stück gewählt ist):
  - Zeigt die Metadaten des Stücks an: Tonart, Hauptreihe, Helferreihe, Balg-Hinweis.

Datenmodelle
-----------
- layout: Objekt mit 'pull' und 'push' jeweils:
  - treble: Reihen 'Heim', 'C', 'G' mit Array-Beschriftungen (z. B. 'C# 10').
  - bass: col1 / col2 Arrays mit Bass-Labels (Groß-/Kleinbuchstaben sind bedeutungsvoll).
- pieces: Objekt mit vordefinierten Stücken. Jedes Stück enthält name, key, row, helper, bellows und notes (unterscheidet pull/push und listet treble/bass-Noten auf).
- CHORD / SCALE / N2S / S2N: Theorie-Utilities zur Berechnung von Akkorden und Skalen.

Datei-Struktur (im Repo)
------------------------
- index.html — gesamte Anwendung (HTML + CSS + JS)
- assets/ (optional) — z. B. assets/screenshots/ für Bilder
- LICENSE — MIT License (bereits vorhanden)

Screenshots
-----------
Die README referenziert standardmäßig die Pfade assets/screenshots/overview.png und assets/screenshots/keyboard.png. Wenn der Upload von PNG-Dateien in der GitHub-Weboberfläche bei dir ausgegraut ist, versuche eine der folgenden Alternativen:

1) Upload per Git (lokal):
   - Lege die Screenshots lokal in assets/screenshots/ ab.
   - Commit & push:
     git add assets/screenshots/*.png
     git commit -m "Add screenshots"
     git push origin main

2) GitHub-Web-UI (Drag & Drop): Öffne die Zielordneransicht (z. B. assets/screenshots/) im Web-Editor und ziehe die Dateien hinein. Falls die Schaltfläche ausgegraut bleibt, prüfe Berechtigungen bzw. Dateityp.

3) Falls deine PNG-Dateien von GitHub blockiert werden: Konvertiere kurz in JPG oder in ein anderes unterstütztes Format und lade diese hoch.

Beispiel-Markdown zum Einfügen der Screenshots (sofern die Dateien im Repo liegen):

![Übersicht](assets/screenshots/overview.png)
![Diskant-Ansicht](assets/screenshots/keyboard.png)

Contributing
------------
- Fehler melden: Erstelle ein Issue.
- Feature-Vorschläge / Änderungen: Fork → Branch → PR.
- Bitte kleine, nachvollziehbare Commits mit Beschreibung.

Automatische Anpassung & nächste Schritte
----------------------------------------
Ich habe die README basierend auf der aktuellen index.html erzeugt und werde die Datei nun im Hauptzweig (main) des Repositories speichern, wie gewünscht.

Wenn du möchtest, kann ich im nächsten Schritt:
- konkrete Screenshots als Platzhalter (geringe Auflösung) in assets/screenshots/ generieren und committen, falls du das wünschst.
- die README weiter anpassen (z. B. zusätzliche Beispiele für Tonbelegungen oder Keyboard-Mappings), nachdem du mir sagst, welche Informationen ergänzt werden sollen.