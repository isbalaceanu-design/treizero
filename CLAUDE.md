# CLAUDE.md — treizero (Ionuț Bălăceanu · 3.0)

Răspunde-i lui Ionuț în română, scurt și direct.

## Modele de generare (regulă fixă, cerută de Ionuț)

- **Imagini:** doar **Seedream 5.0** (`seedream_v5_pro` în Higgsfield), rezoluție **2K**.
- **Video:** doar **MiniMax H3** (`minimax_h3` în Higgsfield), rezoluție **2K**.
- Nu folosi alte modele (GPT Image, Nano Banana, Seedance, Kling etc.) decât dacă Ionuț cere explicit.
- Înainte de orice generare: arată promptul + estimarea de credite și așteaptă OK.
  Repere de cost (oct 2026): Seedream 5.0 Pro 2K ≈ 2,5 credite/imagine; MiniMax H3 2K ≈ 2 credite/secundă
  (6s = 12, 10s = 20).

## Branduri și logo-uri (regulă fixă, cerută de Ionuț)

- De fiecare dată când în voce apare un brand sau un tool (ChatGPT, Higgsfield, Seedance, Midjourney etc.),
  pe ecran apare și **logo-ul lui**, integrat creativ în lumea video-ului (obiect 3D, pe un ecran din lume,
  interfața tool-ului), nu lipit plat peste imagine.
- Logo-uri SVG: pachetul npm `@lobehub/icons-static-svg` (ex. `icons/openai.svg` pentru ChatGPT).

## Stilul reel-urilor (feedback Ionuț pe pilotul v1)

- Nu clipuri AI întregi lipite unul după altul. Lumea e baza: un plan-secvență continuu, camera trece
  dintr-o lume în alta (ecrane-portal), ca în videoclipul muzical de referință.
- Mini-Ionuț decupat se plimbă constant prin lume; din clipurile generate se folosesc doar bucăți.
- Motion graphics curat, stil Apple: tipografie mare, puțină, integrată pe suprafețele din lume.
- Ionuț real rămâne jos (layout Kallaway, capul ieșit peste bandă).
