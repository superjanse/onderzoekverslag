#  power Bi TMD Locks 

| Information | Details |
|---|---|
| auteur | Hugo Janse |
| Datum | 15-11-2026 |
| Versie | 1 |
| classificatie | Intern |
| client | Leonard Heuker of hoek |
| Bedrijf | TMD Locks |

## Voorwoord
Voor u ligt mijn stageonderzoeksrapport, geschreven in het kader van mijn HBO-ICT-opleiding aan de Hogeschool van Amsterdam. Mijn naam is Hugo Janse en sinds 1 september 2026 loop ik stage bij TMD Locks, een onderdeel van TMD Security.

Tijdens mijn stage heb ik de mogelijkheid gekregen om mij te verdiepen in Power BI en het analyseren en visualiseren van bedrijfsgegevens. Mijn opdracht richt zich op het ontwikkelen van een Power BI-dashboard waarmee belangrijke bedrijfsinformatie op een overzichtelijke en begrijpelijke manier wordt weergegeven, zodat de verschillende afdelingen eenvoudig toegang hebben tot de informatie die voor hen relevant is.

Deze stage biedt mij de kans om mijn vaardigheden op het gebied van data-analyse en datavisualisatie verder te ontwikkelen en tegelijkertijd praktijkervaring op te doen binnen een bedrijf. Naast het werken met Power BI leer ik hoe belangrijk het is om rekening te houden met de wensen van verschillende afdelingen en hoe bedrijfsgegevens kunnen bijdragen aan het nemen van goed onderbouwde beslissingen.

Graag wil ik TMD Locks bedanken voor de mogelijkheid om mijn stage binnen het bedrijf uit te voeren. In het bijzonder wil ik mijn opdrachtgever, Leonard Heuker of Hoek, bedanken voor het vertrouwen en de begeleiding tijdens mijn stage. Daarnaast wil ik mijn collega's bedanken voor hun hulp, feedback en de tijd die zij hebben genomen om hun kennis en ervaringen met mij te delen.

Tot slot wil ik mijn stagebegeleider vanuit de Hogeschool van Amsterdam bedanken voor de begeleiding en ondersteuning tijdens dit traject.

Ik wens u veel leesplezier.

Hugo Janse



## Samenvatting

Dit onderzoeksrapport beschrijft een onderzoek naar een voorstel voor een Power BI-dashboard voor TMD Locks. Binnen de organisatie worden bedrijfsgegevens uit verschillende systemen gebruikt, waaronder Exact Online, Excel en Shopify. Het verzamelen, combineren en analyseren van deze gegevens kost medewerkers veel tijd.

Het doel van het onderzoek was om vast te stellen welke bedrijfsgegevens en Key Performance Indicators (KPI's) voor de verschillende afdelingen het belangrijkst zijn en hoe deze informatie overzichtelijk kan worden weergegeven in Power BI.

Hiervoor zijn vijf semigestructureerde interviews afgenomen met medewerkers van verschillende afdelingen. Daaruit bleek dat medewerkers veel tijd kwijt zijn aan het handmatig verzamelen en verwerken van informatie. Een voorraadanalyse kost ongeveer twee uur, de accountmanager B2B Sales besteedt drie tot vier uur per week aan dealerinformatie en de Managing Director besteedde ongeveer zes uur per week aan het bijhouden van Excel-bestanden.

De informatiebehoeften verschillen per afdeling, maar een aantal KPI's werd door meerdere medewerkers genoemd: verkoopaantallen, de verdeling tussen B2B en B2C, de vergelijking tussen gerealiseerde verkoop en forecast en de performance-marketingkosten per verkocht B2C-slot. Daarnaast heeft B2B Sales behoefte aan inzicht in de doorverkoop en voorraad bij dealers, en Customer Support aan de actuele productvoorraad en een besteladvies. Specifieke voorkeuren voor grafiektypen of visualisaties zijn in de interviews niet naar voren gekomen.

Op basis van deze resultaten wordt aanbevolen om één centraal Power BI-rapport te ontwikkelen met afzonderlijke pagina's per afdeling en onderwerp: een salesoverzicht, aparte pagina's voor B2B en B2C, en pagina's voor forecast, finance, voorraad en dealervoorraad. Op elke pagina staan de belangrijkste KPI's direct zichtbaar.

Door bedrijfsgegevens centraal beschikbaar te maken en berekeningen te automatiseren, krijgen medewerkers sneller inzicht in de informatie die voor hun werk relevant is. Dit vermindert handmatig werk en verkleint de kans op menselijke fouten.

## Inhoudsopgave

- [Voorwoord](#voorwoord)
- [Samenvatting](#samenvatting)
- [1. Introductie](#1-introductie)
  - [1.1 Aanleiding](#11-aanleiding)
  - [1.2 Probleemstelling](#12-probleemstelling)
  - [1.3 Doelstelling](#13-doelstelling)
- [2. Betrokken partijen](#2-betrokken-partijen)
- [3. Theoretisch kader](#3-theoretisch-kader)
  - [3.1 Key Performance Indicators](#31-key-performance-indicators)
  - [3.2 Informatiebehoefte van de gebruiker](#32-informatiebehoefte-van-de-gebruiker)
  - [3.3 Overzichtelijke presentatie in dashboards](#33-overzichtelijke-presentatie-in-dashboards)
  - [3.4 Prioriteren met MoSCoW](#34-prioriteren-met-moscow)
  - [3.5 Toepassing binnen dit onderzoek](#35-toepassing-binnen-dit-onderzoek)
- [4. Onderzoeksvragen](#4-onderzoeksvragen)
  - [4.1 Hoofdonderzoeksvraag](#41-hoofdonderzoeksvraag)
  - [4.2 Deelvragen](#42-deelvragen)
- [5. Onderzoek](#5-onderzoek)
  - [5.1 Onderzoeksmethode](#51-onderzoeksmethode)
  - [5.2 Analyse van de interviewresultaten](#52-analyse-van-de-interviewresultaten)
  - [5.3 Interviewleidraad](#53-interviewleidraad)
  - [5.4 Data-inventarisatie](#54-data-inventarisatie)
- [6. Resultaten](#6-resultaten)
  - [6.1 Huidige werkwijze](#61-huidige-werkwijze)
  - [6.2 Knelpunten in de huidige werkwijze](#62-knelpunten-in-de-huidige-werkwijze)
  - [6.3 Informatiebehoeften per afdeling](#63-informatiebehoeften-per-afdeling)
  - [6.4 Gewenste KPI's en functionaliteiten](#64-gewenste-kpis-en-functionaliteiten)
  - [6.5 Prioritering van KPI's](#65-prioritering-van-kpis)
  - [6.6 Beschikbaarheid van gegevens](#66-beschikbaarheid-van-gegevens)
  - [6.7 Samenvatting van de belangrijkste bevindingen](#67-samenvatting-van-de-belangrijkste-bevindingen)
- [7. Conclusie](#7-conclusie)
  - [7.1 Deelvraag 1](#71-deelvraag-1)
  - [7.2 Deelvraag 2](#72-deelvraag-2)
  - [7.3 Deelvraag 3](#73-deelvraag-3)
  - [7.4 Deelvraag 4](#74-deelvraag-4)
  - [7.5 Beantwoording hoofdonderzoeksvraag](#75-beantwoording-hoofdonderzoeksvraag)
- [8. Aanbevelingen](#8-aanbevelingen)
  - [8.1 Indeling van het Power BI-dashboard](#81-indeling-van-het-power-bi-dashboard)
  - [8.2 Samenvatting van de aanbevelingen](#82-samenvatting-van-de-aanbevelingen)
- [9. Bronnen](#9-bronnen)
- [Bijlage A: Begrippenlijst](#bijlage-a-begrippenlijst)
- [Versiebeheer](#versiebeheer)

---

## 1. Introductie 

### 1.1 Aanleiding
Binnen TMD Locks worden bedrijfsgegevens opgeslagen en beheerd in Exact Online, waaronder verkoopcijfers, voorraadgegevens en informatie over de dealers. Deze gegevens zijn belangrijk voor de dagelijkse werkzaamheden van verschillende afdelingen, zoals verkoop, marketing, inkoop en management.

De organisatie heeft behoefte aan een centrale en overzichtelijke manier om deze informatie toegankelijk te maken. Daarom is besloten een Power BI-dashboard te ontwikkelen waarin de belangrijkste bedrijfsgegevens worden samengebracht en op een duidelijke manier worden gepresenteerd. Hierdoor kunnen medewerkers in één oogopslag de informatie vinden die voor hen relevant is.

### 1.2 Probleemstelling

De probleemstelling is gebaseerd op de eerste gesprekken met de opdrachtgever, Leonard Heuker of Hoek. Tijdens deze gesprekken kwamen verschillende problemen naar voren rondom het verzamelen, analyseren en presenteren van bedrijfsgegevens binnen TMD Locks. De interviews die later zijn afgenomen (hoofdstuk 6) bevestigden deze problemen en maakten ze meetbaar.

Naarmate TMD Locks groeide en er meer bedrijfsgegevens beschikbaar kwamen, werd het probleem groter doordat medewerkers steeds meer informatie handmatig moesten verzamelen en verwerken.

Het kost medewerkers momenteel extra tijd om de juiste informatie in Exact Online te vinden. Zij moeten regelmatig in uitgebreide tabellen zoeken en verschillende filters toepassen. Dit geldt onder andere voor verkoopcijfers, het aantal verkochte sloten per dealer, de dealervoorraad en verkoopontwikkelingen. Zo besteedt de accountmanager B2B Sales naar schatting drie tot vier uur per week aan het verzamelen en analyseren van dealerinformatie.

Daarnaast heeft de organisatie behoefte aan KPI's die worden berekend op basis van bestaande bedrijfsgegevens. Deze berekeningen zijn niet direct beschikbaar in Exact Online en worden daarom pas uitgevoerd op het moment dat de informatie nodig is, vaak met behulp van Excel. Dit kost extra tijd: de Managing Director besteedde ongeveer zes uur per week aan het handmatig bijhouden en verwerken van gegevens in Excel. Handmatige berekeningen brengen bovendien het risico op menselijke fouten met zich mee.

Ook voor inkoop en logistiek is overzichtelijke bedrijfsinformatie belangrijk. Een voorraadanalyse kost de Customer Support Manager ongeveer twee uur, omdat gegevens uit verschillende overzichten moeten worden gecombineerd. Hierdoor is het af en toe voorgekomen dat sloten niet op tijd geleverd konden worden doordat ze niet op voorraad waren. Als gevolg daarvan moesten klanten en dealers langer wachten, lieten zij soms een negatieve review achter en moest de verkoop in sommige gevallen tijdelijk worden stilgelegd, waardoor verkopen werden misgelopen.

Verder is het lastig om bedrijfsresultaten duidelijk en professioneel aan potentiële investeerders te presenteren. TMD Locks wil inzicht kunnen geven in omzet, winst, verkoopprestaties en de voortgang ten opzichte van de opgestelde forecasts.

Het centrale probleem is dat belangrijke bedrijfsinformatie binnen TMD Locks niet direct overzichtelijk beschikbaar is en dat aanvullende KPI's afzonderlijk moeten worden berekend. Vooral het management, B2B Sales en Customer Support ondervinden hier last van. Het verzamelen, analyseren en presenteren van informatie kost daardoor wekelijks meerdere uren. Als er niets verandert, blijft deze tijd verloren gaan, blijft het risico op rekenfouten en voorraadtekorten bestaan en blijft het lastig om investeerders snel een betrouwbaar beeld van de bedrijfsprestaties te geven.

### 1.3 Doelstelling

Het doel van dit onderzoek is om een onderbouwd voorstel te doen voor een Power BI-dashboard dat aansluit bij de informatiebehoeften van de verschillende afdelingen binnen TMD Locks. Hiervoor is onderzocht hoe medewerkers momenteel bedrijfsinformatie verzamelen, welke bedrijfsgegevens en Key Performance Indicators (KPI's) voor iedere afdeling het belangrijkst zijn, welke eisen zij stellen aan de presentatie van deze informatie en of de benodigde gegevens beschikbaar zijn in Power BI.

Dit onderzoek maakt deel uit van een bredere stageopdracht. Het doel van de stageopdracht is het ontwikkelen van het Power BI-dashboard zelf. Dit onderzoeksrapport vormt daarvoor de basis: op basis van het voorstel beslist de opdrachtgever welke KPI's en functionaliteiten worden opgenomen, waarna het dashboard wordt gebouwd. Het uitgangspunt daarbij is dat medewerkers in één oogopslag de belangrijkste informatie kunnen vinden, zonder door uitgebreide tabellen te hoeven zoeken of verschillende filters te moeten toepassen.

De betrouwbaarheid van de cijfers valt buiten de scope van dit onderzoek. Of de KPI's in Power BI correct worden berekend en overeenkomen met de gegevens uit Exact Online, wordt gecontroleerd tijdens de bouwfase van het dashboard.

Om de informatiebehoeften goed in kaart te brengen, is inzicht nodig in de afdelingen en belanghebbenden die het dashboard gaan gebruiken of de resultaten ervan ontvangen. Het volgende hoofdstuk beschrijft deze betrokken partijen en hun rol in het onderzoek.

## 2. Betrokken partijen

Bij de ontwikkeling van het Power BI-dashboard zijn verschillende afdelingen en belanghebbenden betrokken. Iedere afdeling heeft eigen informatiebehoeften, die tijdens het onderzoek in kaart zijn gebracht.

Voor het onderzoek zijn vijf medewerkers geïnterviewd om hun informatiebehoeften, belangrijkste KPI's en verwachtingen van het dashboard vast te stellen. Niet iedere afdeling had een eigen respondent; sommige medewerkers spraken namens meerdere afdelingen.

In onderstaande tabel worden de betrokken partijen, hun belangen en hun betrokkenheid bij het onderzoek weergegeven.

| Betrokken partij | Belang bij het dashboard | Betrokkenheid bij het onderzoek |
|---|---|---|
| **Management** | Inzicht in omzet, winst, forecasts en algemene bedrijfsprestaties ter ondersteuning van beslissingen. | De Managing Director (opdrachtgever) en de Head of Finance zijn geïnterviewd over hun informatiebehoeften, gewenste KPI's en verwachtingen van het dashboard. De opdrachtgever beslist op basis van dit rapport welke KPI's en functionaliteiten worden opgenomen. |
| **Sales B2B** | Inzicht in dealerprestaties, dealervoorraad, verkochte sloten per dealer en aanwezigheid van demosloten bij winkels. | De accountmanager B2B Sales is geïnterviewd over de informatiebehoeften rondom dealers en B2B-verkoop. |
| **Sales B2C** | Inzicht in verkoopcijfers via onder andere Amazon en Decathlon, verkoopontwikkelingen en de beschikbare interne magazijnvoorraad. | De informatiebehoeften rondom B2C-verkoop zijn besproken met de CTO en de Managing Director. |
| **Marketing** | Inzicht in advertentiekosten, advertentiekosten per verkocht slot en verkoopontwikkelingen. | De CTO is geïnterviewd over marketingprestaties en advertentiekosten, omdat hij verantwoordelijk is voor de analyse van marketinguitgaven. |
| **Inkoop en logistiek** | Inzicht in actuele voorraadniveaus, beschikbare sloten en verwachte leveringen. | De Customer Support Manager is geïnterviewd over voorraad- en inkoopinformatie, omdat de voorraadanalyses door deze functie worden uitgevoerd. |
| **Investeerders** | Inzicht in omzet, winst, verkoopprestaties en de voortgang ten opzichte van forecasts. | Zijn indirect betrokken en niet geïnterviewd. Zij ontvangen bedrijfsresultaten via presentaties of screenshots en hebben geen dagelijkse toegang tot het dashboard. De Managing Director bepaalt welke informatie aan de investeerders wordt getoond, voornamelijk de totale verkoop B2B en B2C, en heeft in dit onderzoek namens hen gesproken. |

De betrokken partijen hebben ieder eigen informatiebehoeften en belangen bij het dashboard. Deze informatiebehoeften vormen de basis voor het voorstel in dit rapport.

## 3. Theoretisch kader

In dit hoofdstuk worden de theoretische uitgangspunten beschreven die relevant zijn voor het opstellen van het voorstel voor het Power BI-dashboard. Hierbij wordt ingegaan op Key Performance Indicators (KPI's), de informatiebehoeften van gebruikers, de overzichtelijke presentatie van informatie in dashboards en het prioriteren van wensen. Deze theorie wordt gebruikt om de resultaten uit de interviews te beoordelen en te vertalen naar aanbevelingen voor het dashboard. De belangrijkste begrippen uit dit rapport worden toegelicht in de begrippenlijst in bijlage A.

### 3.1 Key Performance Indicators

Een Key Performance Indicator (KPI) is een meetbare indicator waarmee de prestaties van een organisatie, afdeling of bedrijfsproces kunnen worden gevolgd. Volgens Parmenter (2020) moeten KPI's aansluiten bij de factoren die het meest bepalen of een organisatie haar doelen haalt. Een KPI moet bovendien informatie opleveren waarop medewerkers kunnen sturen.

Om te bepalen of een KPI goed is opgesteld, wordt vaak het SMART-model gebruikt (Doran, 1981). Een KPI is dan Specifiek (duidelijk wat er wordt gemeten), Meetbaar (er is een formule en databron), Acceptabel/toewijsbaar (er is een verantwoordelijke), Realistisch en Tijdgebonden (er is een vaste periode, bijvoorbeeld per week of maand).

Daarnaast wordt onderscheid gemaakt tussen lagging en leading indicatoren (Parmenter, 2020). Een lagging indicator laat het resultaat van het verleden zien, zoals de omzet van de afgelopen maand. Een leading indicator geeft een signaal vóórdat een resultaat zichtbaar wordt, zoals een dalende voorraad die op een toekomstige stock-out wijst. Een dashboard met alleen lagging indicatoren laat zien wat er is gebeurd, maar helpt minder bij het op tijd ingrijpen.

Voor TMD Locks betekent dit dat niet iedere beschikbare bedrijfswaarde automatisch een relevante KPI is. De KPI's in het Power BI-dashboard moeten aansluiten bij de werkzaamheden van de verschillende afdelingen. Daarom is in dit onderzoek aan medewerkers gevraagd welke gegevens zij gebruiken en welke KPI's voor hen de hoogste prioriteit hebben.

### 3.2 Informatiebehoefte van de gebruiker

Few (2013) omschrijft een dashboard als een visuele weergave van de belangrijkste informatie die nodig is om één of meer doelen te bereiken, zo samengebracht dat deze in één oogopslag te volgen is. Welke informatie het belangrijkst is, verschilt per gebruiker of afdeling. Microsoft (z.d.) adviseert daarom om bij het ontwerpen van een dashboard eerst te bepalen wie de doelgroep is en welke beslissingen zij met het dashboard nemen.

Voor dit onderzoek betekent dit dat de informatiebehoefte per afdeling apart in kaart moet worden gebracht. Een dashboard moet dan zowel gezamenlijke bedrijfsinformatie als afdelingsspecifieke informatie kunnen weergeven.

### 3.3 Overzichtelijke presentatie in dashboards

Een dashboard moet de belangrijkste informatie duidelijk en overzichtelijk presenteren. Few (2013) noemt hiervoor onder andere de volgende ontwerpprincipes:

- De belangrijkste informatie staat op de opvallendste plek, meestal linksboven, omdat gebruikers daar beginnen met lezen.
- Het dashboard bevat zo weinig mogelijk ruis, zoals overbodige kleuren, randen en decoraties.
- De informatie past zoveel mogelijk op één scherm, zodat de gebruiker niet hoeft te scrollen of te zoeken.

Microsoft (z.d.) geeft vergelijkbaar advies voor Power BI. Het gekozen type visualisatie moet passen bij de gegevens. Voor het vergelijken van waarden zijn staaf- of kolomdiagrammen geschikt, en belangrijke losse waarden kunnen met KPI-kaarten worden weergegeven. Ook moet een dashboard consequent zijn in schaal, volgorde en kleurgebruik.

Voor het Power BI-dashboard van TMD Locks betekent dit dat de belangrijkste KPI's per afdeling direct zichtbaar moeten zijn. Minder belangrijke of meer gedetailleerde informatie kan op afzonderlijke pagina's of op een lager detailniveau worden weergegeven.

### 3.4 Prioriteren met MoSCoW

Omdat niet alle wensen tegelijk kunnen worden gebouwd, moeten zij worden geprioriteerd. Een veelgebruikte methode hiervoor is MoSCoW (Agile Business Consortium, 2014). Hierbij wordt iedere wens ingedeeld in één van vier categorieën:

- **Must have:** zonder deze wens is het dashboard niet bruikbaar.
- **Should have:** belangrijk, maar het dashboard werkt ook zonder.
- **Could have:** wenselijk, maar alleen als er tijd over is.
- **Won't have (this time):** wordt in deze versie niet gebouwd.

In dit onderzoek wordt MoSCoW gebruikt om de gewenste KPI's en functionaliteiten in te delen. Zo wordt duidelijk wat in de eerste versie van het dashboard moet zitten en wat later kan worden toegevoegd.

### 3.5 Toepassing binnen dit onderzoek

De theoretische uitgangspunten uit dit hoofdstuk worden gecombineerd met de resultaten van de interviews. De theorie geeft algemene richtlijnen voor het selecteren, prioriteren en presenteren van KPI's. De interviews geven inzicht in de specifieke informatiebehoeften van medewerkers van TMD Locks.

Bij het opstellen van het voorstel wordt daarom gekeken naar drie punten: de KPI moet relevant zijn voor de werkzaamheden van de gebruiker, de benodigde gegevens moeten beschikbaar zijn en de informatie moet overzichtelijk kunnen worden weergegeven in Power BI. Deze uitgangspunten vormen samen met de onderzoeksresultaten de basis voor de aanbevelingen in dit rapport.

## 4. Onderzoeksvragen

Dit hoofdstuk beschrijft de hoofdvraag en deelvragen van het onderzoek. De vragen richten zich op de huidige werkwijze en knelpunten, de informatiebehoeften van de verschillende afdelingen, de gewenste presentatie van bedrijfsgegevens en KPI’s en de beschikbaarheid van de benodigde gegevens. De antwoorden vormen de basis voor een voorstel voor het Power BI-dashboard.

### 4.1 Hoofdonderzoeksvraag

Welke bedrijfsgegevens, KPI’s en presentatie-eisen moet TMD Locks opnemen in een voorstel voor een Power BI-dashboard dat aansluit bij de informatiebehoeften van de verschillende afdelingen?

### 4.2 Deelvragen 
1. Hoe verzamelen en analyseren medewerkers van TMD Locks momenteel bedrijfsinformatie en welke knelpunten ervaren zij hierbij?

2. Welke bedrijfsgegevens en KPI's zijn voor de verschillende afdelingen binnen TMD Locks het belangrijkst om hun werkzaamheden uit te voeren en beslissingen te ondersteunen?

3. Welke eisen en wensen hebben medewerkers ten aanzien van de overzichtelijkheid en presentatie van bedrijfsgegevens en KPI's?

4. In welke systemen zijn de gegevens voor de gewenste KPI's beschikbaar en kunnen deze in Power BI worden geladen en berekend?

Samen geven de deelvragen richting aan het onderzoek en helpen zij om de hoofdvraag te beantwoorden. Het volgende hoofdstuk beschrijft de onderzoeksmethode waarmee de benodigde informatie wordt verzameld en geanalyseerd.

## 5. Onderzoek

Dit hoofdstuk beschrijft de onderzoeksmethoden die in dit onderzoek zijn gebruikt. Eerst wordt toegelicht hoe de interviews zijn uitgevoerd en geanalyseerd en wordt de interviewleidraad weergegeven. Daarna wordt beschreven hoe met een data-inventarisatie is onderzocht welke gegevens beschikbaar zijn in Exact Online en Power BI.

### 5.1 Onderzoeksmethode

Om de informatiebehoeften van de verschillende afdelingen binnen TMD Locks in kaart te brengen, is gebruikgemaakt van semigestructureerde interviews. Hiervoor zijn vijf medewerkers geïnterviewd, onder wie de opdrachtgever.

Bij een semigestructureerd interview wordt gewerkt met een vooraf opgestelde vragenlijst, waarbij ruimte blijft om aanvullende vragen te stellen en dieper in te gaan op de antwoorden van de geïnterviewde (The Open University, 2025). Deze methode maakt het mogelijk om de resultaten van verschillende interviews met elkaar te vergelijken, terwijl er tegelijkertijd aandacht kan worden besteed aan de specifieke werkzaamheden en informatiebehoeften van iedere afdeling (Verhoeven, 2022).

Voor dit onderzoek is één algemene interviewleidraad opgesteld, met ruimte voor afdelingsspecifieke vragen. Tijdens de interviews is onderzocht welke bedrijfsgegevens medewerkers gebruiken, waarvoor zij Exact Online gebruiken, welke knelpunten zij ervaren en welke KPI's voor hun werkzaamheden belangrijk zijn. Daarnaast is gevraagd welke informatie zij het belangrijkst vinden om in één oogopslag te kunnen zien.

De resultaten van de interviews worden gebruikt om de informatiebehoeften per afdeling vast te stellen en een voorstel te doen voor de belangrijkste KPI's en eisen voor het Power BI-dashboard.

### 5.2 Analyse van de interviewresultaten

Na het afnemen van de interviews zijn de antwoorden per afdeling verzameld en geanalyseerd. Hierbij is gekeken naar de informatiebehoeften, ervaren knelpunten en gewenste KPI's.

De resultaten zijn vervolgens samengevoegd tot één overzicht waarin de belangrijkste KPI's en wensen van de verschillende afdelingen zijn opgenomen.

Op basis van deze resultaten wordt in dit onderzoeksrapport een voorstel gedaan voor de KPI's, functionaliteiten en presentatie van het Power BI-dashboard. Het onderzoeksrapport wordt voorgelegd aan de opdrachtgever, Leonard Heuker of Hoek. Naar aanleiding van dit rapport beslist de opdrachtgever welke voorgestelde KPI's en functionaliteiten worden opgenomen en welke prioriteit krijgen.

### 5.3 Interviewleidraad

**Doel:** Onderzoeken welke bedrijfsinformatie medewerkers momenteel gebruiken, welke KPI's zij belangrijk vinden en wat zij verwachten van het nieuwe Power BI-dashboard.

**Interviewduur:** 5–10 minuten

**1. Huidige informatie**

Welke bedrijfsinformatie uit Exact Online gebruik je momenteel het meest voor je werkzaamheden?

**2. Huidige werkwijze**

Waar en hoe zoek je deze informatie momenteel op?

**3. Tijdsduur**

Hoeveel tijd kost het je gemiddeld om deze informatie te vinden en eventueel te berekenen?

**4. Gewenste informatie**

Welke informatie en KPI's zou je graag terugzien in het nieuwe Power BI-dashboard?

**5. Prioriteiten**

Welke drie gegevens of KPI's zijn voor jou het belangrijkst om in één oogopslag te kunnen zien?

De interviews en de analyse van de antwoorden vormen de basis voor het beantwoorden van de deelvragen.

### 5.4 Data-inventarisatie

Om deelvraag 4 te beantwoorden, is naast de interviews een data-inventarisatie uitgevoerd. Hierbij is voor iedere KPI die in de interviews is genoemd nagegaan welke gegevens nodig zijn om deze te berekenen, in welk systeem deze gegevens zijn opgeslagen en of ze via een custom connector in Power BI kunnen worden geladen.

Hiervoor zijn de gegevensstromen binnen TMD Locks in kaart gebracht. Daarbij is gekeken naar orders uit de webshop, Amazon en Decathlon, de activatie van serienummers via de app en het adminportaal, en de advertentiekosten van Google Ads en Meta Ads. Daarnaast is nagegaan welke gegevens via de custom connector tussen Exact Online en Power BI beschikbaar zijn. Dit is gedaan door zelf in Exact Online en Power BI te controleren welke gegevens aanwezig zijn.

Voor deze methode is gekozen omdat de interviews laten zien welke informatie medewerkers nodig hebben, maar niet of die informatie technisch beschikbaar is. Door beide methoden te combineren, is het voorstel niet alleen gebaseerd op de wensen van medewerkers, maar ook getoetst op haalbaarheid.

## 6. Resultaten


In dit hoofdstuk worden de resultaten van vijf interviews met medewerkers van TMD Locks beschreven. De interviews zijn gehouden om inzicht te krijgen in de huidige werkwijze, de knelpunten bij het verzamelen en analyseren van bedrijfsgegevens en de informatiebehoeften van verschillende afdelingen. Daarnaast worden in paragraaf 6.6 de resultaten van de data-inventarisatie beschreven.

De antwoorden zijn geanalyseerd en gegroepeerd op basis van terugkerende thema's. Hierbij is gekeken naar overeenkomsten en verschillen tussen de geïnterviewde medewerkers.

### 6.1 Huidige werkwijze

Uit de interviews blijkt dat medewerkers van TMD Locks verschillende systemen gebruiken om bedrijfsinformatie te verzamelen en te analyseren. Welke systemen worden gebruikt, verschilt per functie en informatiebehoefte.

De Head of Finance gebruikt Exact Online voor het verzamelen van financiële informatie en verkoopgegevens. Wanneer aanvullende analyses nodig zijn, worden gegevens verwerkt in Excel.

De Customer Support Manager gebruikt gegevens uit Exact Online om voorraadstanden en verkoophistorie te analyseren. Hierbij worden verschillende overzichten gecombineerd en vervolgens in Excel verwerkt met behulp van draaitabellen.

De accountmanager B2B Sales gebruikt Exact Online om inzicht te krijgen in de doorverkoop bij dealers. Hiervoor worden geregistreerde serienummers gebruikt. Daarnaast wordt Shopify geraadpleegd voor informatie over specifieke bestellingen.

De CTO gebruikt verschillende gegevensbronnen om verkoopprestaties en marketinguitgaven te vergelijken. Exact Online wordt hierbij niet rechtstreeks gebruikt voor zijn dagelijkse analyses.

De Managing Director gebruikte Exact Online voornamelijk voor financiële informatie, zoals het banksaldo en de debiteuren- en crediteurenpositie. Andere belangrijke bedrijfsgegevens, waaronder verkoopinformatie en forecasts, werden bijgehouden in afzonderlijke Excel-bestanden.



### 6.2 Knelpunten in de huidige werkwijze

Een terugkerend knelpunt is de tijd die medewerkers besteden aan het verzamelen, combineren en analyseren van bedrijfsgegevens.

De Customer Support Manager geeft aan dat een voorraadanalyse ongeveer twee uur kan kosten. Hierbij moeten gegevens uit verschillende overzichten worden gecombineerd en verwerkt in Excel.

De accountmanager B2B Sales besteedt naar schatting drie tot vier uur per week aan het verzamelen en analyseren van dealerinformatie.

De Managing Director geeft aan dat hij ongeveer zes uur per week besteedde aan het handmatig bijhouden, verzamelen en verwerken van gegevens in verschillende Excel-bestanden.

Daarnaast blijkt uit de interviews dat bedrijfsinformatie niet altijd direct in de gewenste vorm beschikbaar is. Medewerkers moeten daarom gegevens uit verschillende systemen raadplegen of aanvullende berekeningen uitvoeren om de benodigde inzichten te verkrijgen.

Een ander knelpunt is dat financiële gegevens, verkoopinformatie en marketinggegevens verspreid staan over meerdere bronnen. Hierdoor ontbreekt een centrale omgeving waarin deze informatie gezamenlijk kan worden geanalyseerd.

### 6.3 Informatiebehoeften per afdeling

Uit de interviews blijkt dat de informatiebehoefte binnen TMD Locks verschilt per afdeling. Hoewel meerdere medewerkers gebruikmaken van dezelfde bedrijfsgegevens, hebben zij verschillende doelen bij het analyseren van deze informatie.

De Managing Director heeft voornamelijk behoefte aan een overzicht van de algemene verkoopprestaties. Hierbij ligt de nadruk op het onderscheid tussen B2B- en B2C-verkopen, de vergelijking met de forecast en de kosten van performance marketing. Daarnaast wil hij inzicht hebben in de geografische spreiding van de verkopen en de prestaties per verkoopkanaal.

De Head of Finance richt zich op financiële en commerciële prestaties. Belangrijke informatie is onder andere het aantal verkochte sloten, de verkoopresultaten per land en dealer, marketingkosten en de vergelijking tussen de gerealiseerde verkoop en de forecast. Ook wil hij verkoopgegevens kunnen uitsplitsen naar productvarianten.

De CTO heeft voornamelijk behoefte aan informatie over verkoop- en marketingprestaties. Hierbij wil hij advertentiekosten kunnen vergelijken met B2C-verkopen en inzicht krijgen in de prestaties van verschillende verkoopkanalen, zoals Amazon en de eigen webshop.

De accountmanager B2B Sales richt zich op de prestaties van individuele dealers. Hij wil kunnen zien hoeveel sloten iedere dealer heeft doorverkocht en hoeveel sloten gemiddeld per maand worden verkocht. Daarnaast is inzicht in de voorraadpositie bij dealers belangrijk, zodat tijdig kan worden vastgesteld welke dealers mogelijk een herhaalbestelling nodig hebben.

De Customer Support Manager heeft voornamelijk behoefte aan informatie over voorraadbeheer en verkoophistorie. Hierbij zijn de actuele voorraadstanden, verkochte aantallen per productvariant en meest verkochte producten belangrijk. Daarnaast bestaat de wens om op basis van deze gegevens een besteladvies te kunnen opstellen.

Overeenkomsten en verschillen

Ondanks de verschillende informatiebehoeften komt uit meerdere interviews naar voren dat verkoopgegevens een belangrijke rol spelen. Vooral de Managing Director, Head of Finance en CTO hebben behoefte aan inzicht in verkoopprestaties en de mogelijkheid om deze met andere gegevens te vergelijken.

De accountmanager B2B Sales gebruikt verkoopgegevens voornamelijk om dealerprestaties te beoordelen, terwijl de Customer Support Manager deze informatie gebruikt om voorraadbeheer en inkoopbeslissingen te ondersteunen.

Hieruit blijkt dat de verschillende afdelingen deels dezelfde gegevens nodig hebben, maar deze vanuit verschillende invalshoeken willen analyseren.

### 6.4 Gewenste KPI's en functionaliteiten

Tijdens de interviews is aan de medewerkers gevraagd welke informatie en KPI's zij graag in het Power BI-dashboard willen terugzien.

De genoemde KPI's en functionaliteiten zijn in onderstaande tabel samengevoegd.


| KPI of functionaliteit | Genoemd door |
|---|---|
| Verkoopaantallen B2B en B2C | Managing Director, Head of Finance |
| Verkoopaantallen per periode | Managing Director, Head of Finance, CTO |
| Performance-marketingkosten per B2C-slot | Managing Director, Head of Finance, CTO |
| Forecast versus daadwerkelijke verkoop | Managing Director, Head of Finance |
| Verkoop per kanaal | Managing Director, CTO |
| Verkoop per land | Managing Director, Head of Finance |
| ROAS | CTO |
| Doorverkoop per dealer | Accountmanager B2B Sales, Head of Finance, CTO |
| Gemiddelde maandelijkse verkoop per dealer | Accountmanager B2B Sales |
| Voorraad bij dealers | Accountmanager B2B Sales |
| Actuele productvoorraad | Customer Support Manager |
| Verkoopaantallen per productvariant | Customer Support Manager, Head of Finance |
| Besteladvies op basis van voorraad en verkoop | Customer Support Manager |

Uit dit overzicht blijkt dat meerdere medewerkers behoefte hebben aan vergelijkbare verkoopgegevens. Vooral verkoopaantallen, marketingprestaties en de vergelijking met de forecast komen bij verschillende functies terug.

Daarnaast bestaan er specifieke informatiebehoeften die vooral voor één afdeling relevant zijn. Zo richt B2B Sales zich op de doorverkoop en voorraad bij dealers, terwijl Customer Support behoefte heeft aan actuele productvoorraad en ondersteuning bij inkoopbeslissingen.

### 6.5 Prioritering van KPI's

In paragraaf 6.4 zijn alle KPI's en functionaliteiten weergegeven die tijdens de interviews zijn genoemd. Om te bepalen welke KPI's de hoogste prioriteit hebben, is aan iedere medewerker gevraagd welke drie gegevens of KPI's zij het belangrijkst vinden om in één oogopslag te kunnen zien.

De antwoorden zijn samengevoegd in onderstaande tabel.

| Functie | Prioriteit 1 | Prioriteit 2 | Prioriteit 3 |
|---|---|---|---|
| Managing Director | Verkoopaantallen B2B/B2C | Marketingkosten per B2C-slot | Forecast versus verkoop |
| Head of Finance | Maandelijkse verkoopaantallen | B2B/B2C-verdeling | Forecast versus verkoop |
| CTO | Verkoopaantallen | Marketingprestaties | Verkoopkanalen |
| Accountmanager B2B Sales | Doorverkoop per dealer | Gemiddelde verkoop per dealer | Dealervoorraad |
| Customer Support Manager | Actuele productvoorraad | Verkoopaantallen | Besteladvies |


Uit de resultaten blijkt dat verkoopaantallen voor meerdere medewerkers een belangrijke KPI vormen. Daarnaast worden marketingprestaties en de vergelijking met de forecast door verschillende medewerkers genoemd.

Om te voorkomen dat het Power BI-dashboard te veel informatie tegelijkertijd toont, wordt in het voorstel rekening gehouden met deze prioriteiten. Voorgesteld wordt om de belangrijkste KPI's een prominente plaats op de bijbehorende dashboardpagina's te geven. Overige informatie kan op onderliggende pagina's worden weergegeven.

Vervolgens zijn de KPI's met de MoSCoW-methode (paragraaf 3.4) ingedeeld. Hiervoor is de volgende regel gebruikt:

- **Must have:** door een respondent als prioriteit 1 genoemd, of door twee of meer respondenten in de top drie.
- **Should have:** door één respondent in de top drie genoemd, maar niet als prioriteit 1.
- **Could have:** wel genoemd in paragraaf 6.4, maar door niemand in de top drie.
- **Won't have:** KPI's die in deze versie niet worden gebouwd.

| KPI of functionaliteit | Onderbouwing | MoSCoW |
|---|---|---|
| Verkoopaantallen B2B en B2C | Prioriteit 1 (Managing Director), prioriteit 2 (Head of Finance) | Must have |
| Verkoopaantallen per periode | Prioriteit 1 (Head of Finance) | Must have |
| Performance-marketingkosten per B2C-slot | Top drie bij Managing Director en CTO | Must have |
| Forecast versus daadwerkelijke verkoop | Top drie bij Managing Director en Head of Finance | Must have |
| Doorverkoop per dealer | Prioriteit 1 (Accountmanager B2B Sales) | Must have |
| Actuele productvoorraad | Prioriteit 1 (Customer Support Manager) | Must have |
| Verkoop per kanaal | Top drie bij CTO | Should have |
| Gemiddelde maandelijkse verkoop per dealer | Top drie bij Accountmanager B2B Sales | Should have |
| Voorraad bij dealers | Top drie bij Accountmanager B2B Sales | Should have |
| Besteladvies op basis van voorraad en verkoop | Top drie bij Customer Support Manager | Should have |
| Verkoop per land | Genoemd, niet in top drie | Could have |
| ROAS | Genoemd, niet in top drie | Could have |
| Verkoopaantallen per productvariant | Genoemd, niet in top drie | Could have |

Volgens deze indeling bevat de eerste versie van het dashboard in ieder geval de Must have-KPI's. Hierdoor krijgt iedere afdeling vanaf het begin haar belangrijkste KPI. Should have- en Could have-KPI's kunnen daarna worden toegevoegd. Er zijn geen KPI's als Won't have aangemerkt, omdat uit de data-inventarisatie (paragraaf 6.6) blijkt dat alle KPI's haalbaar zijn. Deze indeling is een voorstel; de definitieve prioriteiten worden met de opdrachtgever afgestemd.

### 6.6 Beschikbaarheid van gegevens

Met de data-inventarisatie (paragraaf 5.4) is voor iedere KPI uit paragraaf 6.4 nagegaan waar de benodigde gegevens zijn opgeslagen en of deze in Power BI kunnen worden geladen.

Uit de inventarisatie blijkt dat vrijwel alle gegevens centraal in Exact Online terechtkomen. Orders uit Amazon en Decathlon worden via Shopify verwerkt en Shopify is gekoppeld aan Exact Online, zowel voor B2B- als voor B2C-verkoop. Bij iedere order wordt vastgelegd via welk kanaal deze binnenkwam. De activatie van serienummers door eindklanten wordt via de app en het adminportaal ook in Exact Online vastgelegd. Ook de advertentiekosten van Google Ads en Meta Ads zijn in Exact Online beschikbaar. De forecast is handmatig opgesteld in Excel en vervolgens in Power BI geladen.

De gegevens uit Exact Online worden via een custom connector in Power BI geladen. In onderstaande tabel is per KPI de databron en de beschikbaarheid weergegeven.

| KPI of functionaliteit | Databron | Beschikbaar in Power BI |
|---|---|---|
| Verkoopaantallen B2B en B2C | Exact Online | Ja |
| Verkoopaantallen per periode | Exact Online | Ja |
| Performance-marketingkosten per B2C-slot | Exact Online (advertentiekosten ÷ verkochte B2C-sloten) | Ja, berekend |
| Forecast versus daadwerkelijke verkoop | Excel (forecast, handmatig ingeladen) en Exact Online | Ja, forecast wordt handmatig bijgewerkt |
| Verkoop per kanaal | Exact Online (kanaal per order) | Ja |
| Verkoop per land | Exact Online | Ja |
| ROAS | Exact Online (B2C-omzet ÷ advertentiekosten) | Ja, berekend |
| Doorverkoop per dealer | Exact Online (geactiveerde serienummers) | Ja, berekend |
| Gemiddelde maandelijkse verkoop per dealer | Exact Online | Ja, berekend |
| Voorraad bij dealers | Exact Online (geleverd − geactiveerd) | Ja, berekend |
| Actuele productvoorraad | Exact Online (in- en uitgaande serienummers) | Ja, berekend |
| Verkoopaantallen per productvariant | Exact Online | Ja |
| Besteladvies op basis van voorraad en verkoop | Exact Online (voorraad en verkoophistorie) | Ja, berekend |

Hieruit blijkt dat alle gewenste KPI's met de beschikbare gegevens in Power BI kunnen worden weergegeven. Een deel van de KPI's is niet direct als gegeven beschikbaar, maar moet in Power BI worden berekend op basis van gegevens uit Exact Online. Zo wordt de voorraad bij dealers bepaald door het aantal geleverde sloten te verminderen met het aantal sloten waarvan het serienummer door een eindklant is geactiveerd. Dit blijft een schatting: sloten die al zijn verkocht, maar nog niet zijn geactiveerd, worden als voorraad bij de dealer meegeteld. Daarnaast is de forecast het enige onderdeel dat niet automatisch wordt bijgewerkt; wanneer de forecast verandert, moet deze opnieuw handmatig in Power BI worden geladen.

### 6.7 Samenvatting van de belangrijkste bevindingen

In deze paragraaf worden de belangrijkste bevindingen uit paragraaf 6.1 tot en met 6.6 samengevat.

**Huidige werkwijze (6.1).** Medewerkers verzamelen bedrijfsinformatie uit verschillende systemen, voornamelijk Exact Online, Excel en Shopify. Welke systemen worden gebruikt, verschilt per functie.

**Knelpunten (6.2).** Het handmatig verzamelen, combineren en verwerken van gegevens kost veel tijd: ongeveer twee uur per voorraadanalyse, drie tot vier uur per week voor dealerinformatie en ongeveer zes uur per week voor de Managing Director. Daarnaast staan gegevens verspreid over meerdere bronnen en ontbreekt een centrale omgeving.

**Informatiebehoeften per afdeling (6.3).** Verkoopgegevens zijn voor bijna alle respondenten belangrijk, maar worden vanuit verschillende invalshoeken bekeken. Het management, Finance en de CTO richten zich op algemene verkoop- en marketingprestaties, B2B Sales op dealers en Customer Support op voorraad en inkoop.

**Gewenste KPI's (6.4).** In totaal zijn dertien KPI's en functionaliteiten genoemd. Verkoopaantallen, marketingkosten per B2C-slot, forecast versus verkoop en doorverkoop per dealer werden door meerdere respondenten genoemd.

**Prioritering (6.5).** Verkoopaantallen worden het vaakst als prioriteit genoemd, gevolgd door marketingprestaties en de vergelijking met de forecast. Voor B2B Sales en Customer Support staan afdelingsspecifieke KPI's bovenaan, zoals doorverkoop per dealer en actuele productvoorraad. Met de MoSCoW-methode zijn zes KPI's als Must have, vier als Should have en drie als Could have ingedeeld.

**Beschikbaarheid van gegevens (6.6).** Alle gewenste KPI's kunnen met gegevens uit Exact Online en Excel in Power BI worden weergegeven, waarvan een deel moet worden berekend. De voorraad bij dealers is een schatting en de forecast moet handmatig worden bijgewerkt.

Deze bevindingen vormen de basis voor de beantwoording van de deelvragen in hoofdstuk 7.


## 7. Conclusie
Naar aanleiding van de vijf afgenomen interviews met medewerkers van TMD Locks en de data-inventarisatie worden in dit hoofdstuk de vier deelvragen en de hoofdonderzoeksvraag beantwoord. De interviews hebben inzicht gegeven in de huidige werkwijze, de knelpunten bij het verzamelen en analyseren van bedrijfsinformatie en de belangrijkste informatiebehoeften van de verschillende afdelingen. De data-inventarisatie heeft laten zien welke gegevens beschikbaar zijn en in Power BI kunnen worden geladen. Deze inzichten vormen de basis voor een voorstel voor het Power BI-dashboard.

### 7.1 Deelvraag 1

Hoe verzamelen en analyseren medewerkers van TMD Locks momenteel bedrijfsinformatie en welke knelpunten ervaren zij hierbij?

Uit de interviews blijkt dat medewerkers van TMD Locks voornamelijk gebruikmaken van Exact Online, Excel en Shopify om bedrijfsinformatie te verzamelen en te analyseren. Welke systemen worden gebruikt, hangt af van de afdeling en de informatie die medewerkers nodig hebben.

Een belangrijk knelpunt is dat de benodigde informatie verspreid staat over verschillende systemen en bestanden. Hierdoor moeten medewerkers regelmatig gegevens handmatig verzamelen, combineren en vergelijken om de gewenste inzichten te verkrijgen.

Dit kost medewerkers extra tijd. Zo blijkt uit de interviews dat de Managing Director ongeveer zes uur per week besteedde aan het verwerken en bijhouden van gegevens, terwijl de accountmanager B2B Sales hier naar schatting drie tot vier uur per week aan besteedt.

Geconcludeerd kan worden dat de huidige werkwijze relatief veel handmatige werkzaamheden vereist en dat er behoefte is aan een centrale omgeving waarin bedrijfsinformatie eenvoudiger kan worden geraadpleegd en geanalyseerd.

### 7.2 Deelvraag 2

Welke bedrijfsgegevens en KPI's zijn voor de verschillende afdelingen binnen TMD Locks het belangrijkst om hun werkzaamheden uit te voeren en beslissingen te ondersteunen?

Uit de interviews blijkt dat de belangrijkste bedrijfsgegevens en KPI's per afdeling verschillen. Wel komen bepaalde informatiebehoeften bij meerdere medewerkers terug.

Vooral verkoopaantallen, uitgesplitst naar B2B en B2C, de vergelijking tussen gerealiseerde verkoop en forecast en de performance-marketingkosten per verkocht B2C-slot worden door meerdere medewerkers belangrijk gevonden.

Daarnaast hebben de verschillende afdelingen specifieke informatiebehoeften. Voor B2B Sales zijn vooral de doorverkoop en voorraadpositie bij dealers belangrijk. Voor Customer Support ligt de nadruk op productvoorraad, verkoophistorie en besteladvies.

Wanneer de KPI's worden ingedeeld volgens het onderscheid tussen lagging en leading indicatoren (paragraaf 3.1), valt op dat de meeste genoemde KPI's lagging zijn. Verkoopaantallen, de B2B/B2C-verdeling, verkoop per kanaal en land, marketingkosten per B2C-slot en ROAS laten zien wat er in een afgelopen periode is gebeurd. Deze KPI's werden vooral door de Managing Director, de Head of Finance en de CTO genoemd en zijn geschikt om de prestaties van TMD Locks te beoordelen. De actuele productvoorraad, het besteladvies, de voorraad bij dealers en de gemiddelde maandelijkse verkoop per dealer zijn daarentegen leading: zij geven een signaal voordat een probleem ontstaat. Deze KPI's werden genoemd door Customer Support en B2B Sales en kunnen helpen om voorraadtekorten, zoals beschreven in paragraaf 1.2, op tijd te signaleren. De vergelijking tussen forecast en daadwerkelijke verkoop zit hier tussenin. Achteraf bekeken is deze KPI lagging, maar wanneer tijdens de forecastperiode ook wordt getoond hoeveel sloten nog moeten worden verkocht, kan tijdig worden bijgestuurd. Daarmee krijgt deze KPI ook een leading functie.

Geconcludeerd kan worden dat het Power BI-dashboard zowel gezamenlijke als afdelingsspecifieke KPI's moet bevatten. Hierbij is het belangrijk dat iedere afdeling eenvoudig toegang krijgt tot de informatie die voor haar werkzaamheden relevant is, zonder dat het dashboard onoverzichtelijk wordt.

### 7.3 Deelvraag 3

Welke eisen en wensen hebben medewerkers ten aanzien van de overzichtelijkheid en presentatie van bedrijfsgegevens en KPI's?

Uit de interviews blijkt dat medewerkers van TMD Locks momenteel regelmatig gebruikmaken van tabellen en Excel-bestanden om bedrijfsgegevens te bekijken en te analyseren. Hierbij moeten gegevens soms handmatig worden verwerkt of met elkaar worden vergeleken.

De geïnterviewde medewerkers hebben voornamelijk behoefte aan een overzichtelijke en gestructureerde weergave van de belangrijkste bedrijfsinformatie. Hierbij is het belangrijk dat relevante KPI's direct zichtbaar zijn, zonder dat medewerkers eerst verschillende bestanden of uitgebreide tabellen hoeven te doorzoeken.

Tijdens de interviews lag de nadruk voornamelijk op welke informatie medewerkers nodig hebben en welke KPI's zij het belangrijkst vinden. In de interviewverslagen zijn geen specifieke voorkeuren voor grafiektypen of visualisaties vastgelegd.

Op basis hiervan kan worden geconcludeerd dat het Power BI-dashboard vooral moet worden ingericht rondom de informatiebehoeften en prioriteiten van de verschillende afdelingen. De belangrijkste KPI's moeten in één oogopslag zichtbaar zijn, terwijl aanvullende informatie op een gestructureerde manier toegankelijk blijft.

### 7.4 Deelvraag 4

In welke systemen zijn de gegevens voor de gewenste KPI's beschikbaar en kunnen deze in Power BI worden geladen en berekend?

Uit de data-inventarisatie blijkt dat vrijwel alle benodigde gegevens beschikbaar zijn in Exact Online. Orders uit de webshop, Amazon en Decathlon worden via Shopify verwerkt en komen vervolgens in Exact Online terecht. Ook de activatie van serienummers en de advertentiekosten van Google Ads en Meta Ads worden in Exact Online vastgelegd. Deze gegevens kunnen via de custom connector in Power BI worden geladen. De forecast vormt hierop een uitzondering: deze wordt handmatig opgesteld in Excel en vervolgens in Power BI geladen.

Alle KPI's die tijdens de interviews zijn genoemd, kunnen met de beschikbare gegevens in Power BI worden weergegeven. Een deel van deze KPI's is niet direct als gegeven beschikbaar en moet daarom in Power BI worden berekend. Dit geldt onder andere voor de doorverkoop per dealer, de voorraad bij dealers, de performance-marketingkosten per B2C-slot en ROAS.

De voorraad bij dealers is hierbij een schatting. Deze wordt berekend door het aantal geleverde sloten te verminderen met het aantal sloten waarvan het serienummer door een eindklant is geactiveerd. Hierdoor kunnen sloten die al zijn verkocht, maar nog niet zijn geactiveerd, nog als voorraad bij de dealer worden meegeteld.

Geconcludeerd kan worden dat de voorgestelde KPI's met de huidige beschikbare gegevens in Power BI kunnen worden weergegeven en berekend. Het dashboard is daarmee technisch haalbaar. Wel moet de forecast handmatig worden bijgewerkt wanneer deze verandert.

### 7.5 Beantwoording hoofdonderzoeksvraag

Welke bedrijfsgegevens, KPI’s en presentatie-eisen moet TMD Locks opnemen in een voorstel voor een Power BI-dashboard dat aansluit bij de informatiebehoeften van de verschillende afdelingen?

Uit het onderzoek blijkt dat medewerkers van TMD Locks momenteel bedrijfsinformatie verzamelen en analyseren via verschillende systemen, waaronder Exact Online, Shopify en Excel. Hierbij worden gegevens regelmatig handmatig bijgehouden, gecombineerd en vergeleken. Deze werkwijze kost tijd. Er bestaat daarom behoefte aan een centrale omgeving waarin de belangrijkste bedrijfsinformatie overzichtelijk beschikbaar is.

Tijdens de interviews zijn de belangrijkste informatiebehoeften en KPI's van de verschillende afdelingen vastgesteld. Vooral verkoopaantallen, uitgesplitst naar B2B en B2C, de vergelijking tussen gerealiseerde verkoop en forecast en de performance-marketingkosten per verkocht B2C-slot worden door meerdere medewerkers belangrijk gevonden. Voorgesteld wordt om deze onderdelen op te nemen in het Power BI-dashboard.

Daarnaast hebben de verschillende afdelingen specifieke informatiebehoeften. Voor B2B Sales zijn de doorverkoop per dealer, de gemiddelde maandelijkse doorverkoop en de voorraadpositie bij dealers belangrijk. Voor Customer Support ligt de nadruk op actuele productvoorraad, verkoophistorie en besteladvies. Ook verkoopgegevens per periode, land, verkoopkanaal en productvariant en inzicht in ROAS worden meegenomen in het voorstel. Uit de data-inventarisatie blijkt bovendien dat alle voorgestelde KPI's met de gegevens uit Exact Online en Excel in Power BI kunnen worden weergegeven.

Uit de interviews blijkt daarnaast dat medewerkers behoefte hebben aan een duidelijke en gestructureerde weergave van bedrijfsinformatie. Daarom wordt voorgesteld om de belangrijkste KPI's per afdeling direct zichtbaar te maken op de bijbehorende dashboardpagina's. Aanvullende informatie kan op onderliggende pagina's worden weergegeven. In de interviewverslagen zijn geen specifieke voorkeuren voor grafiektypen of visualisaties vastgelegd.

Geconcludeerd kan worden dat het voorstel voor het Power BI-dashboard zowel gezamenlijke als afdelingsspecifieke bedrijfsgegevens en KPI's moet bevatten. Door de informatiebehoeften en prioriteiten van medewerkers als uitgangspunt te nemen, kan de presentatie worden afgestemd op hun werkzaamheden. De opdrachtgever beslist op basis van dit onderzoeksrapport welke voorgestelde KPI's en functionaliteiten worden opgenomen en welke prioriteit krijgen.


## 8. Aanbevelingen

Op basis van de onderzoeksresultaten en de afgenomen interviews wordt aanbevolen om binnen TMD Locks één centraal Power BI-rapport te ontwikkelen, waarin de belangrijkste bedrijfsgegevens en KPI's worden samengebracht.

Uit de interviews is gebleken dat de informatiebehoeften per afdeling verschillen. Daarom wordt voorgesteld om het rapport op te delen in verschillende pagina's per afdeling en onderwerp. Iedere pagina wordt daarbij afgestemd op de werkzaamheden en informatiebehoeften van de betreffende gebruikers.

### 8.1 Indeling van het Power BI-dashboard

Voor de inrichting van het Power BI-dashboard worden afzonderlijke pagina's per afdeling en onderwerp voorgesteld, waarop de belangrijkste KPI's overzichtelijk worden weergegeven.

Voor de afdeling Sales wordt een algemene overzichtspagina voorgesteld waarop de totale verkoopprestaties zichtbaar zijn. Hierin worden onder andere de totale verkoopaantallen en de verdeling tussen B2B en B2C opgenomen. Om beide verkooptypen uitgebreider te kunnen analyseren, wordt voorgesteld om B2B en B2C daarnaast ieder een eigen pagina te geven met de bijbehorende KPI's.

Op de B2C-pagina wordt voorgesteld om ook de performance-marketingkosten per verkocht B2C-slot, ROAS en de verkoopprestaties per verkoopkanaal weer te geven. Daarmee biedt deze pagina inzicht in zowel verkoop- als marketingprestaties.

Een aparte forecastpagina wordt voorgesteld om inzicht te geven in de voortgang ten opzichte van de verkoopdoelstellingen. Hier worden de daadwerkelijke verkoopresultaten vergeleken met de vooraf opgestelde forecast. Als verdere uitwerking wordt voorgesteld om het behaalde percentage van de doelstelling, het resterende aantal te verkopen sloten en het benodigde gemiddelde aantal verkopen per resterende dag van de forecastperiode te tonen. Zo kan de organisatie beoordelen of de verkopen op schema liggen. Hierdoor wordt de forecast niet alleen achteraf gebruikt, maar ook als leading indicator om tijdens de periode bij te sturen.

Voor Finance wordt een eigen pagina voorgesteld waarin de belangrijkste financiële en commerciële gegevens samenkomen. Op deze manier krijgt de afdeling inzicht in de KPI's die nodig zijn om de prestaties van TMD Locks te beoordelen, zoals maandelijkse verkoopaantallen, de verdeling tussen B2B en B2C en de vergelijking met de forecast.

Ook voor voorraadbeheer en inkoop wordt een eigen pagina voorgesteld. Op deze pagina worden de actuele voorraadstanden, historische verkoopaantallen en verkoopontwikkelingen weergegeven. Met deze informatie kan eventueel een besteladvies worden ontwikkeld om beter te bepalen welke producten en aantallen moeten worden ingekocht. Omdat de actuele voorraad en het besteladvies leading indicatoren zijn, kan deze pagina helpen om voorraadtekorten te signaleren voordat sloten niet meer leverbaar zijn.

Een afzonderlijke pagina voor de voorraad bij dealers wordt voorgesteld om te laten zien hoeveel sloten dealers naar schatting nog op voorraad hebben en hoeveel zij hebben doorverkocht. Hierdoor kan B2B Sales sneller bepalen welke dealers mogelijk nieuwe voorraad nodig hebben en wanneer contact kan worden opgenomen voor een herhaalbestelling. Ook deze informatie is leading: B2B Sales kan actie ondernemen voordat een dealer zonder voorraad zit.

Met deze indeling krijgt iedere afdeling toegang tot de informatie die voor haar werkzaamheden relevant is, terwijl de benodigde bedrijfsgegevens binnen één centrale rapportageomgeving beschikbaar zijn. Door gegevens en KPI's in Power BI samen te brengen en berekeningen te automatiseren, kunnen handmatige werkzaamheden worden verminderd. Wanneer de gegevens en berekeningen correct zijn ingericht en gecontroleerd, kan dit bijdragen aan een betrouwbaardere en efficiëntere informatievoorziening binnen TMD Locks.

### 8.2 Samenvatting van de aanbevelingen

Samenvattend wordt aanbevolen om één centraal Power BI-rapport te ontwikkelen met pagina's per afdeling en onderwerp. Op deze pagina's worden de bijbehorende KPI's en bedrijfsgegevens overzichtelijk weergegeven. Hierdoor kunnen medewerkers de voor hen relevante informatie snel terugvinden en de belangrijkste prestaties in één oogopslag beoordelen.

Door de bedrijfsgegevens centraal beschikbaar te maken en berekeningen zoveel mogelijk te automatiseren, kan de tijd die medewerkers besteden aan het handmatig verzamelen en verwerken van informatie worden verminderd. Daarnaast kan dit bij een correcte inrichting en controle de kans op fouten door handmatige berekeningen verkleinen.

Op deze manier sluit het voorstel voor het Power BI-dashboard aan bij de informatiebehoeften die tijdens de interviews naar voren zijn gekomen en kan het de verschillende afdelingen ondersteunen bij hun dagelijkse werkzaamheden en besluitvorming.

De opdrachtgever beslist op basis van dit onderzoeksrapport welke aanbevelingen worden overgenomen en welke onderdelen als eerste worden uitgewerkt.




## 9. Bronnen

Damen, R. (2026, 30 april). Hoe werkt Exact Online? Kosten, modules & tips (2026). Virtual Computing. Geraadpleegd op 29 oktober 2026, van https://virtualcomputing.nl/inzichten/hoe-werkt-exact-online

Exact. (2026, 28 augustus). Exact Online: de beste business software voor bedrijven en accountants | Exact. Geraadpleegd op 4 november 2026, van https://www.exact.com/nl/software/exact-online

Key Performance Indicators | IBM WebMethods Optimize for Process 11.1.0. (2026, November 2). IBM Documentation. https://www.ibm.com/docs/en/webmethods-bpm/wm-optimize/11.1.0?topic=concepts-key-performance-indicators

Jonker, J. A. A. (2026, 2 april). What are data quality dimensions? Geraadpleegd op 4 november 2026, van https://www.ibm.com/think/topics/data-quality-dimensions

What is data visualization? (2025, 17 november). Geraadpleegd op 4 november 2026, van https://www.ibm.com/think/topics/data-visualization

Whhender. (2026, 10 oktober). Power Query-Connectors - Power query. Microsoft Learn. Geraadpleegd op 4 november 2026, van https://learn.microsoft.com/nl-nl/power-query/connectors/

Wat is het verschil tussen B2B en B2C? - Schot. (2026, 31 juli). Schot. Geraadpleegd op 4 november 2026, van https://schot.nl/onze-diensten/advies-strategie/wat-is-het-verschil-tussen-b2b-en-b2c/

De Snoo, L. (2026, 28 januari). Forecasting: wat is het en hoe kan je er een maken? MKB Servicedesk. https://www.mkbservicedesk.nl/administratie/begroten/wat-is-forecasting

JulCsc. (2023, 25 maart). Wat is Power BI? - Power BI. Microsoft Learn. Geraadpleegd op 4 november 2026, van https://learn.microsoft.com/nl-nl/power-bi/fundamentals/power-bi-overview


The Open University. (2025). *Conducting an interview*. The Open University. Geraadpleegd op 9 november 2026, van https://help.open.ac.uk/postgraduate-study-skills/conducting-an-interview

Verhoeven, N. (2022). *Wat is onderzoek? Praktijkboek voor methoden en technieken* (7e druk). Boom.

Agile Business Consortium. (2014). *The DSDM Agile Project Framework Handbook*. Agile Business Consortium. Geraadpleegd op 23 november 2026, van https://www.agilebusiness.org/wp-content/uploads/2026/05/DSDM-Agile-Project-Framework-Handbook.pdf

Doran, G. T. (1981). There's a S.M.A.R.T. way to write management's goals and objectives. *Management Review, 70*(11), 35–36.

Few, S. (2013). *Information dashboard design: Displaying data for at-a-glance monitoring* (2nd ed.). Analytics Press.

Microsoft. (z.d.). *Tips voor het ontwerpen van een geweldig Power BI-dashboard*. Microsoft Learn. Geraadpleegd op 23 november 2026, van https://learn.microsoft.com/nl-nl/power-bi/create-reports/service-dashboards-design-tips

Parmenter, D. (2020). *Key performance indicators: Developing, implementing, and using winning KPIs* (4th ed.). Wiley.

Performance Marketing: A Beginner’s Guide (2026) - Shopify. (2026, 5 november). Shopify. Geraadpleegd op 15 november 2026, van https://www.shopify.com/blog/performance-marketing

Over doel-ROAS-biedingen - Google Ads help. (z.d.). Geraadpleegd op 15 november 2026, van https://support.google.com/google-ads/answer/6268637?hl=nl 

## Bijlage A: Begrippenlijst

In deze bijlage worden de belangrijkste begrippen uit het onderzoeksrapport toegelicht. De begrippen hebben betrekking op bedrijfsinformatie, data-analyse en het Power BI-dashboard. De onderstaande tabel geeft per begrip de betekenis en de bijbehorende bron.

| Begrip | Betekenis |Bron|
|---|---|---|
| **Power BI** | Een programma van Microsoft waarmee gegevens worden geanalyseerd en weergegeven in interactieve dashboards en rapportages. |(JulCsc, 2023)|
| **Exact Online** | Een online bedrijfssoftwarepakket waarin onder andere verkoop-, financiële en voorraadgegevens worden bijgehouden. |(Exact, 2026)|
| **Dashboard** | Een visueel overzicht van belangrijke bedrijfsinformatie en KPI's. |(JulCsc, 2023)|
| **KPI** | Key Performance Indicator: een meetbare indicator waarmee de prestaties van een organisatie worden beoordeeld. |(Key Performance Indicators, 2026)|
| **Datakwaliteit** | De mate waarin gegevens juist, volledig, actueel en betrouwbaar zijn. |(Jonker, 2026)|
| **Datavisualisatie** | Het weergeven van gegevens met grafieken, tabellen en diagrammen om informatie begrijpelijk te maken. |(What Is Data Visualization?, 2025)|
| **Connector** | Een technische koppeling waarmee gegevens vanuit Exact Online naar Power BI worden overgebracht. |(Whhender, 2026)|
| **B2B (Business-to-Business)** | Verkoop van producten of diensten aan andere bedrijven, zoals dealers en winkels. |(Wat Is het Verschil Tussen B2B en B2C? - Schot, 2026)|
| **B2C (Business-to-Consumer)** | Verkoop van producten of diensten aan consumenten, bijvoorbeeld via webshops. |(Wat Is het Verschil Tussen B2B en B2C? - Schot, 2026)|
| **Forecast** | Een prognose van toekomstige bedrijfsresultaten, bijvoorbeeld de verwachte omzet of verkoopcijfers. |(De Snoo, 2026)|
| **ROAS (Return on Ad Spend)** | De aan advertenties toegeschreven omzet gedeeld door de advertentiekosten. Deze verhouding laat zien hoeveel omzet iedere bestede advertentie-euro oplevert. | (Over doel-ROAS-biedingen - Google Ads Help, z.d.-b)|
| **Performance marketing** | Een vorm van online marketing die gericht is op meetbare resultaten, zoals klikken, aanvragen of verkopen. Campagnes worden beoordeeld en bijgestuurd op basis van deze resultaten. |(Performance Marketing: A Beginner’s Guide (2026) - Shopify, 2026b)|

## Versiebeheer 
|versie |datum | gedaan|
|---|---|-----|
|0.1 |29-10-2026|opzet gemaakt|
|0.11|30-10-2026| -voorwoord -samenvatting|
|0.12|03-11-2026| -inleiding|
|0.13|03-11-2026| -betrokkenpartijen|
|0.14|04-11-2026| - bronnen en begrippen|
|0.15|04-11-2026| - hoofd en deelvragen|
|0.16|05-11-2026| - onderzoeks methode |
|0.17|06-11-2026| - onderzoeks methode |
|0.18|09-11-2026|- onderzoeks methode |
|0.2|09-11-2026| - interview vragen |
|0.21|10-11-2026| - interview 1|
|0.23|12-11-2026| - interview 2,3|
|0.23|13-11-2026| - interview 4,5|
|0.24|14-11-2026| - interview resultaten|
|0.25|14-11-2026| - conclusie|
|0.26|15-11-2026| - aanbeveling|
|1|15-11-2026| - eerste versie|
|1.2|23-11-2026| - verbeteren|
