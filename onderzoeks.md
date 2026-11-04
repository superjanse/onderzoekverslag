#  power Bi TMD Locks 

| Information | Details |
|---|---|
| auteur | Hugo Janse |
| Datum | 01-09-2026 |
| Versie | 0.15 |
| clasievicatie | Intern |
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
Dit onderzoeksrapport richt zich op de ontwikkeling van een Power BI-dashboard voor TMD Locks, een bedrijf dat zich bezighoudt met de ontwikkeling en verkoop van slimme kettingsloten. Deze sloten maken gebruik van technologie om zonder een traditionele sleutel geopend te kunnen worden.

Binnen TMD Locks worden bedrijfsgegevens, zoals verkoopcijfers, voorraadgegevens en informatie over dealers, opgeslagen in Exact Online. Exact Online is een online bedrijfssoftwarepakket waarmee organisaties verschillende bedrijfsprocessen kunnen beheren en administratieve gegevens kunnen opslaan.

Hoewel Exact Online geschikt is voor het beheren van bedrijfsgegevens, is het niet altijd eenvoudig om deze informatie overzichtelijk te analyseren en te presenteren. Daarom wordt Power BI gebruikt om belangrijke bedrijfsinformatie op een centrale plek samen te brengen en inzichtelijk te maken voor de verschillende afdelingen binnen TMD Locks (Damen, 2026). 

Het doel van dit onderzoek is om te bepalen hoe een Power BI-dashboard ontwikkeld kan worden dat aansluit bij de informatiebehoeften van de verschillende afdelingen. Hierbij staan overzichtelijkheid, betrouwbaarheid en gebruiksvriendelijkheid centraal.

Om dit doel te bereiken, wordt onderzocht welke bedrijfsgegevens en Key Performance Indicators (KPI's) belangrijk zijn voor de organisatie. Hiervoor worden gesprekken en interviews gehouden met medewerkers van verschillende afdelingen. Tijdens deze gesprekken wordt onderzocht welke informatie zij nodig hebben, welke verwachtingen zij hebben en hoe deze informatie het beste kan worden weergegeven.

Op basis van de onderzoeksresultaten wordt een nieuw Power BI-dashboard ontwikkeld. Hierbij wordt gebruikgemaakt van een iteratieve werkwijze, waarbij het dashboard stapsgewijs wordt ontwikkeld, beoordeeld en verbeterd aan de hand van feedback van gebruikers.

Table of Contents

## Inhoudsopgave

- [Voorwoord](#voorwoord)
- [Samenvatting](#samenvatting)
- [1. Introductie](#1-introductie)
  - [1.1 Aanleiding](#11-aanleiding)
  - [1.2 Probleemstelling](#12-probleemstelling)
  - [1.3 Doelstelling](#13-doelstelling)
- [2. Betrokken partijen](#14-betrokken-partijen)
- [3. Onderzoeksvragen](#2-onderzoeksvragen)
  - [3.1 Hoofdonderzoeksvraag](#21-hoofdonderzoeksvraag)
- [Bronnen](#bronnen)
- [Versiebeheer](#versiebeheer)

---

## Introductie 

### 1.1 Aanleiding
Binnen TMD Locks worden bedrijfsgegevens opgeslagen en beheerd in Exact Online, waaronder verkoopcijvers, voorraadgegevens en onvormatie over de dealers. Deze gegevens zijn belangrijk voor de dagelijkse werkzaamheden van verschillende afdelingen, zoals verkoop, marketing, inkoop en management.

De organisatie heeft behoefte aan een centrale en overzichtelijke manier om deze informatie toegankelijk te maken. Daarom is besloten een Power BI-dashboard te ontwikkelen waarin de belangrijkste bedrijfsgegevens worden samengebracht en op een duidelijke manier worden gepresenteerd. Hierdoor kunnen medewerkers in één oogopslag de informatie vinden die voor hen relevant is.

### 1.2 Probleemstelling

Tijdens de eerste gesprekken met de opdrachtgever, zijn verschillende problemen rondom het verzamelen, analyseren en presenteren van bedrijfsgegevens binnen TMD Locks naar voren gekomen.

Momenteel kost het medewerkers extra tijd om de juiste informatie in Exact Online te vinden. Zij moeten regelmatig door uitgebreide tabellen zoeken en verschillende filters toepassen. Dit geldt onder andere voor verkoopcijfers, het aantal verkochte sloten per dealer, dealervoorraad en verkoopontwikkelingen.

Daarnaast heeft de organisatie behoefte aan KPI's die worden berekend op basis van bestaande bedrijfsgegevens. Deze berekeningen zijn niet direct beschikbaar in Exact Online en worden daarom uitgevoerd op het moment dat de informatie nodig is, soms met behulp van Excel. Dit kost extra tijd en brengt bij handmatige berekeningen het risico op menselijke fouten met zich mee.

Ook voor inkoop en logistiek is overzichtelijke bedrijfsinformatie belangrijk. Binnen TMD Locks is het voorgekomen dat sloten niet tijdig geleverd konden worden doordat deze niet op voorraad waren. Goed inzicht in de beschikbare voorraad en verwachte leveringen is daarom belangrijk om de voorraadplanning te ondersteunen.

Verder is het momenteel lastig om bedrijfsresultaten op een duidelijke en professionele manier aan potentiële investeerders te presenteren. TMD Locks wil inzicht kunnen geven in omzet, winst, verkoopprestaties en de voortgang ten opzichte van de opgestelde forecasts.

Het centrale probleem is dat belangrijke bedrijfsinformatie binnen TMD Locks niet direct overzichtelijk beschikbaar is en aanvullende KPI's afzonderlijk moeten worden berekend. Hierdoor kost het verzamelen, analyseren en presenteren van informatie extra tijd en is het lastig om snel inzicht te krijgen in de bedrijfsprestaties

### 1.3 Doelstelling

Het doel van dit onderzoek is om inzicht te krijgen in de informatiebehoeften van de verschillende afdelingen binnen TMD Locks. Door middel van gesprekken en interviews met medewerkers wordt onderzocht welke Key Performance Indicators (KPI's) voor iedere afdeling het belangrijkst zijn.

Op basis van deze informatie wordt een Power BI-dashboard ontwikkeld waarin de relevante bedrijfsgegevens op een duidelijke en overzichtelijke manier worden weergegeven. Hierbij staat gebruiksvriendelijkheid centraal, zodat medewerkers in één oogopslag de belangrijkste informatie kunnen vinden, zonder door uitgebreide tabellen te hoeven scrollen of verschillende filters te moeten toepassen.

Daarnaast richt het onderzoek zich op de betrouwbaarheid van de weergegeven cijfers. Hiervoor wordt gecontroleerd of de KPI's binnen Power BI correct worden berekend en overeenkomen met de gegevens uit Exact Online. Hiermee wordt beoogd het risico op fouten door handmatige berekeningen te verminderen en medewerkers te voorzien van betrouwbare informatie.


## 2. Betrokken partijen

Bij de ontwikkeling van het Power BI-dashboard zijn verschillende afdelingen en belanghebbenden betrokken. Iedere afdeling heeft eigen informatiebehoeften die tijdens het onderzoek in kaart worden gebracht.

De hoofdverantwoordelijken van alle betrokken afdelingen worden geïnterviewd om hun informatiebehoeften, belangrijkste KPI's en verwachtingen van het dashboard vast te stellen.

In onderstaande tabel worden de betrokken partijen, hun belangen en hun betrokkenheid bij het onderzoek weergegeven.

| Betrokken partij | Belang bij het dashboard | Betrokkenheid bij het onderzoek |
|---|---|---|
| **Management** | Inzicht in omzet, winst, forecasts en algemene bedrijfsprestaties ter ondersteuning van beslissingen. | Opdrachtgever stelt eisen en beoordeelt het dashboard. |
| **Sales B2B** | Inzicht in dealerprestaties, dealervoorraad, verkochte sloten per dealer en aanwezigheid van demosloten bij winkels. | De hoofdverantwoordelijke wordt geïnterviewd over de gewenste KPI's en informatiebehoeften. |
| **Sales B2C** | Inzicht in verkoopcijfers via onder andere Amazon en Decathlon, verkoopontwikkelingen en de beschikbare interne magazijnvoorraad. | De hoofdverantwoordelijke wordt geïnterviewd over de gewenste verkoop- en voorraadgegevens. |
| **Marketing** | Inzicht in advertentiekosten, advertentiekosten per verkocht slot en verkoopontwikkelingen. | De hoofdverantwoordelijke wordt geïnterviewd over relevante marketing-KPI's. |
| **Inkoop en logistiek** | Inzicht in actuele voorraadniveaus, beschikbare sloten en verwachte leveringen. | De hoofdverantwoordelijken worden geïnterviewd over de benodigde voorraad- en leveringsinformatie. |
| **Investeerders** | Inzicht in omzet, winst, verkoopprestaties en de voortgang ten opzichte van forecasts. | Indirect betrokken. Ontvangen relevante bedrijfsresultaten via presentaties of screenshots, zonder dagelijkse toegang tot het dashboard. |

## 3. Begrippenlijst

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



## 4. Onderzoeksvragen


### 4.1 Hoofdonderzoeksvraag

Hoe kan TMD Locks een Power BI-dashboard ontwikkelen dat aansluit bij de informatiebehoeften en relevante KPI's van de verschillende afdelingen, en deze overzichtelijk, betrouwbaar en gebruiksvriendelijk presenteert?

### 4.2 deelvragen 
1. Hoe verzamelen en analyseren medewerkers van TMD Locks momenteel bedrijfsinformatie en welke knelpunten ervaren zij hierbij?

2. Welke bedrijfsgegevens en KPI's zijn voor de verschillende afdelingen binnen TMD Locks het belangrijkst om hun werkzaamheden uit te voeren en beslissingen te ondersteunen?

3.  In hoeverre komen de gegevens en berekende KPI's in Power BI overeen met de oorspronkelijke gegevens uit Exact Online, en waardoor ontstaan eventuele verschillen?

4.  Hoe kunnen de geselecteerde KPI's en bedrijfsgegevens binnen Power BI op een overzichtelijke en gebruiksvriendelijke manier worden gevisualiseerd, zodat medewerkers in één oogopslag de belangrijkste informatie kunnen vinden?
   
5.  In hoeverre voldoet het ontwikkelde Power BI-dashboard aan de vastgestelde informatiebehoeften en eisen op het gebied van overzichtelijkheid, gebruiksvriendelijkheid en betrouwbaarheid? 


## Bronnen

Damen, R. (2026, 30 april). Hoe werkt Exact Online? Kosten, modules & tips (2026). Virtual Computing. Geraadpleegd op 29 oktober 2026, van https://virtualcomputing.nl/inzichten/hoe-werkt-exact-online

Exact. (2026, 28 augustus). Exact Online: de beste business software voor bedrijven en accountants | Exact. Geraadpleegd op 4 november 2026, van https://www.exact.com/nl/software/exact-online

Key Performance Indicators | IBM WebMethods Optimize for Process 11.1.0. (2026, November 2). IBM Documentation. https://www.ibm.com/docs/en/webmethods-bpm/wm-optimize/11.1.0?topic=concepts-key-performance-indicators

Jonker, J. A. A. (2026, 2 april). What are data quality dimensions? Geraadpleegd op 4 november 2026, van https://www.ibm.com/think/topics/data-quality-dimensions

What is data visualization? (2025, 17 november). Geraadpleegd op 4 november 2026, van https://www.ibm.com/think/topics/data-visualization

Whhender. (2026, 10 oktober). Power Query-Connectors - Power query. Microsoft Learn. Geraadpleegd op 4 november 2016, van https://learn.microsoft.com/nl-nl/power-query/connectors/

Wat is het verschil tussen B2B en B2C? - Schot. (2026, 31 juli). Schot. Geraadpleegd op 4 november 2026, van https://schot.nl/onze-diensten/advies-strategie/wat-is-het-verschil-tussen-b2b-en-b2c/

De Snoo, L. (2026, 28 januari). Forecasting: wat is het en hoe kan je er een maken? MKB Servicedesk. https://www.mkbservicedesk.nl/administratie/begroten/wat-is-forecasting

JulCsc. (2023, 25 maart). Wat is Power BI? - Power BI. Microsoft Learn. Geraadpleegd op 4 november 2026, van https://learn.microsoft.com/nl-nl/power-bi/fundamentals/power-bi-overview
## versie beheer 
|versie |datum | gedaan|
|---|---|-----|
|0.1 |29-10-2026|opzet gemaakt|
|0.11|30-10-2026| -voorwoord -samenvatting|
|0.12|03-11-2026| -inleiding|
|0.13|03-11-2026| -betrokkenpartijen|
|0.14|04-11-2026| - bronnen en begrippen|
|0.15|04-11-2026| - hoofd en deelvragen|