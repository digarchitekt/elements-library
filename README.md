# Elements Library

Kolekcja interaktywnych komponentów UI w estetyce **black metallic glass** — liquid glass, chromowe shadery WebGL, magnetyczne przyciski, particle fields i inne wzorce reagujące na ruch kursora.

**Zero zależności.** Czysty HTML + CSS + vanilla JS (+ WebGL tam, gdzie jest chrom). Każdy plik działa samodzielnie — wystarczy otworzyć w przeglądarce.

## Podgląd

Otwórz `index.html` — to galeria linkująca do wszystkich zestawów.

Jeśli repo jest publiczne, całość można wystawić za darmo przez **GitHub Pages**:
Settings → Pages → Deploy from branch → `main` / root.

## Zawartość

| Plik | Opis |
|---|---|
| `components/liquid-glass-button.html` | Przycisk „Ask agents": dymione szkło, płynący chromatyczny stroke, chromowy dysk z shaderem liquid metal (WebGL), tilt 3D |
| `components/motion-lab-01.html` | 6 komponentów: magnetic button, liquid orb, tilt card, glass toggle, dispersion slider, magnify dock |
| `components/motion-lab-02.html` | 6 świeżych wzorców: spotlight card, elastic tabs, particle field, rotary knob, gooey FAB, kinetic text |
| `components/preiscale-components.html` | Zestaw brandowy pod landing: CTA, proces, chaos→przepływ, kalkulator czasu, karty pilotaży, mini-dashboard |
| `components/luxury-noir-kit.html` | Pełny UI kit „luxury noir": CTA idle→loading→success, segmented control, switch, pole premium z optyczną ramką, toast, stat + sparkline, klikalny proces, karty usług, accordion, paginacja, magnetyczny action dock |

## Jak używać komponentu we własnym projekcie

1. Otwórz plik zestawu i znajdź sekcję komponentu — każda jest oznaczona komentarzem, np. `/* ===== 09 DOT FIELD ===== */` w CSS i JS oraz komentarzem `<!-- 09 ... -->` w HTML.
2. Skopiuj trzy fragmenty: markup, style i skrypt tego komponentu.
3. Kolory brandowe są zdefiniowane jako zmienne CSS w `:root` (`--acc1`, `--acc2`, `--warm`) — podmień je pod swój projekt.

## Uwagi techniczne

- Najlepiej wygląda w Chrome/Edge (pełne wsparcie `backdrop-filter`, `@property`, `conic-gradient` z animowanym kątem).
- Komponenty chromowe używają WebGL 1 — bez indeksowania uniformów zmiennym indeksem, z pętlą `requestAnimationFrame` i pierwszą klatką rysowaną na mount.
- Wszystkie animacje respektują `prefers-reduced-motion`.

## Licencja

MIT — używaj, modyfikuj, wrzucaj do projektów komercyjnych. Gwiazdka mile widziana ⭐
