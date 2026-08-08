# Keycap Forge

Genereert een platte, vierkante G20-keycap (16,3 × 16,3 × 4,5mm) met een tweekleurige
pixel-icoon-inlay, klaar om te printen — al georiënteerd met de platte kant naar
beneden, dus geen supports nodig.

## Hoe het werkt
1. Upload een afbeelding (bij voorkeur PNG met transparante achtergrond)
2. Pas grootte, detail en kleurmodus aan, bekijk live in 3D
3. Download `keycap-base.stl` en `keycap-icon.stl`
4. Beide bestanden in Bambu Studio slepen, per object het juiste filament toewijzen, slicen

Alles draait client-side in de browser (Three.js) — er wordt niets geüpload naar een server.

---

## Zelf online zetten via GitHub Pages

### Stap 1 — GitHub-account
Heb je die al? Sla over. Zo niet: ga naar **github.com** → **Sign up** → volg de stappen (gratis account is genoeg).

### Stap 2 — Nieuwe repository aanmaken
1. Rechtsboven op GitHub: klik het **+**-icoontje → **New repository**
2. Geef een naam, bijv. `keycap-forge`
3. Zet 'm op **Public** (moet, anders werkt GitHub Pages niet gratis)
4. Laat de rest op standaard staan, klik **Create repository**

### Stap 3 — Bestanden uploaden
1. Op je nieuwe (lege) repository-pagina: klik **uploading an existing file** (of **Add file → Upload files**)
2. Sleep alle 3 bestanden erin: `index.html`, `app.js`, `README.md`
3. Onderaan: klik **Commit changes**

### Stap 4 — GitHub Pages inschakelen
1. Ga naar **Settings** (tab bovenaan je repository)
2. Linkermenu: klik **Pages**
3. Bij **Branch**: kies `main`, map `/ (root)` → klik **Save**
4. Wacht ~1 minuut, ververs de pagina — je ziet een groen vinkje met een link zoals:
   `https://jouwgebruikersnaam.github.io/keycap-forge/`

Klaar — dat is je live, publieke tool. Zet die link gerust in je MakerWorld-post.

### Iets aanpassen later?
Ga naar het bestand in je repository → potlood-icoontje (**Edit**) → wijzig → **Commit changes**.
GitHub Pages update vanzelf binnen een minuut, geen aparte stap nodig.

---

## Technische specs (vast, niet aanpasbaar in de UI)

| Onderdeel | Waarde |
|---|---|
| Footprint | 16,3 × 16,3 mm |
| Totale hoogte | 4,5 mm |
| Profiel | Plat / G20 |
| Dikte pixel/icoon-laag | 0,8 mm |
| Stem | Cherry MX kruis (4,0 × 4,0mm, 1,3mm bladdikte), 3,5mm diep |
| Printoriëntatie | Platte vlak op Z=0 (bed), stem-uitsparing opent naar boven — geen supports |
