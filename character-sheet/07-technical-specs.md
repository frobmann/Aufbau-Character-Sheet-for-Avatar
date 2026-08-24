# ⚙️ Technische Spezifikationen

> 3D-Modell-Details, Rigging, Animation und technische Anforderungen.

---

## 3D-Modell-Spezifikationen

| Spezifikation | Wert | Notizen |
|---|---|---|
| **Polygon-Budget** | _[z.B. 20.000-50.000 Tris]_ | Für Echtzeit-Rendering |
| **Modellierungs-Software** | _[VRoid Studio / Blender / ZBrush / Maya]_ | |
| **Export-Format** | VRM / FBX / GLB | VRM für VTuber-Apps |
| **Textur-Auflösung** | _[2K / 4K]_ | |
| **Textur-Typ** | PBR (Albedo, Normal, Roughness) | |
| **Shader-Stil** | _[Toon / PBR / NPR / Custom]_ | |

## Empfohlene Software-Pipeline

### Modellierung & Texturierung

| Software | Zweck | Kosten | Schwierigkeit |
|---|---|---|---|
| **VRoid Studio** | Charakter-Erstellung (Anime-Stil) | Kostenlos | ⭐ Einfach |
| **Blender** | 3D-Modellierung (jeder Stil) | Kostenlos | ⭐⭐⭐ Mittel-Schwer |
| **ZBrush** | High-Detail Sculpting | ~40€/Monat | ⭐⭐⭐⭐ Schwer |
| **Substance Painter** | Texturierung | ~22€/Monat | ⭐⭐⭐ Mittel |

### Rigging & Animation

| Software | Zweck | Kosten |
|---|---|---|
| **Mixamo** | Auto-Rigging & Animationsbibliothek | Kostenlos |
| **Blender** (Rigging) | Manuelles Rigging & Animation | Kostenlos |
| **Cascadeur** | Physik-basierte Animation | Kostenlos (Indie) |

### Face Tracking & Motion Capture

| Software | Zweck | Kosten | Plattform |
|---|---|---|---|
| **VSeeFace** | Face-Tracking + 3D-Avatar-Display | Kostenlos | Windows |
| **VMagicMirror** | VRM-Avatar Face/Hand Tracking | Kostenlos | Windows |
| **iFacialMocap** | Professionelles Face-Tracking | ~7€ | iOS (iPhone X+) |
| **Luppet** | Oberkörper + Face Tracking | ~25€ | Windows |
| **MediaPipe** | Open-Source Face/Body Tracking | Kostenlos | Alle |

### Video-Produktion

| Software | Zweck | Kosten |
|---|---|---|
| **OBS Studio** | Screen Recording + Avatar-Overlay | Kostenlos |
| **DaVinci Resolve** | Video-Schnitt (Profi-Level) | Kostenlos |
| **CapCut** | Schneller Schnitt für Shorts | Kostenlos |
| **After Effects** | Motion Graphics & VFX | ~24€/Monat |
| **Premiere Pro** | Profi-Video-Schnitt | ~24€/Monat |

## Rigging-Anforderungen

### Gesichts-Blendshapes (Minimum)

| Kategorie | Blendshapes | Anzahl |
|---|---|---|
| **Augen** | Blink_L, Blink_R, Wide_L, Wide_R, Squint_L, Squint_R | 6 |
| **Augenbrauen** | BrowUp_L, BrowUp_R, BrowDown_L, BrowDown_R, BrowInner | 5 |
| **Mund** | MouthOpen, MouthSmile, MouthFrown, MouthPucker, Jaw | 5 |
| **Viseme** | A, E, I, O, U, M/B/P, F/V, L/T/D | 8 |
| **Extras** | Tongue, CheekPuff, NoseSneer | 3 |
| | **Gesamt Minimum** | **27** |

### Körper-Rigging

| Knochen-Bereich | Knochen | Notizen |
|---|---|---|
| **Kopf/Nacken** | Head, Neck | Kopfbewegungen |
| **Wirbelsäule** | Spine, Spine1, Spine2, Chest | Oberkörper-Bewegung |
| **Arme** | Shoulder, UpperArm, LowerArm, Hand (×2) | Gestik |
| **Finger** | 3 Knochen × 5 Finger (×2) | Für Peace-Zeichen etc. |
| **Beine** | UpperLeg, LowerLeg, Foot, Toe (×2) | Falls ganzer Körper sichtbar |
| **Haare** | Dynamic Bones / Spring Bones | Natürliche Bewegung |
| **Accessoires** | Je nach Design | Kopfhörer, Ketten etc. |

## Rendering-Setup

| Parameter | Empfehlung |
|---|---|
| **Auflösung** | 1080×1920 (9:16 vertikal für Shorts) |
| **FPS** | 30 fps (Standard) / 60 fps (Smooth) |
| **Beleuchtung** | 3-Punkt-Setup (Key, Fill, Rim) |
| **Hintergrund** | Greenscreen → austauschbar / oder 3D-Szene |

## Performance-Anforderungen

| Komponente | Minimum | Empfohlen |
|---|---|---|
| **GPU** | GTX 1060 / RX 580 | RTX 3060+ / RX 6700+ |
| **CPU** | i5 / Ryzen 5 | i7 / Ryzen 7 |
| **RAM** | 8 GB | 16 GB+ |
| **Speicher** | 50 GB frei | SSD 100 GB+ |
| **Webcam** | 720p | 1080p+ / iPhone (iFacialMocap) |

---

## Checkliste

- [ ] Modellierungs-Software gewählt
- [ ] Polygon-Budget festgelegt
- [ ] Face-Tracking-Lösung ausgewählt
- [ ] Video-Software installiert
- [ ] Rendering-Setup konfiguriert
- [ ] Hardware-Anforderungen geprüft
