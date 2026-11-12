# PROJEKTBRIEF „no dank." — Aktivkohle-Geruchsfilter

> Paket für KIMI Code (Kimi CLI) auf der Debian-VM. Stand: 2026-11-12
> Ziel: Website nodank.ch fertigbauen und deployen.

## 1. Das Produkt
- **Eine SKU:** 50 g staubarmes Kokos-Aktivkohle-Granulat im Non-Woven-Säckchen (Spunbond, 60–80 g/m², weiss), Format 10×14 cm, Kordelzug
- **Aussenverpackung:** luftdichter, bedruckter Mylar-Beutel (Zip Bag) 12×18 cm
- **Faustregel:** 50–100 g Kohle pro m³ Raumvolumen → bei grösseren Räumen Multi-Sack-Strategie kommunizieren
- **Wirkprinzip:** Adsorption (Physik), kein „Überdecken" von Gerüchen — Kernargument gegenüber Generika
- Herkunft: Säckchen + Druck aus China (White-Label), Abfüllung manuell in der Schweiz, Granulat 25-kg-Sack z. B. growshop.ch
- Auf der Packung steht: „Erst vor Gebrauch öffnen"

## 2. Die Marke
- **Name:** „no dank." (mit Punkt am Ende — Teil des Logos)
- **Farben:**
  - Rauch `#6B645A`
  - Stein `#948B7E`
  - Lime `#D8FF3E` (nur ca. 5 % Fläche; steht für Gestank und den Punkt im Logo)
  - Papier `#EFEAE0` (Hintergrund)
- **Logo-Prinzip (final, v4 hell):** Säckchen-Icon mit drei Lime-Gestankpunkten; Wortmarke Inter Bold — „no" in Rauch, „dank" in Stein, runder Lime-Punkt auf der Grundlinie; keine Schwadenlinien. Die Punkte = Gestank, der von der Kohle absorbiert wird.
- **Brand-Stimmung:** dezent, trocken, wissenschaftlich statt wellness-mystisch. Kein Grün, kein Hanf-Blatt, kein Rauch.
- Vektordatei: `brand/logo-no-dank.svg` (Rekonstruktion nach Spezifikation — beim finalen Drucklayout v9 orientieren)

## 3. Geschäftsmodell (für Händler-Sektion)
- **Kommissionsverkauf** an CBD-/Grow-Shops und Kioske: Shop trägt kein Risiko, Rückkaufgarantie, Eigentumsvorbehalt beim Inhaber, Monatsabrechnung
- Retail: 5.90 CHF, Shop behält 40–50 %, Netto ca. 2.10 CHF/Stück bei Wareneinsatz ca. 0.35 CHF
- Akquise läuft über Probemuster + persönliches Gespräch, NICHT über Social Media
- Bezahlte Ads für cannabis-nahe Produkte praktisch gesperrt (Meta/TikTok/Google) → Website ist der einzige organische SEO-Anker

## 4. Technische Basis der Website
- **Schon gebaut (Stand 2026-11-10):** statische HTML-Seiten nach CMS-Schablone, DE/EN, JSON-Daten, Decap CMS, Branding-Farben + Logo-Prinzip, inline-SVG-Visualisierungen. Rendering verifiziert.
- **Noch offen:**
  1. Domain `nodank.ch` kaufen (parallel IGE-Markenregister prüfen)
  2. Deployment: GitHub Pages / Netlify / eigener Server — ENTSCHEIDUNG OFFEN
  3. `admin/config.yml`: Repo-Platzhalter durch echtes Repo ersetzen
  4. Kontakt-E-Mail einrichten (z. B. info@nodank.ch)
  5. Analytics einrichten (empfohlen: privacy-freundlich, z. B. Plausible)

## 5. Struktur des Pakets
- `00-PROJEKTBRIEF.md` — dieser Text
- `01-website-anforderungen.md` — was die Seite braucht (Zielgruppen, Pflichtinhalte, Rechtliches)
- `02-produktdaten-und-packung.md` — Packungsangaben D/F/I, Warnhinweise, EAN, QR
- `03-content-de.md` / `04-content-en.md` — fertige Websitetexte
- `05-offene-entscheidungen.md` — Entscheidungen, die der Mensch treffen muss
- `brand/tokens.css` — Design-Tokens
- `brand/logo-no-dank.svg` — Logo (SVG)

## 6. Arbeitsauftrag an KIMI Code
1. Inhalt aus `content/` in die vorhandenen statischen Seiten einbauen (DE/EN komplett, umschaltbar)
2. Pflichtinhalte aus `01-website-anforderungen.md` abhaken — nichts weglassen
3. Impressum mit Adresse des Inverkehrbringers einbauen (Platzhalter markieren, bis echte Adresse vorliegt)
4. Mobile-first prüfen (Einstieg fast nur über QR-Scan)
5. Meta-Tags / Open-Graph / Social Previews setzen (SEO-Anker, da Ads gesperrt)
6. Deployment nach Entscheid in `05-offene-entscheidungen.md`
