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

## Layout Kallaway — banda cu Ionuț (regulă fixă)

- Studioul lui NU e pe toată lățimea: e un **card cu colțuri rotunjite**, cu spațiu stânga/dreapta
  (și puțin jos), prin care se vede lumea de deasupra. Capul (și mâinile) lui ies din card (decupat
  din filmarea 4K), restul studioului rămâne în card. Tehnica standard din social media.

## Ritm și lizibilitate (conținut educațional)

- Mișcare continuă, DAR nu în viteză mare: privitorul trebuie să aibă timp să vadă și să înțeleagă
  ce e pe ecran. Mai puține whip-uri, mai multe momente ținute (hold) după fiecare reveal.
- Tot ce apare e relevant pentru ce spune Ionuț și îl duce pe privitor într-o „lume” care explică ideea.
- Unghiuri de cameră puternice, compoziții estetice.

## Tipografie și culori

- Culori aprobate: **roșu (nuanțele șepcii) + alb cald**. Paletă: ink #0B0807, blood #3B0A08,
  deep #7E120E, red #D9261C, signal #FF3A2A, ember #FF8A6A, blush #F4D9CF.
- Text: tracking strâns, spațiere mică între cuvinte (fără litere „rărite”), kerning corect.
- Animațiile de text în stilul referinței pdoom (github.com/mexicat/pdoom-video): apar pe cuvânt,
  integrate în imagine (pe curbe, tastate, ștampilate, slide din lateral), easing puternic + hold.
- Fontul: Ionuț alege dintr-o planșă de fonturi premium (nu Archivo Expanded).
