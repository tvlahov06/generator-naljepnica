# Generator Naljepnica

Web aplikacija za generiranje i ispis naljepnica s barcodom na A4 papir (format F-21, 52.5×29.7mm, 40 kom/list).

## Funkcionalnosti

- Ručni unos artikala (naziv + barcode)
- Uvoz iz Excel datoteke (.xlsx / .xls)
- Automatsko generiranje CODE128 barcoda
- Ispis na A4 papir (format F-21, 4×10 naljepnica)
- Više listova ako ima više od 40 naljepnica
- PWA — može se instalirati na mobitel/desktop
- Radi offline

## Korištenje

1. Otvori aplikaciju
2. Dodaj artikle ručno ili uvezi Excel
3. Klikni **Ispis / PDF**
4. U postavkama ispisa postavi margine na **Nema**

## Instalacija (GitHub Pages)

1. Napravi novi repozitorij na GitHubu
2. Uploadaj sve datoteke
3. Idi na **Settings → Pages → Source: main / root**
4. Aplikacija je dostupna na `https://tvoj-username.github.io/naziv-repozitorija`

## Struktura

```
index.html          — glavna aplikacija
manifest.json       — PWA manifest
sw.js               — service worker (offline podrška)
favicon.ico         — favicon
icons/
  icon-192.png      — PWA ikona
  icon-512.png      — PWA ikona
  apple-touch-icon.png
```

## Tehnologije

- Vanilla JavaScript (bez frameworka)
- SheetJS (Excel parsing)
- Inline CODE128 generator (bez CDN ovisnosti)
