# NÉRA — Website

Statični prezentacioni sajt za fiktivni skincare brend NÉRA.

## Hostovanje na GitHub Pages

1. Napravi novi GitHub repozitorijum i otpremi sav sadržaj foldera `dist/` u koren repozitorijuma.
2. U repozitorijumu idi na **Settings → Pages**.
3. Pod **Build and deployment → Source** izaberi **Deploy from a branch**.
4. Izaberi granu (npr. `main`) i folder `/ (root)`, pa **Save**.
5. Sajt će za par minuta biti dostupan na `https://<korisnik>.github.io/<repo>/`.

Ulazna stranica je `index.html` (identična početnoj). Sve stranice su povezane i rade preko relativnih linkova.

## Struktura

- `index.html` / `index.dc.html` — Početna
- `proizvodi.dc.html` — Proizvodi
- `proizvod.dc.html` — Pojedinačni proizvod (`?p=renewal-serum`, `?p=barrier-creme`, `?p=gentle-cleanser`, `?p=night-concentrate`)
- `sastojci.dc.html` — Sastojci
- `ritual.dc.html` — Ritual nege
- `o-nama.dc.html` — O nama
- `journal.dc.html` — Journal
- `clanak.dc.html` — Članak (`?a=kozna-barijera`, `?a=deset-proizvoda`, `?a=niacinamid`, `?a=jednostavnija-rutina`)
- `kontakt.dc.html` — Kontakt (demo forma)
- `uslovi.dc.html`, `privatnost.dc.html` — Pravno
- `Nav`, `Footer`, `Img` — deljene komponente
- `support.js` — runtime
- `assets/` — fotografije

Napomena: sajt se mora otvarati preko HTTP servera (GitHub Pages to obezbeđuje). Lokalno otvaranje duplim klikom (file://) neće učitati stranice — koristi npr. `python3 -m http.server` u `dist/` folderu.
