# Designkonzept — nilufarlayer.com

Stand: 30.10.2026 · Grundlage: der aktuelle Code (Astro) und die Figma-Datei `miros` (Home V.1).

## 1. Ziel und Positionierung

**Was die Seite verkauft:** verkaufspsychologisch fundierte Landingpages und Werbeanzeigen für hochpreisige B2B-Dienstleistungen.

**Ein Ziel pro Besuch:** ein unverbindliches Erstgespräch buchen. Jeder Abschnitt baut Vertrauen auf oder führt zu diesem CTA.

**Zielgruppe:** Inhaber:innen von B2B-Dienstleistungen, die zu wenige oder zu schwache Anfragen bekommen und genug davon haben, Werbebudget zu verbrennen.

**Tonalität:** direkt, per Du, selbstbewusst, mit einem Augenzwinkern („besser als frische Croissants beim Bäcker“). Fachlich kompetent, aber ohne Fachjargon.

## 2. Gestaltungsprinzipien

1. **Klarer Kontrast.** Fast-Schwarz mit Grünstich (#11190c) als Grundton, ein einziger greller Akzent in Lime (#e6ff02). Der Akzent ist für Handlungen und Highlights reserviert, nicht als Deko.
2. **Ruhige Fläche, große Typo.** Viel Weißraum, große Headlines mit enger Laufweite, kurze Absätze.
3. **Weiche Formen.** Große Radien (16–88 px) und Pill-Buttons nehmen dem dunklen Look die Härte.
4. **Beweis vor Behauptung.** Zahlen, Kundenstimmen, Trustmarkt-Widget und Person (Nilufar) stehen prominent.
5. **Bewegung mit Sinn.** Dezente GSAP-Animationen (Hero, Methode, Button-Glanz) lenken den Blick. Bei `prefers-reduced-motion` ist alles aus.

## 3. Farben

| Rolle | Token | Hex |
|---|---|---|
| Primär / dunkler Hintergrund / Text | `--color-primary` | `#11190c` |
| Akzent (CTA, Highlights) | `--color-accent` | `#e6ff02` |
| Hintergrund hell | `--color-bg-white` | `#ffffff` |
| Gedeckter Hintergrund (Taupe) | `--color-bg-muted` | `#9f998a` |
| Sekundärtext | `--color-text-secondary` | `#a0a0a0` |
| Linien | `--color-border` | `#ededed` |
| Neutral Beige | `--color-neutral-2` | `#cfc9bc` |
| Neutral Oliv-Grau | `--color-neutral-6` | `#70756d` |

**Regeln**
- Lime nie als Textfarbe auf Weiß (zu wenig Kontrast). Lime auf Dunkel oder dunkler Text auf Lime.
- Pro Bildschirmhöhe höchstens ein bis zwei Lime-Elemente, damit der CTA heraussticht.
- Beige/Taupe für warme Flächen bei Foto- und Personenbereichen.

## 4. Typografie

| Einsatz | Schrift | Schnitt |
|---|---|---|
| Headlines | Instrument Sans | 500 / 600, SemiBold Italic für Betonungen |
| Fließtext, UI | Inter | 400 / 500 |

- Größen (px): 60 · 48 · 36 · 30 · 24 · 20 · 16 · 14 · 12
- Headlines mit negativer Laufweite (−1,8 px bei 60 px bis −0,1 px bei kleinen Größen).
- Zeilenhöhe als Verhältnis (z. B. 1.2 für Headlines, ~1.5 für Fließtext).
- Fließtext maximal ca. 65 Zeichen pro Zeile.

## 5. Raster, Abstände, Formen

- **Designbreite:** 1280 px, skaliert fluid bis max. 1440 px.
- **Breakpoints:** Desktop ≥ 992 · Tablet 768–991 · Mobil quer 480–767 · Mobil hoch 320–479.
- **Seitenrand:** 52 px Desktop · 24 px Tablet · 16 px Mobil.
- **Abstände:** 4 · 8 · 16 · 24 · 32 · 40 · 48 · 52 · 64 · 100 px (Abschnittsabstand 100 px).
- **Radien:** 16 (klein) · 24 (Karten) · 32 (große Karten) · 56 (Flächen) · 88 (Pill).
- **Schatten:** ein weicher, mehrschichtiger Karten-Schatten (`--shadow-card`), sonst keine.

## 6. Komponenten

| Komponente | Beschreibung |
|---|---|
| **Button** | Pill-Form, Größen `sm/md/lg`. Primär: Lime auf Dunkel. Optionaler Glanz-Sweep (`sweep`) und Kontakt-Variante (`contact`). |
| **Navbar** | Schlank, Name „Nilufar Layer“ links, CTA rechts. |
| **Karten** | Große Radien, weicher Schatten; für Fotos, Kundenstimmen, Statistiken. |
| **Statistik** | Große Zahl + kurzes Label. |
| **Methoden-Schritt** | „Schritt X“ + Titel + Text + Ergebnis-Label („Dein Fundament“, „Dein Wachstum“). |
| **Kundenstimme** | Foto, Zitat, Name/Firma, Sterne. |
| **FAQ-Akkordeon** | Plus/Minus-Symbol, Trennlinien. |
| **Cookie-Banner** | „Nur notwendige“ und „Alle akzeptieren“ gleich gewichtet (DSGVO). |

## 7. Seitenaufbau (Startseite)

| # | Abschnitt | Aufgabe | Kernaussage |
|---|---|---|---|
| 1 | Hero | Aufmerksamkeit + Versprechen | „Hol dir eine Landingpage, die besser konvertiert als frische Croissants beim Bäcker“ + Trustmarkt-Widget |
| 2 | Daten | Problem benennen | „Wähle den effizientesten Weg zu wachsen“ — steigende Werbekosten, schlechte Leads |
| 3 | Methode | Lösung in 3 Schritten | Zielgruppenanalyse → Verkaufsmaschine → Optimierung & Omnipräsenz |
| 4 | Testimonials | Beweis | „Was meine Kunden sagen“ (Slider) |
| 5 | Über mich | Vertrauen in die Person | 16+ Jahre Erfahrung, 100+ Websites, Millionen € Kundenumsatz |
| 6 | Mehr Kundenstimmen | Weiterer Beweis | Kurzbewertungen |
| 7 | FAQ | Einwände ausräumen | Akkordeon |
| 8 | CTA | Abschluss | „Bereit deine Neukundengewinnung zu maximieren?“ → Termin |
| 9 | Footer | Pflicht + Kontakt | Impressum, Datenschutz, hello@nilufarlayer.com |

**Rhythmus:** dunkle und helle Abschnitte wechseln sich ab, damit die Seite beim Scrollen gegliedert wirkt. Spätestens nach jedem zweiten Abschnitt kommt ein CTA.

## 8. Bildsprache

- Echte Fotos (Person, Kund:innen, Mockups) statt Stockfotos.
- Mockups der gebauten Landingpages in Geräte-/Kartenrahmen mit weichem Schatten.
- Warme, natürliche Töne, passend zu Beige/Taupe.
- Bilder als WebP/AVIF, unterhalb des sichtbaren Bereichs mit Lazy Loading.

## 9. Bewegung

- GSAP für Einblendungen im Hero und den Fortschritt in der Methoden-Sektion.
- Button-Glanz in Lime als Blickfang auf dem Haupt-CTA.
- Kurze Dauer (200–600 ms), sanfte Kurven, kein Scroll-Hijacking.
- `prefers-reduced-motion: reduce` schaltet alle Animationen ab.

## 10. Barrierefreiheit und Qualität

- Kontrast nach WCAG AA (Lime nur auf Dunkel).
- Sichtbarer Fokus-Rahmen auf allen Links und Buttons.
- Klickflächen mindestens 44 × 44 px.
- Eine H1 pro Seite, logische Überschriften-Reihenfolge.
- Ziel-Werte: LCP < 2,5 s, CLS < 0,1.

## 11. Nächste Schritte (Vorschläge)

1. Große Bilder (z. B. `member-image.png` mit 2,1 MB) komprimieren und als WebP ausliefern.
2. Lime-Einsatz pro Abschnitt prüfen und reduzieren, wo er nicht auf eine Handlung zeigt.
3. Unterseiten (Leistungen, Referenzen/Cases) mit denselben Bausteinen anlegen.
4. Einheitliche CTA-Formulierung festlegen (z. B. „Kostenloses Erstgespräch buchen“).
