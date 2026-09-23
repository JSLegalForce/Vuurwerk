# Claude-rapport — herbouw e-learning Vuurwerk (0.9.2)

**Datum:** 23 september 2026 · **Juridische peildatum:** 23 september 2026
**Basis:** `HERZIENINGSRAPPORT_Vuurwerk.md` en de beslissingen van Jan van 23 september 2026.
**Backupbranch vóór de herbouw:** `backup-voor-herbouw-compact-2026-09-23` (= `619eba5`).

## Commits

| Commit | Inhoud |
|---|---|
| `c9b23cb` | `assets/app.js` + `assets/soorten.css`: engine-aanpassingen, bevoegdhedenkaart, voortgang v18, cache `vw260923a` |
| `4aaa867` | `index.html`: nieuwe cursusinhoud 0.9.2 (42 pagina's, 18 oefenvragen, 15 eindtoetsvragen) |
| `6a2bc50` | `docs/OPLEVERING.md` en `docs/BEELDPLAN.md` bijgewerkt |
| `d9025ca` | `CLAUDE-RAPPORT.md` |
| `52ce197` | verwijzing naar `docs/BEELDREFERENTIES.md` in `docs/BEELDPLAN.md` |
| `914839c`, `bd91c74`, `d1f0087` | eindcontrole (tweede ronde), zie §8 |

`docs/BEELDSTIJL.md` en `docs/BEELDREFERENTIES.md` zijn **niet** gewijzigd. Er zijn geen afbeeldingen toegevoegd, verwijderd of vervangen.

## 1. Wat is gewijzigd

- **Structuur:** introductie (3) + 5 hoofdstukken met oefenvragen + praktijkcasus (8) + eindtoets. Zie `docs/OPLEVERING.md` voor de volledige paginalijst.
- **Eén denkmodel:** de vier vragen. Verwijderd: vijf-/zevenstappenschema's, 19 "Kort samengevat"-pagina's, 8 leerdoelenpagina's, 6 vooruitblikken, de interne correctiepagina "artikelnummers gecontroleerd". De vier lagen (waarneming/informatie/onderzoek/conclusie) staan alleen nog als inhoud onder vraag 1 (H1 p8), niet als eigen model.
- **Labels:** elke inhoudspagina heeft één label: Herkennen, Wet, Wettelijk bevoegd, Taak/beleid, Veiligheid, Politie of Praktijk.
- **Doelgroep:** in I.2 staat: "Deze e-learning is geschreven voor boa's in domein I en gaat over Europees Nederland." Domein II komt alleen kort voor, bij F4 (H3 p5).
- **Doorlopende casus:** plein, zaterdag 21 november. Intro p1 → H1 p8 → H6 p1–p8. H6 legt geen theorie opnieuw uit; alleen verwijzingen zoals "(art. 52 Sv)".
- **Categoriepagina's F1–F4:** alleen nog herkennen (wat is het, wat zie je, wat weet je nog niet). Verbod, ontheffing en bevoegdheid zijn verplaatst naar H2 en H3.
- **Proces-verbaal:** herbouwd. Het PV noemt nu de gedraging (bezit), onderbouwt het bezit van de tas met waarnemingen, neemt opschriften letterlijk over, noemt de grondslagen, vermeldt de kennisgeving aan de hulpofficier en zegt wat er met het inbeslaggenomen vuurwerk is gebeurd.
- **Techniek:** zie §7.

## 2. Aantallen

| | Oud (0.9.1) | Nieuw (0.9.2) |
|---|---|---|
| Pagina's | 145 | **42** |
| Oefenvragen | 31 | **18** |
| Eindtoetsvragen | 15 | **15** (13 praktijkcasus, 2 kennisvragen) |
| Woorden in de lesstof (zonder wetteksten en bronnen) | ca. 13.900 | **ca. 4.500** |

## 3. Juridische wijzigingen

| # | Oud | Nieuw | Bron |
|---|---|---|---|
| 1 | "Domein I noemt één concreet feit." | Onderdeel 9 is het vuurwerkspecifieke onderdeel. Nergens staat meer dat het het enige is. | Regeling domeinlijsten, Domein I (8-9-2026) |
| 2 | F4: in de praktijk "nooit bevoegd". | "Onderdeel 9 geeft geen algemene bevoegdheid voor feiten uit het Vuurwerkbesluit over F4." Plus één zin over onderdeel 21 (opdracht OvJ) en één zin dat domein II anders is. | Idem, onderdelen 9 en 21 |
| 3 | Beleidsregels boa als bron van de WED-bevoegdheden. | Grondslag: art. 17 lid 1 onder 2° en lid 3 WED jo. de Regeling domeinlijsten ("gelet op … art. 17, derde lid" WED). Beleidsregels alleen genoemd als beleid, niet als grondslag. | WED art. 17; aanhef Regeling domeinlijsten |
| 4 | Art. 24a WED = bevoegdheid "medewerking vorderen". | Lid 1 = medewerkingsplicht; lid 3 = bevoegdheid tot feitelijk handelen; art. 26 = strafbaarstelling. Apart in de bevoegdhedenkaart (H4 p1) en H4 p5. | WED art. 24a, 26 |
| 5 | Eindtoetsvraag 11 rekende "zelf openbreken" fout zonder art. 24a lid 3. | Vervangen door een vraag met één verdedigbaar antwoord (art. 26 WED strafbaarstelling; optie "24a lid 1 is jouw bevoegdheid" is fout). | Idem |
| 6 | F1 "mag het hele jaar worden afgestoken". | Alleen: valt niet onder art. 9.2.2.1a Wm; minimumleeftijd 12 jaar bij verkoop. | Wm 9.2.2.1a; Vb 2.3.5, 2.3.7 |
| 7 | "Boa's in domein I zijn bevoegd…" op herkenpagina's. | Weg van de herkenpagina's; bevoegdheid alleen in H3, altijd met "voor zover noodzakelijk voor functie en taakomschrijving". | Domein I, aanhef |
| 8 | "Zwaar illegaal vuurwerk" als categorie en in titels. | Vervangen door "onbekend of mogelijk zwaar vuurwerk" en "professioneel vuurwerk" (juridisch begrip). "Illegaal" staat alleen nog in het foute PV-voorbeeld en in een fout antwoord (bewust). | Vb 1.1.1 |
| 9 | Samenloop ontbrak. | H2 p5 en H3 p5: art. 9.2.2.1a Wm naast art. 1.2.2, 1.2.3, 1.2.4 en 1.2.5 Vb; boa spoort het feit op waarvoor hij bevoegd is. | Vb; WED 1a |
| 10 | Handhavingsplan "achterhaald". | Alleen de bevoegdhedenpassage is ouder dan de domeinlijst. De beleidslijn staat onder Taak/beleid, samen met de nota van toelichting bij het Besluit veilige jaarwisseling (Stb. 2026, 168). | Handhavingsplan maart 2026; Stb. 2026, 168 |
| 11 | Inwerkingtreding zonder primaire bron. | Stb. 2026, 169 (door Jan gecontroleerd): in werking met ingang van 1 augustus 2026. | Stb. 2026, 169 |
| 12 | Personen met gespecialiseerde kennis zonder lid 2. | Lid 2 (aanwijzing in andere EU-lidstaat) toegevoegd. | Vb 1.1.2a |
| 13 | Art. 96 lid 2 Sv bij "veiligstellen". | Geschrapt. Blijft: "veiligstellen" is geen aparte bevoegdheid. | Sv 96 |
| 14 | Kennisgeving van inbeslagneming zonder hulpofficier. | Kennisgeving zo snel mogelijk naar de hulpofficier. | Sv 94 lid 3 |
| 15 | Uitleg "bezit/gebruik" zonder bron. | Onderbouwd met de aanhef van de Wet veilige jaarwisseling ("voorhanden hebben en afsteken van vuurwerk door consumenten"). | Stb. 2026, 7 |
| 16 | Ontheffingsvoorschriften. | Niet onderwezen als vaste regel onder onderdeel 9. H2 p4 en eindtoetsvraag 5: "leg vast en overleg". | beslissing Jan (C5) |

Alle geciteerde wetteksten zijn letterlijk vergeleken met wetten.overheid.nl (Wm en Vb: geldend 1-8-2026; WED: 1-8-2026; Sv: 1-7-2026; Regeling domeinlijsten: 8-9-2026; Beleidsregels boa: 1-9-2026) en officielebekendmakingen.nl (Stb. 2026, 7 en 168; Stcrt. 2026, 31362). Handhavingsplan-citaten zijn letterlijk teruggevonden in de pdf van maart 2026.

## 4. Pagina's die nog een afbeelding nodig hebben

Zie `docs/BEELDPLAN.md` (19 slots). **Nieuw te maken (CONCEPT):**

- H1 p6 Verpakking en etiket;
- H2 p4 Ontheffing;
- H4 p2 Staande houden;
- H4 p5 Vervoermiddel;
- H4 p6 Inbeslagneming;
- H5 p1 Veiligheid;
- H5 p4 Drie situaties;
- H5 p5 Overdracht;
- H6 p1 De melding (nu tijdelijk hergebruik);
- H6 p2 Detail doos en tas.

**Bestaand, te controleren tegen BEELDSTIJL (CONTROLEREN):** intro p1, H1 p1–p5, H1 p7, H1 p8, H3 p5. Opvallend: `cat-f4-vlinder.webp` toont een merknaam (VIPER), `cat-f4-cobra.webp` de tekst "COBRA 6". Ook de generieke boa-illustraties (`boa-hero*.webp`) moeten tegen BEELDSTIJL §3–5 en BEELDREFERENTIES worden gecontroleerd.

## 5. Resterende twijfelpunten

1. **Ontheffingsvoorschriften en onderdeel 9.** Het Vuurwerkbesluit berust mede op art. 9.2.2.1a Wm (art. IIb Wet veilige jaarwisseling). Of overtreding van ontheffingsvoorschriften (art. 2.3.2a Vb) valt onder "art. 9.2.2.1a Wm jo. art. 1a WED" in onderdeel 9, volgt niet uit de primaire tekst. Niet onderwezen. Advies: navragen bij OM of JenV.
2. **WED-status via de domeinlijst.** Art. 17 lid 1 onder 2° en lid 3 WED en de aanhef van de Regeling domeinlijsten ("gelet op … art. 17, derde lid") maken een WED-aanwijzing via een domein mogelijk. Een bepaling die vaststelt dat élke domein I-akte met onderdeel 9 die aanwijzing omvat, is niet gevonden. Sinds de eindcontrole formuleert de cursus dit daarom voorwaardelijk (H3 p4, H6 p4): de WED-bevoegdheden alleen als je akte je voor dit economische delict aanwijst — "controleer je akte". In de praktijkcasus is dat een uitdrukkelijk benoemde aanname.
3. **Aangepast of zelfgemaakt F2/F3-vuurwerk.** Of aangepast vuurwerk nog "vuurwerk van categorie F2/F3" is in de zin van art. 9.2.2.1a Wm, is niet in de wettekst beantwoord. De cursus zegt: niet gokken, veiligheid en politie gaan voor.
4. **Lokale APV's** zijn niet gecontroleerd. De cursus noemt ze niet als bevoegdheidsgrondslag. Er is geen APV-module, zoals afgesproken.
5. **Art. 67 Sv:** wetten.overheid.nl meldt een toekomstige wijziging per 1 maart 2027. Vóór die datum opnieuw controleren.
6. **Kamerstuk 35 386** (memorie van toelichting) is niet opnieuw gelezen. De uitleg van bezit/gebruik steunt op de aanhef van de wet.

## 6. Kwaliteitscontrole (uitgevoerd vóór de commit)

| # | Controle | Uitkomst |
|---|---|---|
| 1 | Juridische juistheid | Alle artikelen tegen de primaire bronnen (§3). Functie per artikel gecontroleerd: bevoegdheid (52, 53, 54 Sv; 18, 21, 23, 24a lid 3 WED), verplichting (24a lid 1 WED), strafbaarstelling (26 WED). |
| 2 | Dubbele uitleg | Iedere regel één keer volledig. Verwijzingen staan als "(hoofdstuk n)" of alleen een artikelnummer. |
| 3 | B1-taal | Korte zinnen, "je"-vorm, jargon uitgelegd (juncto, NEM, aangemelde instantie). |
| 4 | Paginalengte | 31 van 42 pagina's ≤ 120 woorden. Langer: 4 categoriepagina's en de categorie-overzichtspagina (veel beeldlabels, 124–187 woorden), H2 p4 ontheffing (checklist, 150), H3 p4 art. 17 WED (123), H3 p5 "Welk feit?" (visuele kaarten, 225), H4 p4 en p5 (wettekst, 126–135) en het PV-voorbeeld (296: het PV zelf). |
| 5–7 | Verwijzingen, oude paginanummers en hoofdstuknamen | Geen "onderwerp n", "O2 p…", "Kort samengevat", "Vooruitblik" of oude titels in inhoud of code. Koppen tonen "Introductie" / "Hoofdstuk n", de balk "Deel n van 7". |
| 8 | Meerduidige vragen | Alle 33 vragen nagelopen op één verdedigbaar antwoord; de oude eindtoetsvraag 11 is vervangen. |
| 9 | Wet/bevoegdheid/beleid/veiligheid/politie | Labels per pagina; beleid alleen onder Taak/beleid en Politie. |
| 10–11 | Desktop en mobiel | Playwright-screenshots van alle 60 schermen (42 pagina's + 18 vragen) op 1366 × 900 en 390 × 844: geen scriptfouten, alle composities gerenderd. |
| 12 | Voortgang en hervatten | Herladen midden in de lesstof: hervat op dezelfde pagina. |
| 13 | Eindtoets | Volledige doorloop, 100% → GESLAAGD. |
| 14 | Certificaat | Getoond en na herladen hervat. Migratie v17 → v18: een eerder behaald certificaat (87%, nr. behouden) blijft bereikbaar via "Eerder behaald certificaat". Onvoltooide v17-voortgang → startscherm, antwoorden gewist. |

**Zoekcontrole oude absolute formuleringen** (volledige code, elke treffer handmatig beoordeeld):

- **"nooit bevoegd" (6 treffers):** allemaal ontkenningen of foute antwoordopties ("Dus nooit: «…nooit bevoegd.»", "beleid maakt je nooit bevoegd"). In orde.
- **"F4 =":** 0 treffers.
- **"boa's zijn bevoegd":** 0 treffers. "zijn bevoegd" komt alleen voor in de letterlijke wettekst van art. 23 WED.
- **"24a = bevoegdheid" / "Medewerking vorderen":** 0 treffers.
- **"illegaal vuurwerk" (2 treffers in de inhoud):** het foute PV-voorbeeld en een fout antwoord in de eindtoets, allebei bewust als slecht voorbeeld. "Illegale handel" staat in een parafrase van het Handhavingsplan. Een ongebruikte alt-tekst in `app.js` is verwijderd.
- **"veiligstellen":** alleen in "«Veiligstellen» is geen aparte bevoegdheid". Het oude `BD_KERN`-label is aangepast.

## 7. Techniek

- `app.js`:
  - `ASSET_V` `vw260923a`;
  - `TOPIC_ICON` voor 7 delen;
  - `tLab()` voor de koppen;
  - nieuwe `L_SPEC` (42) en `Q_ART` (18);
  - `FIG` teruggebracht tot `bevkaart` en `beslishulp`;
  - `ART_FILE`/`ART_ALT` `foto-onbekend`;
  - voortgang v18 met `oudCert`;
  - `certificaat(pct, oud)`.
- `soorten.css`: opmaak bevoegdhedenkaart (+ responsive) en een driekoloms notitieregel voor de beslishulp.
- `app.css`: ongewijzigd.
- Behouden: intake, hervatten, oefenvragen + feedback (70%), eindtoets (gehusseld, 80%), resultaat met nabespreking, certificaat/print en responsive layout. Aan de launcher is niets gewijzigd.

## 8. Eindcontrole 23 september 2026 (tweede ronde)

Opdracht: alleen gerichte controle en noodzakelijke correcties; geen herstructurering, geen beeldgeneratie, geen onnodige techniek. Structuur blijft **42 pagina's · 18 oefenvragen · 15 eindtoetsvragen**.

Gelezen vooraf: `CLAUDE-RAPPORT.md`, `docs/OPLEVERING.md`, `docs/BEELDSTIJL.md`, `docs/BEELDREFERENTIES.md`, `docs/BEELDPLAN.md`, de volledige inhoud van `index.html` (alle pagina's, oefenvragen en eindtoetsvragen), `assets/app.js` en `assets/soorten.css`.

### 8.1 Uitkomst van de controle

**Moest worden gecorrigeerd**

| # | Plaats | Probleem | Correctie | Bron |
|---|---|---|---|---|
| 1 | H3 p4 (art. 17 WED) | "Geeft jouw akte je onderdeel 9, dan ben je … WED-opsporingsambtenaar" was stelliger dan de bronnen toelaten. | Voorwaardelijk: WED-bevoegdheden alleen als je voor dit economische delict bent aangewezen als opsporingsambtenaar in de zin van art. 17 WED; "controleer je akte". | WED art. 17; aanhef Regeling domeinlijsten |
| 2 | H6 p4 (casus, vraag 3) | Zelfde stellige formulering; functie/taak als vaststaand feit gepresenteerd. | Voorwaardelijk + uitdrukkelijke casusaanname ("In deze casus gaan we ervan uit … Controleer dat in je eigen akte"). | idem |
| 3 | H3 p2, H3 p3 | Bevoegdheid via onderdeel 9 zonder koppeling aan de akte. | "Verwijst je akte naar domein I, dan …". | Sv art. 142 lid 2; Domein I aanhef |
| 4 | H3 p3 | Onderdeel 9 kon worden gelezen als het enige relevante onderdeel. | Eén alinea: ook andere onderdelen kunnen een rol spelen, bijv. een APV-bepaling waarvoor je bent aangewezen (verschilt per gemeente) of onderdeel 21; kijk naar akte, taak en concreet feit. De "Níet"-opsomming is een alinea geworden, omdat de lijstweergave er vinkjes bij toonde (misleidend bij "niet"). | Domein I, onderdelen 6 en 21 |
| 5 | H3 p5 ("Welk feit?") | De introzin was een reeks van vijf stappen (risico op concurrerend model) en de F2/F3-kaart kon lezen als "F2/F3 = bevoegd". | Introzin gekoppeld aan vraag 1–3 van de vier vragen. F2/F3-kaart: alleen bij bezit/gebruik/verkoop zonder uitzondering kan art. 9.2.2.1a zijn overtreden; voor dát feit bevoegdheid binnen akte, functie en taak. F1-kaart: "Is het echt F1 …". | Wm 9.2.2.1a; Domein I |
| 6 | H3 p5 (beeldkaart) | Het vijfde rondje "Onbekend" naast F1–F4 kon een wettelijke categorie suggereren. | Onderschrift "Niet vast te stellen · geen wettelijke categorie"; kaarttitel "Categorie niet vast te stellen" met de zin "«Onbekend vuurwerk» is geen wettelijke categorie." | Vb 1A.1.3 |
| 7 | H5 p4 (situatie 1) | "Op de verpakking staat F2 … Je bent bevoegd" — categorie → bevoegdheid. | Toegevoegd: geen ontheffing, geen gespecialiseerde kennis; bevoegd "voor dit feit (art. 9.2.2.1a Wm)". | Wm 9.2.2.1a |
| 8 | H6 p7 (PV zo wel) | Ontbrak: identiteitsgegevens, periode van onafgebroken waarneming (onderbouwing bezit tas), waar de boa de etiketten in de tas las, afwezigheid van aanwijzingen voor gespecialiseerde kennis, registratie na overbrenging. | Aangevuld met die feitelijke elementen. Niet ingekort. | Sv 27a, 52, 94; WED 18; Wm 9.2.2.1a; Vb 1.1.2a |
| 9 | Eindtoetsvraag 8 (samenloop) | Stam kon lezen als "F3 op etiket → bevoegd"; uitleg te stellig. | Stam: "iemand zonder gespecialiseerde kennis … op het etiket «F3»"; vraag: "voor welk feit *kan* onderdeel 9 je bevoegd maken?"; uitleg: binnen akte, functie en taak; etiket blijft informatie. | Domein I; Wm 9.2.2.1a |
| 10 | H1 p2 (F1) | CE-markering genoemd zonder bron. | Bron toegevoegd: art. 1A.4.1 Vuurwerkbesluit (gecontroleerd op wetten.overheid.nl). | Vb 1A.4.1 |

**Kon blijven staan (gecontroleerd)**

- Inwerkingtreding: overal 1 augustus 2026, met Stb. 2026, 169 als primaire bron (H2 p1). Geen afwijkende datum gevonden. Geen twijfelpunt meer.
- F4-formulering (H3 p5, oefenvraag H3-2, eindtoetsvraag 7): genuanceerd; geen "nooit bevoegd" behalve als ontkenning of fout antwoord; onderdeel 21 en domein II elk één zin.
- Art. 24a WED: overal lid 1 = plicht, lid 3 = bevoegdheid, art. 26 = strafbaarstelling (H4 p1, H4 p5, oefenvraag H4-2, eindtoetsvraag 10). Nergens lid 1 als bevoegdheid, behalve als bewust fout antwoord.
- Ontheffingsvoorschriften: H2 p4 en eindtoetsvraag 5 vragen alleen "vastleggen en overleggen"; de omstreden bevoegdheidsvraag wordt niet getoetst. Het afsteektijdstip zelf (art. 2.3.2a lid 3 onder a Vb) is geen twijfelpunt.
- Aangepast/zelfgemaakt vuurwerk: H1 p7, H5 p1, oefenvraag H5-1, eindtoetsvragen 2 en 13 — niet gokken, beschrijven, veiligheid, politie.
- APV: alleen genoemd als fout antwoord of (nieuw) als per gemeente verschillend voorbeeld; nergens landelijke grondslag.
- Art. 67 Sv: geldende tekst per 1 juli 2026 gebruikt; geen toekomstige tekst.
- Vier vragen: enige denkmodel; het "vier lagen"-gebruik in H1 p8 blijft inhoud onder vraag 1.
- Eindtoets: per vraag A–F nagelopen. Eén wijziging (vraag 8). Toetsbeelden zijn neutrale illustraties die het antwoord niet verraden. 13 van 15 casusvragen.

**Blijft open / niet zeker** — zie §5, punten 1–6 (punt 2 aangescherpt, zie boven).

### 8.2 Beeldplan (alleen tekstcorrecties, geen beelden)

`docs/BEELDPLAN.md`:
- 04-06 neutraler: dozen liggen stabiel op een ondergrond, administratieve afhandeling, geen onnodige fysieke handeling met vuurwerk, geen gesuggereerde bevoegdheid;
- 01-05: `cat-f4-vlinder.webp` (VIPER) en `cat-f4-cobra.webp` (COBRA 6) → **CONTROLEREN · kandidaat VERVANGEN**, niet definitief;
- regel toegevoegd dat een praktijknaam-beeld nooit F4 bewijst;
- regel toegevoegd dat tekst in (AI-)beelden nooit een juridische bron is;
- uitgeschreven: de statussen, primaire stijlreferentie tegenover scenereferentie, de harde boa-regels en de continuïteitsregels van de doorlopende casus.

Niet gewijzigd: `docs/BEELDSTIJL.md`, `docs/BEELDREFERENTIES.md` en alle bestanden in `assets/images/` en `assets/reference/`. Er zijn geen beelden gegenereerd, vervangen, hernoemd of verwijderd.

### 8.3 Techniek

Alleen:
- de icoonreeks van H3 p3 in `L_SPEC` (`"kruis"` → `"domein"`, zodat de nieuwe alinea geen kruisje krijgt);
- de cachesleutel `vw260923a` → `vw260923b` in `app.js` en `index.html`.

Voortgang v18, migratie, intake, hervatten, oefenvragen, eindtoets-engine, 80%-grens, certificaatnummer, print/PDF, responsive opmaak en launcher zijn **niet** aangeraakt.

### 8.4 Opnieuw uitgevoerde tests

- **Alle schermen:** 42 pagina's + 18 oefenvragen doorlopen op desktop (1366 × 900) en mobiel (390 × 844). Geen scriptfouten, alle composities gerenderd. H3 p3 en H3 p5 visueel gecontroleerd.
- **Eindtoets en certificaat:** volledige doorloop met juiste antwoorden, eindtoets 100% (GESLAAGD), certificaat.
- **Herladen:** het certificaat wordt hervat.
- **Hervatten:** midden in de lesstof hervat de cursist op dezelfde pagina.
- **Migratie v17 met certificaat:** het oude certificaat blijft zichtbaar (87%, nummer JSLF-VW-2026-ABC123 behouden).
- **Migratie v17 onvoltooid:** de cursist gaat naar het startscherm, de antwoorden zijn gewist en er is geen certificaatknop.
- **Zoekcontrole:** herhaald op "WED-opsporingsambtenaar", "WED-bevoegdheden", "ben je bevoegd", "je bent bevoegd", "24a lid 1", "APV", "onbekend", "illegaal" en "nooit bevoegd". Resterende treffers zijn uitsluitend:
  - voorwaardelijke formuleringen;
  - vraagstammen ("Je bent bevoegd. Het vuurwerk is …");
  - bewust foute antwoordopties;
  - het foute PV-voorbeeld.

### 8.5 Commits van deze ronde

| Commit | Inhoud |
|---|---|
| `914839c` | `assets/app.js`: iconen H3 p3, cache `vw260923b` |
| `bd91c74` | `docs/BEELDPLAN.md`, `docs/OPLEVERING.md` |
| `d1f0087` | `index.html`: juridische en redactionele correcties |
| *deze commit* | `CLAUDE-RAPPORT.md` bijgewerkt |
