# Beeldplan e-learning Vuurwerk

Versie 0.9.2 (herbouw compacte cursus, na eindcontrole) · juridische peildatum 23 september 2026 · bijgewerkt 23 september 2026.

> **Leidend document:** `docs/BEELDSTIJL.md`. Dit beeldplan volgt die stijl en wijzigt haar niet. Bij verschil gaat `BEELDSTIJL.md` voor.
>
> **Visuele referentie:** `docs/BEELDREFERENTIES.md` (primaire stijlreferentie `assets/reference/jslf-beeldstijl-hoofdreferentie.jpg`). Volgorde bij tegenstrijdigheid, zoals daar vastgelegd: juridisch gecontroleerde cursusinhoud → `BEELDSTIJL.md` → primaire stijlreferentie → dit beeldplan → secundaire scenereferentie.
>
> **Vervangt** het vorige beeldplan (42 beelden, gekoppeld aan de oude cursus van 145 pagina's). Dat plan is vervallen: de oude pagina's bestaan niet meer. Het staat nog in de git-geschiedenis en op branch `backup-voor-herbouw-compact-2026-09-23`.
>
> **Rolverdeling (BEELDSTIJL §13–14):** ChatGPT maakt en controleert de beelden. Claude genereert of vervangt géén definitieve beelden en plaatst alleen beelden met status **GOEDGEKEURD**.

---

## 1. Uitgangspunten

- **Functioneel, niet decoratief.** Elk beeld heeft minstens één functie: *herkennen*, *praktijksituatie verduidelijken*, *veiligheid verduidelijken* of *doorlopende casus ondersteunen*.
- **Geen beeld op elke pagina.** 19 beeldslots voor 42 pagina's. Wettekst-, bevoegdheids- en toetspagina's krijgen geen nieuw beeld; daar staan iconen en schema's in HTML.
- **Stijl:** zoals `BEELDSTIJL.md` §2–8 en de **primaire stijlreferentie** uit `BEELDREFERENTIES.md`: de losse afbeelding met twee Nederlandse boa's en jongeren. Dus: hoogwaardige semi-realistische digitale illustratie, volwassen en professioneel, realistische anatomie, verfijnde lijnvoering, zachte schaduwen, natuurlijke rijke kleuren, geloofwaardige Nederlandse omgeving. Het overzicht/collage met meerdere situaties is **alleen een scenereferentie**, nooit de stijlreferentie.
- **Boa-uiterlijk (harde regels):** Nederlands gemeentelijk handhavingsuniform, donkerblauw, high-visibility geel waar dit bij het uniform hoort, HANDHAVING waar passend, correct BOA-mouwembleem (geen verzonnen logo, geen politie-embleem), geen Amerikaans uniform, geen vuurwapen, realistische functionele koppel; zichtbare handboeien zijn conventionele metalen handboeien met twee ronde/ovale boeidringen, geen grote ronde fantasiehouders. De boa pakt onbekend of mogelijk gevaarlijk vuurwerk niet zonder inhoudelijke reden vast.
- **Veiligheid in beeld:** nooit een handhaver die onbekend of mogelijk zwaar vuurwerk aanraakt, opent of uit elkaar haalt.
- **Tekst in beeld:** zo min mogelijk. Toegestaan waar functioneel: `F1` `F2` `F3` `F4`, `Geschikt voor particulier gebruik`, `CE`, `NEM`, `HANDHAVING`. Geen verzonnen of onnodige merknamen. Alle andere tekst komt via HTML.
- **Tekst in een (AI-)afbeelding is nooit een juridische bron.** Categorie, CE-markering, NEM, leeftijd, productomschrijving, waarschuwing of merknaam in beeld ondersteunen alleen visueel. Juridisch telt alleen wat de cursustekst uit een gecontroleerde bron onderwijst.
- **Praktijknamen:** een beeld van een «cobra», «nitraat», «vlinder» of vergelijkbare praktijknaam bewijst nooit zelfstandig dat iets F4 is. De cursus leert: categorie vaststellen uit betrouwbare informatie, niet uit naam of uiterlijk.
- **Onbekend vuurwerk:** geen beeld mag suggereren dat «onbekend vuurwerk» een wettelijke categorie naast F1–F4 is.
- **Doorlopende casus (00-01, 01-08, 06-01, 06-02):** hetzelfde Nederlandse plein, dezelfde mannelijke en dezelfde vrouwelijke boa, dezelfde vier jongeren, dezelfde jongen in de **rode jas**, dezelfde **zwarte sporttas**, dezelfde algemene kleding en dezelfde tijd en omgeving (avond, november). Claude wijzigt deze personages of omgeving niet zelfstandig. Andere situaties gebruiken andere personages.
- **Formaat:** lesbeeld 4:3 (1600 × 1200) of 3:2 (1800 × 1200); productbeeld 2:3 (800 × 1200). Belangrijkste onderwerp in het midden (60%) voor mobiele uitsnede. WebP, kwaliteit ca. 80.
- **Naamgeving (BEELDSTIJL §12):** `HH-PP-omschrijving.webp`, waarbij `HH` het hoofdstuk is (00 = introductie) en `PP` de pagina. Map: `assets/images/`.

## 2. Statussen (BEELDSTIJL §13)

`CONCEPT` · `CONTROLEREN` · `GOEDGEKEURD` · `VERVANGEN`

- **CONCEPT** = niet plaatsen.
- **CONTROLEREN** = bestaand beeld blijft voorlopig staan, maar is nog niet definitief goedgekeurd.
- **GOEDGEKEURD** = mag worden geïmplementeerd.
- **VERVANGEN** = niet meer gebruiken zodra de goedgekeurde vervanging aanwezig is.

Een nieuw productiebeeld wordt alleen geplaatst als het hier de status **GOEDGEKEURD** heeft. Definitieve cursusbeelden staan in `assets/images/`. Referentiebeelden in `assets/reference/` worden nooit rechtstreeks in de cursus getoond.

## 3. Beeldslots

| Slot | Pagina | Functie | Nu in de cursus | Status |
|---|---|---|---|---|
| **00-01** `00-01-knal-op-het-plein.webp` | Intro 1 · Een knal op het plein | casus | `plein-knal.webp` | CONTROLEREN |
| **01-01** `01-01-categorieen-f1-f4.webp` (4 deelbeelden) | H1 p1 · Wie bepaalt de categorie? | herkennen | `wet-f1…f4.webp` | CONTROLEREN |
| **01-02** `01-02-categorie-f1.webp` (3 productbeelden) | H1 p2 · F1 | herkennen | `cat-f1-*.webp` | CONTROLEREN |
| **01-03** `01-03-categorie-f2.webp` (3 productbeelden) | H1 p3 · F2 | herkennen | `cat-f2-*.webp` | CONTROLEREN |
| **01-04** `01-04-categorie-f3.webp` (3 productbeelden) | H1 p4 · F3 | herkennen | `cat-f3-*.webp` | CONTROLEREN |
| **01-05** `01-05-categorie-f4.webp` (3 productbeelden) | H1 p5 · F4 en professioneel vuurwerk | herkennen | `cat-f4-*.webp` (`cat-f4-vlinder.webp`: VIPER · `cat-f4-cobra.webp`: COBRA 6) | CONTROLEREN · kandidaat VERVANGEN |
| **01-06** `01-06-etiket-verpakking.webp` | H1 p6 · Verpakking en etiket | herkennen | — (wetboek-icoon) | CONCEPT |
| **01-07** `01-07-onbekend-vuurwerk.webp` | H1 p7 · Onbekend vuurwerk en praktijknamen | herkennen · veiligheid | `concl-onbekend.webp` | CONTROLEREN |
| **01-08** `01-08-plein-tas-waarnemen.webp` | H1 p8 · Terug naar het plein | casus | `boa-jongeren-plein.webp` | CONTROLEREN |
| **02-04** `02-04-afsteekterrein-ontheffing.webp` | H2 p4 · De ontheffing van de burgemeester | praktijksituatie | — (wetboek-icoon) | CONCEPT |
| **03-05** `03-05-categorie-geen-conclusie.webp` (samengesteld) | H3 p5 · Welk feit? | herkennen | `concl-*.webp` | CONTROLEREN |
| **04-02** `04-02-staande-houden.webp` | H4 p2 · Aanspreken en staande houden | praktijksituatie | — (wetboek-icoon) | CONCEPT |
| **04-05** `04-05-auto-kofferbak.webp` | H4 p5 · Vervoermiddel | praktijksituatie | — (wetboek-icoon) | CONCEPT |
| **04-06** `04-06-inbeslagneming.webp` | H4 p6 · Inbeslagneming en uitlevering | praktijksituatie | — (wetboek-icoon) | CONCEPT |
| **05-01** `05-01-afstand-onbekend-vuurwerk.webp` | H5 p1 · Veiligheid | veiligheid | — (iconen) | CONCEPT |
| **05-04** `05-04-drie-situaties.webp` (drieluik) | H5 p4 · Zelf, overleggen of politie? | praktijksituatie · veiligheid | — (iconen) | CONCEPT |
| **05-05** `05-05-overdracht-politie.webp` | H5 p5 · Een goede overdracht | praktijksituatie | — (iconen) | CONCEPT |
| **06-01** `06-01-melding-plein.webp` | H6 p1 · De melding | casus | `boa-jongeren-plein.webp` (tijdelijk hergebruik) | CONCEPT |
| **06-02** `06-02-doos-en-tas-detail.webp` | H6 p2 · Vraag 1 — Wat tref ik aan? | casus · herkennen | — (boa-illustratie) | CONCEPT |

**Totaal: 19 slots.** 9 slots hebben een bestaand beeld dat gecontroleerd moet worden (CONTROLEREN). 10 slots vragen een nieuw beeld (CONCEPT); 06-01 gebruikt tot die tijd tijdelijk `boa-jongeren-plein.webp`.

Geen nieuw beeld nodig: alle wettekstpagina's (H2 p2, p3, p6 · H3 p1, p2, p4 · H4 p3, p4), de schema's (H4 p1 bevoegdhedenkaart, H6 p8 vier vragen), H2 p1, H2 p5, H3 p3, H4 p7, H5 p2, H5 p3, H6 p3–p7, alle oefenvragen en de eindtoets. Daar blijven de bestaande iconen, schema's en neutrale illustraties staan.

## 4. Beschrijving per slot

**00-01 · Knal op het plein** — Avond, Nederlands plein met klinkers en straatverlichting. Vier jongeren (circa 17–20 jaar) bij elkaar; één jongen in een rode jas gooit een lege kartonnen huls op de grond; voor zijn voeten een open zwarte sporttas met dozen en losse voorwerpen. Op de achtergrond twee boa's (man en vrouw) die aan komen lopen. Lichte rookwolk. Geen vuurwerk in handen van boa's.

**01-01 · Categorieën F1–F4** — Vier losse productbeelden, neutrale achtergrond: F1 sterretjes; F2 kleine cake/rollen; F3 grotere cake of vuurpijlen; F4 professionele shells in een kist. Elk met een klein, leesbaar categorie-etiket. Geen merknamen.

**01-02 t/m 01-05 · Categoriepagina's** — Per categorie drie productbeelden (2:3), zelfde lichtval en achtergrond, zodat de vier pagina's één reeks vormen. F4: namen als cobra, nitraat en vlinder worden in de HTML als *praktijknaam* aangeduid; het beeld suggereert geen categorie die niet vaststaat.

**01-06 · Etiket en verpakking** — (Tekst op de verpakking is illustratie, geen bron: de cursustekst op H1 p6 onderwijst de etiketgegevens uit art. 2.1.3 Vuurwerkbesluit.) Close-up van de zijkant van een doos consumentenvuurwerk: `F2`, `Geschikt voor particulier gebruik`, `CE`, `NEM`, minimumleeftijd en een regel gebruiksaanwijzing (onleesbaar mag). Functie: laten zien wat de boa letterlijk overneemt.

**01-07 · Onbekend vuurwerk** — Enkele grote, met grijze tape omwikkelde voorwerpen zonder etiket op straat of in een tas. Geen persoon die ze vasthoudt. Functie: herkennen dat je de categorie niet kunt vaststellen.

**01-08 · Plein: waarnemen** — Zelfde plein en personages als 00-01. Boa staat op enige afstand en kijkt naar de open tas; collega houdt de groep in het oog. Notitieblok zichtbaar. Niets aanraken.

**02-04 · Afsteekterrein met ontheffing** — Oudejaarsavond, afgezet sportveld met hekken/lint; supervisor met vuurwerkbril; op een tafeltje bij de ingang een map met het afschrift van de ontheffing. Boa in gesprek met de supervisor. Geen gevaarlijke situatie.

**04-02 · Staande houden** — Boa vraagt een jongere (andere persoon dan de casus) om zijn identiteitsbewijs; rustige straat. Het gaat om identiteit vaststellen, niet om aanhouden: geen handboeien in gebruik.

**04-05 · Auto en kofferbak** — Geparkeerde auto met open kofferbak; bestuurder opent op verzoek; boa staat naast de auto. In de kofferbak een paar dozen. Geen boa die in de kofferbak grijpt.

**04-06 · Inbeslagneming** — Enkele gesloten vuurwerkdozen liggen stabiel op een geschikte ondergrond. De boa verricht de administratieve afhandeling van de inbeslagneming en legt gegevens vast; een collega noteert. Het beeld ondersteunt beslag en correcte vastlegging, zonder een onnodige of mogelijk onveilige fysieke handeling met vuurwerk te suggereren. Het beeld suggereert geen bevoegdheid die niet uit de cursustekst blijkt.

**05-01 · Afstand bij onbekend vuurwerk** — Open tas met onbekende, met tape omwikkelde voorwerpen op de grond; boa's houden duidelijk afstand en gebaren omstanders weg te blijven; één boa spreekt in de portofoon. Geen afstanden in meters in beeld.

**05-04 · Drie situaties (drieluik)** — (1) Woonstraat in oktober, man steekt een fontein af, boa spreekt hem rustig aan. (2) Park, verlaten tas met verpakt en los vuurwerk, boa belt op afstand. (3) Stationsplein op oudejaarsavond, groep met zwaar vuurwerk, grimmige sfeer, boa's op afstand terwijl politie aankomt (politie in Nederlands politie-uniform, duidelijk anders dan de boa's).

**05-05 · Overdracht aan de politie** — Boa draagt de situatie over aan een politieagent; wijst op de plek waar het vuurwerk ligt; notitieblok. Nederlands politie-uniform bij de agent; BOA-uniform en -embleem bij de boa volgens BEELDSTIJL §3–4.

**06-01 · De melding** — Zelfde situatie als 00-01, iets later: de jongen in de rode jas houdt een doos vast die hij uit de tas pakte; de boa's zijn dichterbij. Rustige groep.

**06-02 · Detail doos en tas** — Detail van de doos in de hand (`F2`, `Geschikt voor particulier gebruik`) en de open tas met drie gesloten `F2`-dozen en vijf losse, met tape omwikkelde voorwerpen. Functie: letterlijk waarnemen.

## 5. Signalering bestaande illustraties

- De generieke boa-figuren (`assets/illustraties/boa-hero*.webp`, `boa-buste*.webp`) worden op veel pagina's als ondersteunend personage gebruikt. Controleer ze tegen `BEELDSTIJL.md` §3–5 (uniform, embleem, uitrusting). Status: **CONTROLEREN**. Niet zelfstandig vervangen.
- `cat-f4-vlinder.webp` toont een merknaam (VIPER) en `cat-f4-cobra.webp` de tekst «COBRA 6». BEELDSTIJL §11 staat geen willekeurige achtergrondtekst toe; bij de controle van slot 01-05 meenemen.
- `plein-knal.webp` en `boa-jongeren-plein.webp` passen inhoudelijk bij de casus, maar moeten worden gecontroleerd op personages (rode jas, open zwarte tas) zodat 00-01, 01-08, 06-01 en 06-02 één lijn vormen.

## 6. Plaatsen (voor Claude, alleen na GOEDGEKEURD)

- Bestand in `assets/images/` met de naam uit §3.
- Koppelen in `assets/app.js`: `ART_FILE` (sleutel → bestand) en `L_SPEC['hoofdstuk.pagina'].a` (0-gebaseerd: introductie = 0, H1 = 1 … H6 = 6), of de `src` in de categoriepagina's (`index.html`).
- Cachesleutel `ASSET_V` verhogen, daarna desktop en mobiel controleren.
