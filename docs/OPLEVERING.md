# Oplevering e-learning Vuurwerk

## VERSIE

**0.9.1** (geen 1.0). De cursus is juridisch, didactisch en technisch nagelopen en verbeterd. Versie 1.0 is bewust nog niet gegeven, omdat de beelden in de nieuwe cartoon-/illustratiestijl nog niet bestaan: in deze werkomgeving is geen beeldgenerator beschikbaar. Zie `BEELDPLAN.md` (42 nieuwe beelden met complete prompt).

- Juridische peildatum: **20 september 2026**.
- Datum eindcorrectie: **22 september 2026**. Cacheversie `vw260922e`, opslag `jslf-vw-v1` met voortgangsversie 17.
- Backupbranch vóór deze ronde: `backup-voor-eindcorrectie-vuurwerk-2026-09-22` (= commit `ffd550e`).
- Blauwdruk Straatintimidatie2: niet gewijzigd. `app.css` niet gewijzigd; nieuwe opmaak staat in `soorten.css`.

---

## EINDCORRECTIE 22 SEPTEMBER 2026 — WAT IS ER ECHT GEDAAN

### 1. Juridische controle (tegen de officiële tekst op wetten.overheid.nl, 22-9-2026)

Letterlijk vergeleken met de cursus:

| Bron | Gecontroleerd | Uitkomst |
|---|---|---|
| Wet milieubeheer, art. 9.2.2.1a lid 1–5 (geldend 1-8-2026) | wettekst | klopt letterlijk (lid 6–7 niet opnieuw vergeleken; ongewijzigd uit vorige ronde) |
| WED art. 2 lid 1, 6 lid 1 (1° en 4°), 17 lid 1–3, 18 lid 1, 21 lid 1–2, 23 lid 1, 24a lid 1, 26 | wettekst en strafmaxima | klopt |
| Sv art. 52 (begin), 54 lid 1–3, 94 lid 1–3, 95 lid 1 (geldend 1-7-2026) | wettekst | klopt |
| Vuurwerkbesluit art. 1.1.1 (definities), 1.2.2 lid 1–5 en 8, 1.2.3, 2.3.2 (a–d), 2.3.2a lid 3 onder a en e, 2.3.3 lid 1–2, 2.3.5, 2.3.7 | tekst | klopt met de cursus |
| Regeling domeinlijsten boa (BWBR0041447, geldend 8-9-2026), Domein I onderdeel 9 | tekst | klopt: “Artikel 9.2.2.1a Wet Milieubeheer juncto artikel 1a Wet op de economische delicten” |
| Beleidsregels boa (BWBR0039766) | citaat titel economische delicten | **gecorrigeerd**: citaat zegt letterlijk “de minister **die** het aangaat” (cursus had “wie”); regeling geldt nu vanaf **1-9-2026** (cursus zei 1-5-2026) |
| Handhavingsplan (rijksoverheid.nl), Stcrt. 2026, 31362, Stb. 2026, 168 | link opent | ja (gecontroleerd in de browser) |

Niet opnieuw letterlijk vergeleken in deze ronde: art. 1A.1.3, 1.1.2a en 2.1.3 Vuurwerkbesluit, art. 27, 27a, 53, 67, 96, 128 en 142 Sv, art. 1a en 24 WED, en de citaten uit het Handhavingsplan. Die zijn ongewijzigd uit de vorige ronde.

Overige juridische verbeteringen:
- O1 p6 “De vier vragen”: “veiligstellen” uit de antwoordmogelijkheden gehaald (cursus leert elders dat veiligstellen geen aparte bevoegdheid is).
- O7 p9 “Situatie 1”: toegevoegd dat bevoegdheid via domein I moet passen bij functie en taak.
- O7 p12 “Zo verloopt een overdracht”: “veilig gesteld” vervangen door “of de plek veilig is”.
- Eindtoetsvraag 13 (openbare orde): toelichting leunt nu alleen op het letterlijke Handhavingsplan; de niet-gecontroleerde verwijzing naar de Beleidsregels is weg.
- Bronlink Regeling domeinlijsten wijst nu naar de geconsolideerde tekst op wetten.overheid.nl (BWBR0041447/2026-09-08); de Staatscourant-vindplaats staat in de toelichting.

### 2. “Opleiding” wordt “cursus”

Vervangen op 9 plaatsen in de inhoud (O1 p1, p2, p3, p6, p7, p8 (titel en figuur), O3 p4, O4 p4, O6 p8), het kaderlabel van onderwerp 1 (“Opleiding” → “Cursus”) en 2 plaatsen in `app.js` (welkomstscherm en inleiding eindtoets). Controle achteraf: het woord komt in geen enkele zichtbare tekst meer voor. `D.opleiding` is alleen een interne veldnaam (waarde “Vuurwerk”).

### 3. Paginalengte, B1 en splitsen

- Gecontroleerde inhoudspagina’s: 141 (vóór) → **145** (na).
- Te lang (> ca. 140 woorden, inclusief wettekst en bronnen): 27 pagina’s. Aangepakt:
  - **Gesplitst (4 → 8 pagina’s, 4 nieuw):**
    - O2 “F4 en ander zwaar/illegaal vuurwerk” (474 woorden) → F4-pagina + nieuw “De categorieën op een rij” (Let op professioneel vuurwerk, Onthoud, Kort samengevat).
    - O3 “Wettekst: artikel 9.2.2.1a Wm” (355) → “lid 1–3” + nieuw “lid 4–7”, elk met eigen uitleg in gewone taal.
    - O4 “WED: wie spoort economische delicten op?” (351) → “Wettekst: artikel 17 WED” + nieuw “Artikel 17 WED en jouw akte”.
    - O5 “Wettekst: aanhouden buiten heterdaad” (365) → alleen art. 54 Sv + nieuw “Buiten heterdaad: wat betekent dit?” (art. 67 Sv en toepassing).
  - **Ingekort / naar B1:** O1 p4 “Waarom vuurwerk bij jouw werk hoort” (korte vragen in plaats van één lange zin), O4 p8 “En F4 of ander professioneel vuurwerk?” (187 → ca. 120 woorden).
  - **Bewust langer gebleven:** O1 p5 “Categorie is nog geen conclusie” en O2 p3–p6 (wettekst categorieën en de categoriepagina’s F1–F3): opgebouwd volgens de door Jan aangeleverde voorbeelddia’s met vastgestelde teksten; wettekstpagina’s (art. 142 Sv, 1.1.2a Vuurwerkbesluit, 52/27a Sv, 53/128 Sv, 23 WED, 24a WED, Handhavingsplan): letterlijke wettekst mag niet worden ingekort buiten een correct gemarkeerd fragment; O8 “Stap 10 – Zo wel”: voorbeeld-proces-verbaal hoort volledig te zijn.
- Wettekst blijft letterlijk; bij een deel staat nu “(lid 1 tot en met 3)” of “(fragment)”.
- Navigatie na splitsen: paginanummers, voortgang, vorige/volgende, hervatten en oefenvragen getest. Opgeslagen voortgang uit versie 16 wordt met een vaste tabel omgezet (`v17` in `hervat()`); getest met 6 oude posities.

### 4. Bronnen

98 bronregels die als “naam – https://…” (niet klikbaar) werden getoond, zijn omgezet naar de vorm die onderwerp 2 al had: een klikbare korte bronnaam plus toelichting (artikel, geldigheidsdatum). De link naar de Wet milieubeheer springt direct naar art. 9.2.2.1a.

### 5. Oefenvragen (31)

- Alle 31 toelichtingen: “Het juiste antwoord is X.” verwijderd (de feedback toont het juiste antwoord al apart; letters zijn niet nodig).
- O4 vraag 5 herschreven: het juiste antwoord viel op doordat het als enige een andere vorm had (“Voor alles wat buiten je functie…”). Nu een praktijkcasus (parkeertoezicht-boa ziet F2 afsteken) met vier gelijkwaardige opties.
- O4 vraag 6, O5 vraag 7: opties gelijk in lengte en vorm gemaakt (het juiste antwoord was duidelijk langer).
- O6 vraag 1: niet-geloofwaardige afleiders (“Is het duur geweest?”) vervangen.
- Oefenvragen worden niet gehusseld (vaste volgorde, ontwerp master).

### 6. Eindtoets (15 vragen, drempel 80 %)

- Alle 15 toelichtingen herschreven: geen “Juist is A/B/C/D” meer, maar inhoudelijke uitleg waarom.
- Technisch gecontroleerd: het antwoord wordt opgeslagen als de oorspronkelijke index van de optie (`data-orig`), niet als de zichtbare letter; score en nabespreking vergelijken die index met `juist`. Vragen én antwoorden worden per poging gehusseld.
- Vervangen (toepassing in plaats van losse kennis):
  - vraag 4 (“waarom is onbekend vuurwerk geen conclusie?”) → praktijkcasus tas met verpakt F2 en losse voorwerpen: wat weet je nog niet, wat doe je.
  - vraag 11 (kaal artikelnummer 24a) → casus weigeren kofferbak openen: art. 24a en 26 WED toegepast.
- Aangescherpt: vraag 10 en 12 (situatie in plaats van definitie), opties gelijkwaardiger bij vraag 2, 7, 8 en 13.
- Spreiding: vier vragen 1 · soorten/etiket 2 · onbekend vuurwerk 1 · de wet 2 · aanhouden 1 · bevoegdheid (domein) 2 · bevoegdheden 3 · taakverdeling 1 · veiligheid 1 · proces-verbaal 1.

### 7. Certificaat

Kerntekst: “Dit certificaat bevestigt dat [naam] de e-learning Vuurwerk en de bijbehorende eindtoets van JS Legal Force met goed gevolg heeft afgerond.” Kleine toelichting eronder: “Dit certificaat is een bewijs van succesvolle afronding en het behaalde toetsresultaat. Het betreft geen wettelijk erkend diploma of beroepskwalificatie.” Getest op scherm (390 px) en als PDF (A4 liggend, 1 pagina).

### 8. Responsive aanpassingen (alleen `soorten.css`)

- Telefoon (≤ 640 px): het decoratieve wetboek boven elke wettekstpagina wordt niet getoond; decoratieve pictogram-/boa-illustraties boven tekstpagina’s en oefenvragen zijn ca. een derde kleiner. Foto’s en inhoudelijke infographics blijven op volle grootte. Gevolg: de titel begint op de telefoon ca. 65–100 px hoger.
- Het label “HANDHAVINGSPLAN” in de wettekstkaart liep op 390/360 px buiten beeld (O7 p5–p6): vervangen door “Beleid”.
- Overzichtspagina “De categorieën op een rij”: eigen kop over de volle breedte.
- Er is niets globaal verkleind (geen kleinere letters, marges of regelafstand).

### 9. Beelden

- Beoordeeld: alle 145 inhoudspagina’s, 31 oefenvragen, 15 eindtoetsvragen, start, resultaat en certificaat. Besluit per scherm in `BEELDPLAN.md` §3.
- **Vervangen of nieuw geplaatst: 0.** Er is geen beeldgenerator beschikbaar; volgens de opdracht is geen slechte vervanging gemaakt en blijven de huidige beelden staan.
- Nieuw beeldplan in de gevraagde cartoon-/illustratiestijl: 42 beelden (26 praktijk-/situatiebeelden, 4 categoriekaarten F1–F4, 12 productillustraties), elk met doel, personages (H1–H6), scène, formaat, verboden elementen, bestandsnaam, alt-tekst en complete prompt.
- Gevonden visuele problemen (nog niet opgelost, staan in het beeldplan): `wet-f2`/`concl-f2` tonen losse knalstaven als F2-voorbeeld; `concl-f4` toont vuurpijlen bij F4; categoriefoto’s zijn uitsneden van 200 × 300 px met deels onzintekst en een echte productnaam; de twee praktijkfoto’s zijn realistisch (geel hesje) en passen niet bij de nieuwe stijl; de boa-illustraties uit de master hebben “BOA” op de borst.

### 10. Technische test (Playwright/Chromium, lokaal, na alle wijzigingen)

- Alle **176** leerstappen (145 pagina’s + 31 oefenvragen) gerenderd op **1440×900, 1280×800, 1024×768, 768×1024, 390×844 en 360×740**: 0 scriptfouten, 0 consolefouten, 0 HTTP-fouten (geen 404), 0 kapotte afbeeldingen, geen horizontaal scrollen, geen element buiten de schermbreedte.
- Visueel beoordeeld (screenshots bekeken): alle nieuwe en gesplitste pagina’s op 1440 en 390; overzichtsbladen van alle 176 schermen op 390 px; steekproef op 1440 en 768. Niet elk scherm is op elk formaat afzonderlijk bekeken.
- Volledige doorloop door klikken (390×844): intake → welkom → alle pagina’s en 31 oefenvragen (juist en onjuist beantwoord, feedback zonder letters) → hervatten na herladen (juiste pagina) → eindtoets 9/15 (60 %, niet geslaagd, geen certificaatknop, wel “opnieuw maken”) → nieuwe poging 15/15 (geslaagd) → certificaat → PDF → herladen op certificaat → “Opnieuw beginnen” wist de opslag.
- Migratie oude voortgang (v16 → v17) getest op 6 posities: komt op dezelfde pagina uit.
- Live-controle na uploaden: zie §11.

### 11. Publicatie

Zie de eindrapportage in de chat en het commitoverzicht op GitHub (uploads via de webinterface op `main`).

### 12. Nog handmatig controleren (door Jan / jurist)

1. Of de nieuwe opzet van eindtoetsvragen 4 en 11 inhoudelijk aansluit bij hoe Jan wil toetsen.
2. Art. 24a WED en de kofferbak (zie punt 3 hieronder) — ongewijzigd open.
3. De citaten uit het Handhavingsplan zijn niet opnieuw letterlijk vergeleken.
4. Weergave op echte telefoons (iOS Safari, Android Chrome): getest is alleen met Chromium in telefoonformaat. De verkleining gebruikt CSS `zoom` en `:has()`; in oudere browsers zonder ondersteuning blijven de illustraties gewoon op de oude grootte.

---

## EERDERE RONDES (historie, ongewijzigd behalve de datum van de Beleidsregels)

### Versie vorige ronde

**0.9** (geen 1.0). Alle juridische, didactische en technische eisen voor 1.0 zijn uitgevoerd, op één punt na: de 21 realistische foto's uit het beeldplan zijn **niet** gemaakt. In deze werkomgeving is geen beeldgenerator beschikbaar. Volgens de opdracht mag de versie dan niet 1.0 heten.

Wat is er wel gedaan: de oude placeholderbeelden met de tekst "Beeld nog aan te leveren" zijn weggehaald. Op die plekken staat nu een pictogrambeeld in de stijl van Straatintimidatie2. Er is nergens meer placeholdertekst te zien. De bestandsnamen, alt-teksten en prompts voor de foto's staan klaar in `BEELDPLAN.md`.

Blauwdruk: Straatintimidatie2. Die is niet gewijzigd. `app.css` is byte-gelijk aan de master.

## PEILDATUM

Juridische peildatum: **20 september 2026**.

## DATUM OPLEVERING

20 september 2026. Online: https://jslegalforce.github.io/Vuurwerk/ (cacheversie `vw260922d`).

## JURIDISCHE BRONNEN

Alleen officiële bronnen. Alle links zijn gecontroleerd (HTTP 200).

- **Wet milieubeheer**, art. 9.2.2.1a (lid 1–7), geldend vanaf 1-8-2026: https://wetten.overheid.nl/BWBR0003245/2026-08-01
- **Wet veilige jaarwisseling**: Stb. 2026, 7.
- **Besluit veilige jaarwisseling**: Stb. 2026, 168 (in werking 1-8-2026): https://zoek.officielebekendmakingen.nl/stb-2026-168.html
- **Vuurwerkbesluit**, geldend vanaf 1-8-2026: https://wetten.overheid.nl/BWBR0013360/2026-08-01
  - Artikelen: 1.1.1, 1.1.2a, 1A.1.3, 1.2.2, 1.2.3, 2.1.3, 2.3.2, 2.3.2a, 2.3.5.
- **Wet op de economische delicten**, geldend vanaf 1-8-2026: https://wetten.overheid.nl/BWBR0002063/2026-08-01
  - Artikelen: 1a, 2, 6, 17, 18, 21, 23, 24, 24a, 26.
- **Wetboek van Strafvordering**, geldend vanaf 1-7-2026: https://wetten.overheid.nl/BWBR0001903/2026-07-01
  - Artikelen: 27, 27a, 52, 53, 54, 67, 94, 95, 96, 142.
- **Regeling domeinlijsten buitengewoon opsporingsambtenaar**, Domein I, onderdeel 9, gewijzigd bij Stcrt. 2026, 31362 (in werking 8-9-2026): https://zoek.officielebekendmakingen.nl/stcrt-2026-31362.html
- **Beleidsregels buitengewoon opsporingsambtenaar**, geldend vanaf 1-9-2026 (onder meer over de titel voor economische delicten, via art. 17 lid 1 onder 2° WED): https://wetten.overheid.nl/BWBR0039766
- **Handhavingsplan jaarwisseling**, Ministerie van JenV, maart 2026. Dit is **beleid**, geen wet: https://www.rijksoverheid.nl/documenten/2026/03/16/tk-bijlage-geactualiseerd-handhavingsplan-jaarwisseling-feb-2026

De wetteksten zijn letterlijk overgenomen uit de geldende versies.

## JURIDISCHE WIJZIGINGEN

Ten opzichte van versie 0.2:

| Onderdeel | Wijziging |
|---|---|
| Art. 17 WED | Nieuw kader dat drie dingen uit elkaar houdt: (A) opsporingsbevoegd zijn voor het feit, (B) een concrete WED-bevoegdheid hebben, en (C) wat past bij je functie en taakomschrijving. Grondslag in letterlijke tekst: de Beleidsregels boa. Een boa krijgt de titel voor economische delicten via art. 17 lid 1 onder 2° WED. De oude placeholder is weg. |
| F4 / Vuurwerkbesluit | De stellige conclusie staat nu in de cursus. Onderdeel 9 noemt alleen art. 9.2.2.1a Wm. Overtredingen van het Vuurwerkbesluit lopen via art. 9.2.2.1 Wm, en dat artikel staat niet in onderdeel 9. Op grond van onderdeel 9 ben je dus niet bevoegd voor F4-feiten. |
| Art. 54 Sv | Nieuwe pagina "Aanhouden buiten heterdaad". Opzettelijke overtreding is een misdrijf met maximaal zes jaar. Daardoor is voorlopige hechtenis toegelaten (art. 67 lid 1 onder a Sv). Aanhouden buiten heterdaad gebeurt in beginsel op bevel van de OvJ (lid 1). Daarna komt de HOvJ (lid 2). Alleen als het bevel niet kan worden afgewacht, mag de opsporingsambtenaar zelf aanhouden (lid 3). Bij een overtreding kan niet buiten heterdaad worden aangehouden. De cursus zegt nergens dat een boa buiten heterdaad dezelfde bevoegdheid heeft als bij heterdaad. |
| Kofferbak | Vier handelingen apart uitgelegd: stilhouden (art. 23 lid 4 WED), onderzoeken (art. 23 lid 1–2), medewerking vorderen zoals de kofferbak laten openen (art. 24a) en opzettelijk weigeren (art. 26). |
| Veiligstellen / art. 96 Sv | "Veiligstellen" is geen aparte bevoegdheid. Inbeslagneming loopt via art. 18 WED en art. 95 en 96 lid 1 Sv. Art. 96 lid 2 geldt alleen binnen de situaties van lid 1. Afstand houden is een veiligheidsmaatregel en geen beslagbevoegdheid. |
| Categorieën | Er staan geen productvoorbeelden meer als vaste categorie. De vorm zegt niets over de categorie; de fabrikant deelt in (art. 1A.1.3 Vuurwerkbesluit, letterlijk). Nieuwe keten van 7 stappen: product → categorie → voor wie → handeling → bepaling → uitzondering/ontheffing → bevoegd. |
| Ontheffing | Controlekaart met 7 vragen, met verwijzing naar art. 9.2.2.1a lid 4–5 Wm en art. 2.3.2 en 2.3.2a Vuurwerkbesluit. |
| Halt / reprimande | Verwijderd. Er is geen afdoende officiële bron over de actuele stand. |
| Veiligheid | Alleen de algemene boodschap staat erin: een bevoegdheid is geen plicht, veiligheid gaat voor, afstand houden en de politie inschakelen. Er zijn geen verzonnen afstanden, meters of protocollen. |
| Proces-verbaal | Checklist van 12 onderdelen, met een "Zo niet"- en een "Zo wel"-voorbeeld. Daarin staan ook de vordering, de reactie van betrokkene en de grondslag van elke bevoegdheid. |
| Pagina “Waarom vuurwerk bij jouw werk hoort” | Onderwerp 1, pagina 4 opnieuw opgebouwd: drie informatiekaarten (nieuwe regels, bevoegdheid domein I, eerst onderzoek doen), een Onthoud-kaart, de aangeleverde foto rechts en een bronnenblok met klikbare bronnen onder elkaar. Opgebouwd met bestaande componenten (`rows`, `kcard`, `split`); `app.css` is niet gewijzigd. De zin over F2 en F3 is aangevuld tot “verboden voor personen zonder gespecialiseerde kennis”, conform artikel 9.2.2.1a, eerste lid, Wm. |
| Pagina “Soorten vuurwerk en de categorieën” | Onderwerp 2, nieuwe pagina 5 (na “Overzicht van de categorieën”). Vier categoriekaarten F1–F4/zwaar-illegaal met illustratieve foto’s, etiketkaart, blok “Is de categorie nog niet duidelijk?”, Onthoud-kaart, korte samenvatting en bronnen. Foto’s (200 × 300 px) uitgesneden uit de aangeleverde voorbeelddia (`assets/images/cat-*.webp`); later te vervangen door scherpere losse foto’s onder dezelfde bestandsnaam. Opmaak in `assets/soorten.css`; `app.css` ongewijzigd. Opgeslagen voortgang schuift automatisch één stap mee (opslag v14). |
| Terminologie art. 9.2.2.1a lid 1 | Onderwerp 3, pagina “De Wet veilige jaarwisseling”: “hebben of afsteken” → “het bezit en het gebruik … is verboden voor anderen dan personen met gespecialiseerde kennis”. Overige vindplaatsen gecontroleerd en bewust behouden (andere bepaling, uitleg, casus of broncitaat). |
| Controle onderwerp 2 (21-9-2026) | Nieuwe pagina: B1-formulering controles F2/F3, statusblok onbekend vuurwerk, “boa bevoegd” → “boa domein I bevoegd voor art. 9.2.2.1a Wm”, F4 als wettelijke categorie benoemd, voorbehoud classificatie bij F1 en F2-bijschriften, bronnen aangevuld (lid 4; art. 2.3.2/2.3.2a). Bronnen in onderwerp 2 als korte klikbare bronnaam in plaats van zichtbare URL. |
| Herontwerp pagina “Soorten vuurwerk en de categorieën” (21-9-2026) | Opbouw volgens aangeleverde voorbeelddia: kop + infoblok, vier kaarten F1–F4/zwaar-illegaal (badge, foto’s, Voorbeelden, Wat moet je weten?), fotonoot, brede Onthoud-kaart met Kort samengevat. Teksten letterlijk volgens opdracht. Statusblok “Is de categorie nog niet duidelijk?” vervallen (niet in voorbeeld; onderwerp 2 behandelt onbekend vuurwerk op eigen pagina’s). |
| Vier categoriepagina’s F1–F4 (22-9-2026) | Overzichtspagina in onderwerp 2 vervangen door vier pagina’s (pagina 5–8): F1, F2, F3 en “F4 en ander zwaar/illegaal vuurwerk”. Per pagina: kop met badge, foto’s, voorbeelden, “Wat moet je weten?” in tegels, korte samenvatting en rustige bronregel; op pagina 8 de Onthoud-kaart voor alle categorieën. Teksten volgens opdracht; F3-foto’s als “Mogelijke voorbeelden”, F4-foto’s als voorbeelden van zwaar/illegaal vuurwerk. Voortgang schuift mee (opslag v15). Onderwerp 2 telt nu 24 pagina’s. |
| Pagina “Categorie is nog geen conclusie” (22-9-2026) | Onderwerp 1, pagina 5 opnieuw vormgegeven volgens aangeleverde voorbeelddia: links vijf ronde beelden (F1, F2, F3, F4, Onbekend) rond een verpakking met etiket, met “Kijk altijd naar de verpakking!” en een fotonoot; rechts introtekst, kaarten F1, F2 en F3, F4 en Onbekend, en een afsluitende conclusie. Teksten volgens opdracht; F4-tekst aangepast. Beelden uitgesneden uit de voorbeelddia (`assets/images/concl-*.webp`). Opmaak in `assets/soorten.css`. |
| Pagina “Wettekst: indeling in categorieën” (22-9-2026) | Onderwerp 2, pagina 3 opnieuw opgebouwd volgens aangeleverde voorbeelddia: vier categorieblokken F1–F4 met kenmerken volgens art. 1A.1.3 lid 3 Vuurwerkbesluit en foto’s (`assets/images/wet-*.webp`), kort wettekstblok (art. 1A.1.3 lid 1, letterlijk), kaarten “Wat betekent dit voor jou als boa?”, “Aangemelde instantie”, bronnen en “In gewone taal”. |
| Opschoning onderwerp 2 (22-9-2026) | Onderwerp 2 van 24 naar 19 pagina’s: figuur “Overzicht van de categorieën” en oude pagina’s “Categorie F1–F4” verwijderd; unieke inhoud (wettelijke betekenis, waarnemen/niet concluderen, fop- en schertsvuurwerk, professioneel vuurwerk art. 1.1.1 en 1.2.2 lid 3, Handhavingsplan-praktijkterm) verplaatst naar de categoriepagina’s F1–F4. F4 niet meer gelabeld als “professioneel vuurwerk”; apart Let op-blok professioneel vuurwerk. “Beperkt gevaar” → “weinig gevaar”. Ontheffing: “aan een vereniging of stichting”; onderscheid voorwaarden (2.3.2) en voorschriften (2.3.2a). “Oudere verpakkingen” verwijderd. Etiketboodschap: belangrijke informatie, geen eindconclusie. F1: hele jaar kopen/afsteken, 12 jaar (art. 2.3.3, 2.3.5, 2.3.7). Nieuwe oefenvraag ontheffing (31 oefenvragen). Voortgang v16 schuift mee. Gecontroleerd tegen wetten.overheid.nl (Vuurwerkbesluit en Wm geldend 1-8-2026; Regeling domeinlijsten geldend 8-9-2026). |
| Eindcorrectie (22-9-2026) | Etiket niet meer “geen bewijs”: etiket geeft belangrijke informatie, vastleggen en betrekken bij het onderzoek (onderwerp 2 oefenvraag 1, onderwerp 8 p6 en p16, eindtoetsvraag 2). Art. 9.2.2.1a lid 1 zonder “verkoop” in de samenvattingen van onderwerp 3 en 8 (verkoop apart als lid 2). F4: geen absolute “niet bevoegd”-formulering meer; “uit onderdeel 9 volgt geen algemene opsporingsbevoegdheid voor F4” (onderwerp 3 p10, onderwerp 4 p8 en oefenvraag 6, onderwerp 8 p18, eindtoetsvraag 8). F1 gecontroleerd tegen art. 1.2.4, 2.3.3, 2.3.5 en 2.3.7 Vuurwerkbesluit. |
| Soortlabels | Pagina's hebben een label: Wet / Bevoegdheid / Domein / Beleid / Veiligheid. |

## WED-BEVOEGDHEDEN

Opnieuw gecontroleerd tegen de letterlijke tekst (geldend vanaf 1-8-2026):

| Handeling | Grondslag |
|---|---|
| In beslag nemen, en daarvoor uitlevering vorderen | art. 18 WED |
| Verpakkingen openen | art. 21 WED |
| Vervoermiddel onderzoeken (ook op lading) | art. 23 lid 1–2 WED |
| Laten stilhouden / overbrengen | art. 23 lid 4 WED |
| Regels over stilhouden en versperringen | art. 24 WED (geen medewerkingsbevoegdheid) |
| Medewerking vorderen | art. 24a WED |
| Opzettelijk niet voldoen aan een vordering | art. 26 WED. Dit is een economisch delict, geen bevoegdheid. |

Alle WED-bevoegdheden gelden alleen "voor zover dat redelijkerwijs voor de vervulling van hun taak nodig is".

## DOMEIN I

- Eén hoofdpagina met 7 stappen: feit → bepaling → domeinlijst → functie/taak → bevoegdheid → voorwaarden → veilig.
- De denkfout "Vuurwerk staat in mijn domein, dus ik ben voor alle vuurwerkfeiten bevoegd" wordt benoemd en weerlegd.
- Onderdeel 9 staat er letterlijk in: art. 9.2.2.1a Wm juncto art. 1a WED, in werking 8-9-2026.
- De oude passage uit het Handhavingsplan (domein I niet bevoegd voor bezit) staat gemarkeerd als achterhaald. Het Handhavingsplan wordt steeds als **beleid/taakverdeling** gelabeld, niet als bron van bevoegdheid.

## OPENSTAANDE JURIDISCHE PUNTEN

| Nr | Punt | Conclusie in de cursus | Zekerheid |
|---|---|---|---|
| 1 | Art. 17 WED | Heb je een akte voor art. 9.2.2.1a Wm jo. 1a WED? Dan ben je voor dat feit WED-opsporingsambtenaar (art. 17 lid 1 onder 2°, volgens de Beleidsregels boa). Dan gelden art. 18–24a WED. | redelijk hoog; per akte controleren |
| 2 | F4 | Niet bevoegd op grond van onderdeel 9 | hoog |
| 3 | Art. 54 Sv | In beginsel op bevel. Zelf alleen als het bevel niet kan worden afgewacht. Niet bij een overtreding. | hoog (wettekst); uitvoering boa: zie controlepunt |
| 4 | Kofferbak | 23 lid 4 / 23 lid 1–2 / 24a / 26 | hoog (wettekst); toepassing 24a: zie controlepunt |
| 5 | Art. 96 / veiligstellen | Geen aparte bevoegdheid | hoog |
| 6 | Categorievoorbeelden | Verwijderd; de fabrikant deelt in | hoog |
| 7 | Halt / reprimande | Verwijderd | n.v.t. (onderwerp niet in de cursus) |
| 8 | Veiligheid | Alleen de algemene boodschap, geen normen | hoog |

## BEELDEN

- 21 foto's vervangen: **nee** (2/21). Beeld N1 (`scene-plein-knal`) staat op de pagina “Een harde knal op het plein” en beeld N22 (`scene-boa-jongeren-plein`) op de pagina “Waarom vuurwerk bij jouw werk hoort” (beide onderwerp 1). Beide foto's zijn door de opdrachtgever aangeleverd. De overige 19 foto's kunnen in deze werkomgeving niet worden gemaakt; er is geen beeldgenerator beschikbaar.
- Tijdelijke oplossing: pictogrambeelden (op één plek de getekende boa uit de master). Er is geen placeholdertekst en er zijn geen kapotte beelden.
- De pictogrambeelden zijn decoratief (`aria-hidden`), zodat de alt-tekst geen scène beschrijft die niet te zien is.
- De map `assets/images/` met placeholderbestanden is verwijderd. In die map staan nu alleen de aangeleverde foto's `plein-knal.webp` (1600 × 829 px, 92 kB) en `boa-jongeren-plein.webp` (729 × 580 px, 67 kB), lokaal opgenomen zodat de e-learning offline blijft werken.
- Dezelfde scene op een andere pagina (onderwerp 4, dezelfde casus) houdt bewust het pictogrambeeld, zodat alleen de gevraagde pagina is gewijzigd.
- Beeldplan, personages A–K, prompts en alt-teksten: `BEELDPLAN.md`. Een foto activeren: zet het bestand in `assets/images/`, voeg de scene-naam toe aan `FOTO_AANWEZIG` in het bouwscript en bouw opnieuw.

## DIDACTISCHE CONTROLE

- Alle 8 onderwerpen zijn nagelopen. De rode draad (de vier vragen) staat in elk onderwerp.
- Theorie wordt gevolgd door een voorbeeld, een praktijkcasus, "Let op" en "Onthoud".
- Taal is B1: korte zinnen en uitleg na elke wettekst ("Wat betekent dit voor jou als boa?").
- Wet, bevoegdheid, domein, beleid en veiligheid zijn visueel van elkaar te onderscheiden.

## TECHNISCHE TEST

Playwright, lokaal en live:

- Volledige doorloop: 178 schermen (intake, 142 pagina's, 30 oefenvragen met feedback, eindtoets, resultaat, certificaat). Geen scriptfouten, geen consolefouten, geen kapotte beelden.
- Regressie op 390 px:
  - hervatten na herladen: scherm "Verdergaan", juiste pagina;
  - eindtoets zakken: geen certificaat, knop "Eindtoets opnieuw maken";
  - opnieuw maken en slagen;
  - certificaat met naam, nummer `JSLF-VW-…` en peildatum;
  - printweergave en PDF (A4 liggend);
  - "Opnieuw beginnen" wist de opslag.
- Opslagsleutel: `jslf-vw-v1`.

## RESPONSIVE TEST

Getest op 1440×900, 1280×800, 1024×768, 768×1024, 390×844 en 360×740: 178/178 schermen, geen horizontaal scrollen, geen elementen buiten beeld.

## VRAGENCONTROLE

- 31 oefenvragen: per onderwerp 6 / 4 / 6 / 7 / 4 / 4.
- Juiste antwoorden verdeeld over A7 / B9 / C8 / D6.
- Elke vraag is een praktijksituatie met een bronvoetnoot. De afleiders zijn gelijkwaardig in vorm en lengte.
- Er komen geen verwijderde onderwerpen in voor (Halt, productvoorbeelden, meters).

## EINDTOETSCONTROLE

- 15 vragen, drempel 80%.
- Spreiding over de thema's:
  - Vier vragen: 1
  - Soorten vuurwerk: 3
  - De wet: 2
  - Aanhouden: 1
  - Bevoegdheid: 2
  - Bevoegdheden: 2
  - Inbeslagneming: 1
  - Taakverdeling: 1
  - Veiligheid: 1
  - Proces-verbaal: 1
- Juiste antwoorden: A3 / B4 / C4 / D4. De volgorde wordt gehusseld.

---

## MENSELIJKE JURIDISCHE CONTROLE NODIG

### 1. Art. 17 WED per individuele akte
- **ONDERWERP:** WED-bevoegdheden van de domein I-boa.
- **VRAAG:** Heeft elke domein I-boa met onderdeel 9 automatisch de bevoegdheden van art. 18–24a WED?
- **WAT ZEGT DE BRON?** Volgens de Beleidsregels boa wordt de titel voor economische delicten verleend op grond van art. 17 lid 1 onder 2° WED. Art. 18–24a WED gelden voor "de opsporingsambtenaren".
- **WAAR ZIT DE TWIJFEL?** Of dit in elke concrete akte of aanwijzing zo is vastgelegd. Ook of de werkgever beperkingen stelt in de taakomschrijving.
- **BRON:** art. 17 WED; Beleidsregels boa (BWBR0039766); Stcrt. 2026, 31362.
- **GEVOLG VOOR DE E-LEARNING:** De cursus geeft de hoofdregel en laat de cursist zijn akte en taakomschrijving controleren. Er staat geen stellige claim voor iedere boa in.
- **ADVIES VOOR CONTROLE:** Laat Justis of de OM-boa-coördinator bevestigen hoe de titel in akten voor onderdeel 9 wordt vermeld.

### 2. Aanhouding buiten heterdaad in de boa-praktijk
- **ONDERWERP:** Art. 54 lid 3 Sv voor boa's.
- **VRAAG:** Mag een boa in de praktijk zelf aanhouden buiten heterdaad, en welke instructie en middelen horen daarbij?
- **WAT ZEGT DE BRON?** Art. 54 lid 1–3 en art. 67 lid 1 onder a Sv: in beginsel op bevel, en zelf alleen als het bevel niet kan worden afgewacht.
- **WAAR ZIT DE TWIJFEL?** De uitvoering hangt af van de instructie van de werkgever en de geweldsmiddelen van de boa. Daar is geen landelijke officiële bron voor gevonden.
- **BRON:** art. 54 en 67 Sv.
- **GEVOLG VOOR DE E-LEARNING:** De cursus leert dat je buiten heterdaad niet zelfstandig aanhoudt, maar overlegt en de politie inschakelt.
- **ADVIES VOOR CONTROLE:** Toets deze lijn aan de werkinstructies van de opdrachtgevers.

### 3. Art. 24a WED en de kofferbak
- **ONDERWERP:** Medewerking vorderen bij onderzoek van een vervoermiddel.
- **VRAAG:** Is "vorderen dat de bestuurder de kofferbak opent" een juiste toepassing van art. 24a WED naast art. 23?
- **WAT ZEGT DE BRON?** Art. 24a lid 1: "alle medewerking ... die deze redelijkerwijs kunnen vorderen bij de uitoefening van de hen krachtens deze titel toekomende bevoegdheden".
- **WAAR ZIT DE TWIJFEL?** Er is geen jurisprudentie of officiële toelichting gevonden over precies dit voorbeeld.
- **BRON:** art. 23, 24a en 26 WED.
- **GEVOLG VOOR DE E-LEARNING:** Het voorbeeld staat erin, met de wettekst en de voorwaarde "redelijkerwijs nodig".
- **ADVIES VOOR CONTROLE:** Laat een OM-jurist het voorbeeld bevestigen.

### 4. Halt en reprimande
- **ONDERWERP:** Afdoening bij jongeren.
- **VRAAG:** Kunnen boa's bij vuurwerkfeiten naar Halt verwijzen of een reprimande geven?
- **WAT ZEGT DE BRON?** Het Handhavingsplan (maart 2026) zegt dat dit "naar verwachting in de loop van 2026" wordt geregeld.
- **WAAR ZIT DE TWIJFEL?** De actuele stand op 20-9-2026 is niet in een officiële bron gevonden.
- **BRON:** Handhavingsplan jaarwisseling, maart 2026.
- **GEVOLG VOOR DE E-LEARNING:** Het onderwerp is volledig verwijderd.
- **ADVIES VOOR CONTROLE:** Controleer de Aanwijzing Halt-afdoening en de Regeling Halt. Voeg het onderwerp alleen toe als het geregeld is.

### 5. Veiligheidsrichtlijn
- **ONDERWERP:** Afstanden, bewaren en afvoeren van in beslag genomen of onbekend vuurwerk.
- **VRAAG:** Welke concrete veiligheidsnormen gelden voor boa's?
- **WAT ZEGT DE BRON?** Er is geen officiële landelijke richtlijn voor boa's gevonden.
- **WAAR ZIT DE TWIJFEL?** Er zijn waarschijnlijk lokale of werkgeversprotocollen.
- **BRON:** geen gevonden.
- **GEVOLG VOOR DE E-LEARNING:** Alleen de algemene boodschap staat erin: veiligheid gaat voor, afstand houden, niet openen of hanteren, politie inschakelen. Er staan geen meters of procedures in.
- **ADVIES VOOR CONTROLE:** Vraag het werkgeversprotocol op en voeg dat als lokale instructie toe.

### 6. Productvorm en categorie
- **ONDERWERP:** Indeling van producttypen in categorieën.
- **VRAAG:** Kan één producttype (fontein, cakebox, pijl) in verschillende categorieën vallen?
- **WAT ZEGT DE BRON?** Art. 1A.1.3 Vuurwerkbesluit: de fabrikant deelt in "op grond van toepassing, doel en gevaar". Een aangemelde instantie bevestigt dat.
- **WAAR ZIT DE TWIJFEL?** De algemene stelling dat een type in meerdere categorieën "kan vallen" is niet letterlijk in een Nederlandse bron gevonden.
- **BRON:** art. 1A.1.3 Vuurwerkbesluit.
- **GEVOLG VOOR DE E-LEARNING:** De stelling is verwijderd. De cursus zegt nu alleen dat de vorm de categorie niet laat zien en dat de fabrikant indeelt.
- **ADVIES VOOR CONTROLE:** Optioneel. Laat een deskundige van de ILT bevestigen of de oorspronkelijke stelling terug mag.
