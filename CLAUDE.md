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

- Sistemul de culori al brandului (aprobat, pentru toate video-urile):
  - **negru cald** #0B0807 (ink) / #170E0C — fundalul, lumea;
  - **roșu** (șapca): signal #FF3A2A, red #D9261C, deep #7E120E, blood #3B0A08, ember #FF8A6A —
    cuvintele-cheie, linia/scânteia (motivul recurent);
  - **alb cald** #F4D9CF (blush) — textul de citit;
  - **chihlimbar-tungsten #FFB547** (din becul Edison și neonul din studioul lui) — DOAR lumină:
    cuvântul aprins în karaoke, liniuța de sub el, lumina care pulsează în spatele textului, scânteile.
    Niciodată suprafețe mari.
- Fără albastru/mov/neon rece.
- Text: tracking strâns, spațiere mică între cuvinte (fără litere „rărite”), kerning corect.
- Animațiile de text în stilul referinței pdoom (github.com/mexicat/pdoom-video): apar pe cuvânt,
  integrate în imagine (pe curbe, tastate, ștampilate, slide din lateral), easing puternic + hold.
- Tipografia ca la pdoom + Barsol Media: fonturi MIXATE pe cuvânt (majuscule late și grele, condensat
  foarte gros pentru accent, serif italic pentru cuvinte emoționale, mono tastat cu cursor ca „subtitlu de
  mașină”), mărimi diferite pe cuvânt. Karaoke: cuvântul se aprinde când e spus + liniuță care alunecă sub
  el; literele sar în val când se colorează. Text pe traseu (literele rotite după curbă), text pe panouri
  în lume văzute din unghiuri care se schimbă. NU o planșă de un singur font „curat” (arată generic).

## Fluxul de lucru pentru fiecare video (regulă fixă, aprobată de Ionuț)

Inspirat din „The 3 Levels of AI Motion Graphics” (RoboNuggets): storyboard → directing, cu feedback
fixat pe cadru. Nu construi videoul întreg înainte ca Ionuț să aprobe direcția.

1. **Script + timpi.** Transcriere cu timpi pe cuvânt (faster-whisper / `npx hyperframes transcribe`).
2. **Storyboard înainte de animație.** Cadre statice din fiecare scenă, în look-ul FINAL (fonturi,
   culori, post-procesare), randate din aceeași scenă (capturi HyperFrames la secunde exacte), puse în
   ordine pe o pagină privată (Artifact claude.ai), fiecare cu timpul de start și o descriere scurtă a
   ce se întâmplă. Apoi STOP și aștepți comentariile.
   - Pagina permite click pe cadru → comentariu fixat cu scena, secunda și poziția
     (ex. `Shot 07, 5.90s, pin la 52% din lățime, 46% din înălțime: prea mult text`) + buton „Copy all”.
   - La comentarii: aplici FIECARE comentariu și NU schimbi nimic altceva. Arăți un storyboard nou sau,
     la cerere, construiești videoul.
3. **Generări Higgsfield doar după storyboard aprobat** (prompt + cost, apoi OK).
4. **Directing pe videoul real.** Pagină de review: player 1x/2x, timeline, click pe imagine → comentariu
   fixat pe secundă și loc, comentarii pe sunet, tăieturi ajustabile prin tragere, „Copy all”.
   Aplici doar ce e comentat, actualizezi pagina de review.
5. **Randarea finală (1080×1920 MP4) doar când Ionuț spune „gata”.** Nu randa versiuni întregi
   ne-cerute (în cloud o randare durează 18–60 min).
6. **Biblioteca de elemente.** Ce iese bun se salvează pentru reutilizare (cu notă despre cum se
   refolosește): fața care iese prin ecran, curba incandescentă cu scânteia, monedele 3D,
   post-procesarea HDR (bloom/halation/grain/CA + motion blur din sub-cadre), sistemul de culori.

## Unelte

- **HyperFrames** rămâne scheletul: sincronizare voce + filmare, randare MP4, capturi la secunde exacte
  (pentru storyboard), remove-background, transcriere. Look-ul premium vine din motorul WebGL propriu
  (Three.js) rulat în compoziție, nu din blocurile HyperFrames.
- Referințe de stil: github.com/mexicat/pdoom-video (MIT, docs/TREATMENT.md + docs/ENGINE.md) și
  videoul Barsol Media (text pe traseu, fonturi mixate, karaoke).
