#  power Bi TMD Locks 

| Information | Details |
|---|---|
| auteur | Hugo Janse |
| Datum | 01-09-2026 |
| Versie | 0.13 |
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

Binnen TMD Locks kost het medewerkers veel tijd om de juiste bedrijfsinformatie te vinden. Bij het gebruik van Exact Online moeten medewerkers regelmatig zoeken, door uitgebreide tabellen scrollen en verschillende filters toepassen om de gewenste gegevens te verkrijgen. Dit maakt het opzoeken en analyseren van bedrijfsinformatie tijdrovend en inefficiënt.

Daarnaast is uit gesprekken met de opdrachtgever gebleken dat een deel van de bedrijfsgegevens handmatig wordt berekend buiten Exact Online om. Hierdoor bestaat het risico op menselijke fouten, waardoor niet altijd zeker is of de berekende cijfers een correct beeld geven van de bedrijfsprestaties.

Ook bij het presenteren van bedrijfsresultaten aan bijvoorbeeld potentiële investeerders levert dit problemen op. Het verzamelen van de juiste informatie kost tijd en uitgebreide tabellen uit Exact Online bieden onvoldoende overzicht om belangrijke resultaten op een duidelijke en professionele manier te presenteren.

Het centrale probleem is dat bedrijfsinformatie niet snel en overzichtelijk genoeg beschikbaar is en dat handmatige berekeningen risico's voor de betrouwbaarheid met zich meebrengen. Dit leidt tot onnodig tijdverlies en bemoeilijkt het analyseren en presenteren van bedrijfsresultaten.

### 1.3 Doelstelling

Het doel van dit onderzoek is om inzicht te krijgen in de informatiebehoeften van de verschillende afdelingen binnen TMD Locks. Door middel van gesprekken en interviews met medewerkers wordt onderzocht welke Key Performance Indicators (KPI's) voor iedere afdeling het belangrijkst zijn.

Op basis van deze informatie wordt een Power BI-dashboard ontwikkeld waarin de relevante bedrijfsgegevens op een duidelijke en overzichtelijke manier worden weergegeven. Hierbij staat gebruiksvriendelijkheid centraal, zodat medewerkers in één oogopslag de belangrijkste informatie kunnen vinden, zonder door uitgebreide tabellen te hoeven scrollen of verschillende filters te moeten toepassen.

Daarnaast richt het onderzoek zich op de betrouwbaarheid van de weergegeven cijfers. Hiervoor wordt gecontroleerd of de KPI's binnen Power BI correct worden berekend en overeenkomen met de gegevens uit Exact Online. Hiermee wordt beoogd het risico op fouten door handmatige berekeningen te verminderen en medewerkers te voorzien van betrouwbare informatie.

## 2. betrokken partijen 
Bij de ontwikkeling van het Power BI-dashboard zijn verschillende afdelingen en belanghebbenden betrokken. Iedere afdeling heeft eigen informatiebehoeften die tijdens het onderzoek in kaart worden gebracht. In onderstaande tabel worden de betrokken partijen en hun belangrijkste belangen weergegeven.

| Betrokken partij | Belang |
|---|---|
| **Management** | Overzicht van bedrijfsprestaties en onderbouwing van beslissingen. |
| **Verkoopafdeling** | Inzicht in verkoopcijfers, dealerprestaties, dealervoorraad en demosloten. |
| **Marketingafdeling** | Inzicht in verkoopontwikkelingen en productprestaties. |
| **Inkoop** | Verkoop- en voorraadgegevens als basis voor bestellingen. |
| **Overige medewerkers** | Snel relevante bedrijfsinformatie kunnen vinden. |
| **Investeerders** | Inzicht in belangrijke financiële resultaten, zoals omzet en winst, die op een duidelijke en professionele manier worden gepresenteerd. |

## 2. Onderzoeksvragen


Hoofdonderzoeksvraag

Hoe kan TMD Locks een Power BI-dashboard ontwikkelen dat aansluit bij de informatiebehoeften en relevante KPI's van de verschillende afdelingen, en deze overzichtelijk, betrouwbaar en gebruiksvriendelijk presenteert?


## Bronnen

Damen, R. (2026, 30 april). Hoe werkt Exact Online? Kosten, modules & tips (2026). Virtual Computing. Geraadpleegd op 29 oktober 2026, van https://virtualcomputing.nl/inzichten/hoe-werkt-exact-online

## versie beheer 
|versie |datum | gedaan|
|---|---|-----|
|0.1 |29-10-2026|opzet gemaakt|
|0.11|30-10-2026| -voorwoord -samenvatting|
|0.12|03-11-2026| -inleiding|
|0.13|03-11-2026| -betrokkenpartijen|