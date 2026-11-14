#  power Bi TMD Locks 

| Information | Details |
|---|---|
| auteur | Hugo Janse |
| Datum | 01-09-2026 |
| Versie | 0.24 |
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


## 5. Onderzoek

### 5.1 Onderzoeksmethode

Interviews

Om de informatiebehoeften van de verschillende afdelingen binnen TMD Locks in kaart te brengen, wordt gebruikgemaakt van semigestructureerde interviews. Hiervoor worden de hoofdverantwoordelijken van de betrokken afdelingen geïnterviewd.

Bij een semigestructureerd interview wordt gewerkt met een vooraf opgestelde vragenlijst, waarbij ruimte blijft om aanvullende vragen te stellen en dieper in te gaan op de antwoorden van de geïnterviewde. Deze methode maakt het mogelijk om de resultaten van verschillende interviews met elkaar te vergelijken, terwijl er tegelijkertijd aandacht kan worden besteed aan de specifieke werkzaamheden en informatiebehoeften van iedere afdeling.

Voor dit onderzoek wordt één algemene interviewleidraad opgesteld, die waar nodig wordt aangevuld met afdelingsspecifieke vragen. Tijdens de interviews wordt onderzocht welke bedrijfsgegevens medewerkers momenteel gebruiken, waarvoor zij Exact Online gebruiken, welke knelpunten zij ervaren en welke KPI's voor hun werkzaamheden belangrijk zijn. Daarnaast wordt besproken hoe zij deze informatie het liefst terugzien in het nieuwe Power BI-dashboard.

De resultaten van de interviews worden gebruikt om de informatiebehoeften per afdeling vast te stellen en de belangrijkste KPI's en eisen voor het Power BI-dashboard te selecteren.

#### Analyse van de interviewresultaten

Na het afnemen van de interviews worden de antwoorden per afdeling verzameld en geanalyseerd. Hierbij wordt gekeken naar de huidige informatiebehoeften, ervaren knelpunten en gewenste KPI's.

De resultaten worden vervolgens samengevoegd tot één overzicht waarin de belangrijkste KPI's en wensen van de verschillende afdelingen worden opgenomen.

Het overzicht met de verzamelde KPI's en informatiebehoeften wordt voorgelegd aan de opdrachtgever, Leonard Heuker of Hoek. Tijdens dit gesprek worden de onderzoeksresultaten besproken en bepaalt de opdrachtgever welke KPI's en functionaliteiten de hoogste prioriteit krijgen.

Op basis van deze prioritering worden de definitieve eisen voor het Power BI-dashboard vastgesteld.


**Doel:** Onderzoeken welke bedrijfsinformatie medewerkers momenteel gebruiken, welke KPI's zij belangrijk vinden en wat zij verwachten van het nieuwe Power BI-dashboard.

**Interviewduur:** 5–10 minuten

**1. Huidige informatie**

Welke bedrijfsinformatie uit exact online gebruik je momenteel het meest voor je werkzaamheden?

**2. Huidige werkwijze**

Waar en hoe zoek je deze informatie momenteel op?

**3. Tijdsduur**

Hoeveel tijd kost het je gemiddeld om deze informatie te vinden en eventueel te berekenen?

**4. Gewenste informatie**

Welke informatie en KPI's zou je graag terugzien in het nieuwe Power BI-dashboard?

**5. Prioriteiten**

Welke drie gegevens of KPI's zijn voor jou het belangrijkst om in één oogopslag te kunnen zien?


## 6. Resultaten van de interviews


In dit hoofdstuk worden de resultaten van vijf interviews met medewerkers van TMD Locks beschreven. De interviews zijn gehouden om inzicht te krijgen in de huidige werkwijze, de knelpunten bij het verzamelen en analyseren van bedrijfsgegevens en de informatiebehoeften van verschillende afdelingen.

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
| Verkoopaantallen B2B en B2C | Leonard, Arie |
| Verkoopaantallen per periode | Leonard, Arie, Marnix |
| Performance-marketingkosten per B2C-slot | Leonard, Arie, Marnix |
| Forecast versus daadwerkelijke verkoop | Leonard, Arie |
| Verkoop per kanaal | Leonard, Marnix |
| Verkoop per land | Leonard, Arie |
| ROAS | Marnix |
| Doorverkoop per dealer | Timo, Arie, Marnix |
| Gemiddelde maandelijkse verkoop per dealer | Timo |
| Voorraad bij dealers | Timo |
| Actuele productvoorraad | Gisela |
| Verkoopaantallen per productvariant | Gisela, Arie |
| Besteladvies op basis van voorraad en verkoop | Gisela |

Uit dit overzicht blijkt dat meerdere medewerkers behoefte hebben aan vergelijkbare verkoopgegevens. Vooral verkoopaantallen, marketingprestaties en de vergelijking met de forecast komen bij verschillende functies terug.

Daarnaast bestaan er specifieke informatiebehoeften die vooral voor één afdeling relevant zijn. Zo richt B2B Sales zich op de doorverkoop en voorraad bij dealers, terwijl Customer Support behoefte heeft aan actuele productvoorraad en ondersteuning bij inkoopbeslissingen.



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


The Open University. (2025). *Conducting an interview*. The Open University. Geraadpleegd op 9 november 2026, van https://help.open.ac.uk/postgraduate-study-skills/conducting-an-interview

## versie beheer 
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