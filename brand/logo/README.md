# S'Atelier — identitate vizuală

Ghid de brand și fișiere sursă pentru logo-ul firmei **S'Atelier**.

## Concept

Numele „S'Atelier" evocă un atelier artizanal de creație — o casă de meșteșug cu
rădăcini franțuzești. Identitatea propusă se sprijină pe trei piloni:

1. **Eleganță serif** — o literă cu contrast înalt (Didot / Bodoni / Playfair),
   care transmite rafinament și tradiție.
2. **Detaliu artizanal** — un ac cu fir stilizat sub wordmark, metaforă pentru
   meșteșug și atenția la detaliu.
3. **Apostrof ca semnătură** — apostroful tipografic (’) în accent auriu este
   elementul distinctiv: un mic gest care separă „S" de „Atelier" și care poate
   fi folosit izolat ca marker de brand.

## Fișiere

| Fișier                   | Utilizare                                                          |
|--------------------------|--------------------------------------------------------------------|
| `satelier-primary.svg`   | Logo principal orizontal, cu tagline. Website, signalistică, print.|
| `satelier-monogram.svg`  | Monogramă circulară. Favicon, ștampilă, etichetă cusută, sigiliu.  |
| `satelier-minimal.svg`   | Doar wordmark, fără ornamente. Header site, semnătură email.       |
| `satelier-reversed.svg`  | Variantă pe fundal negru. Ambalaje premium, materiale de lux.      |
| `preview.html`           | Pagină de preview cu toate variantele și paleta.                   |

Deschide `preview.html` într-un browser pentru a compara toate variantele.

## Paletă cromatică

| Rol        | Hex       | Utilizare                                          |
|------------|-----------|----------------------------------------------------|
| Ink Black  | `#1A1A1A` | Text principal, contur, fundal versiune dark.      |
| Antique Gold | `#B8860B` | Accente, apostrof, ornamente, linii fine.       |
| Warm Cream | `#F5EFE6` | Text pe fundal închis, materiale tipărite.         |
| Paper      | `#FAF7F2` | Fundal principal site și materiale.                |

Pe fundal închis, aurul se deschide la `#C9A227` pentru contrast optim.

## Tipografie recomandată

- **Wordmark**: Didot, Bodoni 72, Playfair Display sau Cormorant Garamond
  (italic pentru logo, regular pentru titluri).
- **Tagline & UI**: Futura, Avenir Next sau Helvetica Neue Light
  cu letter-spacing generos (0.4–0.6em) pentru aerul editorial.

## Reguli de utilizare

- **Spațiu minim de respirație**: cel puțin înălțimea literei „S" din wordmark
  în jurul logo-ului.
- **Dimensiune minimă**: 120 px lățime pentru varianta primară,
  32 px pentru monogramă (favicon).
- **Nu deforma, nu schimba culorile, nu adăuga efecte** (umbre, gradient,
  contur). Folosește variantele livrate.
- **Pe fundal color**: preferă variantele mono (negru sau cream), nu cea cu
  accent auriu, decât dacă fundalul este neutru.

## Generare bitmap

SVG-urile sunt vectoriale și pot fi convertite la orice rezoluție:

```bash
# PNG @2x pentru print
rsvg-convert -w 2400 satelier-primary.svg -o satelier-primary@2x.png

# Favicon
rsvg-convert -w 64 satelier-monogram.svg -o favicon-64.png
```

## Next steps

- Validarea direcției cu clientul (elegant-artizanal vs. modern-minimal).
- Testare la dimensiuni mici (etichetă 20×20 mm, embossing).
- Livrare finală: set complet PNG / PDF / EPS + manual de brand.
