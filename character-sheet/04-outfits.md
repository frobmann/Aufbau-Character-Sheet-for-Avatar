# 👕 Outfit-System für Fashion Affiliate Marketing

> Dein Avatar ist ein virtuelles Fashion-Model. Er muss beliebige Kleidungsstücke aus Online-Shops tragen können, um Produkte zu präsentieren und Affiliate-Links zu bewerben.

---

## Konzept: Modulares Kleidungssystem

> Statt fester Outfits brauchst du ein **modulares System** — einzelne Kleidungsstücke, die du frei kombinieren und schnell wechseln kannst.

### Kleidungs-Slots

```
┌─────────────────────────────────────────┐
│              KOPF / ACCESSOIRES         │
│   Hüte · Mützen · Caps · Sonnenbrillen │
├─────────────────────────────────────────┤
│              OBERKÖRPER                 │
│   T-Shirts · Hemden · Hoodies ·         │
│   Pullover · Jacken · Blazer            │
├─────────────────────────────────────────┤
│              LAYER (DARÜBER)            │
│   Mäntel · Lederjacken · Westen ·       │
│   Übergangsjacken · Cardigans           │
├─────────────────────────────────────────┤
│              UNTERKÖRPER                │
│   Jeans · Chinos · Jogginghosen ·       │
│   Shorts · Cargos                       │
├─────────────────────────────────────────┤
│              SCHUHE                     │
│   Sneaker · Boots · Loafer ·            │
│   Sandalen · Laufschuhe                 │
├─────────────────────────────────────────┤
│              ACCESSOIRES                │
│   Uhren · Ketten · Ringe · Taschen ·    │
│   Gürtel · Armbänder                    │
└─────────────────────────────────────────┘
```

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

### Style-Kategorien

| Kategorie | Beschreibung | Typische Pieces | Content-Anlass |
|---|---|---|---|
| **Casual Everyday** | Alltagslook, entspannt | T-Shirt + Jeans + Sneaker | "Was ich heute trage" |
| **Business Casual** | Smart, aber nicht overdressed | Hemd + Chino + Loafer | "Office-Look unter 100€" |
| **Streetwear** | Urban, trendy | Hoodie + Cargos + Jordans | "Streetwear Haul" |
| **Date Night** | Schick, elegant | Blazer + Hemd + dunkle Jeans | "Date-Outfit Ideen" |
| **Sport / Athleisure** | Sportlich, funktional | Jogger + Funktions-Shirt + Runner | "Gym-to-Street Looks" |
| **Saisonal** | Jahreszeit-spezifisch | Mäntel, Boots, Sommer-Pieces | "Herbst-Essentials 2026" |

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
| **Gesicht & Frisur** | Immer gleich — dein Wiedererkennungsmerkmal | Du bist die Marke, nicht die Kleidung |
| **Fantasy-Accessoire** | Dein Signatur-Ring/Armband (siehe 02-visual-design.md) | Macht dich einzigartig unter Fashion-Creators |
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
