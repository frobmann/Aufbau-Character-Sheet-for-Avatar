# 👕 Outfit-System für Fashion Affiliate Marketing

> Dein Avatar ist ein virtuelles Fashion-Model für Frauen 35–45. Sie trägt Mid-Range-Pieces (50–150€) aus Shops wie COS, Massimo Dutti, Arket und & Other Stories und präsentiert sie in Social-Media-Shorts.

---

## Konzept: Modulares Kleidungssystem

> Statt fester Outfits brauchst du ein **modulares System** — einzelne Kleidungsstücke, die du frei kombinieren und schnell wechseln kannst.

### Kleidungs-Slots (Damenmode)

```
┌─────────────────────────────────────────┐
│              KOPF / ACCESSOIRES         │
│   Sonnenbrillen · Haarreifen · Hüte ·   │
│   Tücher · Schals                       │
├─────────────────────────────────────────┤
│              OBERKÖRPER                 │
│   Blusen · Tops · Strickpullover ·      │
│   T-Shirts · Rollkragen · Bodys         │
├─────────────────────────────────────────┤
│              LAYER (DARÜBER)            │
│   Blazer · Trenchcoats · Strickjacken · │
│   Lederjacken · Mäntel · Westen         │
├─────────────────────────────────────────┤
│              UNTERKÖRPER                │
│   Stoffhosen · Jeans · Röcke ·          │
│   Kleider · Culottes · Leggings         │
├─────────────────────────────────────────┤
│              SCHUHE                     │
│   Loafer · Pumps · Flats · Sneaker ·    │
│   Boots · Sandalen · Mules              │
├─────────────────────────────────────────┤
│              ACCESSOIRES                │
│   Handtaschen · Schmuck · Gürtel ·      │
│   Schals · Uhren · Sonnenbrillen        │
└─────────────────────────────────────────┘
```

### Zusätzlich: One-Piece-Slot (Kleider & Jumpsuits)

> Kleider und Jumpsuits ersetzen Oberkörper + Unterkörper gleichzeitig. Sehr beliebt bei der Zielgruppe für unkomplizierte "Ein Teil = fertig"-Looks.

### Workflow: Vom Shop-Produkt zum Avatar-Outfit

```
1. PRODUKT FINDEN
   └── Kleidungsstück im Online-Shop aussuchen
       └── Produktbilder + Farbcodes sichern

2. KLEIDUNG NACHBAUEN
   ├── Option A: Marvelous Designer / CLO 3D (Profi)
   │   └── Schnittmuster erstellen → Stoff simulieren → Export
   ├── Option B: Blender (Kostenlos)
   │   └── Mesh modellieren → Textur malen → Rigging
   └── Option C: VRoid Studio (Einfach)
       └── Vorhandene Templates anpassen → Textur/Farbe ändern

3. ANZIEHEN & RENDERN
   └── Kleidungsstück auf Avatar-Body laden
       └── Posing → Beleuchtung → Screenshot/Video

4. CONTENT ERSTELLEN
   └── Video mit Affiliate-Link produzieren
       └── Upload + Produktlink in Bio/Beschreibung
```

---

## Basis-Avatar: Der "nackte" Body

> Dein Avatar braucht einen sauberen Basis-Körper, auf den alle Kleidung drübergelegt wird.

| Anforderung | Detail |
|---|---|
| **Body-Mesh** | Sauber modelliert, gleichmäßige Topology |
| **UV-Mapping** | Ordentlich, damit Kleidung nicht verzerrt |
| **Rigging** | Standard-Humanoid-Skeleton (Mixamo-kompatibel) |
| **Blendshapes** | Gesicht: 27+ (siehe 03-expressions.md) |
| **Hautfarbe** | Als Material/Textur, leicht anpassbar |
| **Unterwäsche-Layer** | Basis-Layer für "darunter" bei offenen Jacken etc. |

---

## Kleidungsstück-Template

> Für jedes Produkt, das du präsentierst, dokumentiere:

### [Produktname] — [Shop-Name]

| Feld | Wert |
|---|---|
| **Produkt** | _[Name des Kleidungsstücks]_ |
| **Shop** | _[Name des Online-Shops]_ |
| **Affiliate-Link** | _[Link]_ |
| **Preis** | _[€]_ |
| **Kategorie** | _[Oberteil / Hose / Schuhe / Accessoire / Layer]_ |
| **Farbe(n)** | _[Farbbeschreibung + HEX wenn möglich]_ |
| **Material** | _[Baumwolle / Polyester / Leder / Denim / etc.]_ |
| **3D-Datei** | _[Dateipfad in /assets/clothing/]_ |
| **Status** | _[⬜ Geplant / 🔨 In Arbeit / ✅ Fertig]_ |
| **Verwendet in** | _[Links zu Videos, in denen es vorkommt]_ |

---

## Outfit-Kombinationen für Content

> Stelle fertige Outfit-Kombinationen zusammen für wiederkehrende Formate.

### Style-Kategorien (Frauen 35–45)

| Kategorie | Beschreibung | Typische Pieces | Content-Anlass |
|---|---|---|---|
| **Büro / Smart Casual** | Professionell aber nicht steif | Blazer + Bluse + Stoffhose + Loafer | "Office-Look unter 150€" |
| **Casual Alltag** | Schick-entspannt, Wochenende | Strickpullover + Jeans + Sneaker | "Samstags-Outfit in 2 Minuten" |
| **Abendessen / Date** | Elegant ohne overdressed | Seidenbluse + Hose + Pumps | "Von Büro zu Dinner — 1 Outfit" |
| **Elternabend / Events** | Zusammengestellt, altersgerecht | Midi-Kleid oder Blazer-Kombi | "Event-Looks die immer funktionieren" |
| **Capsule Wardrobe** | Die 10 Basics, die alles können | Trench + Jeans + Weißes Shirt + etc. | "10 Teile, 30 Outfits" |
| **Saisonal** | Jahreszeit-spezifisch | Mäntel, Boots, Leinen, Sommerkleider | "Herbst-Essentials 2026" |
| **Reise / Urlaub** | Vielseitig, knitterfrei | Midi-Rock + Leinenshirt + Sandalen | "Koffer packen: 7 Tage, 5 Pieces" |

### Was die Zielgruppe NICHT will

> Verstehe, was 35-45-Jährige ablehnen — vermeide es im Content:

- ❌ "Anti-Aging"-Framing — niemand will gesagt bekommen, dass sie alt aussieht
- ❌ Zu junge Trends (Crop Tops, Low-Rise) — wirkt aufgesetzt
- ❌ "Mutti-Mode"-Klischees — die Zielgruppe will modern sein
- ❌ Unrealistische Body-Standards — der Avatar hat bewusst natürliche Proportionen
- ❌ Billige Qualität — lieber weniger Pieces, aber überzeugend

---

## Farbkonsistenz bei Produkten

> So stellst du sicher, dass die Kleidungsfarben auf dem Avatar zum echten Produkt passen:

1. **Produktbilder als Referenz** — Nutze die offiziellen Produktfotos als Textur-Grundlage
2. **Farben abgleichen** — Vergleiche HEX-Codes: Online-Shop vs. 3D-Rendering
3. **Beleuchtung standardisieren** — Immer das gleiche 3-Punkt-Licht-Setup für Farbkonsistenz
4. **Disclaimer** — "Farben können am Bildschirm leicht abweichen" (rechtlich wichtig!)

---

## Erkennungsmerkmale (bleiben bei JEDEM Outfit)

> Diese Elemente sind IMMER sichtbar, egal was der Avatar trägt — sie sind deine Marke.

| Element | Beschreibung | Warum? |
|---|---|---|
| **Gesicht & Frisur** | Immer gleich — Wiedererkennungsmerkmal | Sie ist die Marke, nicht die Kleidung |
| **Ear Cuff** | Goldener Signatur-Ear Cuff (siehe 02-visual-design.md) | Macht sie einzigartig unter Fashion-Creators |
| **Augen-Shift** | Bernstein-Glow bei Begeisterung | Subtiles Branding-Element |
| **Haltung & Gestik** | Gleiche selbstbewusst-entspannte Körpersprache | Konsistenz über alle Videos |

---

## Software für Fashion-Kleidungswechsel

### Empfohlen: Schneller Kleidungswechsel

| Software | Eignung | Kosten | Schwierigkeit |
|---|---|---|---|
| **Marvelous Designer** | ⭐⭐⭐⭐⭐ Beste Stoff-Simulation | ~40€/Monat | ⭐⭐⭐ Mittel |
| **CLO 3D** | ⭐⭐⭐⭐⭐ Wie Marvelous, für Fashion | ~50€/Monat | ⭐⭐⭐ Mittel |
| **Blender (Cloth Sim)** | ⭐⭐⭐ Gut, aber aufwendiger | Kostenlos | ⭐⭐⭐⭐ Schwerer |
| **VRoid Studio** | ⭐⭐ Nur vorgefertigte Templates | Kostenlos | ⭐ Einfach |
| **DAZ 3D + Marketplace** | ⭐⭐⭐ Viele fertige Kleidungsstücke | Kostenlos + Marketplace | ⭐⭐ Einfach-Mittel |

### Empfohlene Pipeline für Fashion-Content

```
SCHNELL (Einstieg):
VRoid Studio → Farben/Texturen der Templates anpassen → Screenshot/Video

MITTEL (Besser):
Blender → Kleidung modellieren → Cloth Sim → Rendern

PROFI (Beste Qualität):
Marvelous Designer → Realistisches Kleidungsstück → Blender → Render-Pipeline
```

---

## Ordnerstruktur für Kleidungsstücke

```
assets/
└── clothing/
    ├── tops/           # T-Shirts, Hemden, Hoodies
    ├── bottoms/        # Hosen, Shorts
    ├── layers/         # Jacken, Mäntel
    ├── shoes/          # Schuhe
    ├── accessories/    # Uhren, Ketten, Taschen
    └── outfits/        # Fertige Kombinationen (Szenen-Dateien)
```

---

## Checkliste

- [x] Modulares Kleidungssystem verstanden
- [ ] Basis-Avatar-Body erstellt (ohne Kleidung)
- [ ] Erste Kleidungs-Software gewählt
- [ ] Ordnerstruktur für Clothing-Assets angelegt
- [ ] Erstes Kleidungsstück nachgebaut (Test)
- [ ] Erstes Outfit-Video produziert
- [ ] Affiliate-Link-System eingerichtet
