# 🐾 VetDose

A veterinary drug dosage calculator for dogs and cats, tailored to the **Egyptian pharmaceutical market**.

Built as a single-file Progressive Web App (PWA) — no server, no install, works fully offline.

---

## Features

- **Dosage calculator** — weight-based mg/kg calculations with syringe guide and tablet count
- **Egyptian drug library** — 55 pre-loaded medications with local brand names (Baytril, Novalgin, Synulox, etc.)
- **Patient tracking** — free-text patient IDs with autocomplete from history
- **History** — searchable by patient name and date range, grouped per patient
- **Drug interaction warnings** — session-based drug-drug interaction checking
- **Max dose alerts** — per-route safe dose limits with red warning on exceed
- **Doctor profile** — name shown in header and embedded in shared files
- **VDP sharing** — export/import `.vdp` medication packages (medications only, no patient history)
- **IndexedDB storage** — reliable persistent storage, not cleared by browser pressure
- **Offline-ready PWA** — add to home screen on iOS/Android for native app experience

---

## Drug Library Categories

| Category | Drugs |
|---|---|
| 💊 Antibiotics | Amoxicillin, Synulox, Baytril, Marbocyl, Vibramycin, Flagyl, Dalacin, Stomorgyl, Bactrim, Tylan, Cefalin |
| 🩹 NSAIDs & Analgesics | Metacam, Novalgin, Rimadyl, Ketofen, Tramal, Torbugesic, Temgesic |
| 💉 Anaesthesia & Sedation | Ketalar, Rompun, Domitor, Diprivan, Valium, Dormicum, Atropine, Atravet, Antisedan |
| ❤️ Cardiac & Diuretics | Lasix, Enacard, Tenormin, Aldactone, Lanoxin |
| 🫃 GI & Gastric | Primperan, Cerenia, Losec, Pepcid, Ulcogant, Duphalac |
| 💊 Steroids | Dexasone, Predsol, Solu-Medrol |
| 🦠 Antiparasitics | Ivomec, Panacur, Droncit, Milbemax, Stronghold |
| 🧴 Dermatology | Zyrtec, Piriton, Atarax |
| 🚨 Emergency | Adrenaline, Calcium Gluconate, Glucose 50%, Xylocaine, NaHCO3, Solu-Cortef |

---

## Installation (PWA)

### iOS
1. Open `index.html` in **Safari**
2. Tap the **Share** button → **Add to Home Screen**
3. App launches in full-screen standalone mode

### Android
1. Open in **Chrome**
2. Tap the menu → **Add to Home Screen** or **Install App**

### GitHub Pages
1. Push this repo to GitHub
2. Go to **Settings → Pages → Source: main / root**
3. App is live at `https://yourusername.github.io/vetdose/`

---

## File Structure

```
vetdose/
├── index.html          # Full app (single file)
├── manifest.json       # PWA manifest
├── service-worker.js   # Offline caching
├── apple-touch-icon.png
├── icon-152.png
├── icon-167.png
├── icon-192.png
└── icon-512.png
```

---

## Data & Privacy

- All data stored **locally on device** using IndexedDB (primary) + localStorage (mirror)
- No server, no analytics, no external requests except Google Fonts
- `.vdp` exports contain **medications only** — patient history is never shared
- Patient records can be deleted individually or bulk-pruned (inactive > 1 year)

---

## Disclaimer

VetDose is a **clinical aid tool** only. Always verify dosages against current references and use professional judgment. The authors accept no liability for clinical decisions made using this tool.

---

## Version

**v4.0** — May 2026
