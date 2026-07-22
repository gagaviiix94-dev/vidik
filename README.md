# VIDIK — Luksuzne vikendice Fruška gora

Statički sajt (HTML). Sve stranice se otvaraju direktno u pregledaču, bez build koraka.

## Pokretanje lokalno
Zbog učitavanja `.js` fajlova preko `fetch`, otvorite preko lokalnog servera (ne dvoklikom):

```bash
python3 -m http.server 8000
# pa otvorite http://localhost:8000/
```

## Hosting na GitHub Pages
1. Napravite repo i push-ujte sve fajlove iz ovog foldera u koren (`main` grana).
2. Settings → Pages → Source: `Deploy from a branch`, grana `main`, folder `/root`.
3. Sajt će biti dostupan na `https://<korisnik>.github.io/<repo>/` — `index.html` automatski preusmerava na početnu.

## Struktura
- `index.html` — ulazna tačka (preusmerava na početnu)
- `Vikendica Vidik.dc.html` — Početna
- `Galerija.dc.html` — Galerija
- `Meni.dc.html` — Meni / ketering
- `Rezervacija.dc.html` — Rezervacija i konsultacije
- `Okolina.dc.html` — Lokacija i okolina
- `Utisci.dc.html` — Utisci gostiju
- `Mobilni pregled.html` — Pregled svih strana u telefonskim okvirima (390px)
- `support.js`, `image-slot.js`, `doc-page.js` — runtime i komponente
- `uploads/` — slike i fontovi

## Napomena
Sajt je responzivan; mobilni layout se aktivira na širinama ≤880px.
