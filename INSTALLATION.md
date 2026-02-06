# 🪗 Castagnari Benny Visualizer - Installation & Nutzung (v4.0)

## ✨ Was ist das?

Eine **interaktive Web-App** zur Visualisierung deines **Castagnari Benny C/G (3-reihig, Heim)** – perfekt zum Lernen von Akkorden, Skalen und Stücken.

### 🆕 Neue Features (v4.0)

- ✅ **iOS-Design:** Grautöne, minimale Farben, klare Hierarchie
- ✅ **Optimierter Workflow:** Akkordmodus ohne Scrollen – alles auf einen Blick
- ✅ **Grundton-Buttons:** Direkt unter Akkordtyp-Auswahl
- ✅ **Bass-Triaden:** Großbuchstabe = Dur, Kleinbuchstabe = Moll
- ✅ **Auto-Clear:** Moduswechsel löscht automatisch
- ❌ **MIDI entfernt:** Konzentration auf visuelles Lernen

---

## 📱 Auf dem iPhone nutzen

### ✅ Empfohlene Methode: Als Web-App

#### Schritt-für-Schritt:

1. **Datei auf iPhone übertragen:**
   - Per AirDrop von Mac/PC
   - ODER via iCloud Drive hochladen

2. **In Safari öffnen:**
   - Datei antippen → "Mit Safari öffnen"

3. **Zum Home-Bildschirm hinzufügen:**
   - Tippe auf das "Teilen"-Symbol (Quadrat mit Pfeil)
   - Scrolle zu "Zum Home-Bildschirm"
   - Name: "Benny Visualizer"
   - Tippe "Hinzufügen"

✅ **Fertig!** Du hast jetzt eine App auf dem Home-Screen!

**Was funktioniert auf iPhone:**
- ✅ Button-Layout Visualisierung (Push/Pull)
- ✅ Vordefinierte Stücke
- ✅ Akkordmodus (Dur/Moll/7/dim/aug/Skalen)
- ✅ Grundton-Auswahl
- ✅ Bass-Triaden (Normal-Modus)

---

## 💻 Auf dem Computer nutzen

### Lokal verwenden:

1. **Datei öffnen:**
   - Doppelklick auf `benny-visualizer.html`
   - Öffnet sich in deinem Standard-Browser

2. **Loslegen!**
   - Keine Installation nötig
   - Keine Internet-Verbindung nötig (nach erstem Laden)

**Unterstützte Browser:**
- ✅ Safari
- ✅ Chrome
- ✅ Firefox
- ✅ Edge

---

## 🌐 Online hosten (für Zugriff von allen Geräten)

### Option A: GitHub Pages (kostenlos, dauerhaft)

#### 1. GitHub Account erstellen
- Gehe zu [github.com](https://github.com)
- Erstelle einen kostenlosen Account

#### 2. Neues Repository erstellen
- Klicke auf "New Repository"
- Name: `benny-visualizer`
- Public ✅
- **NICHT** "Add a README file" anklicken
- "Create repository"

#### 3. Datei hochladen
- Klicke "uploading an existing file"
- Ziehe `benny-visualizer.html` in den Browser
- **WICHTIG:** Benenne die Datei um in `index.html`
- Klicke "Commit changes"

#### 4. GitHub Pages aktivieren
- Gehe zu "Settings" (Zahnrad-Symbol)
- Linke Sidebar: "Pages"
- Source: "Deploy from a branch"
- Branch: `main` → Ordner: `/root`
- "Save"

#### 5. Fertig!
- **URL:** `https://DEINNAME.github.io/benny-visualizer`
- Nach 1-2 Minuten live!
- Auf allen Geräten abrufbar

---

### Option B: Netlify Drop (noch einfacher)

1. Gehe zu [app.netlify.com/drop](https://app.netlify.com/drop)
2. Ziehe `benny-visualizer.html` in den Browser
3. **Fertig!** Du bekommst sofort eine URL wie:
   `https://awesome-benny-123.netlify.app`

**Vorteile:**
- ✅ Keine Anmeldung nötig
- ✅ Sofort live (keine Wartezeit)
- ✅ Custom Domain möglich (kostenlos)

**Nachteile:**
- ⚠️ URL ist zufällig generiert
- ⚠️ Datei wird nach 24h gelöscht (außer du meldest dich an)

---

### Option C: IONOS Server (für eigene Domain)

#### Voraussetzungen:
- IONOS Webhosting-Paket
- FTP-Zugang oder File Manager Zugriff

#### Via FTP (FileZilla/Cyberduck):

1. **FTP-Verbindung einrichten:**
   - Host: `ftp.DEINE-DOMAIN.de`
   - Benutzername: (von IONOS E-Mail)
   - Passwort: (von IONOS E-Mail)
   - Port: 21

2. **Datei hochladen:**
   - Navigiere zum Ordner `/` oder `/htdocs/`
   - Lade `benny-visualizer.html` hoch
   - **Optional:** Benenne um in `index.html` (dann ist es die Startseite)

3. **Fertig!**
   - URL: `https://DEINE-DOMAIN.de/benny-visualizer.html`
   - Oder: `https://DEINE-DOMAIN.de` (wenn als index.html)

#### Via IONOS File Manager:

1. **Einloggen:**
   - Gehe zu [ionos.de](https://www.ionos.de)
   - Login → "Webhosting" → "File Manager"

2. **Datei hochladen:**
   - Navigiere zu `/htdocs/` oder `/`
   - Klicke "Hochladen"
   - Wähle `benny-visualizer.html`
   - Upload abwarten

3. **Fertig!**
   - Direkt verfügbar unter deiner Domain

**Tipp:** Erstelle einen Unterordner `/akkordeon/` für bessere Organisation!

---

## 🎯 Verwendung

### Normal-Modus

**Stück lernen:**
1. Dropdown: Stück auswählen
2. Balgrichtung (Pull/Push) umschalten
3. Aktive Tasten werden angezeigt
4. Info-Panel zeigt Details (Tonart, Balg, etc.)

**Bass-Triaden visualisieren:**
1. Klicke eine **Bass-Taste** (z.B. `C`)
2. → Diskant zeigt sofort die passende Triade:
   - **Großbuchstabe** (`C`) = Dur-Triade (C-E-G)
   - **Kleinbuchstabe** (`c`) = Moll-Triade (C-Eb-G)
3. Vergleiche direkt: `C` vs `c` hin und her klicken!

**Tipp:** So lernst du die Akkordstruktur auf deinem Instrument!

---

### Akkordmodus

**Akkorde lernen – Workflow:**

1. **Modus aktivieren:**
   - Klicke "🎼 Akkorde"
   - Panel öffnet sich direkt darunter

2. **Akkordtyp wählen:**
   - Dur / Moll / Dom 7 / Maj 7 / dim / aug
   - ODER: Modale Skala (Dorisch/Mixolydisch/Phrygisch/Lydisch)

3. **Grundton wählen:**
   - Buttons direkt darunter: C, D, E, F, G, A, Bb, Ab, Eb
   - Ein Klick → Akkord leuchtet sofort auf

4. **Ergebnis sehen:**
   - **Dunkles Grau + blauer Rand** = Grundton
   - **Helles Grau** = Terz, Quinte, Septime
   - Alles **ohne Scrollen** auf einen Blick!

**Akkorde vergleichen:**
- Grundton `C` klicken → C-Dur leuchtet
- Grundton `D` klicken → D-Dur leuchtet (Akkord springt um!)
- Direkt visueller Vergleich: Welche Töne bewegen sich?

**Modale Skalen:**
1. "Dorisch" (oder andere Skala) wählen
2. Grundton klicken
3. → Alle Skalentöne werden angezeigt
4. Charakteristische Töne erkennen!

**Beispiel: G-Dur vs G-Dorisch**
1. "Dur" → "G" → Sehe: G, B, D, F#
2. "Dorisch" → "G" → Sehe: G, A, Bb, C, D, E, F
3. → Unterschied: F statt F# (charakteristischer Ton!)

---

## 🎨 Visuelle Kodierung

### Legende

| Symbol | Bedeutung | Farbe |
|--------|-----------|-------|
| ○ | Taste – nicht aktiv | Perlmutt |
| ● | Taste – aktiv (Akkordton / Stück) | Helles Grau |
| ◉ | Grundton des Akkords | Dunkles Grau + blauer Rand |
| ◌ | Skalenton (bei modalen Skalen) | Leichter Rand-Hinweis |

### Design-Prinzipien

**iOS-Stil:**
- Grautöne dominieren
- **Eine** Farbakzentuierung (Grundton = blau)
- Klare Hierarchie
- Keine schreienden Farben

**Perlmutt-Buttons:**
- Sichtbar auf **hellen** Displays
- Sichtbar auf **dunklen** Displays
- Realistischer 3D-Effekt

---

## 🎓 Lern-Beispiele

### Beispiel 1: Dur vs Moll verstehen

**Aufgabe:** Was ist der Unterschied zwischen C-Dur und c-Moll?

**Lösung:**
1. Normal-Modus
2. Bass-Taste `C` (groß) klicken
   - → Sehe: C (Grundton), E (Terz), G (Quinte)
3. Bass-Taste `c` (klein) klicken
   - → Sehe: C (Grundton), Eb (Terz!), G (Quinte)

**Erkenntnis:** Die Terz macht den Unterschied! E (Dur) vs Eb (Moll)

---

### Beispiel 2: Dorisch vs Dur

**Aufgabe:** Was macht G-Dorisch "dorisch"?

**Lösung:**
1. Akkordmodus → "Dur" → "G"
   - → Sehe: G, B, D, F# (alle Töne der G-Dur-Tonleiter)
2. Wechsel zu "Dorisch" → "G" klicken
   - → Sehe: G, A, Bb, C, D, E, F
3. Vergleiche: **F statt F#** = charakteristischer Ton!

**Erkenntnis:** Dorisch = wie Dur, aber mit kleiner 7

---

### Beispiel 3: Akkordfolge visualisieren

**Aufgabe:** Wie bewegen sich die Töne bei G → D → Em → C?

**Lösung:**
1. Akkordmodus → "Dur"
2. Nacheinander klicken:
   - `G` → Merke Position
   - `D` → Sehe wie Töne springen
   - Wechsel zu "Moll" → `E` (für Em)
   - Zurück zu "Dur" → `C`
3. Beobachte: Welche Töne bleiben, welche bewegen sich?

---

## 🎯 Deployment-Vergleich

| Methode | Aufwand | Kosten | Dauerhaft | Custom Domain |
|---------|---------|--------|-----------|---------------|
| **iPhone (lokal)** | ⭐ Einfach | Kostenlos | ✅ Ja | ❌ Nein |
| **Computer (lokal)** | ⭐ Einfach | Kostenlos | ✅ Ja | ❌ Nein |
| **GitHub Pages** | ⭐⭐ Mittel | Kostenlos | ✅ Ja | ✅ Ja (gratis) |
| **Netlify Drop** | ⭐ Sehr einfach | Kostenlos | ⚠️ 24h* | ✅ Ja (€) |
| **IONOS** | ⭐⭐⭐ Komplex | ~5€/Monat | ✅ Ja | ✅ Ja (inklusive) |

*Mit Account dauerhaft

**Empfehlung:**
- **Lernen zuhause:** Computer (lokal)
- **Unterwegs üben:** iPhone (lokal)
- **Mit anderen teilen:** GitHub Pages (kostenlos + dauerhaft)
- **Professionell:** IONOS (eigene Domain)

---

## 🔄 Updates & Versionsverwaltung

### Neue Version deployen:

**GitHub Pages:**
1. Gehe zu deinem Repository
2. Klicke auf `index.html`
3. Stift-Symbol (Edit) → Datei überschreiben
4. "Commit changes"
5. Nach 1-2 Min live!

**Netlify:**
1. Neues Deployment = neue URL
2. ODER: Mit Account → Update auf gleicher URL

**IONOS:**
1. Alte Datei löschen
2. Neue hochladen
3. Sofort live!

---

## ❓ Häufige Fragen (FAQ)

### Allgemein

**Q: Funktioniert offline?**  
A: Ja! Nach erstem Laden komplett offline nutzbar.

**Q: Welche Browser werden unterstützt?**  
A: Alle modernen Browser (Safari, Chrome, Firefox, Edge).

**Q: Funktioniert auf iPad/Android?**  
A: Ja! Alle Features funktionieren auf allen Geräten.

**Q: Warum wurde MIDI entfernt?**  
A: Braucht spezielle Hardware (USB-MIDI-Interface), die kaum jemand hat. Die App konzentriert sich auf visuelles Lernen ohne zusätzliche Hardware.

---

### Akkordmodus

**Q: Warum leuchten manche Töne nicht?**  
A: Nicht alle Töne existieren auf jeder Balgrichtung. Wechsel zwischen Push/Pull!

**Q: Was bedeutet "dunkles Grau"?**  
A: Das ist der Grundton des Akkords – der wichtigste Ton, visuell hervorgehoben.

**Q: Kann ich eigene Akkorde definieren?**  
A: Aktuell nein, aber geplant für v5.0 als "Custom Chords".

**Q: Warum gibt es nur bestimmte Grundtöne?**  
A: Die Grundtöne (C, D, E, F, G, A, Bb, Ab, Eb) entsprechen den tatsächlichen Bass-Tönen auf deinem Benny. Alle anderen Grundtöne würden Töne erfordern, die auf dem Instrument nicht existieren.

---

### Normal-Modus

**Q: Bass-Taste zeigt keine Triade?**  
A: Du bist im Akkordmodus. Wechsel zu "Normal" für Bass-Triaden.

**Q: Was ist der Unterschied zwischen Bass und Akkord-Taste?**  
A: **Großbuchstabe** (C, D, E...) = einzelner Bass-Ton. **Kleinbuchstabe** (c, d, e...) = Dreiklang (Akkord). Im Normal-Modus zeigt die App bei beiden die passende Triade auf dem Diskant.

**Q: Warum wird beim Moduswechsel alles gelöscht?**  
A: Für einen sauberen Slate. Verhindert Verwirrung zwischen Normal-Modus-Markierungen und Akkordmodus-Markierungen.

---

### Deployment

**Q: GitHub Pages lädt nicht?**  
A: Warte 2-3 Minuten. Check Settings → Pages → Status.

**Q: IONOS: Datei hochgeladen, aber 404 Error?**  
A: Check ob im richtigen Ordner (`/htdocs/`) und korrekte Berechtigungen.

**Q: Kann ich die App auf mehreren Geräten nutzen?**  
A: Ja! Entweder lokal auf jedem Gerät ODER online hosten (dann synchron auf allen Geräten).

---

## 🚀 Geplante Features (v5.0)

- [ ] Custom Chords definieren
- [ ] Akkordfolgen speichern & abspielen
- [ ] PDF-Export (Grifftabellen)
- [ ] Multi-Akkord-Vergleich (3+ gleichzeitig)
- [ ] Cloud-Sync (Einstellungen synchronisieren)
- [ ] Dark/Light Mode Toggle
- [ ] Weitere Instrumente (D/G, G/C...)

---

## 🎯 GitHub Etiquette & Open Source

### Forken vs. Kopieren
- **Forken:** Macht eine verknüpfte Kopie → respektiert den Ursprung
- **Kopieren:** Trennt die Verbindung → weniger respektvoll

### Attribution (Quellenangabe)
Wenn du Code von anderen übernimmst:
- Nenne die Quelle im README
- Oder: Kommentar im Code (`// Basiert auf github.com/user/projekt`)

### Branching
- `main` = stabiler Code
- Feature-Branches: `feature/neue-funktion`
- Bug-Fixes: `fix/button-bug`

### Pull Requests
Wenn du zum Original beitragen willst:
- Fork → Änderungen → Pull Request
- Beschreibe, was du gemacht hast
- Maintainer entscheiden über Übernahme

### Lizenzen
- MIT/Apache 2.0: Sehr permissiv, fast alles erlaubt
- GPL: Dein Projekt muss auch GPL werden
- **Diese App:** Persönliche Nutzung, bei Weiterentwicklung Quellenangabe erwünscht

---

## 📧 Support & Feedback

Bei Fragen, Bugs oder Feature-Wünschen:
- GitHub Issues (wenn auf GitHub gehostet)
- Direkte Nachricht

**Version:** 4.0  
**Letzte Aktualisierung:** Februar 2026  
**Kompatibilität:** Alle modernen Browser, iOS 14+, Android 8+

---

## 📄 Quellcode > Steuerungslogik

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

**Made with ❤️ for diatonic accordion players**# Benny