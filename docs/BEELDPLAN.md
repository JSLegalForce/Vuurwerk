# Beeldplan e-learning Vuurwerk

Versie 0.9.1 · juridische peildatum 20 september 2026 · bijgewerkt 22 september 2026. Hoort bij `OPLEVERING.md`.

> **Stijlwijziging (opdracht 22-9-2026).** Voor Vuurwerk geldt vanaf nu een **moderne, professionele cartoon-/illustratiestijl** (semi-realistisch, volwassen), niet meer realistische fotografie. Het vorige beeldplan (foto-prompts N1–N22) is hiermee vervangen. De voorbeeldsheets van Jan (22-9-2026) zijn visuele referentie; ze worden niet letterlijk gekopieerd.

> **Status.** In deze werkomgeving is **geen beeldgenerator** beschikbaar. Er zijn in deze ronde dus **geen** nieuwe afbeeldingen gemaakt of geplaatst. Alle bestaande beelden blijven staan tot het vervangende beeld er is (opdracht: geen slechte vervanging maken). Dit document bevat per scherm het besluit en per nieuw beeld een complete prompt, zodat Jan de beelden één voor één kan laten genereren.

## 1. Vaste beeldstijl

- Moderne professionele cartoon-/illustratiestijl, semi-realistisch, duidelijke vormen, nette contouren, zachte schaduwen; volwassen uitstraling.
- Niet: kinderboekstijl, overdreven stripgezichten, 3D-plastic, fotorealisme, Amerikaanse politie-uitstraling.
- Kleuren JS Legal Force: donkerblauw, midden-/lichtblauw, wit, zilvergrijs; oranje als accent. Vuurwerkverpakkingen en categoriekaarten mogen eigen kleuren hebben (F1 groen, F2 geel, F3 oranje, F4 rood).
- Eén hoofdbeeld per pagina; meerdere beelden alleen bij vergelijken (F1–F4, verpakt tegenover los).
- Belangrijke personen en objecten in het midden (60 %) van de compositie, zodat een uitsnede op de telefoon werkt.
- Zo weinig mogelijk tekst in beeld. Toegestaan, als het betrouwbaar lukt: `F1` `F2` `F3` `F4` `HANDHAVING` `POLITIE` `PROCES-VERBAAL` `CE` `NEM 250 g` `Geschikt voor particulier gebruik` `GEVAAR – NIET BETREDEN`. Alle andere tekst komt via HTML.
- Veiligheid: nooit een handhaver die onbekend of zwaar vuurwerk vastpakt, opent of uit elkaar haalt; afstand houden; geen onveilige opslag.
- Toetsbeelden verraden het antwoord niet (geen vinkje, geen tekst met het antwoord).

### Handhavingskleding (harde regel)

- Donkerblauw Nederlands handhavingsuniform. Op de rug: **HANDHAVING**. Niet standaard groot “BOA”.
- Op de **arm**: het schildvormige BOA-embleem (donker/zwart schild, lichte rand, wit BOA-symbool). Niet op dozen, laptops, dossiers, bekers, auto’s, muren of verpakkingen.
- Nooit “POLITIE” op handhavingskleding; geen politie-embleem, geen gemeentewapen, geen verzonnen schild, geen Amerikaanse badge.
- Politie alleen waar dat inhoudelijk nodig is, en dan duidelijk anders gekleed (Nederlands politie-uniform met POLITIE).

### Techniek

- Formaat: lesbeelden 4:3 (1600 × 1200) of 3:2 (1800 × 1200); productillustraties 3:4 (900 × 1200); afsluiting 16:9 (1920 × 1080).
- Export: WebP, kwaliteit ca. 80, zonder zichtbaar kwaliteitsverlies; doel < 250 kB per lesbeeld, < 120 kB per productillustratie.
- Bestandsnamen: kleine letters, underscores, geen spaties (zie tabel). Map: `assets/images/`.
- Plaatsen: lever het bestand aan; het wordt gekoppeld in `assets/app.js` (`ART_FILE` + de pagina-instelling in `L_SPEC`, of de `src` in de categoriepagina’s). Controleer daarna desktop en telefoon.

### Basisprompt (plak voor elke scène)

```
Modern professional editorial cartoon illustration, semi-realistic proportions, clean confident line work, soft cel shading, calm adult tone, Dutch setting, colour palette dominated by dark navy blue, mid/light blue, white and silver grey with orange as accent colour, uncluttered background, main subjects in the central 60% of the frame so the image can be cropped for mobile. Dutch municipal enforcement officers (boa's) wear a dark navy Dutch enforcement uniform (jacket and trousers, subtle light-blue/white checkered band), the word HANDHAVING in white capital letters on the back; on the upper LEFT SLEEVE the official Dutch BOA emblem: a black shield with a light border and the white BOA symbol; no other badges, no police badge, no municipal coat of arms, no weapons drawn.
```

### Negatieve prompt (altijd meegeven)

```
NOT: the word POLITIE or POLICE on enforcement clothing, American police uniforms, sheriff stars, fantasy badges, the BOA emblem on objects (boxes, laptops, cups, walls, cars, documents), children's-book style, exaggerated cartoon faces, 3D/plastic render, photorealism, gore, explosions near people, anyone holding, opening or dismantling unknown or heavy fireworks, readable brand names, gibberish text, extra fingers, distorted hands
```

## 2. Personages

Regel: **dezelfde casus = dezelfde personen**; **nieuwe casus = andere personen**. Burgers variëren in leeftijd, uiterlijk, kleding en huidskleur; geen stereotype “verdachte” — gedrag en situatie vertellen wat er gebeurt.

| Code | Naam (intern) | Beschrijving | Casussen |
|---|---|---|---|
| H1 | Noor | vrouw, ca. 30 jaar, donker haar in een lage knot, lichtgetinte huid | plein (N01/N02), park (N23), overdracht (N17) |
| H2 | Daan | man, ca. 35 jaar, kort donker haar, lichte huid, gladgeschoren | plein (N01/N02), kofferbak F4 (N11), station (N24), briefing (N21) |
| H3 | Ingrid | vrouw, ca. 40 jaar, blond halflang haar in paardenstaart, lichte huid | etiket (N03), staande houden (N12), inbeslagneming (N15), afzetten (N19), woonstraat (N22) |
| H4 | Tim | man, ca. 28 jaar, lichtbruin kort haar, lichte huid, kort baardje | onbekend vuurwerk (N06), ontheffing (N08), staande houden (N12), tas zonder etiket (N18), parkeerplaats (N25) |
| H5 | Esther | vrouw, ca. 35 jaar, donkere huid, kort zwart krullend haar | zien en bevoegd (N10), aanhouden (N13), tas zonder etiket (N18), briefing (N21), parkeerplaats (N25) |
| H6 | Karim | man, ca. 45 jaar, kaal/zeer kort haar, getinte huid, grijzende baard | kofferbak F4 (N11), aanhouden (N13), proces-verbaal (N16), briefing (N21), station (N24) |

Let op: N14 (auto/kofferbak) is een eigen casus. Gebruik daar **H4 en H5** als N01 al met H1/H2 is gemaakt.

## 3. Besluit per scherm

Besluiten: **BEHOUDEN** (goed of functioneel, bijvoorbeeld HTML-infographic), **VERVANGEN** (bestaand beeld wordt later vervangen), **NIEUW** (nu een generiek pictogram of niets; nieuw situatiebeeld gewenst), **GEEN BEELD NODIG** (pictogram mag blijven, geen investering nodig). Status “door Jan te genereren” betekent: in deze ronde niet gemaakt.

### 3a. Inhoudspagina’s

| Onderwerp | Pagina | Titel | Huidig beeld | Besluit | Nieuw beeld | Status |
|---|---|---|---|---|---|---|
| 1 | 1 | Leerdoelen | boa-illustratie (master) | VERVANGEN | N02 `onderwerp1_gesprek_jongeren.webp` | door Jan te genereren |
| 1 | 2 | Een harde knal op het plein | foto (plein-knal) | VERVANGEN | N01 `onderwerp1_plein_knal.webp` — huidige foto (realistisch, geel hesje) blijft tot N01 er is | door Jan te genereren |
| 1 | 3 | Een harde knal op het plein — wat gaat er door je heen? | boa-illustratie (master) | VERVANGEN | N01 `onderwerp1_plein_knal.webp` — zelfde casus | door Jan te genereren |
| 1 | 4 | Waarom vuurwerk bij jouw werk hoort | foto (boa-jongeren-plein) | VERVANGEN | N02 `onderwerp1_gesprek_jongeren.webp` — huidige foto blijft tot N02 er is | door Jan te genereren |
| 1 | 5 | Categorie is nog geen conclusie | vijf ronde uitsneden (concl-*.webp) | VERVANGEN | N-F1 `onderwerp2_categorie_f1.webp`, N-F2 `onderwerp2_categorie_f2.webp`, N-F3 `onderwerp2_categorie_f3.webp`, N-F4 `onderwerp2_categorie_f4.webp`, N03 `onderwerp2_etiket_verpakking.webp` — ronde beelden F2 (knalstaven) en F4 (vuurpijlen) suggereren een categorie die het beeld niet bewijst | door Jan te genereren |
| 1 | 6 | De vier vragen | HTML-infographic | BEHOUDEN | — — HTML-infographic van de vier vragen; tekst exact en toegankelijk | blijft |
| 1 | 7 | Vijf soorten vragen, niet door elkaar | pictogram weegschaal | GEEN BEELD NODIG | — — pictogram weegschaal mag blijven | n.v.t. |
| 1 | 8 | Opzet van de cursus | HTML-infographic | BEHOUDEN | — — HTML-routeplaat | blijft |
| 1 | 9 | Kort samengevat | boa-illustratie (master) | GEEN BEELD NODIG | — | n.v.t. |
| 2 | 1 | Leerdoelen | boa-illustratie (master) | VERVANGEN | N-F2 `onderwerp2_categorie_f2.webp` | door Jan te genereren |
| 2 | 2 | Waarom categorieën? | pictogram lagen | VERVANGEN | N-F1 `onderwerp2_categorie_f1.webp`, N-F2 `onderwerp2_categorie_f2.webp`, N-F3 `onderwerp2_categorie_f3.webp`, N-F4 `onderwerp2_categorie_f4.webp` — categorieserie | door Jan te genereren |
| 2 | 3 | Wettekst: indeling in categorieën | vier uitsneden (wet-*.webp) + wetboek | VERVANGEN | N-F1 `onderwerp2_categorie_f1.webp`, N-F2 `onderwerp2_categorie_f2.webp`, N-F3 `onderwerp2_categorie_f3.webp`, N-F4 `onderwerp2_categorie_f4.webp` — wet-f2 toont losse knalstaven als F2-voorbeeld: kan misleiden | door Jan te genereren |
| 2 | 4 | F1 – Zeer licht vuurwerk | foto-uitsneden 200 × 300 (voorbeelddia) | VERVANGEN | P-F1a `onderwerp2_product_f1_sterretjes.webp`, P-F1b `onderwerp2_product_f1_knalerwten.webp`, P-F1c `onderwerp2_product_f1_fonteintje.webp` — huidige uitsneden 200 × 300 px (te laag voor HiDPI) | door Jan te genereren |
| 2 | 5 | F2 – Vuurwerk met weinig gevaar | foto-uitsneden 200 × 300 (voorbeelddia) | VERVANGEN | P-F2a `onderwerp2_product_f2_fontein.webp`, P-F2b `onderwerp2_product_f2_cake.webp`, P-F2c `onderwerp2_product_f2_compound.webp` — huidige uitsneden bevatten onzintekst (“66 SHOTE”) | door Jan te genereren |
| 2 | 6 | F3 – Vuurwerk met middelmatig gevaar | foto-uitsneden 200 × 300 (voorbeelddia) | VERVANGEN | P-F3a `onderwerp2_product_f3_cake.webp`, P-F3b `onderwerp2_product_f3_vuurpijlen.webp`, P-F3c `onderwerp2_product_f3_batterij.webp` | door Jan te genereren |
| 2 | 7 | F4 en ander zwaar/illegaal vuurwerk | foto-uitsneden 200 × 300 (voorbeelddia) | VERVANGEN | P-Z1 `onderwerp2_zwaar_cobra.webp`, P-Z2 `onderwerp2_zwaar_nitraat.webp`, P-Z3 `onderwerp2_zwaar_mortier.webp` — huidige uitsnede toont echte productnaam | door Jan te genereren |
| 2 | 8 | De categorieën op een rij | geen | GEEN BEELD NODIG | — — overzichtspagina; kaarten in HTML | n.v.t. |
| 2 | 9 | Personen met gespecialiseerde kennis | wetboek-illustratie | NIEUW | N04 `onderwerp2_personen_gespecialiseerde_kennis.webp` | door Jan te genereren |
| 2 | 10 | Verpakking en etiket | wetboek-illustratie | NIEUW | N03 `onderwerp2_etiket_verpakking.webp` | door Jan te genereren |
| 2 | 11 | Zelfde tas, andere informatie | HTML-infographic | VERVANGEN | N05 `onderwerp2_tas_verpakt_los.webp` — HTML-vergelijking blijft; beeld ondersteunt | door Jan te genereren |
| 2 | 12 | Onbekend vuurwerk | pictogram vraag | VERVANGEN | N06 `onderwerp2_onbekend_vuurwerk.webp` | door Jan te genereren |
| 2 | 13 | Van waarneming naar juridische conclusie | HTML-infographic | BEHOUDEN | — — HTML-lagenplaat | blijft |
| 2 | 14 | Op straat weet je het niet altijd | boa-illustratie (master) | VERVANGEN | N06 `onderwerp2_onbekend_vuurwerk.webp` | door Jan te genereren |
| 2 | 15 | Terug naar het plein: de tas | pictogram tas | VERVANGEN | N05 `onderwerp2_tas_verpakt_los.webp` — zelfde casus plein | door Jan te genereren |
| 2 | 16 | Wat kun je wel en nog niet vaststellen? | HTML-infographic | BEHOUDEN | — — HTML-checklist | blijft |
| 2 | 17 | Van product naar juridische conclusie | HTML-infographic | BEHOUDEN | — — HTML-ketenplaat | blijft |
| 2 | 18 | Kort samengevat | pictogram document | GEEN BEELD NODIG | — | n.v.t. |
| 2 | 19 | Kort samengevat | boa-illustratie (master) | GEEN BEELD NODIG | — | n.v.t. |
| 2 | 20 | Vooruitblik: Wat zegt de wet? | pictogram | GEEN BEELD NODIG | — | n.v.t. |
| 3 | 1 | Leerdoelen | boa-illustratie (master) | VERVANGEN | N07 `onderwerp3_wet_regelgeving.webp` | door Jan te genereren |
| 3 | 2 | Van soort naar strafbaarheid | pictogram wetboek | VERVANGEN | N07 `onderwerp3_wet_regelgeving.webp` | door Jan te genereren |
| 3 | 3 | De Wet veilige jaarwisseling | pictogram kalender | GEEN BEELD NODIG | — — pictogram kalender mag blijven | n.v.t. |
| 3 | 4 | Wettekst: artikel 9.2.2.1a Wm, lid 1–3 | wetboek-illustratie | BEHOUDEN | — — vaste wetboek-illustratie bij wettekst; op telefoon verborgen | blijft |
| 3 | 5 | Wettekst: artikel 9.2.2.1a Wm, lid 4–7 | wetboek-illustratie | BEHOUDEN | — — vaste wetboek-illustratie bij wettekst; op telefoon verborgen | blijft |
| 3 | 6 | Lid 1: bezit en gebruik | pictogram tas | GEEN BEELD NODIG | — | n.v.t. |
| 3 | 7 | Lid 2, 6 en 7: verkoop | pictogram winkel | NIEUW | N09 `onderwerp3_verkoop_winkel.webp` | door Jan te genereren |
| 3 | 8 | Ontheffing van de burgemeester | pictogram akte | GEEN BEELD NODIG | — | n.v.t. |
| 3 | 9 | Ontheffing — voorbeeld uit de praktijk | pictogram akte | NIEUW | N08 `onderwerp3_ontheffing_sportveld.webp` | door Jan te genereren |
| 3 | 10 | Controlekaart: ontheffing aangetroffen | pictogram wetboek | NIEUW | N08 `onderwerp3_ontheffing_sportveld.webp` — zelfde casus | door Jan te genereren |
| 3 | 11 | Artikel 9.2.2.1a Wm — let op | boa-illustratie (master) | GEEN BEELD NODIG | — — boa-illustratie uit de master mag blijven | n.v.t. |
| 3 | 12 | Wettekst: artikel 1a en artikel 2 WED | wetboek-illustratie | BEHOUDEN | — — vaste wetboek-illustratie bij wettekst; op telefoon verborgen | blijft |
| 3 | 13 | Straffen | pictogram wetboek | GEEN BEELD NODIG | — | n.v.t. |
| 3 | 14 | Van regel naar opsporingsbevoegdheid | HTML-infographic | BEHOUDEN | — — HTML-tijdlijn | blijft |
| 3 | 15 | Kort samengevat | pictogram wetboek | GEEN BEELD NODIG | — | n.v.t. |
| 3 | 16 | Kort samengevat | pictogram lagen | GEEN BEELD NODIG | — | n.v.t. |
| 3 | 17 | Vooruitblik: Wanneer ben jij als boa bevoegd? | pictogram | GEEN BEELD NODIG | — | n.v.t. |
| 4 | 1 | Leerdoelen | boa-illustratie (master) | VERVANGEN | N10 `onderwerp4_zien_en_bevoegd.webp` | door Jan te genereren |
| 4 | 2 | Ben ik bevoegd? | pictogram knal | VERVANGEN | N01 `onderwerp1_plein_knal.webp` — zelfde casus plein | door Jan te genereren |
| 4 | 3 | Zien is iets anders dan bevoegd zijn | pictogram weegschaal | NIEUW | N10 `onderwerp4_zien_en_bevoegd.webp` | door Jan te genereren |
| 4 | 4 | Wettekst: de buitengewoon opsporingsambtenaar | wetboek-illustratie | BEHOUDEN | — — vaste wetboek-illustratie bij (wet)tekst; op telefoon verborgen | blijft |
| 4 | 5 | Domein I, onderdeel 9 | wetboek-illustratie | BEHOUDEN | — — vaste wetboek-illustratie bij (wet)tekst; op telefoon verborgen | blijft |
| 4 | 6 | Domeinlijst is niet: alles mag | pictogram domein | GEEN BEELD NODIG | — | n.v.t. |
| 4 | 7 | Let op: oudere teksten zijn achterhaald | boa-illustratie (master) | GEEN BEELD NODIG | — | n.v.t. |
| 4 | 8 | En F4 of ander professioneel vuurwerk? | pictogram vuurwerk | NIEUW | N11 `onderwerp4_kofferbak_f4.webp` | door Jan te genereren |
| 4 | 9 | Wettekst: artikel 17 WED | wetboek-illustratie | BEHOUDEN | — — vaste wetboek-illustratie bij (wet)tekst; op telefoon verborgen | blijft |
| 4 | 10 | Artikel 17 WED en jouw akte | wetboek-illustratie | BEHOUDEN | — — vaste wetboek-illustratie bij (wet)tekst; op telefoon verborgen | blijft |
| 4 | 11 | Wanneer ben jij als boa bevoegd? | pictogram domein | GEEN BEELD NODIG | — | n.v.t. |
| 4 | 12 | Zeven stappen: ben ik bevoegd en mag ik dit doen? | HTML-infographic | BEHOUDEN | — — HTML-stappenplaat | blijft |
| 4 | 13 | Je weet de categorie nog niet | pictogram vraag | VERVANGEN | N05 `onderwerp2_tas_verpakt_los.webp` — zelfde casus plein | door Jan te genereren |
| 4 | 14 | Je weet de categorie nog niet — betekenis | boa-illustratie (master) | VERVANGEN | N05 `onderwerp2_tas_verpakt_los.webp` | door Jan te genereren |
| 4 | 15 | Kort samengevat | pictogram weegschaal | GEEN BEELD NODIG | — | n.v.t. |
| 4 | 16 | Kort samengevat | boa-illustratie (master) | GEEN BEELD NODIG | — | n.v.t. |
| 4 | 17 | Vooruitblik: Wat mag je als boa doen? | pictogram | GEEN BEELD NODIG | — | n.v.t. |
| 5 | 1 | Leerdoelen | boa-illustratie (master) | VERVANGEN | N12 `onderwerp5_staande_houden.webp` | door Jan te genereren |
| 5 | 2 | Van mogen naar doen: vijf stappen | HTML-infographic | BEHOUDEN | — — HTML-stappenplaat | blijft |
| 5 | 3 | Bevoegdhedenkaart | HTML-infographic | BEHOUDEN | — — HTML-bevoegdhedenkaart | blijft |
| 5 | 4 | Let op: artikelnummers gecontroleerd | pictogram wetboek | GEEN BEELD NODIG | — | n.v.t. |
| 5 | 5 | Aanspreken, staande houden, aanhouden | boa-illustratie (master) | NIEUW | N12 `onderwerp5_staande_houden.webp` | door Jan te genereren |
| 5 | 6 | Wettekst: staande houden | wetboek-illustratie | BEHOUDEN | — — vaste wetboek-illustratie bij wettekst; op telefoon verborgen | blijft |
| 5 | 7 | Wie is verdachte? | wetboek-illustratie | BEHOUDEN | — — vaste wetboek-illustratie bij wettekst; op telefoon verborgen | blijft |
| 5 | 8 | Staande houden — situatie | boa-illustratie (master) | NIEUW | N12 `onderwerp5_staande_houden.webp` — zelfde casus | door Jan te genereren |
| 5 | 9 | Staande houden — vijf stappen | boa-illustratie (master) | NIEUW | N12 `onderwerp5_staande_houden.webp` — zelfde casus | door Jan te genereren |
| 5 | 10 | Wettekst: aanhouden op heterdaad | wetboek-illustratie | BEHOUDEN | — — vaste wetboek-illustratie bij wettekst; op telefoon verborgen | blijft |
| 5 | 11 | Aanhouden op heterdaad — vijf stappen | pictogram afspraak | NIEUW | N13 `onderwerp5_aanhouden.webp` | door Jan te genereren |
| 5 | 12 | Wettekst: aanhouden buiten heterdaad | wetboek-illustratie | BEHOUDEN | — — vaste wetboek-illustratie bij wettekst; op telefoon verborgen | blijft |
| 5 | 13 | Buiten heterdaad: wat betekent dit? | wetboek-illustratie | BEHOUDEN | — — vaste wetboek-illustratie bij wettekst; op telefoon verborgen | blijft |
| 5 | 14 | Let op: heterdaad en buiten heterdaad | boa-illustratie (master) | GEEN BEELD NODIG | — | n.v.t. |
| 5 | 15 | Wettekst: vervoermiddelen onderzoeken | wetboek-illustratie | BEHOUDEN | — — vaste wetboek-illustratie bij wettekst; op telefoon verborgen | blijft |
| 5 | 16 | Vervoermiddelen onderzoeken — situatie | pictogram bus | NIEUW | N14 `onderwerp5_auto_kofferbak.webp` | door Jan te genereren |
| 5 | 17 | Vervoermiddelen onderzoeken — vijf stappen | pictogram bus | NIEUW | N14 `onderwerp5_auto_kofferbak.webp` — zelfde casus | door Jan te genereren |
| 5 | 18 | Wettekst: medewerking vorderen | wetboek-illustratie | BEHOUDEN | — — vaste wetboek-illustratie bij wettekst; op telefoon verborgen | blijft |
| 5 | 19 | Medewerking vorderen — vijf stappen | pictogram bus | NIEUW | N14 `onderwerp5_auto_kofferbak.webp` — zelfde casus | door Jan te genereren |
| 5 | 20 | Wettekst: inbeslagneming en uitlevering vorderen | wetboek-illustratie | BEHOUDEN | — — vaste wetboek-illustratie bij wettekst; op telefoon verborgen | blijft |
| 5 | 21 | Inbeslagneming | pictogram slot | NIEUW | N15 `onderwerp5_inbeslagneming.webp` | door Jan te genereren |
| 5 | 22 | Inbeslagneming — vijf stappen | pictogram tas | NIEUW | N15 `onderwerp5_inbeslagneming.webp` — zelfde casus | door Jan te genereren |
| 5 | 23 | Wettekst: niet voldoen aan een vordering | wetboek-illustratie | BEHOUDEN | — — vaste wetboek-illustratie bij wettekst; op telefoon verborgen | blijft |
| 5 | 24 | Veiligstellen is geen aparte bevoegdheid | pictogram afstand | GEEN BEELD NODIG | — | n.v.t. |
| 5 | 25 | Proces-verbaal | HTML-infographic | NIEUW | N16 `onderwerp5_proces_verbaal.webp` | door Jan te genereren |
| 5 | 26 | Overdracht aan de politie | pictogram afspraak | NIEUW | N17 `onderwerp5_overdracht_politie.webp` | door Jan te genereren |
| 5 | 27 | Let op: redelijkerwijs nodig | boa-illustratie (master) | GEEN BEELD NODIG | — | n.v.t. |
| 5 | 28 | Kort samengevat | boa-illustratie (master) | GEEN BEELD NODIG | — | n.v.t. |
| 5 | 29 | Kort samengevat | pictogram pv-document | GEEN BEELD NODIG | — | n.v.t. |
| 5 | 30 | Vooruitblik: Onbekend en zwaar illegaal vuurwerk | pictogram | GEEN BEELD NODIG | — | n.v.t. |
| 6 | 1 | Leerdoelen | boa-illustratie (master) | VERVANGEN | N19 `onderwerp6_veiligheid_afstand.webp` | door Jan te genereren |
| 6 | 2 | Een tas zonder etiketten | pictogram tas | NIEUW | N18 `onderwerp6_tas_zonder_etiket.webp` | door Jan te genereren |
| 6 | 3 | Praktijkterm is geen wettelijke categorie | pictogram waarschuwing | NIEUW | N20 `onderwerp6_praktijktermen.webp` | door Jan te genereren |
| 6 | 4 | Aangepast of zelfgemaakt vuurwerk | pictogram waarschuwing | NIEUW | N20 `onderwerp6_praktijktermen.webp` | door Jan te genereren |
| 6 | 5 | Onbekend vuurwerk: wat weet je wel en niet? | pictogram vraag | VERVANGEN | N06 `onderwerp2_onbekend_vuurwerk.webp` | door Jan te genereren |
| 6 | 6 | Bevoegd is niet hetzelfde als veilig | pictogram afstand | NIEUW | N19 `onderwerp6_veiligheid_afstand.webp` | door Jan te genereren |
| 6 | 7 | Drie aparte vragen | HTML-infographic | BEHOUDEN | — — HTML-plaat drie vragen | blijft |
| 6 | 8 | Wanneer stop je met zelf onderzoeken? | pictogram afstand | NIEUW | N19 `onderwerp6_veiligheid_afstand.webp` | door Jan te genereren |
| 6 | 9 | Zelf optreden of politie inschakelen? | pictogram tas | NIEUW | N18 `onderwerp6_tas_zonder_etiket.webp` — zelfde casus | door Jan te genereren |
| 6 | 10 | Zelf optreden of politie inschakelen? — betekenis | boa-illustratie (master) | NIEUW | N18 `onderwerp6_tas_zonder_etiket.webp` — zelfde casus | door Jan te genereren |
| 6 | 11 | Kort samengevat | pictogram waarschuwing | GEEN BEELD NODIG | — | n.v.t. |
| 6 | 12 | Kort samengevat | boa-illustratie (master) | GEEN BEELD NODIG | — | n.v.t. |
| 6 | 13 | Vooruitblik: Taakverdeling tussen boa en politie | pictogram | GEEN BEELD NODIG | — | n.v.t. |
| 7 | 1 | Leerdoelen | boa-illustratie (master) | VERVANGEN | N21 `onderwerp7_briefing_jaarwisseling.webp` | door Jan te genereren |
| 7 | 2 | Mogen en doen zijn twee dingen | pictogram weegschaal | GEEN BEELD NODIG | — | n.v.t. |
| 7 | 3 | Bevoegdheid naast taakverdeling | HTML-infographic | BEHOUDEN | — — HTML-plaat | blijft |
| 7 | 4 | Het Handhavingsplan jaarwisseling | pictogram afspraak | NIEUW | N21 `onderwerp7_briefing_jaarwisseling.webp` | door Jan te genereren |
| 7 | 5 | Tekst uit het Handhavingsplan: inzet van boa’s | wetboek-illustratie | BEHOUDEN | — — vaste wetboek-illustratie; op telefoon verborgen | blijft |
| 7 | 6 | Tekst uit het Handhavingsplan: gevaar en openbare orde | wetboek-illustratie | BEHOUDEN | — — vaste wetboek-illustratie; op telefoon verborgen | blijft |
| 7 | 7 | Lokale afspraken | pictogram domein | GEEN BEELD NODIG | — | n.v.t. |
| 7 | 8 | Zelf afhandelen, overleggen of politie inschakelen | HTML-infographic | BEHOUDEN | — — HTML-routeplaat | blijft |
| 7 | 9 | Situatie 1: zelf afhandelen | pictogram straat | NIEUW | N22 `onderwerp7_woonstraat_fontein.webp` | door Jan te genereren |
| 7 | 10 | Situatie 2: overleggen | pictogram tas | NIEUW | N23 `onderwerp7_park_tas.webp` | door Jan te genereren |
| 7 | 11 | Situatie 3: politie inschakelen | pictogram mensen | NIEUW | N24 `onderwerp7_station_groep.webp` | door Jan te genereren |
| 7 | 12 | Zo verloopt een overdracht | pictogram afspraak | NIEUW | N17 `onderwerp5_overdracht_politie.webp` | door Jan te genereren |
| 7 | 13 | Kort samengevat | pictogram weegschaal | GEEN BEELD NODIG | — | n.v.t. |
| 7 | 14 | Kort samengevat | pictogram afspraak | GEEN BEELD NODIG | — | n.v.t. |
| 7 | 15 | Vooruitblik: Van melding tot proces-verbaal | pictogram | GEEN BEELD NODIG | — | n.v.t. |
| 8 | 1 | Leerdoelen | boa-illustratie (master) | VERVANGEN | N25 `onderwerp8_parkeerplaats_casus.webp` | door Jan te genereren |
| 8 | 2 | Terugblik | HTML-overzicht | BEHOUDEN | — — HTML-overzicht | blijft |
| 8 | 3 | De casus: een knal op de parkeerplaats | pictogram mensen | NIEUW | N25 `onderwerp8_parkeerplaats_casus.webp` | door Jan te genereren |
| 8 | 4 | Stap 1 – Wat neem je waar? | boa-illustratie (master) | NIEUW | N25 `onderwerp8_parkeerplaats_casus.webp` — zelfde casus parkeerplaats | door Jan te genereren |
| 8 | 5 | Stap 2 – Is er mogelijk sprake van een strafbaar feit? | pictogram wetboek | GEEN BEELD NODIG | — | n.v.t. |
| 8 | 6 | Stap 3 – Welk vuurwerk kan dit zijn? | pictogram tas | NIEUW | N05 `onderwerp2_tas_verpakt_los.webp` — zelfde casus parkeerplaats | door Jan te genereren |
| 8 | 7 | Stap 4 – Welke informatie heb je nog nodig? | boa-illustratie (master) | GEEN BEELD NODIG | — | n.v.t. |
| 8 | 8 | Stap 5 – Ben je hiervoor opsporingsbevoegd? | pictogram schild | GEEN BEELD NODIG | — | n.v.t. |
| 8 | 9 | Stap 6 – Welke bevoegdheden kun je toepassen? | boa-illustratie (master) | NIEUW | N15 `onderwerp5_inbeslagneming.webp` | door Jan te genereren |
| 8 | 10 | Stap 7 – Is het veilig om zelf verder te handelen? | pictogram afstand | NIEUW | N19 `onderwerp6_veiligheid_afstand.webp` | door Jan te genereren |
| 8 | 11 | Stap 8 – Moet de politie worden ingeschakeld? | pictogram afspraak | NIEUW | N17 `onderwerp5_overdracht_politie.webp` | door Jan te genereren |
| 8 | 12 | Stap 9 – Wat neem je in beslag of draag je over? | pictogram slot | NIEUW | N15 `onderwerp5_inbeslagneming.webp` | door Jan te genereren |
| 8 | 13 | Stap 10 – Wat komt in het proces-verbaal? | pictogram pv-document | NIEUW | N16 `onderwerp5_proces_verbaal.webp` | door Jan te genereren |
| 8 | 14 | Stap 10 – Zo niet | pictogram pv-document | NIEUW | N16 `onderwerp5_proces_verbaal.webp` | door Jan te genereren |
| 8 | 15 | Stap 10 – Zo wel | boa-illustratie (master) | NIEUW | N16 `onderwerp5_proces_verbaal.webp` | door Jan te genereren |
| 8 | 16 | Kort samengevat | pictogram document | GEEN BEELD NODIG | — | n.v.t. |
| 8 | 17 | Kort samengevat | pictogram wetboek | GEEN BEELD NODIG | — | n.v.t. |
| 8 | 18 | Kort samengevat | pictogram weegschaal | GEEN BEELD NODIG | — | n.v.t. |
| 8 | 19 | Kort samengevat | boa-illustratie (master) | GEEN BEELD NODIG | — | n.v.t. |
| 8 | 20 | Kort samengevat | pictogram waarschuwing | GEEN BEELD NODIG | — | n.v.t. |
| 8 | 21 | Kort samengevat | pictogram afspraak | GEEN BEELD NODIG | — | n.v.t. |
| 8 | 22 | Beslishulp: de vier vragen op straat | boa-illustratie (master) | GEEN BEELD NODIG | — | n.v.t. |
| 8 | 23 | Beslishulp: de vier vragen op straat | HTML-infographic | BEHOUDEN | — — HTML-beslishulp | blijft |
| 8 | 24 | Klaar voor de eindtoets | boa-illustratie (master) | VERVANGEN | N26 `afsluiting_veilige_jaarwisseling.webp` | door Jan te genereren |

### 3b. Oefenvragen

| Onderwerp | Vraag | Vraagtekst (begin) | Huidig beeld | Besluit | Nieuw beeld | Status |
|---|---|---|---|---|---|---|
| 2 | vraag 1 | Je ziet vuurwerk in een verpakking. Op het etiket staat «F2». Wat kun … | wetboek (neutraal) | VERVANGEN | N03 `onderwerp2_etiket_verpakking.webp` | door Jan te genereren |
| 2 | vraag 2 | Wie bepaalt volgens het Vuurwerkbesluit in welke categorie vuurwerk va… | doelwit (neutraal) | BEHOUDEN | neutraal pictogram (verraadt het antwoord niet) | blijft |
| 2 | vraag 3 | In een tas ligt vuurwerk zonder verpakking en zonder etiket. Hoe noem … | boa-uitleg (neutraal) | VERVANGEN | N05 `onderwerp2_tas_verpakt_los.webp` | door Jan te genereren |
| 2 | vraag 4 | Een collega zegt: «Dit is een nitraat, dus het is F4.» Er zit geen eti… | weegschaal (neutraal) | VERVANGEN | N20 `onderwerp6_praktijktermen.webp` | door Jan te genereren |
| 2 | vraag 5 | Een man zegt dat hij vuurwerk mag hebben omdat hij «persoon met gespec… | boa-notitie (neutraal) | VERVANGEN | N04 `onderwerp2_personen_gespecialiseerde_kennis.webp` | door Jan te genereren |
| 2 | vraag 6 | Voor welke categorie bestaat de ontheffingsmogelijkheid van de burgeme… | vraag (neutraal) | BEHOUDEN | neutraal pictogram (verraadt het antwoord niet) | blijft |
| 3 | vraag 1 | Op 15 oktober steekt een vrouw in haar tuin vuurwerk af. Op de verpakk… | doelwit (neutraal) | BEHOUDEN | neutraal pictogram (verraadt het antwoord niet) | blijft |
| 3 | vraag 2 | Het is 31 december, 20.00 uur. Een vereniging steekt op een afgezet sp… | boa-uitleg (neutraal) | VERVANGEN | N08 `onderwerp3_ontheffing_sportveld.webp` | door Jan te genereren |
| 3 | vraag 3 | Een overtreding van artikel 9.2.2.1a Wm is met opzet gepleegd. Wat is … | weegschaal (neutraal) | BEHOUDEN | neutraal pictogram (verraadt het antwoord niet) | blijft |
| 3 | vraag 4 | Een jongere heeft F2-vuurwerk met op de verpakking «Geschikt voor part… | boa-notitie (neutraal) | VERVANGEN | N03 `onderwerp2_etiket_verpakking.webp` | door Jan te genereren |
| 4 | vraag 1 | Je ziet dat iemand een strafbaar feit pleegt. Betekent dit dat jij als… | boa-uitleg (neutraal) | VERVANGEN | N10 `onderwerp4_zien_en_bevoegd.webp` | door Jan te genereren |
| 4 | vraag 2 | Wat staat sinds 8 september 2026 in domein I, onderdeel 9? | weegschaal (neutraal) | BEHOUDEN | neutraal pictogram (verraadt het antwoord niet) | blijft |
| 4 | vraag 3 | Een collega wijst op het Handhavingsplan (maart 2026): «Domein I-boa’s… | boa-notitie (neutraal) | BEHOUDEN | neutraal pictogram (verraadt het antwoord niet) | blijft |
| 4 | vraag 4 | Je vindt vuurwerk zonder etiket. Je weet de categorie niet. Wat is jui… | vraag (neutraal) | VERVANGEN | N06 `onderwerp2_onbekend_vuurwerk.webp` | door Jan te genereren |
| 4 | vraag 5 | Je bent domein I-boa bij een gemeente. Je taak is vooral parkeertoezic… | wetboek (neutraal) | VERVANGEN | N10 `onderwerp4_zien_en_bevoegd.webp` | door Jan te genereren |
| 4 | vraag 6 | Je bent domein I-boa. In een kofferbak zie je een doos met op het etik… | doelwit (neutraal) | VERVANGEN | N11 `onderwerp4_kofferbak_f4.webp` | door Jan te genereren |
| 5 | vraag 1 | Je spreekt een jongere aan die naast een tas staat. Je hebt nog geen a… | weegschaal (neutraal) | VERVANGEN | N12 `onderwerp5_staande_houden.webp` | door Jan te genereren |
| 5 | vraag 2 | De jongeren leggen een tas met vuurwerk in de kofferbak van een auto. … | boa-notitie (neutraal) | VERVANGEN | N14 `onderwerp5_auto_kofferbak.webp` | door Jan te genereren |
| 5 | vraag 3 | De bestuurder weigert de kofferbak te openen. Op welk artikel baseer j… | vraag (neutraal) | VERVANGEN | N14 `onderwerp5_auto_kofferbak.webp` | door Jan te genereren |
| 5 | vraag 4 | Je wilt verpakt F2-vuurwerk van een verdachte in beslag nemen. Wat is … | wetboek (neutraal) | VERVANGEN | N15 `onderwerp5_inbeslagneming.webp` | door Jan te genereren |
| 5 | vraag 5 | Je vordert uitlevering van het vuurwerk. De verdachte weigert opzettel… | doelwit (neutraal) | VERVANGEN | N15 `onderwerp5_inbeslagneming.webp` | door Jan te genereren |
| 5 | vraag 6 | Je neemt op straat twee verpakkingen met «F2» in beslag. Wat maak je d… | boa-uitleg (neutraal) | VERVANGEN | N15 `onderwerp5_inbeslagneming.webp` | door Jan te genereren |
| 5 | vraag 7 | Een collega zag gisteren dat een jongen opzettelijk F3-vuurwerk afstak… | weegschaal (neutraal) | VERVANGEN | N12 `onderwerp5_staande_houden.webp` | door Jan te genereren |
| 6 | vraag 1 | Welke drie vragen beoordeel je los van elkaar bij onbekend of zwaar vu… | boa-notitie (neutraal) | BEHOUDEN | neutraal pictogram (verraadt het antwoord niet) | blijft |
| 6 | vraag 2 | Je bent bevoegd, maar het vuurwerk is groot, met tape omwikkeld en zon… | vraag (neutraal) | VERVANGEN | N18 `onderwerp6_tas_zonder_etiket.webp` | door Jan te genereren |
| 6 | vraag 3 | Artikel 21 WED geeft opsporingsambtenaren de bevoegdheid om verpakking… | wetboek (neutraal) | VERVANGEN | N18 `onderwerp6_tas_zonder_etiket.webp` | door Jan te genereren |
| 6 | vraag 4 | Bij onbekend vuurwerk weet je de categorie niet. Wat leg je wél vast? | doelwit (neutraal) | VERVANGEN | N06 `onderwerp2_onbekend_vuurwerk.webp` | door Jan te genereren |
| 7 | vraag 1 | Wat is het verschil tussen juridische bevoegdheid en taakverdeling? | vraag (neutraal) | BEHOUDEN | neutraal pictogram (verraadt het antwoord niet) | blijft |
| 7 | vraag 2 | Waarop is de inzet van boa’s volgens het Handhavingsplan jaarwisseling… | wetboek (neutraal) | BEHOUDEN | neutraal pictogram (verraadt het antwoord niet) | blijft |
| 7 | vraag 3 | Bij een station zie je een groep met zwaar vuurwerk. De sfeer wordt gr… | doelwit (neutraal) | VERVANGEN | N24 `onderwerp7_station_groep.webp` | door Jan te genereren |
| 7 | vraag 4 | Een afspraak in je gemeente zegt dat jij iets oppakt, maar je bent er … | boa-uitleg (neutraal) | BEHOUDEN | neutraal pictogram (verraadt het antwoord niet) | blijft |

### 3c. Eindtoets, resultaat en certificaat

| Onderdeel | Vraag | Vraagtekst (begin) | Huidig beeld | Besluit | Nieuw beeld | Status |
|---|---|---|---|---|---|---|
| eindtoets | vraag 1 | Wat is de juiste volgorde van de vier vragen? | pictogram (roteert) | BEHOUDEN | neutraal pictogram | blijft |
| eindtoets | vraag 2 | Je vindt een verpakking met op het etiket «F3». Hoe gebruik je die inf… | boa-illustratie (roteert) | VERVANGEN | N03 `onderwerp2_etiket_verpakking.webp` | door Jan te genereren |
| eindtoets | vraag 3 | Wat is volgens het Vuurwerkbesluit «professioneel vuurwerk»? | pictogram (roteert) | BEHOUDEN | neutraal pictogram | blijft |
| eindtoets | vraag 4 | Op een parkeerplaats staat een tas. Daarin zitten verpakkingen met «F2… | boa-illustratie (roteert) | VERVANGEN | N05 `onderwerp2_tas_verpakt_los.webp` | door Jan te genereren |
| eindtoets | vraag 5 | Wat verbiedt artikel 9.2.2.1a, eerste lid, Wet milieubeheer? | pictogram (roteert) | BEHOUDEN | neutraal pictogram | blijft |
| eindtoets | vraag 6 | Op 31 december om 19.00 uur steekt een stichting op een afgezet terrei… | boa-illustratie (roteert) | VERVANGEN | N08 `onderwerp3_ontheffing_sportveld.webp` | door Jan te genereren |
| eindtoets | vraag 7 | Je ziet een man vuurwerk afsteken. Op de verpakking staat «F2». Hij lo… | boa-illustratie (roteert) | VERVANGEN | N12 `onderwerp5_staande_houden.webp` | door Jan te genereren |
| eindtoets | vraag 8 | Bij een controle zie je een doos met op het etiket «F4». Je bent domei… | boa-illustratie (roteert) | VERVANGEN | N11 `onderwerp4_kofferbak_f4.webp` | door Jan te genereren |
| eindtoets | vraag 9 | Een collega zegt: «Omdat het in de domeinlijst staat, mag ik als boa i… | boa-illustratie (roteert) | BEHOUDEN | neutraal pictogram | blijft |
| eindtoets | vraag 10 | Je ziet iemand F2-vuurwerk afsteken. Je wilt hem laten stoppen om zijn… | boa-illustratie (roteert) | BEHOUDEN | neutraal pictogram | blijft |
| eindtoets | vraag 11 | Je onderzoekt de lading van een auto (art. 23 WED). Je vordert dat de … | boa-illustratie (roteert) | VERVANGEN | N14 `onderwerp5_auto_kofferbak.webp` | door Jan te genereren |
| eindtoets | vraag 12 | Je wilt verpakt F2-vuurwerk van een verdachte in beslag nemen. Welk ar… | boa-illustratie (roteert) | BEHOUDEN | neutraal pictogram | blijft |
| eindtoets | vraag 13 | Op oudejaarsavond loopt een groep met zwaar vuurwerk uit de hand op ee… | boa-illustratie (roteert) | VERVANGEN | N24 `onderwerp7_station_groep.webp` | door Jan te genereren |
| eindtoets | vraag 14 | Je bent bevoegd, maar het vuurwerk is groot, zonder etiket en met tape… | boa-illustratie (roteert) | VERVANGEN | N18 `onderwerp6_tas_zonder_etiket.webp` | door Jan te genereren |
| eindtoets | vraag 15 | Welke zin hoort in een goed proces-verbaal? | pictogram (roteert) | VERVANGEN | N16 `onderwerp5_proces_verbaal.webp` | door Jan te genereren |
| resultaat | – | Resultaat eindtoets | boa-illustratie (master) | BEHOUDEN | — (optioneel N26 bij geslaagd) | blijft |
| certificaat | – | Certificaat | JS-schildlogo | GEEN BEELD NODIG | — (een certificaat hoort rustig te blijven) | n.v.t. |
| start | – | Intake en welkom | boa-illustratie (master) | BEHOUDEN | — (optioneel N26 als brede kop) | blijft |

### Totalen

- Beoordeelde inhoudspagina’s: **145**; oefenvragen: **31**; eindtoetsvragen: **15**; plus start, resultaat en certificaat.
- Besluiten inhoudspagina’s: BEHOUDEN 32 · VERVANGEN 28 · NIEUW 40 · GEEN BEELD NODIG 45.
- Oefenvragen met nieuw situatiebeeld: 21; eindtoetsvragen met nieuw situatiebeeld: 9.
- Unieke nieuwe beelden in dit plan: **42** — waarvan 4 categoriekaarten (F1–F4), 12 productillustraties en 26 situatie-/praktijkbeelden.
- In deze ronde vervangen of nieuw geplaatst: **0** (geen beeldgenerator). Nog door Jan te genereren: **42**.

## 4. Specificatie per nieuw beeld

### N01 · `onderwerp1_plein_knal.webp`

- **Gebruikt op:** O1 p2, O1 p3, O4 p2
- **Doel:** Casus “plein”: de eerste waarneming. Waarom je eerst denkt en dan doet.
- **Personages:** H1 Noor en H2 Daan; groep van vier jongeren (divers, 16–19 jaar, winterjassen)
- **Scène/handeling:** Begin van de avond op een Nederlands plein met bakstenen bestrating en winkelpuien. Een groep jongeren staat bij elkaar; één jongere houdt een ongeopende vuurwerkverpakking vast; naast de groep staat een sporttas. De twee handhavers staan op enkele meters afstand, rustig observerend, van achteren/half van opzij gezien (HANDHAVING op de rug leesbaar).
- **Kleding/embleem:** handhavers volgens §1 (HANDHAVING op de rug, BOA-embleem op de arm)
- **Formaat:** 3:2, 1800 × 1200 px
- **Absoluut niet in beeld:** geen ontstoken vuurwerk, geen agressie, geen herkenbare merknamen
- **Alt-tekst:** Twee handhavers kijken op een plein vanaf enige afstand naar een groep jongeren met een tas vuurwerk.
- **Prompt:**

```
Modern professional editorial cartoon illustration, semi-realistic proportions, clean confident line work, soft cel shading, calm adult tone, Dutch setting, colour palette dominated by dark navy blue, mid/light blue, white and silver grey with orange as accent colour, uncluttered background, main subjects in the central 60% of the frame so the image can be cropped for mobile. Dutch municipal enforcement officers (boa's) wear a dark navy Dutch enforcement uniform (jacket and trousers, subtle light-blue/white checkered band), the word HANDHAVING in white capital letters on the back; on the upper LEFT SLEEVE the official Dutch BOA emblem: a black shield with a light border and the white BOA symbol; no other badges, no police badge, no municipal coat of arms, no weapons drawn. Scene: early evening on a Dutch brick-paved town square with shopfronts; a group of four teenagers of mixed backgrounds in winter jackets stand together, one holds an unopened firework package, a sports bag on the ground beside them; two enforcement officers (a woman ~30 with dark hair in a low bun, a man ~35 with short dark hair) stand a few metres away, calm and observant, seen from behind at three-quarter angle so HANDHAVING on their backs is visible. Aspect ratio 3:2.
Negative: NOT: the word POLITIE or POLICE on enforcement clothing, American police uniforms, sheriff stars, fantasy badges, the BOA emblem on objects (boxes, laptops, cups, walls, cars, documents), children's-book style, exaggerated cartoon faces, 3D/plastic render, photorealism, gore, explosions near people, anyone holding, opening or dismantling unknown or heavy fireworks, readable brand names, gibberish text, extra fingers, distorted hands
```

### N02 · `onderwerp1_gesprek_jongeren.webp`

- **Gebruikt op:** O1 p1, O1 p4
- **Doel:** Waarom vuurwerk bij jouw werk hoort: in gesprek, preventief en rustig.
- **Personages:** H1 Noor en H2 Daan (zelfde casus als N01); dezelfde jongeren
- **Scène/handeling:** Dezelfde plek als N01. De handhavers spreken de jongeren rustig aan; open lichaamshouding; de tas staat op de grond.
- **Kleding/embleem:** handhavers volgens §1 (HANDHAVING op de rug, BOA-embleem op de arm)
- **Formaat:** 4:3, 1600 × 1200 px
- **Absoluut niet in beeld:** geen dreiging, geen handboeien
- **Alt-tekst:** Handhavers spreken op een plein rustig een groep jongeren aan.
- **Prompt:**

```
Modern professional editorial cartoon illustration, semi-realistic proportions, clean confident line work, soft cel shading, calm adult tone, Dutch setting, colour palette dominated by dark navy blue, mid/light blue, white and silver grey with orange as accent colour, uncluttered background, main subjects in the central 60% of the frame so the image can be cropped for mobile. Dutch municipal enforcement officers (boa's) wear a dark navy Dutch enforcement uniform (jacket and trousers, subtle light-blue/white checkered band), the word HANDHAVING in white capital letters on the back; on the upper LEFT SLEEVE the official Dutch BOA emblem: a black shield with a light border and the white BOA symbol; no other badges, no police badge, no municipal coat of arms, no weapons drawn. Scene: the same Dutch square as before; the two enforcement officers talk calmly with the group of teenagers, open body language, the sports bag stays on the ground, relaxed atmosphere. Aspect ratio 4:3.
Negative: NOT: the word POLITIE or POLICE on enforcement clothing, American police uniforms, sheriff stars, fantasy badges, the BOA emblem on objects (boxes, laptops, cups, walls, cars, documents), children's-book style, exaggerated cartoon faces, 3D/plastic render, photorealism, gore, explosions near people, anyone holding, opening or dismantling unknown or heavy fireworks, readable brand names, gibberish text, extra fingers, distorted hands
```

### N03 · `onderwerp2_etiket_verpakking.webp`

- **Gebruikt op:** O1 p5, O2 p10, oefenvraag O2 v1, oefenvraag O3 v4, eindtoets v2
- **Doel:** Kijk wat er werkelijk op het etiket staat.
- **Personages:** optioneel: hand van H3 Ingrid (mouw met BOA-embleem zichtbaar) die de verpakking vasthoudt; alleen bij verpakt F2-vuurwerk
- **Scène/handeling:** Close-up van een consumentenvuurwerkverpakking met etiket. Leesbaar alleen: “F2”, “CE”, “NEM 250 g” en “Geschikt voor particulier gebruik”. Overige etikettekst onscherp.
- **Kleding/embleem:** handhavers volgens §1 (HANDHAVING op de rug, BOA-embleem op de arm)
- **Formaat:** 4:3, 1600 × 1200 px
- **Absoluut niet in beeld:** geen andere leesbare tekst, geen merknaam, geen BOA-logo op de verpakking
- **Alt-tekst:** Close-up van een vuurwerketiket met categorie F2, CE-markering en NEM.
- **Prompt:**

```
Modern professional editorial cartoon illustration, semi-realistic proportions, clean confident line work, soft cel shading, calm adult tone, Dutch setting, colour palette dominated by dark navy blue, mid/light blue, white and silver grey with orange as accent colour, uncluttered background, main subjects in the central 60% of the frame so the image can be cropped for mobile. Dutch municipal enforcement officers (boa's) wear a dark navy Dutch enforcement uniform (jacket and trousers, subtle light-blue/white checkered band), the word HANDHAVING in white capital letters on the back; on the upper LEFT SLEEVE the official Dutch BOA emblem: a black shield with a light border and the white BOA symbol; no other badges, no police badge, no municipal coat of arms, no weapons drawn. Scene: close-up of a consumer firework package label; the only legible text is "F2", "CE", "NEM 250 g" and "Geschikt voor particulier gebruik", all other label text softly out of focus; optionally a gloved hand of an enforcement officer holding the sealed package, sleeve with the BOA shield emblem visible. Aspect ratio 4:3.
Negative: NOT: the word POLITIE or POLICE on enforcement clothing, American police uniforms, sheriff stars, fantasy badges, the BOA emblem on objects (boxes, laptops, cups, walls, cars, documents), children's-book style, exaggerated cartoon faces, 3D/plastic render, photorealism, gore, explosions near people, anyone holding, opening or dismantling unknown or heavy fireworks, readable brand names, gibberish text, extra fingers, distorted hands
```

### N04 · `onderwerp2_personen_gespecialiseerde_kennis.webp`

- **Gebruikt op:** O2 p9, oefenvraag O2 v5
- **Doel:** Wie zijn personen met gespecialiseerde kennis?
- **Personages:** pyrotechnicus (vrouw, ca. 50) met vergunningsmap, brandweerman, politieagent; géén boa
- **Scène/handeling:** Drie vakmensen naast elkaar bij een afgezet professioneel afsteekterrein overdag: pyrotechnicus in werkkleding, brandweer, politie. Op de achtergrond gesloten transportdozen.
- **Kleding/embleem:** geen handhavers in beeld
- **Formaat:** 4:3, 1600 × 1200 px
- **Absoluut niet in beeld:** geen boa in dit beeld (boa’s staan niet in de lijst)
- **Alt-tekst:** Een pyrotechnicus, een brandweerman en een politieagent bij een professioneel afsteekterrein.
- **Prompt:**

```
Modern professional editorial cartoon illustration, semi-realistic proportions, clean confident line work, soft cel shading, calm adult tone, Dutch setting, colour palette dominated by dark navy blue, mid/light blue, white and silver grey with orange as accent colour, uncluttered background, main subjects in the central 60% of the frame so the image can be cropped for mobile. Scene: three professionals standing side by side at a fenced professional fireworks show site in daylight: a female pyrotechnician ~50 in work clothes holding a permit folder, a Dutch firefighter, a Dutch police officer; sealed transport boxes in the background; no enforcement officer in this image. Aspect ratio 4:3.
Negative: NOT: the word POLITIE or POLICE on enforcement clothing, American police uniforms, sheriff stars, fantasy badges, the BOA emblem on objects (boxes, laptops, cups, walls, cars, documents), children's-book style, exaggerated cartoon faces, 3D/plastic render, photorealism, gore, explosions near people, anyone holding, opening or dismantling unknown or heavy fireworks, readable brand names, gibberish text, extra fingers, distorted hands
```

### N05 · `onderwerp2_tas_verpakt_los.webp`

- **Gebruikt op:** O2 p11, O2 p15, O4 p13, O4 p14, O8 p6, oefenvraag O2 v3, eindtoets v4
- **Doel:** Zelfde tas, andere informatie: verpakt met etiket tegenover los zonder etiket.
- **Personages:** geen personen (of alleen voeten van H1/H2 op afstand)
- **Scène/handeling:** Open sporttas op straattegels. Links in de tas verpakkingen met klein etiket “F2”; rechts losse hulzen zonder verpakking of etiket. Niemand raakt het aan.
- **Kleding/embleem:** handhavers volgens §1 (HANDHAVING op de rug, BOA-embleem op de arm)
- **Formaat:** 3:2, 1800 × 1200 px
- **Absoluut niet in beeld:** geen aangestoken vuurwerk, geen hand in de tas
- **Alt-tekst:** Open tas met verpakt vuurwerk met etiket en los vuurwerk zonder etiket.
- **Prompt:**

```
Modern professional editorial cartoon illustration, semi-realistic proportions, clean confident line work, soft cel shading, calm adult tone, Dutch setting, colour palette dominated by dark navy blue, mid/light blue, white and silver grey with orange as accent colour, uncluttered background, main subjects in the central 60% of the frame so the image can be cropped for mobile. Scene: an open sports bag on Dutch pavement; on the left side packaged fireworks with a small label that reads only "F2", on the right loose unlabelled cardboard tubes without packaging; nobody touching the bag. Aspect ratio 3:2.
Negative: NOT: the word POLITIE or POLICE on enforcement clothing, American police uniforms, sheriff stars, fantasy badges, the BOA emblem on objects (boxes, laptops, cups, walls, cars, documents), children's-book style, exaggerated cartoon faces, 3D/plastic render, photorealism, gore, explosions near people, anyone holding, opening or dismantling unknown or heavy fireworks, readable brand names, gibberish text, extra fingers, distorted hands
```

### N06 · `onderwerp2_onbekend_vuurwerk.webp`

- **Gebruikt op:** O2 p12, O2 p14, O6 p5, oefenvraag O4 v4, oefenvraag O6 v4
- **Doel:** Onbekend vuurwerk: je weet wat je ziet, niet welke categorie.
- **Personages:** op de achtergrond onscherp H4 Tim die afstand houdt
- **Scène/handeling:** Enkele losse, onbekende vuurwerkachtige voorwerpen zonder etiket op nat plaveisel bij een lantaarnpaal ’s avonds. Op de achtergrond, op afstand, een handhaver die niet dichterbij komt.
- **Kleding/embleem:** handhavers volgens §1 (HANDHAVING op de rug, BOA-embleem op de arm)
- **Formaat:** 4:3, 1600 × 1200 px
- **Absoluut niet in beeld:** niemand die de voorwerpen aanraakt
- **Alt-tekst:** Losse vuurwerkachtige voorwerpen zonder etiket op straat; een handhaver houdt afstand.
- **Prompt:**

```
Modern professional editorial cartoon illustration, semi-realistic proportions, clean confident line work, soft cel shading, calm adult tone, Dutch setting, colour palette dominated by dark navy blue, mid/light blue, white and silver grey with orange as accent colour, uncluttered background, main subjects in the central 60% of the frame so the image can be cropped for mobile. Dutch municipal enforcement officers (boa's) wear a dark navy Dutch enforcement uniform (jacket and trousers, subtle light-blue/white checkered band), the word HANDHAVING in white capital letters on the back; on the upper LEFT SLEEVE the official Dutch BOA emblem: a black shield with a light border and the white BOA symbol; no other badges, no police badge, no municipal coat of arms, no weapons drawn. Scene: several loose unlabelled firework-like cylinders lying on wet pavement under a street lamp at night; in the background, out of focus, an enforcement officer keeps his distance and does not approach. Aspect ratio 4:3.
Negative: NOT: the word POLITIE or POLICE on enforcement clothing, American police uniforms, sheriff stars, fantasy badges, the BOA emblem on objects (boxes, laptops, cups, walls, cars, documents), children's-book style, exaggerated cartoon faces, 3D/plastic render, photorealism, gore, explosions near people, anyone holding, opening or dismantling unknown or heavy fireworks, readable brand names, gibberish text, extra fingers, distorted hands
```

### N07 · `onderwerp3_wet_regelgeving.webp`

- **Gebruikt op:** O3 p1, O3 p2
- **Doel:** Onderwerp 3 “Wat zegt de wet?”: van soort naar strafbaarheid.
- **Personages:** geen personen
- **Scène/handeling:** Nederlands wetboek (donkerblauw, zonder leesbare titel) met een kleine rechtershamer en een vuurwerkverpakking op een bureau; rustig licht.
- **Kleding/embleem:** geen handhavers in beeld
- **Formaat:** 4:3, 1600 × 1200 px
- **Absoluut niet in beeld:** geen wapens, geen Amerikaanse rechtbank
- **Alt-tekst:** Wetboek en rechtershamer naast een vuurwerkverpakking.
- **Prompt:**

```
Modern professional editorial cartoon illustration, semi-realistic proportions, clean confident line work, soft cel shading, calm adult tone, Dutch setting, colour palette dominated by dark navy blue, mid/light blue, white and silver grey with orange as accent colour, uncluttered background, main subjects in the central 60% of the frame so the image can be cropped for mobile. Scene: a dark navy Dutch law book without readable title, a small judge’s gavel and a sealed firework package on a tidy desk, calm light, subtle legal imagery. Aspect ratio 4:3.
Negative: NOT: the word POLITIE or POLICE on enforcement clothing, American police uniforms, sheriff stars, fantasy badges, the BOA emblem on objects (boxes, laptops, cups, walls, cars, documents), children's-book style, exaggerated cartoon faces, 3D/plastic render, photorealism, gore, explosions near people, anyone holding, opening or dismantling unknown or heavy fireworks, readable brand names, gibberish text, extra fingers, distorted hands
```

### N08 · `onderwerp3_ontheffing_sportveld.webp`

- **Gebruikt op:** O3 p9, O3 p10, oefenvraag O3 v2, eindtoets v6
- **Doel:** Ontheffing: F2 is niet altijd verboden.
- **Personages:** H4 Tim; supervisor van de vereniging (man, ca. 60, kaal, bril) met ontheffing in hand
- **Scène/handeling:** 31 december, avond. Afgezet sportveld met hekken en lint; verderop een klein team dat vuurwerk klaarzet. De handhaver bekijkt samen met de supervisor een document (ontheffing) aan de rand van het terrein.
- **Kleding/embleem:** handhavers volgens §1 (HANDHAVING op de rug, BOA-embleem op de arm)
- **Formaat:** 3:2, 1800 × 1200 px
- **Absoluut niet in beeld:** geen vuurwerk dat afgaat vlak bij mensen, geen leesbare tekst op het document
- **Alt-tekst:** Een handhaver bekijkt op een afgezet sportveld de ontheffing met de supervisor van de vereniging.
- **Prompt:**

```
Modern professional editorial cartoon illustration, semi-realistic proportions, clean confident line work, soft cel shading, calm adult tone, Dutch setting, colour palette dominated by dark navy blue, mid/light blue, white and silver grey with orange as accent colour, uncluttered background, main subjects in the central 60% of the frame so the image can be cropped for mobile. Dutch municipal enforcement officers (boa's) wear a dark navy Dutch enforcement uniform (jacket and trousers, subtle light-blue/white checkered band), the word HANDHAVING in white capital letters on the back; on the upper LEFT SLEEVE the official Dutch BOA emblem: a black shield with a light border and the white BOA symbol; no other badges, no police badge, no municipal coat of arms, no weapons drawn. Scene: New Year’s Eve evening at a fenced-off Dutch sports field with barriers and tape; in the distance a small crew prepares ground fireworks; at the edge of the field an enforcement officer (man ~28, light brown hair, short beard) reviews a permit document together with the association supervisor (man ~60, bald, glasses); document text not readable. Aspect ratio 3:2.
Negative: NOT: the word POLITIE or POLICE on enforcement clothing, American police uniforms, sheriff stars, fantasy badges, the BOA emblem on objects (boxes, laptops, cups, walls, cars, documents), children's-book style, exaggerated cartoon faces, 3D/plastic render, photorealism, gore, explosions near people, anyone holding, opening or dismantling unknown or heavy fireworks, readable brand names, gibberish text, extra fingers, distorted hands
```

### N09 · `onderwerp3_verkoop_winkel.webp`

- **Gebruikt op:** O3 p7
- **Doel:** Verkoop van F2 en F3 (lid 2, 6 en 7).
- **Personages:** verkoper (vrouw, ca. 45); koper (man, ca. 50) met ontheffingsdocument; géén boa nodig
- **Scène/handeling:** Toonbank van een vuurwerkverkooppunt op 31 december overdag; de verkoper controleert een document van de koper; verpakte dozen op de achtergrond.
- **Kleding/embleem:** geen handhavers in beeld
- **Formaat:** 4:3, 1600 × 1200 px
- **Absoluut niet in beeld:** geen leesbare merknamen of prijzen
- **Alt-tekst:** Een verkoper controleert bij de toonbank het document van een koper.
- **Prompt:**

```
Modern professional editorial cartoon illustration, semi-realistic proportions, clean confident line work, soft cel shading, calm adult tone, Dutch setting, colour palette dominated by dark navy blue, mid/light blue, white and silver grey with orange as accent colour, uncluttered background, main subjects in the central 60% of the frame so the image can be cropped for mobile. Scene: a Dutch fireworks sales counter on 31 December in daytime; a female shop assistant ~45 checks a document shown by a male customer ~50; sealed boxes on shelves in the background; no readable brand names or prices. Aspect ratio 4:3.
Negative: NOT: the word POLITIE or POLICE on enforcement clothing, American police uniforms, sheriff stars, fantasy badges, the BOA emblem on objects (boxes, laptops, cups, walls, cars, documents), children's-book style, exaggerated cartoon faces, 3D/plastic render, photorealism, gore, explosions near people, anyone holding, opening or dismantling unknown or heavy fireworks, readable brand names, gibberish text, extra fingers, distorted hands
```

### N10 · `onderwerp4_zien_en_bevoegd.webp`

- **Gebruikt op:** O4 p1, O4 p3, oefenvraag O4 v1, oefenvraag O4 v5
- **Doel:** Zien is iets anders dan bevoegd zijn.
- **Personages:** H5 Esther
- **Scène/handeling:** Handhaver staat op een stoep en ziet verderop iemand een fontein afsteken; ze pakt haar portofoon/notitieboek en denkt na (geen gedachtewolkjes met tekst).
- **Kleding/embleem:** handhavers volgens §1 (HANDHAVING op de rug, BOA-embleem op de arm)
- **Formaat:** 4:3, 1600 × 1200 px
- **Absoluut niet in beeld:** geen tekst in het beeld
- **Alt-tekst:** Een handhaver ziet op afstand iemand vuurwerk afsteken en beoordeelt de situatie.
- **Prompt:**

```
Modern professional editorial cartoon illustration, semi-realistic proportions, clean confident line work, soft cel shading, calm adult tone, Dutch setting, colour palette dominated by dark navy blue, mid/light blue, white and silver grey with orange as accent colour, uncluttered background, main subjects in the central 60% of the frame so the image can be cropped for mobile. Dutch municipal enforcement officers (boa's) wear a dark navy Dutch enforcement uniform (jacket and trousers, subtle light-blue/white checkered band), the word HANDHAVING in white capital letters on the back; on the upper LEFT SLEEVE the official Dutch BOA emblem: a black shield with a light border and the white BOA symbol; no other badges, no police badge, no municipal coat of arms, no weapons drawn. Scene: an enforcement officer (woman ~35, dark skin, short black curly hair) stands on a pavement and sees, some distance away, a person lighting a small ground fountain; she holds a notebook and looks thoughtful and calm. Aspect ratio 4:3.
Negative: NOT: the word POLITIE or POLICE on enforcement clothing, American police uniforms, sheriff stars, fantasy badges, the BOA emblem on objects (boxes, laptops, cups, walls, cars, documents), children's-book style, exaggerated cartoon faces, 3D/plastic render, photorealism, gore, explosions near people, anyone holding, opening or dismantling unknown or heavy fireworks, readable brand names, gibberish text, extra fingers, distorted hands
```

### N11 · `onderwerp4_kofferbak_f4.webp`

- **Gebruikt op:** O4 p8, oefenvraag O4 v6, eindtoets v8
- **Doel:** F4 of ander professioneel vuurwerk: bevoegdheid niet automatisch.
- **Personages:** H6 Karim en H2 Daan op afstand; geen bestuurder in beeld
- **Scène/handeling:** Geopende kofferbak van een geparkeerde auto met gesloten transportdozen met oranje gevarenetiket; de handhavers staan op afstand en overleggen; één pakt zijn portofoon.
- **Kleding/embleem:** handhavers volgens §1 (HANDHAVING op de rug, BOA-embleem op de arm)
- **Formaat:** 3:2, 1800 × 1200 px
- **Absoluut niet in beeld:** kenteken niet leesbaar; niemand opent de dozen; geen “F4”-tekst als het antwoord van een toetsvraag daarmee wordt verraden
- **Alt-tekst:** Twee handhavers houden afstand van een geopende kofferbak met dozen met een gevarenetiket.
- **Prompt:**

```
Modern professional editorial cartoon illustration, semi-realistic proportions, clean confident line work, soft cel shading, calm adult tone, Dutch setting, colour palette dominated by dark navy blue, mid/light blue, white and silver grey with orange as accent colour, uncluttered background, main subjects in the central 60% of the frame so the image can be cropped for mobile. Dutch municipal enforcement officers (boa's) wear a dark navy Dutch enforcement uniform (jacket and trousers, subtle light-blue/white checkered band), the word HANDHAVING in white capital letters on the back; on the upper LEFT SLEEVE the official Dutch BOA emblem: a black shield with a light border and the white BOA symbol; no other badges, no police badge, no municipal coat of arms, no weapons drawn. Scene: the open boot of a parked car containing sealed brown transport boxes with orange hazard labels; two enforcement officers (man ~45 bald with greying beard, man ~35 short dark hair) keep their distance and consult each other, one uses his radio; licence plate not readable. Aspect ratio 3:2.
Negative: NOT: the word POLITIE or POLICE on enforcement clothing, American police uniforms, sheriff stars, fantasy badges, the BOA emblem on objects (boxes, laptops, cups, walls, cars, documents), children's-book style, exaggerated cartoon faces, 3D/plastic render, photorealism, gore, explosions near people, anyone holding, opening or dismantling unknown or heavy fireworks, readable brand names, gibberish text, extra fingers, distorted hands
```

### N12 · `onderwerp5_staande_houden.webp`

- **Gebruikt op:** O5 p1, O5 p5, O5 p8, O5 p9, oefenvraag O5 v1, oefenvraag O5 v7, eindtoets v7
- **Doel:** Staande houden: identiteit vaststellen van een verdachte.
- **Personages:** H3 Ingrid en H4 Tim; jongeman (ca. 18, rossig haar, capuchon)
- **Scène/handeling:** Woonstraat, avond. De jongeman heeft net een vuurpijl afgestoken en een verpakking weggegooid; de handhavers spreken hem rustig aan; hij toont een identiteitsbewijs.
- **Kleding/embleem:** handhavers volgens §1 (HANDHAVING op de rug, BOA-embleem op de arm)
- **Formaat:** 4:3, 1600 × 1200 px
- **Absoluut niet in beeld:** geen fysiek geweld, geen handboeien
- **Alt-tekst:** Twee handhavers vragen een jongeman om zijn identiteitsbewijs.
- **Prompt:**

```
Modern professional editorial cartoon illustration, semi-realistic proportions, clean confident line work, soft cel shading, calm adult tone, Dutch setting, colour palette dominated by dark navy blue, mid/light blue, white and silver grey with orange as accent colour, uncluttered background, main subjects in the central 60% of the frame so the image can be cropped for mobile. Dutch municipal enforcement officers (boa's) wear a dark navy Dutch enforcement uniform (jacket and trousers, subtle light-blue/white checkered band), the word HANDHAVING in white capital letters on the back; on the upper LEFT SLEEVE the official Dutch BOA emblem: a black shield with a light border and the white BOA symbol; no other badges, no police badge, no municipal coat of arms, no weapons drawn. Scene: a Dutch residential street at night; a young man ~18 with reddish hair and a hoodie shows an ID card to two enforcement officers (woman ~40 blond ponytail, man ~28 light brown hair short beard) who speak to him calmly; a discarded firework package on the ground. Aspect ratio 4:3.
Negative: NOT: the word POLITIE or POLICE on enforcement clothing, American police uniforms, sheriff stars, fantasy badges, the BOA emblem on objects (boxes, laptops, cups, walls, cars, documents), children's-book style, exaggerated cartoon faces, 3D/plastic render, photorealism, gore, explosions near people, anyone holding, opening or dismantling unknown or heavy fireworks, readable brand names, gibberish text, extra fingers, distorted hands
```

### N13 · `onderwerp5_aanhouden.webp`

- **Gebruikt op:** O5 p11
- **Doel:** Aanhouden is een zware maatregel.
- **Personages:** H5 Esther en H6 Karim; volwassen man (ca. 30)
- **Scène/handeling:** Rustige aanhouding in een winkelstraat: één handhaver legt uit, de ander staat ondersteunend naast de persoon; omstanders op afstand. Professioneel, geen dramatiek.
- **Kleding/embleem:** handhavers volgens §1 (HANDHAVING op de rug, BOA-embleem op de arm)
- **Formaat:** 4:3, 1600 × 1200 px
- **Absoluut niet in beeld:** geen geweld, geen wapens, geen Amerikaanse handboeienscène
- **Alt-tekst:** Twee handhavers houden rustig een man aan in een winkelstraat.
- **Prompt:**

```
Modern professional editorial cartoon illustration, semi-realistic proportions, clean confident line work, soft cel shading, calm adult tone, Dutch setting, colour palette dominated by dark navy blue, mid/light blue, white and silver grey with orange as accent colour, uncluttered background, main subjects in the central 60% of the frame so the image can be cropped for mobile. Dutch municipal enforcement officers (boa's) wear a dark navy Dutch enforcement uniform (jacket and trousers, subtle light-blue/white checkered band), the word HANDHAVING in white capital letters on the back; on the upper LEFT SLEEVE the official Dutch BOA emblem: a black shield with a light border and the white BOA symbol; no other badges, no police badge, no municipal coat of arms, no weapons drawn. Scene: a calm arrest in a Dutch shopping street: one enforcement officer explains, the other stands supportively beside the adult man; bystanders at a distance; professional, no drama, no weapons. Aspect ratio 4:3.
Negative: NOT: the word POLITIE or POLICE on enforcement clothing, American police uniforms, sheriff stars, fantasy badges, the BOA emblem on objects (boxes, laptops, cups, walls, cars, documents), children's-book style, exaggerated cartoon faces, 3D/plastic render, photorealism, gore, explosions near people, anyone holding, opening or dismantling unknown or heavy fireworks, readable brand names, gibberish text, extra fingers, distorted hands
```

### N14 · `onderwerp5_auto_kofferbak.webp`

- **Gebruikt op:** O5 p16, O5 p17, O5 p19, oefenvraag O5 v2, oefenvraag O5 v3, eindtoets v11
- **Doel:** Vervoermiddel onderzoeken, medewerking vorderen.
- **Personages:** H2 Daan en H1 Noor (andere casus dan plein: gebruik bij voorkeur H4/H5 als je N01 al met H1/H2 gebruikt); bestuurder: vrouw, ca. 50, grijs kort haar
- **Scène/handeling:** Parkeerplaats; auto stilgehouden; bestuurder opent op verzoek de kofferbak; daarin een sporttas en enkele verpakkingen. Handhavers op veilige afstand, één noteert.
- **Kleding/embleem:** handhavers volgens §1 (HANDHAVING op de rug, BOA-embleem op de arm)
- **Formaat:** 3:2, 1800 × 1200 px
- **Absoluut niet in beeld:** kenteken niet leesbaar, niet laten zien dat alles verboden is
- **Alt-tekst:** Een bestuurder opent op verzoek van handhavers de kofferbak.
- **Prompt:**

```
Modern professional editorial cartoon illustration, semi-realistic proportions, clean confident line work, soft cel shading, calm adult tone, Dutch setting, colour palette dominated by dark navy blue, mid/light blue, white and silver grey with orange as accent colour, uncluttered background, main subjects in the central 60% of the frame so the image can be cropped for mobile. Dutch municipal enforcement officers (boa's) wear a dark navy Dutch enforcement uniform (jacket and trousers, subtle light-blue/white checkered band), the word HANDHAVING in white capital letters on the back; on the upper LEFT SLEEVE the official Dutch BOA emblem: a black shield with a light border and the white BOA symbol; no other badges, no police badge, no municipal coat of arms, no weapons drawn. Scene: a Dutch car park; a stopped car; the driver (woman ~50, short grey hair) opens the boot at the request of two enforcement officers; inside a sports bag and a few firework packages; the officers stand at a safe distance, one takes notes; licence plate not readable. Aspect ratio 3:2.
Negative: NOT: the word POLITIE or POLICE on enforcement clothing, American police uniforms, sheriff stars, fantasy badges, the BOA emblem on objects (boxes, laptops, cups, walls, cars, documents), children's-book style, exaggerated cartoon faces, 3D/plastic render, photorealism, gore, explosions near people, anyone holding, opening or dismantling unknown or heavy fireworks, readable brand names, gibberish text, extra fingers, distorted hands
```

### N15 · `onderwerp5_inbeslagneming.webp`

- **Gebruikt op:** O5 p21, O5 p22, O8 p9, O8 p12, oefenvraag O5 v4, oefenvraag O5 v5, oefenvraag O5 v6
- **Doel:** Inbeslagneming van verpakt vuurwerk en kennisgeving.
- **Personages:** H3 Ingrid
- **Scène/handeling:** Handhaver neemt twee gesloten verpakkingen aan van een jongere en vult op een tablet een formulier in; de verpakkingen gaan in een grijze krat.
- **Kleding/embleem:** handhavers volgens §1 (HANDHAVING op de rug, BOA-embleem op de arm)
- **Formaat:** 4:3, 1600 × 1200 px
- **Absoluut niet in beeld:** geen BOA-logo op tablet of krat, geen leesbare tekst
- **Alt-tekst:** Een handhaver neemt verpakt vuurwerk in beslag en maakt een kennisgeving op.
- **Prompt:**

```
Modern professional editorial cartoon illustration, semi-realistic proportions, clean confident line work, soft cel shading, calm adult tone, Dutch setting, colour palette dominated by dark navy blue, mid/light blue, white and silver grey with orange as accent colour, uncluttered background, main subjects in the central 60% of the frame so the image can be cropped for mobile. Dutch municipal enforcement officers (boa's) wear a dark navy Dutch enforcement uniform (jacket and trousers, subtle light-blue/white checkered band), the word HANDHAVING in white capital letters on the back; on the upper LEFT SLEEVE the official Dutch BOA emblem: a black shield with a light border and the white BOA symbol; no other badges, no police badge, no municipal coat of arms, no weapons drawn. Scene: an enforcement officer (woman ~40 blond ponytail) receives two sealed firework packages from a young person and fills in a form on a tablet; the packages go into a grey plastic crate; no logos on the tablet or crate. Aspect ratio 4:3.
Negative: NOT: the word POLITIE or POLICE on enforcement clothing, American police uniforms, sheriff stars, fantasy badges, the BOA emblem on objects (boxes, laptops, cups, walls, cars, documents), children's-book style, exaggerated cartoon faces, 3D/plastic render, photorealism, gore, explosions near people, anyone holding, opening or dismantling unknown or heavy fireworks, readable brand names, gibberish text, extra fingers, distorted hands
```

### N16 · `onderwerp5_proces_verbaal.webp`

- **Gebruikt op:** O5 p25, O8 p13, O8 p14, O8 p15, eindtoets v15
- **Doel:** Proces-verbaal: feitelijk beschrijven.
- **Personages:** H6 Karim
- **Scène/handeling:** Handhaver achter een computer op kantoor; op het scherm alleen de kop “PROCES-VERBAAL” en onleesbare regels. Op tafel notitieblok, uitgeprinte foto van een etiket.
- **Kleding/embleem:** handhavers volgens §1 (HANDHAVING op de rug, BOA-embleem op de arm)
- **Formaat:** 4:3, 1600 × 1200 px
- **Absoluut niet in beeld:** geen BOA-logo op kantoorspullen, geen lange neptekst
- **Alt-tekst:** Een handhaver schrijft achter de computer een proces-verbaal.
- **Prompt:**

```
Modern professional editorial cartoon illustration, semi-realistic proportions, clean confident line work, soft cel shading, calm adult tone, Dutch setting, colour palette dominated by dark navy blue, mid/light blue, white and silver grey with orange as accent colour, uncluttered background, main subjects in the central 60% of the frame so the image can be cropped for mobile. Dutch municipal enforcement officers (boa's) wear a dark navy Dutch enforcement uniform (jacket and trousers, subtle light-blue/white checkered band), the word HANDHAVING in white capital letters on the back; on the upper LEFT SLEEVE the official Dutch BOA emblem: a black shield with a light border and the white BOA symbol; no other badges, no police badge, no municipal coat of arms, no weapons drawn. Scene: an enforcement officer (man ~45, bald, greying beard) at a desk computer in a Dutch office; the screen shows only the heading "PROCES-VERBAAL" and unreadable lines; on the desk a notebook and a printed photo of a firework label. Aspect ratio 4:3.
Negative: NOT: the word POLITIE or POLICE on enforcement clothing, American police uniforms, sheriff stars, fantasy badges, the BOA emblem on objects (boxes, laptops, cups, walls, cars, documents), children's-book style, exaggerated cartoon faces, 3D/plastic render, photorealism, gore, explosions near people, anyone holding, opening or dismantling unknown or heavy fireworks, readable brand names, gibberish text, extra fingers, distorted hands
```

### N17 · `onderwerp5_overdracht_politie.webp`

- **Gebruikt op:** O5 p26, O7 p12, O8 p11
- **Doel:** Samenwerking en overdracht aan de politie.
- **Personages:** H1 Noor (links, HANDHAVING) en een politieagent (rechts, geel-blauw politie-jack met POLITIE)
- **Scène/handeling:** Twee mensen overleggen naast een politiebus op straat; duidelijke verschillen in kleding: links donkerblauw HANDHAVING met BOA-embleem op de arm, rechts Nederlandse politie.
- **Kleding/embleem:** handhavers volgens §1 (HANDHAVING op de rug, BOA-embleem op de arm)
- **Formaat:** 4:3, 1600 × 1200 px
- **Absoluut niet in beeld:** POLITIE alleen op de politieagent, nooit op de handhaver
- **Alt-tekst:** Een handhaver draagt een situatie over aan een politieagent.
- **Prompt:**

```
Modern professional editorial cartoon illustration, semi-realistic proportions, clean confident line work, soft cel shading, calm adult tone, Dutch setting, colour palette dominated by dark navy blue, mid/light blue, white and silver grey with orange as accent colour, uncluttered background, main subjects in the central 60% of the frame so the image can be cropped for mobile. Dutch municipal enforcement officers (boa's) wear a dark navy Dutch enforcement uniform (jacket and trousers, subtle light-blue/white checkered band), the word HANDHAVING in white capital letters on the back; on the upper LEFT SLEEVE the official Dutch BOA emblem: a black shield with a light border and the white BOA symbol; no other badges, no police badge, no municipal coat of arms, no weapons drawn. Scene: on the left an enforcement officer (woman ~30 dark hair low bun, navy uniform with HANDHAVING and BOA shield on sleeve), on the right a Dutch police officer in the yellow and blue police jacket with POLITIE; they consult next to a Dutch police van on the street. Aspect ratio 4:3.
Negative: NOT: the word POLITIE or POLICE on enforcement clothing, American police uniforms, sheriff stars, fantasy badges, the BOA emblem on objects (boxes, laptops, cups, walls, cars, documents), children's-book style, exaggerated cartoon faces, 3D/plastic render, photorealism, gore, explosions near people, anyone holding, opening or dismantling unknown or heavy fireworks, readable brand names, gibberish text, extra fingers, distorted hands
```

### N18 · `onderwerp6_tas_zonder_etiket.webp`

- **Gebruikt op:** O6 p2, O6 p9, O6 p10, oefenvraag O6 v2, oefenvraag O6 v3, eindtoets v14
- **Doel:** Casus: tas met onbekend, mogelijk zelfgemaakt vuurwerk.
- **Personages:** H5 Esther en H4 Tim; omstanders (divers) op afstand
- **Scène/handeling:** Tas op de grond met grote, met tape omwikkelde voorwerpen zonder etiket. Handhavers staan op ruime afstand, één vraagt omstanders met een armgebaar achteruit te gaan, de ander belt.
- **Kleding/embleem:** handhavers volgens §1 (HANDHAVING op de rug, BOA-embleem op de arm)
- **Formaat:** 3:2, 1800 × 1200 px
- **Absoluut niet in beeld:** niemand raakt de tas aan, geen explosie
- **Alt-tekst:** Handhavers houden afstand van een tas met onbekend vuurwerk en houden omstanders weg.
- **Prompt:**

```
Modern professional editorial cartoon illustration, semi-realistic proportions, clean confident line work, soft cel shading, calm adult tone, Dutch setting, colour palette dominated by dark navy blue, mid/light blue, white and silver grey with orange as accent colour, uncluttered background, main subjects in the central 60% of the frame so the image can be cropped for mobile. Dutch municipal enforcement officers (boa's) wear a dark navy Dutch enforcement uniform (jacket and trousers, subtle light-blue/white checkered band), the word HANDHAVING in white capital letters on the back; on the upper LEFT SLEEVE the official Dutch BOA emblem: a black shield with a light border and the white BOA symbol; no other badges, no police badge, no municipal coat of arms, no weapons drawn. Scene: a bag on the ground containing large objects wrapped in tape without labels; two enforcement officers stand well away, one gestures bystanders to step back, the other makes a phone call; nobody touches the bag. Aspect ratio 3:2.
Negative: NOT: the word POLITIE or POLICE on enforcement clothing, American police uniforms, sheriff stars, fantasy badges, the BOA emblem on objects (boxes, laptops, cups, walls, cars, documents), children's-book style, exaggerated cartoon faces, 3D/plastic render, photorealism, gore, explosions near people, anyone holding, opening or dismantling unknown or heavy fireworks, readable brand names, gibberish text, extra fingers, distorted hands
```

### N19 · `onderwerp6_veiligheid_afstand.webp`

- **Gebruikt op:** O6 p1, O6 p6, O6 p8, O8 p10
- **Doel:** Bevoegd is niet hetzelfde als veilig: afstand houden en afzetten.
- **Personages:** H3 Ingrid (van achteren, HANDHAVING leesbaar)
- **Scène/handeling:** Handhaver spant afzetlint “GEVAAR – NIET BETREDEN” tussen twee palen; op de achtergrond onscherp een voorwerp op straat en omstanders achter het lint.
- **Kleding/embleem:** handhavers volgens §1 (HANDHAVING op de rug, BOA-embleem op de arm)
- **Formaat:** 4:3, 1600 × 1200 px
- **Absoluut niet in beeld:** geen andere tekst dan het lint
- **Alt-tekst:** Een handhaver zet een gebied af met lint; omstanders blijven op afstand.
- **Prompt:**

```
Modern professional editorial cartoon illustration, semi-realistic proportions, clean confident line work, soft cel shading, calm adult tone, Dutch setting, colour palette dominated by dark navy blue, mid/light blue, white and silver grey with orange as accent colour, uncluttered background, main subjects in the central 60% of the frame so the image can be cropped for mobile. Dutch municipal enforcement officers (boa's) wear a dark navy Dutch enforcement uniform (jacket and trousers, subtle light-blue/white checkered band), the word HANDHAVING in white capital letters on the back; on the upper LEFT SLEEVE the official Dutch BOA emblem: a black shield with a light border and the white BOA symbol; no other badges, no police badge, no municipal coat of arms, no weapons drawn. Scene: an enforcement officer seen from behind (HANDHAVING readable) stretches barrier tape reading only "GEVAAR - NIET BETREDEN" between two posts; in the soft background an object on the street and bystanders behind the tape. Aspect ratio 4:3.
Negative: NOT: the word POLITIE or POLICE on enforcement clothing, American police uniforms, sheriff stars, fantasy badges, the BOA emblem on objects (boxes, laptops, cups, walls, cars, documents), children's-book style, exaggerated cartoon faces, 3D/plastic render, photorealism, gore, explosions near people, anyone holding, opening or dismantling unknown or heavy fireworks, readable brand names, gibberish text, extra fingers, distorted hands
```

### N20 · `onderwerp6_praktijktermen.webp`

- **Gebruikt op:** O6 p3, O6 p4, oefenvraag O2 v4
- **Doel:** Praktijktermen zijn geen wettelijke categorie.
- **Personages:** geen personen
- **Scène/handeling:** Grijze bewijskrat op een tafel met in beslag genomen zwaar vuurwerk zonder etiket, sommige met tape; een liniaal als schaal; neutrale ruimte.
- **Kleding/embleem:** geen handhavers in beeld
- **Formaat:** 4:3, 1600 × 1200 px
- **Absoluut niet in beeld:** geen merknamen, geen labels met categorie
- **Alt-tekst:** In beslag genomen zwaar vuurwerk zonder etiket in een bewijskrat.
- **Prompt:**

```
Modern professional editorial cartoon illustration, semi-realistic proportions, clean confident line work, soft cel shading, calm adult tone, Dutch setting, colour palette dominated by dark navy blue, mid/light blue, white and silver grey with orange as accent colour, uncluttered background, main subjects in the central 60% of the frame so the image can be cropped for mobile. Scene: a grey evidence crate on a table with seized heavy fireworks without labels, some wrapped in tape; a ruler for scale; neutral institutional room; no people. Aspect ratio 4:3.
Negative: NOT: the word POLITIE or POLICE on enforcement clothing, American police uniforms, sheriff stars, fantasy badges, the BOA emblem on objects (boxes, laptops, cups, walls, cars, documents), children's-book style, exaggerated cartoon faces, 3D/plastic render, photorealism, gore, explosions near people, anyone holding, opening or dismantling unknown or heavy fireworks, readable brand names, gibberish text, extra fingers, distorted hands
```

### N21 · `onderwerp7_briefing_jaarwisseling.webp`

- **Gebruikt op:** O7 p1, O7 p4
- **Doel:** Handhavingsplan en taakverdeling: afspraken vooraf.
- **Personages:** H2 Daan, H5 Esther, H6 Karim en twee politiemensen
- **Scène/handeling:** Briefing in een vergaderruimte voor de jaarwisseling: handhavers en politie rond een tafel met een kaart van de wijk.
- **Kleding/embleem:** handhavers volgens §1 (HANDHAVING op de rug, BOA-embleem op de arm)
- **Formaat:** 4:3, 1600 × 1200 px
- **Absoluut niet in beeld:** geen leesbare tekst op de kaart
- **Alt-tekst:** Handhavers en politie bespreken samen de aanpak voor de jaarwisseling.
- **Prompt:**

```
Modern professional editorial cartoon illustration, semi-realistic proportions, clean confident line work, soft cel shading, calm adult tone, Dutch setting, colour palette dominated by dark navy blue, mid/light blue, white and silver grey with orange as accent colour, uncluttered background, main subjects in the central 60% of the frame so the image can be cropped for mobile. Dutch municipal enforcement officers (boa's) wear a dark navy Dutch enforcement uniform (jacket and trousers, subtle light-blue/white checkered band), the word HANDHAVING in white capital letters on the back; on the upper LEFT SLEEVE the official Dutch BOA emblem: a black shield with a light border and the white BOA symbol; no other badges, no police badge, no municipal coat of arms, no weapons drawn. Scene: a briefing in a meeting room before New Year’s Eve: enforcement officers and two Dutch police officers around a table with a neighbourhood map, calm professional atmosphere; no readable text. Aspect ratio 4:3.
Negative: NOT: the word POLITIE or POLICE on enforcement clothing, American police uniforms, sheriff stars, fantasy badges, the BOA emblem on objects (boxes, laptops, cups, walls, cars, documents), children's-book style, exaggerated cartoon faces, 3D/plastic render, photorealism, gore, explosions near people, anyone holding, opening or dismantling unknown or heavy fireworks, readable brand names, gibberish text, extra fingers, distorted hands
```

### N22 · `onderwerp7_woonstraat_fontein.webp`

- **Gebruikt op:** O7 p9
- **Doel:** Situatie 1: zelf afhandelen.
- **Personages:** H3 Ingrid; bewoner (man, ca. 65, wit haar)
- **Scène/handeling:** Oktoberavond in een Nederlandse woonstraat; een oudere man steekt een kleine fontein af op de stoep; de handhaver komt rustig aanlopen.
- **Kleding/embleem:** handhavers volgens §1 (HANDHAVING op de rug, BOA-embleem op de arm)
- **Formaat:** 4:3, 1600 × 1200 px
- **Absoluut niet in beeld:** geen gevaar, geen agressie
- **Alt-tekst:** Een handhaver loopt op een man af die in een woonstraat een fontein afsteekt.
- **Prompt:**

```
Modern professional editorial cartoon illustration, semi-realistic proportions, clean confident line work, soft cel shading, calm adult tone, Dutch setting, colour palette dominated by dark navy blue, mid/light blue, white and silver grey with orange as accent colour, uncluttered background, main subjects in the central 60% of the frame so the image can be cropped for mobile. Dutch municipal enforcement officers (boa's) wear a dark navy Dutch enforcement uniform (jacket and trousers, subtle light-blue/white checkered band), the word HANDHAVING in white capital letters on the back; on the upper LEFT SLEEVE the official Dutch BOA emblem: a black shield with a light border and the white BOA symbol; no other badges, no police badge, no municipal coat of arms, no weapons drawn. Scene: an October evening in a Dutch residential street; an older man ~65 with white hair lights a small fountain on the pavement; an enforcement officer (woman ~40 blond ponytail) approaches calmly. Aspect ratio 4:3.
Negative: NOT: the word POLITIE or POLICE on enforcement clothing, American police uniforms, sheriff stars, fantasy badges, the BOA emblem on objects (boxes, laptops, cups, walls, cars, documents), children's-book style, exaggerated cartoon faces, 3D/plastic render, photorealism, gore, explosions near people, anyone holding, opening or dismantling unknown or heavy fireworks, readable brand names, gibberish text, extra fingers, distorted hands
```

### N23 · `onderwerp7_park_tas.webp`

- **Gebruikt op:** O7 p10
- **Doel:** Situatie 2: overleggen.
- **Personages:** H1 Noor
- **Scène/handeling:** Park overdag; een tas met vuurwerk ligt op een bankje of in het gras; de handhaver staat op afstand en belt met haar leidinggevende of de politie.
- **Kleding/embleem:** handhavers volgens §1 (HANDHAVING op de rug, BOA-embleem op de arm)
- **Formaat:** 4:3, 1600 × 1200 px
- **Absoluut niet in beeld:** niemand raakt de tas aan
- **Alt-tekst:** Een handhaver belt op afstand van een achtergelaten tas met vuurwerk in een park.
- **Prompt:**

```
Modern professional editorial cartoon illustration, semi-realistic proportions, clean confident line work, soft cel shading, calm adult tone, Dutch setting, colour palette dominated by dark navy blue, mid/light blue, white and silver grey with orange as accent colour, uncluttered background, main subjects in the central 60% of the frame so the image can be cropped for mobile. Dutch municipal enforcement officers (boa's) wear a dark navy Dutch enforcement uniform (jacket and trousers, subtle light-blue/white checkered band), the word HANDHAVING in white capital letters on the back; on the upper LEFT SLEEVE the official Dutch BOA emblem: a black shield with a light border and the white BOA symbol; no other badges, no police badge, no municipal coat of arms, no weapons drawn. Scene: a Dutch park in daylight; a bag with fireworks lies on the grass next to a bench; an enforcement officer (woman ~30 dark hair low bun) stands at a distance and makes a phone call. Aspect ratio 4:3.
Negative: NOT: the word POLITIE or POLICE on enforcement clothing, American police uniforms, sheriff stars, fantasy badges, the BOA emblem on objects (boxes, laptops, cups, walls, cars, documents), children's-book style, exaggerated cartoon faces, 3D/plastic render, photorealism, gore, explosions near people, anyone holding, opening or dismantling unknown or heavy fireworks, readable brand names, gibberish text, extra fingers, distorted hands
```

### N24 · `onderwerp7_station_groep.webp`

- **Gebruikt op:** O7 p11, oefenvraag O7 v3, eindtoets v13
- **Doel:** Situatie 3: politie inschakelen bij zwaar vuurwerk en ordeverstoring.
- **Personages:** H2 Daan en H6 Karim (op afstand); groep jongvolwassenen onherkenbaar
- **Scène/handeling:** Stationsplein ’s avonds; verderop een onrustige groep met groot vuurwerk; de handhavers staan ver weg bij de ingang en melden via de portofoon.
- **Kleding/embleem:** handhavers volgens §1 (HANDHAVING op de rug, BOA-embleem op de arm)
- **Formaat:** 3:2, 1800 × 1200 px
- **Absoluut niet in beeld:** geen geweld, geen herkenbare gezichten in de groep
- **Alt-tekst:** Handhavers melden op afstand een onrustige groep met zwaar vuurwerk bij een station.
- **Prompt:**

```
Modern professional editorial cartoon illustration, semi-realistic proportions, clean confident line work, soft cel shading, calm adult tone, Dutch setting, colour palette dominated by dark navy blue, mid/light blue, white and silver grey with orange as accent colour, uncluttered background, main subjects in the central 60% of the frame so the image can be cropped for mobile. Dutch municipal enforcement officers (boa's) wear a dark navy Dutch enforcement uniform (jacket and trousers, subtle light-blue/white checkered band), the word HANDHAVING in white capital letters on the back; on the upper LEFT SLEEVE the official Dutch BOA emblem: a black shield with a light border and the white BOA symbol; no other badges, no police badge, no municipal coat of arms, no weapons drawn. Scene: a Dutch station square at night; further away a restless group of young adults with large fireworks (faces not recognisable); two enforcement officers stand far away near the entrance and report via radio. Aspect ratio 3:2.
Negative: NOT: the word POLITIE or POLICE on enforcement clothing, American police uniforms, sheriff stars, fantasy badges, the BOA emblem on objects (boxes, laptops, cups, walls, cars, documents), children's-book style, exaggerated cartoon faces, 3D/plastic render, photorealism, gore, explosions near people, anyone holding, opening or dismantling unknown or heavy fireworks, readable brand names, gibberish text, extra fingers, distorted hands
```

### N25 · `onderwerp8_parkeerplaats_casus.webp`

- **Gebruikt op:** O8 p1, O8 p3, O8 p4
- **Doel:** Eindcasus: van melding tot proces-verbaal.
- **Personages:** H4 Tim en H5 Esther; vier jongeren (andere personen dan N01)
- **Scène/handeling:** 22 november, 21.00 uur; parkeerplaats met lantaarns; vier jongeren, één met een verpakking in de hand, een tas op de grond; de handhavers komen aanlopen.
- **Kleding/embleem:** handhavers volgens §1 (HANDHAVING op de rug, BOA-embleem op de arm)
- **Formaat:** 3:2, 1800 × 1200 px
- **Absoluut niet in beeld:** geen ontstoken vuurwerk vlak bij mensen
- **Alt-tekst:** Twee handhavers lopen op een parkeerplaats naar vier jongeren met een tas vuurwerk.
- **Prompt:**

```
Modern professional editorial cartoon illustration, semi-realistic proportions, clean confident line work, soft cel shading, calm adult tone, Dutch setting, colour palette dominated by dark navy blue, mid/light blue, white and silver grey with orange as accent colour, uncluttered background, main subjects in the central 60% of the frame so the image can be cropped for mobile. Dutch municipal enforcement officers (boa's) wear a dark navy Dutch enforcement uniform (jacket and trousers, subtle light-blue/white checkered band), the word HANDHAVING in white capital letters on the back; on the upper LEFT SLEEVE the official Dutch BOA emblem: a black shield with a light border and the white BOA symbol; no other badges, no police badge, no municipal coat of arms, no weapons drawn. Scene: a Dutch car park at 9 pm in November under street lights; four young people (different from earlier scenes), one holds a firework package, a bag on the ground; two enforcement officers (man ~28 light brown hair, woman ~35 dark skin short curly hair) walk towards them. Aspect ratio 3:2.
Negative: NOT: the word POLITIE or POLICE on enforcement clothing, American police uniforms, sheriff stars, fantasy badges, the BOA emblem on objects (boxes, laptops, cups, walls, cars, documents), children's-book style, exaggerated cartoon faces, 3D/plastic render, photorealism, gore, explosions near people, anyone holding, opening or dismantling unknown or heavy fireworks, readable brand names, gibberish text, extra fingers, distorted hands
```

### N26 · `afsluiting_veilige_jaarwisseling.webp`

- **Gebruikt op:** O8 p24
- **Doel:** Afsluiting: klaar voor de eindtoets / samen voor een veilige jaarwisseling.
- **Personages:** H1–H6 samen
- **Scène/handeling:** Nederlandse stad tijdens de jaarwisseling; vuurwerk ver weg boven de skyline; publiek op veilige afstand; zes handhavers als team zichtbaar aanwezig, rustig en positief.
- **Kleding/embleem:** handhavers volgens §1 (HANDHAVING op de rug, BOA-embleem op de arm)
- **Formaat:** 16:9, 1920 × 1080 px (brede kop) én 4:3 uitsnede
- **Absoluut niet in beeld:** geen chaos, geen oorlogssfeer
- **Alt-tekst:** Handhavers als team in een Nederlandse stad tijdens de jaarwisseling, met vuurwerk in de verte.
- **Prompt:**

```
Modern professional editorial cartoon illustration, semi-realistic proportions, clean confident line work, soft cel shading, calm adult tone, Dutch setting, colour palette dominated by dark navy blue, mid/light blue, white and silver grey with orange as accent colour, uncluttered background, main subjects in the central 60% of the frame so the image can be cropped for mobile. Dutch municipal enforcement officers (boa's) wear a dark navy Dutch enforcement uniform (jacket and trousers, subtle light-blue/white checkered band), the word HANDHAVING in white capital letters on the back; on the upper LEFT SLEEVE the official Dutch BOA emblem: a black shield with a light border and the white BOA symbol; no other badges, no police badge, no municipal coat of arms, no weapons drawn. Scene: a Dutch city centre on New Year’s Eve; fireworks far away above the skyline; public at a safe distance; six diverse enforcement officers visible as a calm, positive team; professional and safe atmosphere. Aspect ratio 16:9.
Negative: NOT: the word POLITIE or POLICE on enforcement clothing, American police uniforms, sheriff stars, fantasy badges, the BOA emblem on objects (boxes, laptops, cups, walls, cars, documents), children's-book style, exaggerated cartoon faces, 3D/plastic render, photorealism, gore, explosions near people, anyone holding, opening or dismantling unknown or heavy fireworks, readable brand names, gibberish text, extra fingers, distorted hands
```

### N-F1 · `onderwerp2_categorie_f1.webp`

- **Gebruikt op:** O1 p5, O2 p2, O2 p3
- **Doel:** Categoriekaart F1 in een identieke serie van vier (vergelijken).
- **Personages:** geen personen
- **Scène/handeling:** Kaart met groene kopbalk, groot label “F1”, eronder enkele passende productillustraties zonder merknaam. Geen verdere tekst in het beeld; de omschrijving (“zeer weinig gevaar”) zet de website er in HTML onder.
- **Kleding/embleem:** geen handhavers in beeld
- **Formaat:** 4:3, 1600 × 1200 px; vier kaarten exact dezelfde opbouw
- **Absoluut niet in beeld:** geen absolute juridische teksten, geen merknamen, geen extra woorden
- **Alt-tekst:** Categoriekaart F1 met voorbeelden van vuurwerk.
- **Prompt:**

```
Modern professional editorial cartoon illustration, semi-realistic proportions, clean confident line work, soft cel shading, calm adult tone, Dutch setting, colour palette dominated by dark navy blue, mid/light blue, white and silver grey with orange as accent colour, uncluttered background, main subjects in the central 60% of the frame so the image can be cropped for mobile. Scene: a clean flat category card on a light background with a green header bar showing only the large label "F1", below it neat illustrations of sparklers, snap pops (knalerwten) and a tiny indoor fountain, no brand names, no other text; identical layout for all four cards in the series. Aspect ratio 4:3.
Negative: NOT: the word POLITIE or POLICE on enforcement clothing, American police uniforms, sheriff stars, fantasy badges, the BOA emblem on objects (boxes, laptops, cups, walls, cars, documents), children's-book style, exaggerated cartoon faces, 3D/plastic render, photorealism, gore, explosions near people, anyone holding, opening or dismantling unknown or heavy fireworks, readable brand names, gibberish text, extra fingers, distorted hands
```

### N-F2 · `onderwerp2_categorie_f2.webp`

- **Gebruikt op:** O1 p5, O2 p1, O2 p2, O2 p3
- **Doel:** Categoriekaart F2 in een identieke serie van vier (vergelijken).
- **Personages:** geen personen
- **Scène/handeling:** Kaart met gele kopbalk, groot label “F2”, eronder enkele passende productillustraties zonder merknaam. Geen verdere tekst in het beeld; de omschrijving (“weinig gevaar”) zet de website er in HTML onder.
- **Kleding/embleem:** geen handhavers in beeld
- **Formaat:** 4:3, 1600 × 1200 px; vier kaarten exact dezelfde opbouw
- **Absoluut niet in beeld:** geen absolute juridische teksten, geen merknamen, geen extra woorden
- **Alt-tekst:** Categoriekaart F2 met voorbeelden van vuurwerk.
- **Prompt:**

```
Modern professional editorial cartoon illustration, semi-realistic proportions, clean confident line work, soft cel shading, calm adult tone, Dutch setting, colour palette dominated by dark navy blue, mid/light blue, white and silver grey with orange as accent colour, uncluttered background, main subjects in the central 60% of the frame so the image can be cropped for mobile. Scene: a clean flat category card on a light background with a yellow header bar showing only the large label "F2", below it neat illustrations of a small ground fountain, a small cake box and a compound box, no brand names, no other text; identical layout for all four cards in the series. Aspect ratio 4:3.
Negative: NOT: the word POLITIE or POLICE on enforcement clothing, American police uniforms, sheriff stars, fantasy badges, the BOA emblem on objects (boxes, laptops, cups, walls, cars, documents), children's-book style, exaggerated cartoon faces, 3D/plastic render, photorealism, gore, explosions near people, anyone holding, opening or dismantling unknown or heavy fireworks, readable brand names, gibberish text, extra fingers, distorted hands
```

### N-F3 · `onderwerp2_categorie_f3.webp`

- **Gebruikt op:** O1 p5, O2 p2, O2 p3
- **Doel:** Categoriekaart F3 in een identieke serie van vier (vergelijken).
- **Personages:** geen personen
- **Scène/handeling:** Kaart met oranje kopbalk, groot label “F3”, eronder enkele passende productillustraties zonder merknaam. Geen verdere tekst in het beeld; de omschrijving (“middelmatig gevaar”) zet de website er in HTML onder.
- **Kleding/embleem:** geen handhavers in beeld
- **Formaat:** 4:3, 1600 × 1200 px; vier kaarten exact dezelfde opbouw
- **Absoluut niet in beeld:** geen absolute juridische teksten, geen merknamen, geen extra woorden
- **Alt-tekst:** Categoriekaart F3 met voorbeelden van vuurwerk.
- **Prompt:**

```
Modern professional editorial cartoon illustration, semi-realistic proportions, clean confident line work, soft cel shading, calm adult tone, Dutch setting, colour palette dominated by dark navy blue, mid/light blue, white and silver grey with orange as accent colour, uncluttered background, main subjects in the central 60% of the frame so the image can be cropped for mobile. Scene: a clean flat category card on a light background with a orange header bar showing only the large label "F3", below it neat illustrations of a large cake box, a rocket set and a battery, no brand names, no other text; identical layout for all four cards in the series. Aspect ratio 4:3.
Negative: NOT: the word POLITIE or POLICE on enforcement clothing, American police uniforms, sheriff stars, fantasy badges, the BOA emblem on objects (boxes, laptops, cups, walls, cars, documents), children's-book style, exaggerated cartoon faces, 3D/plastic render, photorealism, gore, explosions near people, anyone holding, opening or dismantling unknown or heavy fireworks, readable brand names, gibberish text, extra fingers, distorted hands
```

### N-F4 · `onderwerp2_categorie_f4.webp`

- **Gebruikt op:** O1 p5, O2 p2, O2 p3
- **Doel:** Categoriekaart F4 in een identieke serie van vier (vergelijken).
- **Personages:** geen personen
- **Scène/handeling:** Kaart met rode kopbalk, groot label “F4”, eronder enkele passende productillustraties zonder merknaam. Geen verdere tekst in het beeld; de omschrijving (“veel gevaar, alleen voor vakmensen”) zet de website er in HTML onder.
- **Kleding/embleem:** geen handhavers in beeld
- **Formaat:** 4:3, 1600 × 1200 px; vier kaarten exact dezelfde opbouw
- **Absoluut niet in beeld:** geen absolute juridische teksten, geen merknamen, geen extra woorden
- **Alt-tekst:** Categoriekaart F4 met voorbeelden van vuurwerk.
- **Prompt:**

```
Modern professional editorial cartoon illustration, semi-realistic proportions, clean confident line work, soft cel shading, calm adult tone, Dutch setting, colour palette dominated by dark navy blue, mid/light blue, white and silver grey with orange as accent colour, uncluttered background, main subjects in the central 60% of the frame so the image can be cropped for mobile. Scene: a clean flat category card on a light background with a red header bar showing only the large label "F4", below it neat illustrations of professional display shells in sealed transport boxes with a class 1.3G hazard label, no brand names, no other text; identical layout for all four cards in the series. Aspect ratio 4:3.
Negative: NOT: the word POLITIE or POLICE on enforcement clothing, American police uniforms, sheriff stars, fantasy badges, the BOA emblem on objects (boxes, laptops, cups, walls, cars, documents), children's-book style, exaggerated cartoon faces, 3D/plastic render, photorealism, gore, explosions near people, anyone holding, opening or dismantling unknown or heavy fireworks, readable brand names, gibberish text, extra fingers, distorted hands
```

### P-F1a · `onderwerp2_product_f1_sterretjes.webp`

- **Gebruikt op:** O2 p4
- **Doel:** Productvoorbeeld op categoriepagina: sterretjes in verpakking.
- **Personages:** geen personen
- **Scène/handeling:** Losse productillustratie: sterretjes in verpakking. Neutrale lichte achtergrond, zelfde lichtval voor de hele serie.
- **Kleding/embleem:** geen handhavers in beeld
- **Formaat:** 3:4, 900 × 1200 px (portret, past in de fotokaders van 200 × 300)
- **Absoluut niet in beeld:** geen merknamen, geen onzintekst, niemand die het vuurwerk vasthoudt
- **Alt-tekst:** Voorbeeld: sterretjes in verpakking.
- **Prompt:**

```
Modern professional editorial cartoon illustration, semi-realistic proportions, clean confident line work, soft cel shading, calm adult tone, Dutch setting, colour palette dominated by dark navy blue, mid/light blue, white and silver grey with orange as accent colour, uncluttered background, main subjects in the central 60% of the frame so the image can be cropped for mobile. Scene: a packet of sparklers in plain retail packaging, centred on a light neutral background, product illustration, same lighting as the rest of the series. Aspect ratio 3:4.
Negative: NOT: the word POLITIE or POLICE on enforcement clothing, American police uniforms, sheriff stars, fantasy badges, the BOA emblem on objects (boxes, laptops, cups, walls, cars, documents), children's-book style, exaggerated cartoon faces, 3D/plastic render, photorealism, gore, explosions near people, anyone holding, opening or dismantling unknown or heavy fireworks, readable brand names, gibberish text, extra fingers, distorted hands
```

### P-F1b · `onderwerp2_product_f1_knalerwten.webp`

- **Gebruikt op:** O2 p4
- **Doel:** Productvoorbeeld op categoriepagina: knalerwten in doosje.
- **Personages:** geen personen
- **Scène/handeling:** Losse productillustratie: knalerwten in doosje. Neutrale lichte achtergrond, zelfde lichtval voor de hele serie.
- **Kleding/embleem:** geen handhavers in beeld
- **Formaat:** 3:4, 900 × 1200 px (portret, past in de fotokaders van 200 × 300)
- **Absoluut niet in beeld:** geen merknamen, geen onzintekst, niemand die het vuurwerk vasthoudt
- **Alt-tekst:** Voorbeeld: knalerwten in doosje.
- **Prompt:**

```
Modern professional editorial cartoon illustration, semi-realistic proportions, clean confident line work, soft cel shading, calm adult tone, Dutch setting, colour palette dominated by dark navy blue, mid/light blue, white and silver grey with orange as accent colour, uncluttered background, main subjects in the central 60% of the frame so the image can be cropped for mobile. Scene: a small box of snap pops (knalerwten) with a few loose ones, centred on a light neutral background, product illustration, same lighting as the rest of the series. Aspect ratio 3:4.
Negative: NOT: the word POLITIE or POLICE on enforcement clothing, American police uniforms, sheriff stars, fantasy badges, the BOA emblem on objects (boxes, laptops, cups, walls, cars, documents), children's-book style, exaggerated cartoon faces, 3D/plastic render, photorealism, gore, explosions near people, anyone holding, opening or dismantling unknown or heavy fireworks, readable brand names, gibberish text, extra fingers, distorted hands
```

### P-F1c · `onderwerp2_product_f1_fonteintje.webp`

- **Gebruikt op:** O2 p4
- **Doel:** Productvoorbeeld op categoriepagina: klein fonteintje.
- **Personages:** geen personen
- **Scène/handeling:** Losse productillustratie: klein fonteintje. Neutrale lichte achtergrond, zelfde lichtval voor de hele serie.
- **Kleding/embleem:** geen handhavers in beeld
- **Formaat:** 3:4, 900 × 1200 px (portret, past in de fotokaders van 200 × 300)
- **Absoluut niet in beeld:** geen merknamen, geen onzintekst, niemand die het vuurwerk vasthoudt
- **Alt-tekst:** Voorbeeld: klein fonteintje.
- **Prompt:**

```
Modern professional editorial cartoon illustration, semi-realistic proportions, clean confident line work, soft cel shading, calm adult tone, Dutch setting, colour palette dominated by dark navy blue, mid/light blue, white and silver grey with orange as accent colour, uncluttered background, main subjects in the central 60% of the frame so the image can be cropped for mobile. Scene: a tiny indoor cone fountain, centred on a light neutral background, product illustration, same lighting as the rest of the series. Aspect ratio 3:4.
Negative: NOT: the word POLITIE or POLICE on enforcement clothing, American police uniforms, sheriff stars, fantasy badges, the BOA emblem on objects (boxes, laptops, cups, walls, cars, documents), children's-book style, exaggerated cartoon faces, 3D/plastic render, photorealism, gore, explosions near people, anyone holding, opening or dismantling unknown or heavy fireworks, readable brand names, gibberish text, extra fingers, distorted hands
```

### P-F2a · `onderwerp2_product_f2_fontein.webp`

- **Gebruikt op:** O2 p5
- **Doel:** Productvoorbeeld op categoriepagina: grondfontein met etiket “F2”.
- **Personages:** geen personen
- **Scène/handeling:** Losse productillustratie: grondfontein met etiket “F2”. Neutrale lichte achtergrond, zelfde lichtval voor de hele serie.
- **Kleding/embleem:** geen handhavers in beeld
- **Formaat:** 3:4, 900 × 1200 px (portret, past in de fotokaders van 200 × 300)
- **Absoluut niet in beeld:** geen merknamen, geen onzintekst, niemand die het vuurwerk vasthoudt
- **Alt-tekst:** Voorbeeld: grondfontein met etiket “F2”.
- **Prompt:**

```
Modern professional editorial cartoon illustration, semi-realistic proportions, clean confident line work, soft cel shading, calm adult tone, Dutch setting, colour palette dominated by dark navy blue, mid/light blue, white and silver grey with orange as accent colour, uncluttered background, main subjects in the central 60% of the frame so the image can be cropped for mobile. Scene: a ground fountain with a small label that reads only "F2", centred on a light neutral background, product illustration, same lighting as the rest of the series. Aspect ratio 3:4.
Negative: NOT: the word POLITIE or POLICE on enforcement clothing, American police uniforms, sheriff stars, fantasy badges, the BOA emblem on objects (boxes, laptops, cups, walls, cars, documents), children's-book style, exaggerated cartoon faces, 3D/plastic render, photorealism, gore, explosions near people, anyone holding, opening or dismantling unknown or heavy fireworks, readable brand names, gibberish text, extra fingers, distorted hands
```

### P-F2b · `onderwerp2_product_f2_cake.webp`

- **Gebruikt op:** O2 p5
- **Doel:** Productvoorbeeld op categoriepagina: kleine cake met etiket “F2”.
- **Personages:** geen personen
- **Scène/handeling:** Losse productillustratie: kleine cake met etiket “F2”. Neutrale lichte achtergrond, zelfde lichtval voor de hele serie.
- **Kleding/embleem:** geen handhavers in beeld
- **Formaat:** 3:4, 900 × 1200 px (portret, past in de fotokaders van 200 × 300)
- **Absoluut niet in beeld:** geen merknamen, geen onzintekst, niemand die het vuurwerk vasthoudt
- **Alt-tekst:** Voorbeeld: kleine cake met etiket “F2”.
- **Prompt:**

```
Modern professional editorial cartoon illustration, semi-realistic proportions, clean confident line work, soft cel shading, calm adult tone, Dutch setting, colour palette dominated by dark navy blue, mid/light blue, white and silver grey with orange as accent colour, uncluttered background, main subjects in the central 60% of the frame so the image can be cropped for mobile. Scene: a small firework cake box with a label that reads only "F2", centred on a light neutral background, product illustration, same lighting as the rest of the series. Aspect ratio 3:4.
Negative: NOT: the word POLITIE or POLICE on enforcement clothing, American police uniforms, sheriff stars, fantasy badges, the BOA emblem on objects (boxes, laptops, cups, walls, cars, documents), children's-book style, exaggerated cartoon faces, 3D/plastic render, photorealism, gore, explosions near people, anyone holding, opening or dismantling unknown or heavy fireworks, readable brand names, gibberish text, extra fingers, distorted hands
```

### P-F2c · `onderwerp2_product_f2_compound.webp`

- **Gebruikt op:** O2 p5
- **Doel:** Productvoorbeeld op categoriepagina: compoundbox met etiket “F2”.
- **Personages:** geen personen
- **Scène/handeling:** Losse productillustratie: compoundbox met etiket “F2”. Neutrale lichte achtergrond, zelfde lichtval voor de hele serie.
- **Kleding/embleem:** geen handhavers in beeld
- **Formaat:** 3:4, 900 × 1200 px (portret, past in de fotokaders van 200 × 300)
- **Absoluut niet in beeld:** geen merknamen, geen onzintekst, niemand die het vuurwerk vasthoudt
- **Alt-tekst:** Voorbeeld: compoundbox met etiket “F2”.
- **Prompt:**

```
Modern professional editorial cartoon illustration, semi-realistic proportions, clean confident line work, soft cel shading, calm adult tone, Dutch setting, colour palette dominated by dark navy blue, mid/light blue, white and silver grey with orange as accent colour, uncluttered background, main subjects in the central 60% of the frame so the image can be cropped for mobile. Scene: a compound firework box with a label that reads only "F2", centred on a light neutral background, product illustration, same lighting as the rest of the series. Aspect ratio 3:4.
Negative: NOT: the word POLITIE or POLICE on enforcement clothing, American police uniforms, sheriff stars, fantasy badges, the BOA emblem on objects (boxes, laptops, cups, walls, cars, documents), children's-book style, exaggerated cartoon faces, 3D/plastic render, photorealism, gore, explosions near people, anyone holding, opening or dismantling unknown or heavy fireworks, readable brand names, gibberish text, extra fingers, distorted hands
```

### P-F3a · `onderwerp2_product_f3_cake.webp`

- **Gebruikt op:** O2 p6
- **Doel:** Productvoorbeeld op categoriepagina: grote cake met etiket “F3”.
- **Personages:** geen personen
- **Scène/handeling:** Losse productillustratie: grote cake met etiket “F3”. Neutrale lichte achtergrond, zelfde lichtval voor de hele serie.
- **Kleding/embleem:** geen handhavers in beeld
- **Formaat:** 3:4, 900 × 1200 px (portret, past in de fotokaders van 200 × 300)
- **Absoluut niet in beeld:** geen merknamen, geen onzintekst, niemand die het vuurwerk vasthoudt
- **Alt-tekst:** Voorbeeld: grote cake met etiket “F3”.
- **Prompt:**

```
Modern professional editorial cartoon illustration, semi-realistic proportions, clean confident line work, soft cel shading, calm adult tone, Dutch setting, colour palette dominated by dark navy blue, mid/light blue, white and silver grey with orange as accent colour, uncluttered background, main subjects in the central 60% of the frame so the image can be cropped for mobile. Scene: a large firework cake with a label that reads only "F3", centred on a light neutral background, product illustration, same lighting as the rest of the series. Aspect ratio 3:4.
Negative: NOT: the word POLITIE or POLICE on enforcement clothing, American police uniforms, sheriff stars, fantasy badges, the BOA emblem on objects (boxes, laptops, cups, walls, cars, documents), children's-book style, exaggerated cartoon faces, 3D/plastic render, photorealism, gore, explosions near people, anyone holding, opening or dismantling unknown or heavy fireworks, readable brand names, gibberish text, extra fingers, distorted hands
```

### P-F3b · `onderwerp2_product_f3_vuurpijlen.webp`

- **Gebruikt op:** O2 p6
- **Doel:** Productvoorbeeld op categoriepagina: set vuurpijlen met etiket “F3”.
- **Personages:** geen personen
- **Scène/handeling:** Losse productillustratie: set vuurpijlen met etiket “F3”. Neutrale lichte achtergrond, zelfde lichtval voor de hele serie.
- **Kleding/embleem:** geen handhavers in beeld
- **Formaat:** 3:4, 900 × 1200 px (portret, past in de fotokaders van 200 × 300)
- **Absoluut niet in beeld:** geen merknamen, geen onzintekst, niemand die het vuurwerk vasthoudt
- **Alt-tekst:** Voorbeeld: set vuurpijlen met etiket “F3”.
- **Prompt:**

```
Modern professional editorial cartoon illustration, semi-realistic proportions, clean confident line work, soft cel shading, calm adult tone, Dutch setting, colour palette dominated by dark navy blue, mid/light blue, white and silver grey with orange as accent colour, uncluttered background, main subjects in the central 60% of the frame so the image can be cropped for mobile. Scene: a set of rockets on sticks with a label that reads only "F3", centred on a light neutral background, product illustration, same lighting as the rest of the series. Aspect ratio 3:4.
Negative: NOT: the word POLITIE or POLICE on enforcement clothing, American police uniforms, sheriff stars, fantasy badges, the BOA emblem on objects (boxes, laptops, cups, walls, cars, documents), children's-book style, exaggerated cartoon faces, 3D/plastic render, photorealism, gore, explosions near people, anyone holding, opening or dismantling unknown or heavy fireworks, readable brand names, gibberish text, extra fingers, distorted hands
```

### P-F3c · `onderwerp2_product_f3_batterij.webp`

- **Gebruikt op:** O2 p6
- **Doel:** Productvoorbeeld op categoriepagina: batterij met etiket “F3”.
- **Personages:** geen personen
- **Scène/handeling:** Losse productillustratie: batterij met etiket “F3”. Neutrale lichte achtergrond, zelfde lichtval voor de hele serie.
- **Kleding/embleem:** geen handhavers in beeld
- **Formaat:** 3:4, 900 × 1200 px (portret, past in de fotokaders van 200 × 300)
- **Absoluut niet in beeld:** geen merknamen, geen onzintekst, niemand die het vuurwerk vasthoudt
- **Alt-tekst:** Voorbeeld: batterij met etiket “F3”.
- **Prompt:**

```
Modern professional editorial cartoon illustration, semi-realistic proportions, clean confident line work, soft cel shading, calm adult tone, Dutch setting, colour palette dominated by dark navy blue, mid/light blue, white and silver grey with orange as accent colour, uncluttered background, main subjects in the central 60% of the frame so the image can be cropped for mobile. Scene: a firework battery with a label that reads only "F3", centred on a light neutral background, product illustration, same lighting as the rest of the series. Aspect ratio 3:4.
Negative: NOT: the word POLITIE or POLICE on enforcement clothing, American police uniforms, sheriff stars, fantasy badges, the BOA emblem on objects (boxes, laptops, cups, walls, cars, documents), children's-book style, exaggerated cartoon faces, 3D/plastic render, photorealism, gore, explosions near people, anyone holding, opening or dismantling unknown or heavy fireworks, readable brand names, gibberish text, extra fingers, distorted hands
```

### P-Z1 · `onderwerp2_zwaar_cobra.webp`

- **Gebruikt op:** O2 p7
- **Doel:** Productvoorbeeld op categoriepagina: zwaar knalvuurwerk (praktijknaam “Cobra”), zonder merknaam.
- **Personages:** geen personen
- **Scène/handeling:** Losse productillustratie: zwaar knalvuurwerk (praktijknaam “Cobra”), zonder merknaam. Neutrale lichte achtergrond, zelfde lichtval voor de hele serie.
- **Kleding/embleem:** geen handhavers in beeld
- **Formaat:** 3:4, 900 × 1200 px (portret, past in de fotokaders van 200 × 300)
- **Absoluut niet in beeld:** geen merknamen, geen onzintekst, niemand die het vuurwerk vasthoudt
- **Alt-tekst:** Voorbeeld: zwaar knalvuurwerk (praktijknaam “Cobra”), zonder merknaam.
- **Prompt:**

```
Modern professional editorial cartoon illustration, semi-realistic proportions, clean confident line work, soft cel shading, calm adult tone, Dutch setting, colour palette dominated by dark navy blue, mid/light blue, white and silver grey with orange as accent colour, uncluttered background, main subjects in the central 60% of the frame so the image can be cropped for mobile. Scene: a heavy cylindrical banger in plain cardboard with a fuse, no brand name, no label, centred on a light neutral background, product illustration, same lighting as the rest of the series. Aspect ratio 3:4.
Negative: NOT: the word POLITIE or POLICE on enforcement clothing, American police uniforms, sheriff stars, fantasy badges, the BOA emblem on objects (boxes, laptops, cups, walls, cars, documents), children's-book style, exaggerated cartoon faces, 3D/plastic render, photorealism, gore, explosions near people, anyone holding, opening or dismantling unknown or heavy fireworks, readable brand names, gibberish text, extra fingers, distorted hands
```

### P-Z2 · `onderwerp2_zwaar_nitraat.webp`

- **Gebruikt op:** O2 p7
- **Doel:** Productvoorbeeld op categoriepagina: kartonnen hulzen (praktijknaam “nitraat”).
- **Personages:** geen personen
- **Scène/handeling:** Losse productillustratie: kartonnen hulzen (praktijknaam “nitraat”). Neutrale lichte achtergrond, zelfde lichtval voor de hele serie.
- **Kleding/embleem:** geen handhavers in beeld
- **Formaat:** 3:4, 900 × 1200 px (portret, past in de fotokaders van 200 × 300)
- **Absoluut niet in beeld:** geen merknamen, geen onzintekst, niemand die het vuurwerk vasthoudt
- **Alt-tekst:** Voorbeeld: kartonnen hulzen (praktijknaam “nitraat”).
- **Prompt:**

```
Modern professional editorial cartoon illustration, semi-realistic proportions, clean confident line work, soft cel shading, calm adult tone, Dutch setting, colour palette dominated by dark navy blue, mid/light blue, white and silver grey with orange as accent colour, uncluttered background, main subjects in the central 60% of the frame so the image can be cropped for mobile. Scene: three plain cardboard tubes of heavy illegal bangers, no text, centred on a light neutral background, product illustration, same lighting as the rest of the series. Aspect ratio 3:4.
Negative: NOT: the word POLITIE or POLICE on enforcement clothing, American police uniforms, sheriff stars, fantasy badges, the BOA emblem on objects (boxes, laptops, cups, walls, cars, documents), children's-book style, exaggerated cartoon faces, 3D/plastic render, photorealism, gore, explosions near people, anyone holding, opening or dismantling unknown or heavy fireworks, readable brand names, gibberish text, extra fingers, distorted hands
```

### P-Z3 · `onderwerp2_zwaar_mortier.webp`

- **Gebruikt op:** O2 p7
- **Doel:** Productvoorbeeld op categoriepagina: mortierbom/shell zonder etiket.
- **Personages:** geen personen
- **Scène/handeling:** Losse productillustratie: mortierbom/shell zonder etiket. Neutrale lichte achtergrond, zelfde lichtval voor de hele serie.
- **Kleding/embleem:** geen handhavers in beeld
- **Formaat:** 3:4, 900 × 1200 px (portret, past in de fotokaders van 200 × 300)
- **Absoluut niet in beeld:** geen merknamen, geen onzintekst, niemand die het vuurwerk vasthoudt
- **Alt-tekst:** Voorbeeld: mortierbom/shell zonder etiket.
- **Prompt:**

```
Modern professional editorial cartoon illustration, semi-realistic proportions, clean confident line work, soft cel shading, calm adult tone, Dutch setting, colour palette dominated by dark navy blue, mid/light blue, white and silver grey with orange as accent colour, uncluttered background, main subjects in the central 60% of the frame so the image can be cropped for mobile. Scene: a spherical display shell without any label lying on a surface, centred on a light neutral background, product illustration, same lighting as the rest of the series. Aspect ratio 3:4.
Negative: NOT: the word POLITIE or POLICE on enforcement clothing, American police uniforms, sheriff stars, fantasy badges, the BOA emblem on objects (boxes, laptops, cups, walls, cars, documents), children's-book style, exaggerated cartoon faces, 3D/plastic render, photorealism, gore, explosions near people, anyone holding, opening or dismantling unknown or heavy fireworks, readable brand names, gibberish text, extra fingers, distorted hands
```

## 5. Bestaande beelden: beoordeling

| Bestand | Waar | Beoordeling |
|---|---|---|
| `images/plein-knal.webp` | O1 p2 | Goede praktijkscène, maar realistische foto met geel hesje; past niet bij de nieuwe cartoonstijl. Blijft tot N01 er is. |
| `images/boa-jongeren-plein.webp` | O1 p4 | Idem; vervangen door N02. |
| `images/cat-*.webp` (12) | O2 p4–p7 | Uitsneden van 200 × 300 px uit een voorbeelddia: te laag voor HiDPI; deels onzintekst (“66 SHOTE”) en een echte productnaam. Vervangen door P-F1a … P-Z3. |
| `images/concl-*.webp` (6) | O1 p5 | `concl-f2` (losse knalstaven) en `concl-f4` (vuurpijlen) suggereren een categorie die het beeld niet aantoont. Vervangen door categoriekaarten/productillustraties. |
| `images/wet-*.webp` (4) | O2 p3 | `wet-f2` toont losse knalstaven als F2-voorbeeld: kan misleiden. Vervangen door N-F1 … N-F4. |
| `illustraties/boa-*.webp` | sjablonen, toets, resultaat | Gedeeld met de master (Straatintimidatie2). Borstlabel “BOA” en embleem wijken af van de nieuwe Vuurwerk-regel (HANDHAVING op de rug, embleem op de arm). Niet gewijzigd, omdat de master niet mag veranderen; optioneel later een eigen Vuurwerk-set. |
| `illustraties/*.svg` (wetboek, weegschaal, doelwit, vraag) | pictogrammen | Functioneel en neutraal; blijven waar “GEEN BEELD NODIG” of “BEHOUDEN” staat. |
