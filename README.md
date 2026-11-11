# sdh-arukereso-feed

Az Árukereső termékfeedjének tükre a sexdolleurope.com boltból.

- **Feed címe (ezt kapja az Árukereső):** `https://pda77hu.github.io/sdh-arukereso-feed/arukereso.xml`
- **Forrás:** `https://sexdolleurope.com/collections/keszletrol?view=arukereso` (Shopify Liquid sablon, csak a készletes babák).
- **Miért kell:** a Shopify az Árukereső letöltőjét 429-cel (Too Many Requests) tartósan korlátozza, ezért a feed innen, a GitHub Pages-ről érhető el.
- **Frissítés:** a `.github/workflows/update-feed.yml` minden nap 13:15 UTC-kor letölti, ellenőrzi és csak változás esetén menti. Kézzel: Actions → „Árukereső feed frissítése” → Run workflow.
- Ha a letöltés vagy az ellenőrzés hibás, a régi feed marad, és a GitHub e-mailt küld a hibáról.
