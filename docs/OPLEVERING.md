# Oplevering e-learning Vuurwerk

## Versie

**0.9.2 — herbouw compacte cursus** (23 september 2026). Nog geen 1.0: de beelden uit `BEELDPLAN.md` zijn nog niet gemaakt en goedgekeurd.

- Juridische peildatum: **23 september 2026**.
- Doelgroep: **boa's in domein I**, Europees Nederland.
- Cacheversie `vw260923b` · opslag `jslf-vw-v1`, voortgangsversie **18**.
- Backupbranch vóór deze herbouw: `backup-voor-herbouw-compact-2026-09-23` (= commit `619eba5`).
- Basis: `HERZIENINGSRAPPORT_Vuurwerk.md` (23-9-2026) en de beslissingen van Jan van 23-9-2026.
- De oude opleveringsnotities (versie 0.9.1, 145 pagina's) staan in de git-geschiedenis en op de backupbranch.

## Opbouw

| Deel | Pagina's | Oefenvragen |
|---|---|---|
| Introductie | 3 | – |
| 1 Vuurwerk herkennen | 8 | 4 |
| 2 Wat zegt de wet? | 6 | 4 |
| 3 Wanneer ben jij als boa bevoegd? | 5 | 4 |
| 4 Wat kun je als boa doen? | 7 | 4 |
| 5 Wanneer doe je het niet zelf? | 5 | 2 |
| 6 Praktijkcasus: van melding tot proces-verbaal | 8 | – |
| Eindtoets | – | 15 (13 praktijkcasus, 2 kennisvragen) |
| **Totaal** | **42** | **18 + 15** |

Was: 145 pagina's, 31 oefenvragen, 15 eindtoetsvragen.

### Pagina's per deel

- **Introductie:** Een knal op het plein · Wat je leert en hoe de cursus werkt (doelgroep domein I, Europees Nederland) · De vier vragen (met de labels Herkennen, Wet, Wettelijk bevoegd, Taak/beleid, Veiligheid, Politie).
- **1 Vuurwerk herkennen:** Wie bepaalt de categorie? · F1 · F2 · F3 · F4 en professioneel vuurwerk · Verpakking en etiket · Onbekend vuurwerk en praktijknamen · Terug naar het plein: wat kun je vaststellen?
- **2 Wat zegt de wet?:** De Wet veilige jaarwisseling · Art. 9.2.2.1a Wm: bezit, gebruik en verkoop · Personen met gespecialiseerde kennis · De ontheffing van de burgemeester · Andere vuurwerkregels en samenloop · Economisch delict en straffen.
- **3 Wanneer ben jij als boa bevoegd?:** Zien is niet hetzelfde als bevoegd zijn (art. 142 Sv) · Domein I, onderdeel 9 · Wat volgt wél en níet uit onderdeel 9? · WED-opsporingsambtenaar: art. 17 WED · Welk feit? De categorie is nog geen conclusie.
- **4 Wat kun je als boa doen?:** Bevoegdheid, verplichting of strafbaarstelling? · Aanspreken en staande houden · Aanhouden op heterdaad · Aanhouden buiten heterdaad · Vervoermiddel: stilhouden, onderzoeken, meewerken · Inbeslagneming en uitlevering · Grenzen en vastleggen.
- **5 Wanneer doe je het niet zelf?:** Veiligheid · Taak en beleid · Politie · Zelf, overleggen of politie? · Een goede overdracht.
- **6 Praktijkcasus:** De melding · Vraag 1 t/m 4 · Het proces-verbaal — zo niet · Het proces-verbaal — zo wel · De vier vragen op straat (visuele eindpagina).

## Didactische regels in deze versie

1. Eén regel wordt één keer volledig uitgelegd. Daarna alleen verwijzen of toepassen.
2. De vier vragen zijn het enige denkmodel. De oude vijf/zeven-stappenschema's, de losse "Kort samengevat"-, "Leerdoelen"- en "Vooruitblik"-pagina's zijn vervallen.
3. Elke pagina heeft één label: Herkennen, Wet, Wettelijk bevoegd, Taak/beleid, Veiligheid, Politie of Praktijk. Beleid wordt nooit als bevoegdheidsgrondslag gebruikt.
4. Eén doorlopende casus (plein, 21 november): intro → H1 p8 → H6.

## Techniek

- Inhoud: `index.html` (`window.__DATA__`). Paginaopmaak: `L_SPEC` in `assets/app.js` (sleutel `deel.pagina`, 0-gebaseerd).
- Nieuw in `app.js`: `tLab()` (koppen "Introductie" / "Hoofdstuk n"), `FIG.bevkaart` (bevoegdheid · verplichting · strafbaarstelling), vernieuwde `FIG.beslishulp`. Ongebruikte oude figuren verwijderd.
- Nieuw in `soorten.css`: opmaak bevoegdhedenkaart. `app.css` ongewijzigd.
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
