# 🪗 Castagnari Benny Visualizer

**Interaktive Web-App für Castagnari Benny C/G (3-reihig, Heim)**

![Version](https://img.shields.io/badge/version-4.0-blue)
![License](https://img.shields.io/badge/license-Personal-green)

<p align="center">
  <img src="https://github.com/wdeu/benny-visualizer/blob/main/assets/screenshots/Benny.png?raw=true" alt="Castagnari Benny" width="400"/>
</p>

---

## 📸 Screenshots

<p align="center">
  <img src="https://github.com/wdeu/benny-visualizer/blob/main/assets/screenshots/benny-visualizer-iphone.png?raw=true" alt="iPhone View" width="20%"/>
  <img src="https://github.com/wdeu/benny-visualizer/blob/main/assets/screenshots/benny-visualizer-mac.png?raw=true" alt="Desktop View" width="30%"/>
  <img src="https://github.com/wdeu/benny-visualizer/blob/main/assets/screenshots/Push_Pull.png?raw=true" alt="Push-Pull-View" width="40%"/>
  
  
</p>

---

## ✨ Features

### 🎵 Basis
- **Button-Layout Visualisierung** (Push/Pull getrennt)
- **Spieler-Perspektive** (wie du von oben draufschaust: Helfer links, G rechts)
- **Side-by-Side Layout** – Bass & Diskant nebeneinander bei genug Platz (Desktop, Tablet Landscape)
- **Responsive Design** – automatische Anpassung an Portrait/Landscape
- **Perlmutt-Design** – sichtbar auf hellen & dunklen Displays
- **iOS-typisches Design** – Grautöne, minimale Farben, klare Hierarchie
- **Vordefinierte Stücke** (Bourrées, Polkas, Scottishs)

### 🎼 Akkordmodus
- **Direkter Grundton-Zugriff** – Buttons direkt unter Modus-Auswahl
- **Kein Scrollen nötig** – alles auf einen Blick
- **Live-Vergleich** – Grundton wechseln → Akkorde springen sofort um
- **Akkordtypen:** Dur, Moll, Dom 7, Maj 7, dim, aug
- **Modale Skalen:** Dorisch, Mixolydisch, Phrygisch, Lydisch
- **Visuelle Kodierung:**
  - **Dunkles Grau + blauer Rand** = Grundton (einzige Farbakzentuierung)
  - **Helles Grau** = andere Akkordtöne
  - **Perlmutt** = nicht aktive Tasten

### 🎹 Bass-Intelligenz (Normal-Modus)
- **Großbuchstabe klicken** (z.B. `C`) → zeigt C-Dur-Triade auf Diskant
- **Kleinbuchstabe klicken** (z.B. `c`) → zeigt c-Moll-Triade auf Diskant
- Perfekt zum schnellen Vergleichen: `C` vs `c` hin und her klicken!

### 🧹 Auto-Clear
- **Moduswechsel löscht alles** – kein "Alle löschen"-Button nötig
- Wechsel zwischen Normal/Akkord → sauberer Slate

---

## 🚀 Schnellstart

### Lokal nutzen
1. `benny-visualizer.html` doppelklicken
2. Im Browser öffnen
3. Loslegen!

### iPhone/iPad
1. Datei per AirDrop übertragen
2. In Safari öffnen
3. "Zum Home-Bildschirm hinzufügen"

### Online hosten
- **GitHub Pages:** Kostenlos, dauerhaft → [Anleitung](INSTALLATION.md#option-a-github-pages)
- **Netlify Drop:** Ultra-schnell → [Anleitung](INSTALLATION.md#option-b-netlify-drop)
- **IONOS:** Eigene Domain → [Anleitung](INSTALLATION.md#option-c-ionos-server)

📖 **Vollständige Anleitung:** [INSTALLATION.md](INSTALLATION.md)

---

## 🎯 Verwendung

### Normal-Modus
**Stück lernen:**
1. Stück aus Dropdown wählen
2. Balgrichtung (Pull/Push) anpassen
3. Aktive Tasten werden angezeigt

**Bass → Diskant Triaden:**
1. Klicke eine Bass-Taste
2. → Diskant zeigt sofort die passende Triade
   - `C` (groß) = C-Dur (C-E-G)
   - `c` (klein) = c-Moll (C-Eb-G)
3. Vergleiche direkt: `C` vs `c` hin und her klicken!

### Akkordmodus
**Akkorde lernen:**
1. Klick auf "🎼 Akkorde"
2. Wähle Akkordtyp (Dur/Moll/7/...)
3. **Direkt darunter:** Klicke Grundton (C, D, E, ...)
4. → Diskant zeigt sofort den Akkord:
   - **Dunkles Grau + blauer Rand** = Grundton
   - **Helles Grau** = Terz, Quinte, ...

**Akkorde vergleichen:**
1. Grundton `C` klicken → C-Dur leuchtet
2. Grundton `D` klicken → D-Dur leuchtet (Akkord springt sofort um!)
3. → Direkter visueller Vergleich ohne Scrollen

**Modale Skalen:**
1. Klicke "Dorisch" (oder andere Skala)
2. Grundton wählen
3. → Alle Skalentöne werden angezeigt
4. Charakteristische Töne erkennen!

---

## 🎨 Design-Philosophie

### iOS-Stil
- **Grautöne dominieren** – ruhig, professionell
- **Eine Farbakzentuierung** – nur der Grundton (blau)
- **Perlmutt-Buttons** – sichtbar auf allen Display-Modi
- **Klare Hierarchie** – wichtigste Funktion zuerst

### Visuelle Kodierung
```
┌─────────────────────────────────────┐
│ ○  Perlmutt – nicht aktiv           │
│ ●  Helles Grau – aktiv (Akkordton)  │
│ ◉  Dunkles Grau + blau – Grundton   │
│ ◌  Leichter Rand – Skalenton        │
└─────────────────────────────────────┘
```

### Workflow-Optimierung
**Problem:** Vorher musste man oben Modus wählen, nach unten scrollen zum Bass, wieder hoch zum Diskant.

**Lösung:** Jetzt alles direkt untereinander ohne Scrollen:
```
Modus wählen
    ↓
Akkordtyp wählen (direkt darunter)
    ↓
Grundton wählen (direkt darunter)
    ↓
Diskant sehen (direkt darunter)
```

---

## 🛠️ Technische Details

### Datei
- **Single HTML File** – keine Dependencies
- **~680 Zeilen** – kompakter, sauberer Code
- **Offline-fähig** nach erstem Laden

### Browser-Kompatibilität
| Browser | Status |
|---------|--------|
| Safari (iOS/macOS) | ✅ Vollständig |
| Chrome | ✅ Vollständig |
| Firefox | ✅ Vollständig |
| Edge | ✅ Vollständig |

### Responsive Design
- **Desktop (≥800px):** Side-by-Side – Bass links, Diskant rechts, kein Scrollen
- **Tablet Landscape:** Side-by-Side – optimale Übersicht
- **iPhone Landscape:** Side-by-Side – Bass & Diskant nebeneinander
- **Portrait (<800px):** Vertikal gestapelt – Diskant oben, Bass unten
- **Smartphone:** Kompakte Darstellung (ab 320px)

---

## 🎓 Lern-Beispiele

### Akkorde verstehen
```
Aufgabe: Was ist der Unterschied zwischen C-Dur und c-Moll?

1. Normal-Modus → Bass "C" klicken
   → Sehe: C (Grundton), E (Terz), G (Quinte)

2. Bass "c" klicken
   → Sehe: C (Grundton), Eb (Terz!), G (Quinte)

Erkenntnis: Die Terz macht den Unterschied! E vs Eb.
```

### Modale Skalen erforschen
```
Aufgabe: Was macht Dorisch "dorisch"?

1. Akkordmodus → "Dur" wählen → "G" klicken
   → Merke: F# ist dabei

2. "Dorisch" wählen → "G" klicken
   → Sehe: F statt F# (charakteristischer Ton!)

3. Hin und her wechseln → direkter Vergleich

Erkenntnis: Dorisch = wie Dur, aber mit kleiner 7 (F statt F#)
```

### Akkordfolgen visualisieren
```
Aufgabe: Wie sieht die Folge G - D - Em - C aus?

1. Akkordmodus → "Dur"
2. Klicke nacheinander: G → D → C
3. Zwischendurch "Moll" wählen → E klicken (für Em)
4. → Sehe, wie sich die Töne bewegen!
```

---

## 📊 Version History

### v4.0 (Februar 2026) – iOS Design Refresh + Side-by-Side
- 🎨 **iOS-typisches Design** mit Grautönen
- 🖥️ **Side-by-Side Layout** – Bass & Diskant nebeneinander (Desktop/Tablet Landscape)
- 📱 **Auto-Rotation** – iPhone Landscape → automatisch Side-by-Side
- 🎯 **Grundton-Buttons** direkt im Akkord-Panel
- 🔄 **Workflow optimiert** – kein Scrollen mehr nötig
- 🎹 **Bass-Triaden** im Normal-Modus (Groß-/Kleinbuchstabe)
- 🧹 **Auto-Clear** beim Moduswechsel
- 🗑️ **"Alle löschen"** Button entfernt (überflüssig)
- 💎 **Perlmutt-Optik** verbessert (helle + dunkle Displays)
- ❌ **MIDI entfernt** (zu Nische, kaum Hardware vorhanden)

### v3.0 (Februar 2026)
- ➕ Akkordmodus (Dur/Moll/7/maj7/dim/aug)
- ➕ Modale Skalen
- ➕ MIDI-Erkennung
- ➕ Farbcodierung

### v2.0 (Februar 2026)
- 🔧 Korrekte Belegung nach Fotos
- 🔧 Spieler-Perspektive
- 🔧 Perlmutt-Design

### v1.0 (Februar 2026)
- ✨ Initial Release
- ✨ Basic Layout-Visualisierung

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
- **Lernen zuhause:** Lokal (Doppelklick)
- **Unterwegs üben:** iPhone (Home-Screen)
- **Mit anderen teilen:** GitHub Pages
- **Professionell:** IONOS (eigene Domain)

---

## ❓ Häufige Fragen (FAQ)

### Allgemein

**Q: Funktioniert offline?**  
A: Ja! Nach erstem Laden komplett offline nutzbar.

**Q: Warum kein MIDI mehr?**  
A: Braucht USB-MIDI-Interface (sehr selten). App konzentriert sich auf visuelles Lernen.

**Q: Funktioniert auf iPad/Android?**  
A: Ja! Alle modernen Browser werden unterstützt.

### Akkordmodus

**Q: Warum leuchten manche Töne nicht?**  
A: Nicht alle Töne existieren auf beiden Balgrichtungen. Wechsel zwischen Push/Pull!

**Q: Was bedeutet "dunkles Grau"?**  
A: Das ist der Grundton des Akkords – der wichtigste Ton, daher visuell hervorgehoben.

**Q: Kann ich eigene Akkorde definieren?**  
A: Aktuell nein, aber geplant für v5.0.

### Normal-Modus

**Q: Bass-Taste zeigt nichts?**  
A: Du bist im Akkordmodus. Wechsel zu "Normal" für Bass-Triaden.

**Q: Wie merke ich mir die Belegung?**  
A: Gar nicht! Nutze die App als visuelles Nachschlagewerk während des Übens.

---

## 🚀 Geplante Features (v5.0)

- [ ] Custom Chords definieren
- [ ] Akkordfolgen speichern & abspielen
- [ ] PDF-Export (Grifftabellen)
- [ ] Multi-Akkord-Vergleich (3+ gleichzeitig)
- [ ] Playback-Modus (gespeicherte Stücke)
- [ ] Cloud-Sync (Einstellungen synchronisieren)
- [ ] Dark/Light Mode Toggle

---

## 🙏 Credits

**Entwickelt für:** Castagnari Benny C/G (3-reihig, Heim-Belegung)  
**Design-Philosophie:** iOS Human Interface Guidelines  
**Musiktheorie:** Standard westliche Harmonielehre  
**Perlmutt-Optik:** Custom CSS mit iOS-Grautönen

---

## 📄 Lizenz

**Persönliche Nutzung**  
Diese App ist für deinen persönlichen Gebrauch entwickelt worden.

Bei Weiterentwicklung:
- ✅ Forken & anpassen ist erlaubt
- ✅ Mit Quellenangabe teilen
- ✅ Für eigene Projekte nutzen
- ❌ Kommerziell verkaufen ohne Rücksprache

Viel Spaß beim Lernen! 🪗🎵

---

## 📞 Support

Fragen oder Feature-Wünsche?  
→ Siehe [INSTALLATION.md](INSTALLATION.md) für FAQ & Troubleshooting

---

**Made with ❤️ for diatonic accordion players**