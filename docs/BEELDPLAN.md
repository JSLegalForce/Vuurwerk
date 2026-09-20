# Beeldplan e-learning Vuurwerk

Versie 0.9 · peildatum 20 september 2026. Dit document hoort bij de oplevering; zie ook `OPLEVERING.md`.

## 1. Stijl en regels voor alle nieuwe beelden

- Realistische professionele fotografie in Nederland; geen cartoon, strip of 3D; geen Amerikaanse uniformen of omgeving.
- Boa’s: donkerblauw Nederlands handhavingsuniform, **nooit “POLITIE” op boa-kleding**, zichtbare tekst minimaal. Boa en politie visueel duidelijk verschillend.
- Geen onveilig gedrag: niemand houdt onbekend/zwaar vuurwerk vast, niemand opent of demonteert vuurwerk, boa’s staan op afstand.
- Beeld suggereert juridisch niet meer dan zichtbaar is: alleen een categorie tonen als die leesbaar op een (fictief) etiket staat.
- Formaat: 16:9, minimaal 3000 × 1688 px, export als WebP (kwaliteit ±80). Bestandsnaam = kolom “Bestand” zonder `scene-`, in `assets/images/`. Activeren: zet de scene-naam in `FOTO_AANWEZIG` (bouwscript `beelden.py`) en bouw opnieuw; dan vervangt de foto het tijdelijke pictogrambeeld. Pas de alt-tekst aan als de foto afwijkt van de beschrijving.
- Basisstijl voor elke prompt: Documentary-style professional photograph, the Netherlands, natural light, realistic skin texture, calm and serious mood, 35mm lens, shallow depth of field, no text or logos except where specified, no cartoon, no 3D, no AI-plastic faces, no American police uniforms or badges, 16:9, 3000x1688 px.

## 2. Personages (variatie en consistentie)

| Code | Casus | Personage(s) |
|---|---|---|
| A | Casus plein (onderwerp 1–5) | Boa Sanne: vrouw, ca. 30, blond haar in staart, lichte huid |
| B | Casus parkeerplaats (onderwerp 8) | Boa Mehmet: man, ca. 40, kort donker haar en baard, getinte huid |
| C | Casus auto/kofferbak (onderwerp 5) | Boa Daan: man, ca. 26, kort blond haar, lichte huid; bestuurder: vrouw, ca. 50, grijs kort haar |
| D | Casus staande houden (onderwerp 5) | Boa Ricardo: man, ca. 35, zwart kort haar, donkere huid; jongere: ca. 17, rossig haar, capuchon |
| E | Overdracht aan politie (onderwerp 5, 7, 8) | Boa Eva: vrouw, ca. 52, grijzend donker haar in knot, lichte huid; twee politiemensen |
| F | Ontheffing sportveld (onderwerp 3) | Boa Noah: man, ca. 24, krullend donkerbruin haar, lichtbruine huid; supervisor vereniging: man, ca. 60, kaal, bril |
| G | Woonstraat fontein (onderwerp 7) | Boa Lotte: vrouw, ca. 38, rood haar, sproeten; bewoner: man, ca. 65, wit haar |
| H | Park tas (onderwerp 7) | Boa Samira: vrouw, ca. 33, donker haar met donkerblauwe hoofddoek, getinte huid |
| I | Station groep (onderwerp 7) | Boa Kees (man, ca. 58, grijs kort haar) en boa Priya (vrouw, ca. 29, lang zwart haar); groep jongvolwassenen op afstand, onherkenbaar |
| J | Tas zonder etiket (onderwerp 6) | Geen herkenbare boa; omstanders onscherp op de achtergrond |
| K | Afstand en melden (onderwerp 5, 6, 8) | Boa van achteren gezien, gezicht niet zichtbaar (bewust generiek, want gebruikt bij meerdere casussen) |

Regel: dezelfde casus → hetzelfde personage; een andere casus → bewust een andere persoon. Beelden die bij meerdere casussen worden gebruikt (code K) tonen geen herkenbaar gezicht.

## 3. Nieuwe beelden met exacte prompts

| Nr | Bestand | Personage | Alt-tekst | Prompt |
|---|---|---|---|---|
| N1 | `plein-knal.webp` | A | Twee boa’s in handhavingsuniform spreken op straat een groep jonge mannen aan. Eén van hen houdt een doos vuurwerk vast; een ander heeft ook vuurwerk in zijn hand. | Evening on a Dutch brick-paved town square with shopfronts, five teenagers (mixed ethnicities, casual winter clothing) standing together; one holds an unlit firework tube; a sports bag on the ground next to them; in the foreground at a distance of about 15 m, Dutch municipal enforcement officer (boa) in a dark navy uniform jacket and trousers, reflective details, a small generic badge patch without readable text, no weapons, NO 'POLITIE' text anywhere on the boa's clothing (Sanne: woman, ~30, blond ponytail) observing calmly. Faces of the teenagers not in sharp focus. Documentary-style professional photograph, the Netherlands, natural light, realistic skin texture, calm and serious mood, 35mm lens, shallow depth of field, no text or logos except where specified, no cartoon, no 3D, no AI-plastic faces, no American police uniforms or badges, 16:9, 3000x1688 px. |
| N2 | `vuurwerk-f1.webp` | – | Klein vuurwerk voor binnengebruik, zoals sterretjes, in de originele verpakking met categorieaanduiding. | Product photograph on a neutral light-grey surface: small indoor novelty fireworks such as sparklers in their original retail packaging, with a clearly legible generic label reading "F1" and a CE mark; fictitious brand name "Pyrona"; no other readable text. Documentary-style professional photograph, the Netherlands, natural light, realistic skin texture, calm and serious mood, 35mm lens, shallow depth of field, no text or logos except where specified, no cartoon, no 3D, no AI-plastic faces, no American police uniforms or badges, 16:9, 3000x1688 px. |
| N3 | `vuurwerk-f2.webp` | – | Verpakt vuurwerk met op het etiket de categorieaanduiding F2, op een neutrale ondergrond. | Product photograph on a neutral light-grey surface: consumer firework products (a small cake box and a ground fountain) in retail packaging with a clearly legible label "F2" and CE mark, fictitious brand "Pyrona", no other readable text. Documentary-style professional photograph, the Netherlands, natural light, realistic skin texture, calm and serious mood, 35mm lens, shallow depth of field, no text or logos except where specified, no cartoon, no 3D, no AI-plastic faces, no American police uniforms or badges, 16:9, 3000x1688 px. |
| N4 | `vuurwerk-f3.webp` | – | Verpakt vuurwerk met op het etiket de categorieaanduiding F3, op een neutrale ondergrond. | Product photograph on a neutral grey surface: a larger firework cake box in packaging with a clearly legible label "F3" and a CE mark, fictitious brand, no other readable text. Documentary-style professional photograph, the Netherlands, natural light, realistic skin texture, calm and serious mood, 35mm lens, shallow depth of field, no text or logos except where specified, no cartoon, no 3D, no AI-plastic faces, no American police uniforms or badges, 16:9, 3000x1688 px. |
| N5 | `vuurwerk-professioneel.webp` | – | Professioneel vuurwerk in transportverpakking bij een afgezette vuurwerkshowlocatie. | Professional display fireworks in sealed brown transport boxes with orange hazard labels (explosive class 1.3G pictogram) inside a fenced-off professional show site in daylight; a person in professional pyrotechnic workwear seen from behind; no readable brand names. Documentary-style professional photograph, the Netherlands, natural light, realistic skin texture, calm and serious mood, 35mm lens, shallow depth of field, no text or logos except where specified, no cartoon, no 3D, no AI-plastic faces, no American police uniforms or badges, 16:9, 3000x1688 px. |
| N6 | `etiket-categorie.webp` | – | Close-up van een vuurwerkverpakking met etiket, categorieaanduiding en CE-markering. Fictief merk. | Macro close-up of a firework packaging label: legible generic text "Categorie F2", "CE", "NEM 250 g", a pictogram-style usage instruction; fictitious brand; the rest of the text blurred naturally by depth of field. Documentary-style professional photograph, the Netherlands, natural light, realistic skin texture, calm and serious mood, 35mm lens, shallow depth of field, no text or logos except where specified, no cartoon, no 3D, no AI-plastic faces, no American police uniforms or badges, 16:9, 3000x1688 px. |
| N7 | `vuurwerk-los.webp` | – | Los vuurwerk zonder verpakking of etiket op de grond. De categorie is niet te zien. | Several loose, unlabelled cylindrical firework-like objects without packaging lying on wet pavement at night under a street lamp; no labels visible; nobody touching them. Documentary-style professional photograph, the Netherlands, natural light, realistic skin texture, calm and serious mood, 35mm lens, shallow depth of field, no text or logos except where specified, no cartoon, no 3D, no AI-plastic faces, no American police uniforms or badges, 16:9, 3000x1688 px. |
| N8 | `zwaar-illegaal.webp` | – | In beslag genomen vuurwerk zonder etiket in een bak op een tafel, gefotografeerd voor het dossier. | Evidence photo: a grey plastic evidence crate on a table containing unlabelled heavy firework objects, some wrapped in tape; a ruler for scale; neutral institutional room; no people. Documentary-style professional photograph, the Netherlands, natural light, realistic skin texture, calm and serious mood, 35mm lens, shallow depth of field, no text or logos except where specified, no cartoon, no 3D, no AI-plastic faces, no American police uniforms or badges, 16:9, 3000x1688 px. |
| N9 | `tas-inhoud.webp` | A | Open sporttas op de grond met verschillende soorten vuurwerk: een deel in de verpakking, een deel los. | Close view from about 2 m of an open black sports bag on a paved square at dusk: some fireworks in retail packaging, some loose without labels; a blurred pair of legs of teenagers in the background. Documentary-style professional photograph, the Netherlands, natural light, realistic skin texture, calm and serious mood, 35mm lens, shallow depth of field, no text or logos except where specified, no cartoon, no 3D, no AI-plastic faces, no American police uniforms or badges, 16:9, 3000x1688 px. |
| N10 | `boa-staandehouden.webp` | D | Een boa spreekt een jongere aan op straat en vraagt naar zijn identiteitsbewijs. | Dutch municipal enforcement officer (boa) in a dark navy uniform jacket and trousers, reflective details, a small generic badge patch without readable text, no weapons, NO 'POLITIE' text anywhere on the boa's clothing (Ricardo: man, ~35, short black hair, dark skin) speaking calmly with a teenager (~17, reddish hair, hoodie) on a Dutch shopping street in the evening, asking for an ID card; respectful body language; the teenager is not holding fireworks. Documentary-style professional photograph, the Netherlands, natural light, realistic skin texture, calm and serious mood, 35mm lens, shallow depth of field, no text or logos except where specified, no cartoon, no 3D, no AI-plastic faces, no American police uniforms or badges, 16:9, 3000x1688 px. |
| N11 | `boa-politie-overdracht.webp` | E | Een boa praat met twee politiemensen bij een politieauto en draagt de situatie over. | Dutch municipal enforcement officer (boa) in a dark navy uniform jacket and trousers, reflective details, a small generic badge patch without readable text, no weapons, NO 'POLITIE' text anywhere on the boa's clothing (Eva: woman, ~52, greying dark hair in a bun) talking with two Dutch police officers in the current Dutch police uniform (dark blue with reflective yellow-blue details), clearly distinguishable from the boa next to a Dutch police car in a residential street at dusk; a closed sports bag stands on the ground at a distance. Documentary-style professional photograph, the Netherlands, natural light, realistic skin texture, calm and serious mood, 35mm lens, shallow depth of field, no text or logos except where specified, no cartoon, no 3D, no AI-plastic faces, no American police uniforms or badges, 16:9, 3000x1688 px. |
| N12 | `parkeerplaats.webp` | B | Parkeerplaats in de avond: vier jongeren. Eén jongere houdt vuurwerk in zijn hand. Op de grond staat een tas. | Evening at a Dutch supermarket parking lot, four young men (mixed ethnicities) standing near a car; one holds an unlit firework; a sports bag on the ground; Dutch municipal enforcement officer (boa) in a dark navy uniform jacket and trousers, reflective details, a small generic badge patch without readable text, no weapons, NO 'POLITIE' text anywhere on the boa's clothing (Mehmet: man, ~40, short dark hair and beard) approaching from a distance of about 20 m. Documentary-style professional photograph, the Netherlands, natural light, realistic skin texture, calm and serious mood, 35mm lens, shallow depth of field, no text or logos except where specified, no cartoon, no 3D, no AI-plastic faces, no American police uniforms or badges, 16:9, 3000x1688 px. |
| N13 | `afstand-melden.webp` | K | Een boa, van achteren gezien, houdt afstand van een tas op de grond en meldt zich via de portofoon. | Dutch municipal enforcement officer (boa) in a dark navy uniform jacket and trousers, reflective details, a small generic badge patch without readable text, no weapons, NO 'POLITIE' text anywhere on the boa's clothing seen from behind, standing well away from a bag on the pavement, speaking into a handheld radio; face not visible; evening street light. Documentary-style professional photograph, the Netherlands, natural light, realistic skin texture, calm and serious mood, 35mm lens, shallow depth of field, no text or logos except where specified, no cartoon, no 3D, no AI-plastic faces, no American police uniforms or badges, 16:9, 3000x1688 px. |
| N14 | `vervoermiddel-onderzoek.webp` | C | Een boa staat naast een geparkeerde personenauto met open kofferbak en spreekt de bestuurder aan. In de kofferbak ligt een tas. | Dutch municipal enforcement officer (boa) in a dark navy uniform jacket and trousers, reflective details, a small generic badge patch without readable text, no weapons, NO 'POLITIE' text anywhere on the boa's clothing (Daan: man, ~26, short blond hair) standing next to a parked Dutch hatchback with the boot open, talking with the driver (woman, ~50, short grey hair); a closed bag visible in the boot; daylight residential parking area. Documentary-style professional photograph, the Netherlands, natural light, realistic skin texture, calm and serious mood, 35mm lens, shallow depth of field, no text or logos except where specified, no cartoon, no 3D, no AI-plastic faces, no American police uniforms or badges, 16:9, 3000x1688 px. |
| N15 | `ontheffing-sportveld.webp` | F | Afgezet sportveld op oudejaarsavond. Een supervisor van een vereniging laat een boa een document zien. | New Year's Eve at a fenced-off local sports field with safety tape; a club supervisor (man, ~60, bald, glasses, high-visibility vest) shows a printed document to Dutch municipal enforcement officer (boa) in a dark navy uniform jacket and trousers, reflective details, a small generic badge patch without readable text, no weapons, NO 'POLITIE' text anywhere on the boa's clothing (Noah: man, ~24, curly dark-brown hair, light-brown skin); packaged fireworks lined up on the grass in the background at a distance. Documentary-style professional photograph, the Netherlands, natural light, realistic skin texture, calm and serious mood, 35mm lens, shallow depth of field, no text or logos except where specified, no cartoon, no 3D, no AI-plastic faces, no American police uniforms or badges, 16:9, 3000x1688 px. |
| N16 | `inbeslagname-tafel.webp` | – | Handen met handschoenen leggen verpakt vuurwerk in een bak op een tafel. Op tafel ligt een formulier. Geen gezichten. | Top-down view of a table: gloved hands placing packaged fireworks into a grey evidence crate; a generic seizure form ("Kennisgeving van inbeslagneming" as the only readable heading) and a pen next to it; no faces. Documentary-style professional photograph, the Netherlands, natural light, realistic skin texture, calm and serious mood, 35mm lens, shallow depth of field, no text or logos except where specified, no cartoon, no 3D, no AI-plastic faces, no American police uniforms or badges, 16:9, 3000x1688 px. |
| N17 | `tas-zonder-etiket.webp` | J | Tas op een stoep met groot vuurwerk zonder etiket, deels met tape omwikkeld. Op de achtergrond kijken omstanders toe. | A bag on a Dutch pavement containing large unlabelled firework objects, some wrapped in grey tape; bystanders blurred in the background at a distance; evening. Documentary-style professional photograph, the Netherlands, natural light, realistic skin texture, calm and serious mood, 35mm lens, shallow depth of field, no text or logos except where specified, no cartoon, no 3D, no AI-plastic faces, no American police uniforms or badges, 16:9, 3000x1688 px. |
| N18 | `woonstraat-fontein.webp` | G | Woonstraat in de avond: een man van middelbare leeftijd staat naast een brandende grondfontein. Een boa komt aanlopen. | Dutch residential street with terraced houses in the evening; a man (~65, white hair) stands next to a burning ground fountain firework on the street; Dutch municipal enforcement officer (boa) in a dark navy uniform jacket and trousers, reflective details, a small generic badge patch without readable text, no weapons, NO 'POLITIE' text anywhere on the boa's clothing (Lotte: woman, ~38, red hair, freckles) walking towards him at a safe distance. Documentary-style professional photograph, the Netherlands, natural light, realistic skin texture, calm and serious mood, 35mm lens, shallow depth of field, no text or logos except where specified, no cartoon, no 3D, no AI-plastic faces, no American police uniforms or badges, 16:9, 3000x1688 px. |
| N19 | `park-tas.webp` | H | Pad in een park: een achtergelaten tas met vuurwerk naast een bankje. Een boa staat op afstand en belt. | Footpath in a Dutch park at dusk; an abandoned bag with fireworks next to a bench; Dutch municipal enforcement officer (boa) in a dark navy uniform jacket and trousers, reflective details, a small generic badge patch without readable text, no weapons, NO 'POLITIE' text anywhere on the boa's clothing (Samira: woman, ~33, dark-blue headscarf) standing about 10 m away making a phone call. Documentary-style professional photograph, the Netherlands, natural light, realistic skin texture, calm and serious mood, 35mm lens, shallow depth of field, no text or logos except where specified, no cartoon, no 3D, no AI-plastic faces, no American police uniforms or badges, 16:9, 3000x1688 px. |
| N20 | `station-groep.webp` | I | Stationsplein in de avond: een drukke groep met vuurwerk. Twee boa’s houden afstand en melden zich via de portofoon. | Busy Dutch station square at night; a lively group of young adults with large fireworks in the mid-distance, faces not recognisable; in the foreground two boas (Kees: man ~58 grey hair; Priya: woman ~29 long black hair) in a dark navy uniform jacket and trousers, reflective details, a small generic badge patch without readable text, no weapons, NO 'POLITIE' text anywhere on the boa's clothing keeping distance and using a radio. Documentary-style professional photograph, the Netherlands, natural light, realistic skin texture, calm and serious mood, 35mm lens, shallow depth of field, no text or logos except where specified, no cartoon, no 3D, no AI-plastic faces, no American police uniforms or badges, 16:9, 3000x1688 px. |
| N21 | `parkeerplaats-tas.webp` | B | Detail van de tas op de parkeerplaats: verpakkingen met etiket en los vuurwerk zonder etiket. | Detail photo at a parking lot at night: an open sports bag on the asphalt with some fireworks in packaging with labels and some loose unlabelled items; nobody touching the bag. Documentary-style professional photograph, the Netherlands, natural light, realistic skin texture, calm and serious mood, 35mm lens, shallow depth of field, no text or logos except where specified, no cartoon, no 3D, no AI-plastic faces, no American police uniforms or badges, 16:9, 3000x1688 px. |

## 4. Te vervangen: boa-illustratie in sjablonen

De getekende boa-illustratie (één vrouwelijke boa) komt uit Straatintimidatie2 en staat op leerdoelen-, samenvattings- en uitlegpagina’s. Advies: vervangen door een serie van zes fotografische boa-portretten (halflichaam, vrijstaand, lichte achtergrond, 448×840 en 500×520 px zoals de bestaande bestanden), met personages uit tabel 2 die niet in een casus voorkomen: man ~45 grijs haar; vrouw ~27 donkere huid, kort kroeshaar; man ~32 Aziatisch-Nederlands; vrouw ~40 blond kort haar; man ~55 baard; vrouw ~30 met hoofddoek. Technisch moeten dan `boa-hero(-spiegel).webp` en `boa-buste(-spiegel).webp` per pose worden uitgebreid; dat vraagt een kleine codewijziging in `boaHTML` (nu één persoon).

## 5. Inventarisatie per pagina

| Pagina | Titel | Huidig beeld | Actie |
|---|---|---|---|
| 1.1 | Leerdoelen | boa-armen | VERVANGEN (fotografisch boa-portret, per casus ander personage) |
| 1.2 | Een harde knal op het plein | scene-plein-knal | NIEUW — foto nog niet geleverd; nu tijdelijk pictogrambeeld (geen placeholdertekst) |
| 1.3 | Een harde knal op het plein — wat gaat er door je heen? | boa-observeer | VERVANGEN (fotografisch boa-portret, per casus ander personage) |
| 1.4 | Waarom vuurwerk jouw werk is | boa-uitleg | VERVANGEN (fotografisch boa-portret, per casus ander personage) |
| 1.5 | Categorie is nog geen conclusie | icoonvisual | BEHOUDEN (functionele vectorvisual) |
| 1.6 | De vier vragen | infographic bestanddelen | BEHOUDEN (functionele vectorvisual) |
| 1.7 | Vijf soorten vragen, niet door elkaar | weegschaal | BEHOUDEN (functionele illustratie) |
| 1.8 | Opzet van de opleiding | infographic opzet | BEHOUDEN |
| 1.9 | Kort samengevat | boa-armen | VERVANGEN (fotografisch boa-portret, per casus ander personage) |
| 2.1 | Leerdoelen | boa-armen | VERVANGEN (fotografisch boa-portret, per casus ander personage) |
| 2.2 | Waarom categorieën? | icoonvisual | BEHOUDEN (functionele vectorvisual) |
| 2.3 | Wettekst: indeling in categorieën | — | — |
| 2.4 | Overzicht van de categorieën | infographic categorieen | BEHOUDEN |
| 2.5 | Categorie F1 | scene-vuurwerk-f1 | NIEUW — foto nog niet geleverd; nu tijdelijk pictogrambeeld (geen placeholdertekst) |
| 2.6 | Categorie F2 | scene-vuurwerk-f2 | NIEUW — foto nog niet geleverd; nu tijdelijk pictogrambeeld (geen placeholdertekst) |
| 2.7 | Categorie F3 | scene-vuurwerk-f3 | NIEUW — foto nog niet geleverd; nu tijdelijk pictogrambeeld (geen placeholdertekst) |
| 2.8 | Categorie F4 / professioneel vuurwerk | scene-vuurwerk-professioneel | NIEUW — foto nog niet geleverd; nu tijdelijk pictogrambeeld (geen placeholdertekst) |
| 2.9 | Personen met gespecialiseerde kennis | — | — |
| 2.10 | Verpakking en etiket | — | — |
| 2.11 | Zelfde tas, andere informatie | infographic vergelijk | BEHOUDEN |
| 2.12 | Onbekend vuurwerk | scene-vuurwerk-los | NIEUW — foto nog niet geleverd; nu tijdelijk pictogrambeeld (geen placeholdertekst) |
| 2.13 | Van waarneming naar juridische conclusie | infographic lagen4 | BEHOUDEN |
| 2.14 | Op straat weet je het niet altijd | boa-notitie | VERVANGEN (fotografisch boa-portret, per casus ander personage) |
| 2.15 | Terug naar het plein: de tas | scene-tas-inhoud | NIEUW — foto nog niet geleverd; nu tijdelijk pictogrambeeld (geen placeholdertekst) |
| 2.16 | Wat kun je wel en nog niet vaststellen? | infographic checklist | BEHOUDEN |
| 2.17 | Van product naar juridische conclusie | infographic keten7 | BEHOUDEN |
| 2.18 | Kort samengevat | scene-etiket-categorie | NIEUW — foto nog niet geleverd; nu tijdelijk pictogrambeeld (geen placeholdertekst) |
| 2.19 | Kort samengevat | boa-notitie | VERVANGEN (fotografisch boa-portret, per casus ander personage) |
| 2.20 | Vooruitblik: Wat zegt de wet? | boa-illustratie (sjabloon) | BEHOUDEN |
| 3.1 | Leerdoelen | boa-armen | VERVANGEN (fotografisch boa-portret, per casus ander personage) |
| 3.2 | Van soort naar strafbaarheid | wetboek | BEHOUDEN (functionele illustratie) |
| 3.3 | De Wet veilige jaarwisseling | icoonvisual | BEHOUDEN (functionele vectorvisual) |
| 3.4 | Wettekst: artikel 9.2.2.1a Wet milieubeheer | — | — |
| 3.5 | Lid 1: bezit en gebruik | scene-tas-inhoud | NIEUW — foto nog niet geleverd; nu tijdelijk pictogrambeeld (geen placeholdertekst) |
| 3.6 | Lid 2, 6 en 7: verkoop | icoonvisual | BEHOUDEN (functionele vectorvisual) |
| 3.7 | Ontheffing van de burgemeester | icoonvisual | BEHOUDEN (functionele vectorvisual) |
| 3.8 | Ontheffing — voorbeeld uit de praktijk | scene-ontheffing-sportveld | NIEUW — foto nog niet geleverd; nu tijdelijk pictogrambeeld (geen placeholdertekst) |
| 3.9 | Controlekaart: ontheffing aangetroffen | wetboek | BEHOUDEN (functionele illustratie) |
| 3.10 | Artikel 9.2.2.1a Wm — let op | boa-uitleg | VERVANGEN (fotografisch boa-portret, per casus ander personage) |
| 3.11 | Wettekst: artikel 1a en artikel 2 WED | — | — |
| 3.12 | Straffen | wetboek | BEHOUDEN (functionele illustratie) |
| 3.13 | Van regel naar opsporingsbevoegdheid | infographic tijdlijn | BEHOUDEN |
| 3.14 | Kort samengevat | wetboek | BEHOUDEN (functionele illustratie) |
| 3.15 | Kort samengevat | icoonvisual | BEHOUDEN (functionele vectorvisual) |
| 3.16 | Vooruitblik: Wanneer ben jij als boa bevoegd? | boa-illustratie (sjabloon) | BEHOUDEN |
| 4.1 | Leerdoelen | boa-armen | VERVANGEN (fotografisch boa-portret, per casus ander personage) |
| 4.2 | Ben ik bevoegd? | scene-plein-knal | NIEUW — foto nog niet geleverd; nu tijdelijk pictogrambeeld (geen placeholdertekst) |
| 4.3 | Zien is iets anders dan bevoegd zijn | weegschaal | BEHOUDEN (functionele illustratie) |
| 4.4 | Wettekst: de buitengewoon opsporingsambtenaar | — | — |
| 4.5 | Domein I, onderdeel 9 | — | — |
| 4.6 | Domeinlijst is niet: alles mag | icoonvisual | BEHOUDEN (functionele vectorvisual) |
| 4.7 | Let op: oudere teksten zijn achterhaald | boa-uitleg | VERVANGEN (fotografisch boa-portret, per casus ander personage) |
| 4.8 | En F4 of ander professioneel vuurwerk? | scene-vuurwerk-professioneel | NIEUW — foto nog niet geleverd; nu tijdelijk pictogrambeeld (geen placeholdertekst) |
| 4.9 | WED: wie spoort economische delicten op? | — | — |
| 4.10 | Wanneer ben jij als boa bevoegd? | icoonvisual | BEHOUDEN (functionele vectorvisual) |
| 4.11 | Zeven stappen: ben ik bevoegd en mag ik dit doen? | infographic bevoegd | BEHOUDEN |
| 4.12 | Je weet de categorie nog niet | scene-vuurwerk-los | NIEUW — foto nog niet geleverd; nu tijdelijk pictogrambeeld (geen placeholdertekst) |
| 4.13 | Je weet de categorie nog niet — betekenis | boa-notitie | VERVANGEN (fotografisch boa-portret, per casus ander personage) |
| 4.14 | Kort samengevat | weegschaal | BEHOUDEN (functionele illustratie) |
| 4.15 | Kort samengevat | boa-notitie | VERVANGEN (fotografisch boa-portret, per casus ander personage) |
| 4.16 | Vooruitblik: Wat mag je als boa doen? | boa-illustratie (sjabloon) | BEHOUDEN |
| 5.1 | Leerdoelen | boa-armen | VERVANGEN (fotografisch boa-portret, per casus ander personage) |
| 5.2 | Van mogen naar doen: vijf stappen | infographic stappen | BEHOUDEN |
| 5.3 | Bevoegdhedenkaart | infographic kaart | BEHOUDEN |
| 5.4 | Let op: artikelnummers gecontroleerd | wetboek | BEHOUDEN (functionele illustratie) |
| 5.5 | Aanspreken, staande houden, aanhouden | scene-boa-staandehouden | NIEUW — foto nog niet geleverd; nu tijdelijk pictogrambeeld (geen placeholdertekst) |
| 5.6 | Wettekst: staande houden | — | — |
| 5.7 | Wie is verdachte? | — | — |
| 5.8 | Staande houden — situatie | scene-boa-staandehouden | NIEUW — foto nog niet geleverd; nu tijdelijk pictogrambeeld (geen placeholdertekst) |
| 5.9 | Staande houden — vijf stappen | boa-uitleg | VERVANGEN (fotografisch boa-portret, per casus ander personage) |
| 5.10 | Wettekst: aanhouden op heterdaad | — | — |
| 5.11 | Aanhouden op heterdaad — vijf stappen | scene-boa-politie-overdracht | NIEUW — foto nog niet geleverd; nu tijdelijk pictogrambeeld (geen placeholdertekst) |
| 5.12 | Wettekst: aanhouden buiten heterdaad | — | — |
| 5.13 | Let op: heterdaad en buiten heterdaad | boa-uitleg | VERVANGEN (fotografisch boa-portret, per casus ander personage) |
| 5.14 | Wettekst: vervoermiddelen onderzoeken | — | — |
| 5.15 | Vervoermiddelen onderzoeken — situatie | scene-vervoermiddel-onderzoek | NIEUW — foto nog niet geleverd; nu tijdelijk pictogrambeeld (geen placeholdertekst) |
| 5.16 | Vervoermiddelen onderzoeken — vijf stappen | scene-vervoermiddel-onderzoek | NIEUW — foto nog niet geleverd; nu tijdelijk pictogrambeeld (geen placeholdertekst) |
| 5.17 | Wettekst: medewerking vorderen | — | — |
| 5.18 | Medewerking vorderen — vijf stappen | scene-vervoermiddel-onderzoek | NIEUW — foto nog niet geleverd; nu tijdelijk pictogrambeeld (geen placeholdertekst) |
| 5.19 | Wettekst: inbeslagneming en uitlevering vorderen | — | — |
| 5.20 | Inbeslagneming | scene-inbeslagname-tafel | NIEUW — foto nog niet geleverd; nu tijdelijk pictogrambeeld (geen placeholdertekst) |
| 5.21 | Inbeslagneming — vijf stappen | scene-tas-inhoud | NIEUW — foto nog niet geleverd; nu tijdelijk pictogrambeeld (geen placeholdertekst) |
| 5.22 | Wettekst: niet voldoen aan een vordering | — | — |
| 5.23 | Veiligstellen is geen aparte bevoegdheid | scene-afstand-melden | NIEUW — foto nog niet geleverd; nu tijdelijk pictogrambeeld (geen placeholdertekst) |
| 5.24 | Proces-verbaal | infographic proces | BEHOUDEN (functionele vectorvisual) |
| 5.25 | Overdracht aan de politie | scene-boa-politie-overdracht | NIEUW — foto nog niet geleverd; nu tijdelijk pictogrambeeld (geen placeholdertekst) |
| 5.26 | Let op: redelijkerwijs nodig | boa-armen | VERVANGEN (fotografisch boa-portret, per casus ander personage) |
| 5.27 | Kort samengevat | boa-uitleg | VERVANGEN (fotografisch boa-portret, per casus ander personage) |
| 5.28 | Kort samengevat | pv-document | BEHOUDEN (functionele illustratie) |
| 5.29 | Vooruitblik: Onbekend en zwaar illegaal vuurwerk | boa-illustratie (sjabloon) | BEHOUDEN |
| 6.1 | Leerdoelen | boa-armen | VERVANGEN (fotografisch boa-portret, per casus ander personage) |
| 6.2 | Een tas zonder etiketten | scene-tas-zonder-etiket | NIEUW — foto nog niet geleverd; nu tijdelijk pictogrambeeld (geen placeholdertekst) |
| 6.3 | Praktijkterm is geen wettelijke categorie | scene-zwaar-illegaal | NIEUW — foto nog niet geleverd; nu tijdelijk pictogrambeeld (geen placeholdertekst) |
| 6.4 | Aangepast of zelfgemaakt vuurwerk | icoonvisual | BEHOUDEN (functionele vectorvisual) |
| 6.5 | Onbekend vuurwerk: wat weet je wel en niet? | scene-vuurwerk-los | NIEUW — foto nog niet geleverd; nu tijdelijk pictogrambeeld (geen placeholdertekst) |
| 6.6 | Bevoegd is niet hetzelfde als veilig | scene-afstand-melden | NIEUW — foto nog niet geleverd; nu tijdelijk pictogrambeeld (geen placeholdertekst) |
| 6.7 | Drie aparte vragen | infographic drie | BEHOUDEN |
| 6.8 | Wanneer stop je met zelf onderzoeken? | scene-afstand-melden | NIEUW — foto nog niet geleverd; nu tijdelijk pictogrambeeld (geen placeholdertekst) |
| 6.9 | Zelf optreden of politie inschakelen? | scene-tas-zonder-etiket | NIEUW — foto nog niet geleverd; nu tijdelijk pictogrambeeld (geen placeholdertekst) |
| 6.10 | Zelf optreden of politie inschakelen? — betekenis | boa-uitleg | VERVANGEN (fotografisch boa-portret, per casus ander personage) |
| 6.11 | Kort samengevat | scene-zwaar-illegaal | NIEUW — foto nog niet geleverd; nu tijdelijk pictogrambeeld (geen placeholdertekst) |
| 6.12 | Kort samengevat | boa-observeer | VERVANGEN (fotografisch boa-portret, per casus ander personage) |
| 6.13 | Vooruitblik: Taakverdeling tussen boa en politie | boa-illustratie (sjabloon) | BEHOUDEN |
| 7.1 | Leerdoelen | boa-armen | VERVANGEN (fotografisch boa-portret, per casus ander personage) |
| 7.2 | Mogen en doen zijn twee dingen | weegschaal | BEHOUDEN (functionele illustratie) |
| 7.3 | Bevoegdheid naast taakverdeling | infographic taak | BEHOUDEN |
| 7.4 | Het Handhavingsplan jaarwisseling | icoonvisual | BEHOUDEN (functionele vectorvisual) |
| 7.5 | Tekst uit het Handhavingsplan: inzet van boa’s | — | — |
| 7.6 | Tekst uit het Handhavingsplan: gevaar en openbare orde | — | — |
| 7.7 | Lokale afspraken | icoonvisual | BEHOUDEN (functionele vectorvisual) |
| 7.8 | Zelf afhandelen, overleggen of politie inschakelen | infographic routes | BEHOUDEN |
| 7.9 | Situatie 1: zelf afhandelen | scene-woonstraat-fontein | NIEUW — foto nog niet geleverd; nu tijdelijk pictogrambeeld (geen placeholdertekst) |
| 7.10 | Situatie 2: overleggen | scene-park-tas | NIEUW — foto nog niet geleverd; nu tijdelijk pictogrambeeld (geen placeholdertekst) |
| 7.11 | Situatie 3: politie inschakelen | scene-station-groep | NIEUW — foto nog niet geleverd; nu tijdelijk pictogrambeeld (geen placeholdertekst) |
| 7.12 | Zo verloopt een overdracht | scene-boa-politie-overdracht | NIEUW — foto nog niet geleverd; nu tijdelijk pictogrambeeld (geen placeholdertekst) |
| 7.13 | Kort samengevat | weegschaal | BEHOUDEN (functionele illustratie) |
| 7.14 | Kort samengevat | scene-boa-politie-overdracht | NIEUW — foto nog niet geleverd; nu tijdelijk pictogrambeeld (geen placeholdertekst) |
| 7.15 | Vooruitblik: Van melding tot proces-verbaal | boa-illustratie (sjabloon) | BEHOUDEN |
| 8.1 | Leerdoelen | boa-armen | VERVANGEN (fotografisch boa-portret, per casus ander personage) |
| 8.2 | Terugblik | boa-illustratie (sjabloon) | BEHOUDEN |
| 8.3 | De casus: een knal op de parkeerplaats | scene-parkeerplaats | NIEUW — foto nog niet geleverd; nu tijdelijk pictogrambeeld (geen placeholdertekst) |
| 8.4 | Stap 1 – Wat neem je waar? | boa-observeer | VERVANGEN (fotografisch boa-portret, per casus ander personage) |
| 8.5 | Stap 2 – Is er mogelijk sprake van een strafbaar feit? | wetboek | BEHOUDEN (functionele illustratie) |
| 8.6 | Stap 3 – Welk vuurwerk kan dit zijn? | scene-parkeerplaats-tas | NIEUW — foto nog niet geleverd; nu tijdelijk pictogrambeeld (geen placeholdertekst) |
| 8.7 | Stap 4 – Welke informatie heb je nog nodig? | boa-notitie | VERVANGEN (fotografisch boa-portret, per casus ander personage) |
| 8.8 | Stap 5 – Ben je hiervoor opsporingsbevoegd? | icoonvisual | BEHOUDEN (functionele vectorvisual) |
| 8.9 | Stap 6 – Welke bevoegdheden kun je toepassen? | scene-boa-staandehouden | NIEUW — foto nog niet geleverd; nu tijdelijk pictogrambeeld (geen placeholdertekst) |
| 8.10 | Stap 7 – Is het veilig om zelf verder te handelen? | scene-afstand-melden | NIEUW — foto nog niet geleverd; nu tijdelijk pictogrambeeld (geen placeholdertekst) |
| 8.11 | Stap 8 – Moet de politie worden ingeschakeld? | scene-boa-politie-overdracht | NIEUW — foto nog niet geleverd; nu tijdelijk pictogrambeeld (geen placeholdertekst) |
| 8.12 | Stap 9 – Wat neem je in beslag of draag je over? | scene-inbeslagname-tafel | NIEUW — foto nog niet geleverd; nu tijdelijk pictogrambeeld (geen placeholdertekst) |
| 8.13 | Stap 10 – Wat komt in het proces-verbaal? | pv-document | BEHOUDEN (functionele illustratie) |
| 8.14 | Stap 10 – Zo niet | pv-document | BEHOUDEN (functionele illustratie) |
| 8.15 | Stap 10 – Zo wel | boa-notitie | VERVANGEN (fotografisch boa-portret, per casus ander personage) |
| 8.16 | Kort samengevat | scene-etiket-categorie | NIEUW — foto nog niet geleverd; nu tijdelijk pictogrambeeld (geen placeholdertekst) |
| 8.17 | Kort samengevat | wetboek | BEHOUDEN (functionele illustratie) |
| 8.18 | Kort samengevat | weegschaal | BEHOUDEN (functionele illustratie) |
| 8.19 | Kort samengevat | boa-uitleg | VERVANGEN (fotografisch boa-portret, per casus ander personage) |
| 8.20 | Kort samengevat | scene-zwaar-illegaal | NIEUW — foto nog niet geleverd; nu tijdelijk pictogrambeeld (geen placeholdertekst) |
| 8.21 | Kort samengevat | scene-boa-politie-overdracht | NIEUW — foto nog niet geleverd; nu tijdelijk pictogrambeeld (geen placeholdertekst) |
| 8.22 | Beslishulp: de vier vragen op straat | boa-uitleg | VERVANGEN (fotografisch boa-portret, per casus ander personage) |
| 8.23 | Beslishulp: de vier vragen op straat | infographic beslishulp | BEHOUDEN |
| 8.24 | Klaar voor de eindtoets | boa-armen | VERVANGEN (fotografisch boa-portret, per casus ander personage) |
