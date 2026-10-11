# Oplevering e-learning Vuurwerk

## Versie

**0.9.2 — herbouw compacte cursus** (23 september 2026). Nog geen 1.0: de beelden uit `BEELDPLAN.md` zijn nog niet gemaakt en goedgekeurd.

- Juridische peildatum: **12 oktober 2026**.
- Doelgroep: **boa's in domein I**, Europees Nederland.
- Cacheversies in `index.html`: `app.css?v=vw260924a` · `responsive.css?v=vw260925r` · `soorten.css?v=vw261010b` · `app.js?v=vw261010c`.
- Opslag `jslf-vw-v1`, voortgangsversie **30**.
- Stand van de technische gegevens: 11 oktober 2026 (main `6f55979`).
- Backupbranch vóór deze herbouw: `backup-voor-herbouw-compact-2026-09-23` (= commit `619eba5`).
- Basis: `HERZIENINGSRAPPORT_Vuurwerk.md` (23-9-2026) en de beslissingen van Jan van 23-9-2026.
- De oude opleveringsnotities (versie 0.9.1, 145 pagina's) staan in de git-geschiedenis en op de backupbranch.

## Opbouw

| Deel | Pagina's | Oefenvragen |
|---|---|---|
| Goed om te weten (vóór de introductie) | 1 | – |
| Introductie | 3 | – |
| 1 Vuurwerk herkennen | 7 | 3 |
| 2 Wat zegt de wet? | 5 | 3 |
| 3 Wanneer ben jij als boa bevoegd? | 2 | 4 |
| 4 Wat kun je als boa doen? | 10 | 4 |
| 5 Wanneer doe je het niet zelf? | 4 | 2 |
| 6 Praktijkcasus: van melding tot proces-verbaal | 8 | – |
| Eindtoets | – | 15 (13 praktijkcasus, 2 kennisvragen) |
| **Totaal** | **40** | **16 + 15** |

Leerstappen: **56** (40 pagina's en 16 oefenvragen), daarna de eindtoets.

Bij oplevering van 0.9.2 (23-9-2026): 42 pagina's, 18 oefenvragen, 15 eindtoetsvragen.
Was: 145 pagina's, 31 oefenvragen, 15 eindtoetsvragen.

### Pagina's per deel

- **Goed om te weten** (startpagina vóór de introductie): feitcodes nog niet bekend · waarop de e-learning is gebaseerd · lokale afspraken niet opgenomen · nieuwe ontwikkelingen · controleer altijd zelf · juridische peildatum.
- **Introductie:** Een knal op het plein · Na deze cursus weet je wat je moet doen · De vier vragen.
- **1 Vuurwerk herkennen:** Wie bepaalt de categorie? · F1 – Zeer licht vuurwerk · F2 – Vuurwerk met weinig gevaar · F3 – Vuurwerk met middelmatig gevaar · F4 – Professioneel vuurwerk · Verpakking en etiket · Onbekend vuurwerk en veelgebruikte namen.
- **2 Wat zegt de wet?:** De Wet veilige jaarwisseling · Artikel 9.2.2.1a Wm: bezit, gebruik en verkoop · Personen met gespecialiseerde kennis · De ontheffing van de burgemeester · Economisch delict: overtreding of misdrijf?
- **3 Wanneer ben jij als boa bevoegd?:** Domein I, onderdeel 9 · Artikel 17 WED: wanneer mag je de WED-bevoegdheden gebruiken?
- **4 Wat kun je als boa doen?:** Bevoegdheid, verplichting of strafbaarstelling? · Staande houden · Vorderen van inzage in een identiteitsbewijs · Aanhouden op heterdaad · Inbeslagneming en uitlevering vorderen · Inzage van gegevens en bescheiden vorderen · Plaatsen betreden · Zaken onderzoeken en monsters nemen · Vervoermiddel stilhouden en onderzoeken · Medewerking vorderen.
- **5 Wanneer doe je het niet zelf?:** Veiligheid: stop met zelf onderzoeken · Taak en beleid: wat wordt van jou verwacht? · Politie: wanneer schakel je in? · Mogelijk zwaar illegaal vuurwerk.
- **6 Praktijkcasus:** De melding · Wat tref ik aan? · Is dit strafbaar? · Ben ik hiervoor bevoegd? · Wat doe ik nu? · Wat zet ik in het proces-verbaal? · Voorbeeld proces-verbaal · De vier vragen op straat.

## Didactische regels in deze versie

1. Eén regel wordt één keer volledig uitgelegd. Daarna alleen verwijzen of toepassen.
2. De vier vragen zijn het enige denkmodel. De oude vijf/zeven-stappenschema's, de losse "Kort samengevat"-, "Leerdoelen"- en "Vooruitblik"-pagina's zijn vervallen.
3. Elke pagina heeft één label: Herkennen, Wet, Wettelijk bevoegd, Taak/beleid, Veiligheid, Politie of Praktijk. Beleid wordt nooit als bevoegdheidsgrondslag gebruikt.
4. Eén doorlopende casus (plein, 21 november): intro → H1 p8 → H6.
5. Bronvermeldingen (vastgesteld 2-10-2026): bij bronvermeldingen van wet- en regelgeving wordt standaard alleen de wet en het artikel genoemd. Voeg niet automatisch 'geldend vanaf [datum]' toe. Een datum wordt alleen vermeld wanneer de datum zelf juridisch relevant is voor de uitleg, bijvoorbeeld bij de inwerkingtreding van een nieuwe wet of specifieke wetswijziging.

## Techniek

- Inhoud: `index.html` (`window.__DATA__`). Paginaopmaak: `L_SPEC` in `assets/app.js` (sleutel `deel.pagina`, 0-gebaseerd).
- Nieuw in `app.js`: `tLab()` (koppen "Introductie" / "Hoofdstuk n"), `FIG.bevkaart` (bevoegdheid · verplichting · strafbaarstelling), vernieuwde `FIG.beslishulp`. Ongebruikte oude figuren verwijderd.
- Nieuw in `soorten.css`: opmaak bevoegdhedenkaart. `app.css` ongewijzigd.
- **Startpagina 'Goed om te weten'** (sinds 10-10-2026): eerste leerstap (`{type:'info'}` in `buildSteps()`, `infoScreen()` in `app.js`, opmaak `.gotw-*` in `soorten.css`), direct na de welkompagina en vóór de Introductie. Daardoor telt de cursus 56 leerstappen.
- **Voortgang v30 (huidig):** opgeslagen voortgang van v18 t/m v29 wordt bij hervatten omgezet naar de huidige opbouw; bij v29 → v30 schuift de positie één stap op vanwege de nieuwe startpagina. Antwoorden blijven bewaard.
- **Eindtoets (huidig):** 15 vragen. Per poging worden de volgorde van de vragen en de volgorde van de antwoorden geschud (`nieuweEindtoets()`). De beoordeling vergelijkt de gekozen oorspronkelijke antwoordindex met `juist`, niet de getoonde letter. Tijdens de toets geen feedback; slagingsgrens 80%.
- **Nabespreking (huidig, `exResult()`):** overzicht met aantal vragen, goed en fout; per vraag Juist/Onjuist. Bij een goed antwoord één kaart "Jouw antwoord is juist", bij een fout antwoord "Jouw antwoord" en "Juiste antwoord". "Waarom?" altijd zichtbaar; "Meer uitleg" en "Bronnen" standaard ingeklapt. Eén vraag tegelijk open, met vorige/volgende. Opmaak `.nb-*` in `soorten.css`.
- **Voortgang v18:** oude voortgang (v17 of lager) past niet op de nieuwe opbouw. Bij hervatten gaat de cursist naar het startscherm en begint de lesstof opnieuw. **Een eerder behaald certificaat blijft bewaard** (`oudCert`) en is bereikbaar via de knop "Eerder behaald certificaat" op het startscherm, met het oorspronkelijke percentage en certificaatnummer.
- Ongewijzigd: intake, hervatten, oefenvragen met feedback (drempel 70%), eindtoets met gehusselde volgorde, slagingsgrens 80%, resultaat met nabespreking, certificaat (printen/PDF), responsive opmaak.

## Controles (23-9-2026)

- Alle 42 pagina's en 18 oefenvragen automatisch doorlopen op desktop (1366 × 900) en mobiel (390 × 844): geen scriptfouten, alle composities gerenderd.
- Volledige doorloop met juiste antwoorden → eindtoets 100% → certificaat. Herladen → certificaat hervat.
- Hervatten midden in de lesstof werkt.
- Migratie getest: v17 met behaald certificaat → startscherm met certificaatknop, oud percentage en nummer behouden; v17 midden in de cursus → startscherm, antwoorden gewist, geen certificaatknop.
- Zoekcontrole op oude absolute formuleringen: zie `CLAUDE-RAPPORT.md`.

## Eindcontrole 23-9-2026 (tweede ronde)

Gerichte juridische en redactionele correcties, geen herstructurering: zie `CLAUDE-RAPPORT.md` §8. Structuur ongewijzigd (42 · 18 · 15). Cacheversie `vw260923b`.

## Open

- Beelden: zie `BEELDPLAN.md` (19 slots; 10 nieuw, 9 bestaande te controleren).
- Juridische twijfelpunten: zie `CLAUDE-RAPPORT.md`.
