#  power Bi TMD Locks 

| Information | Details |
|---|---|
| auteur | Hugo Janse |
| Datum | 01-09-2026 |
| Versie | 0.4 |
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

## Table of Contents
- [Voorwoord](#voorwoord)
- [samenvatting](#samenvatting)
- [Introductie ](#introductie )
- [1. Normal Traffic Lights](#1-normal-traffic-lights)
- [2. Smart Traffic Lights](#2-smart-traffic-lights)
- [3. Sensors in Smart Traffic Lights](#3-sensors-in-smart-traffic-lights)
- [Sensors](#sensors)
- [Result](#result)
- [Recommendation](#recommendation)
- [Conclusion](#conclusion)

---

## Introductie 

### 1.1 Aanleiding
Binnen TMD Locks worden bedrijfsgegevens opgeslagen in Exact Online. In de praktijk blijkt dat medewerkers veel tijd kwijt zijn aan het zoeken, scrollen en toepassen van filters om de juiste informatie te vinden. Gegevens zijn daardoor niet altijd snel en overzichtelijk beschikbaar wanneer dat nodig is.

Om deze reden is behoefte ontstaan aan een nieuw dashboard in Power BI, waarin belangrijke bedrijfsgegevens op een duidelijke en toegankelijke manier worden gepresenteerd voor de verschillende afdelingen.

### 1.2 Probleemstelling

Binnen TMD Locks kost het medewerkers veel tijd om de juiste bedrijfsinformatie te vinden. Bij het gebruik van Exact Online moeten medewerkers regelmatig zoeken, door uitgebreide tabellen scrollen en verschillende filters toepassen om de gewenste gegevens te verkrijgen. Dit maakt het opzoeken en analyseren van bedrijfsinformatie tijdrovend en inefficiënt.

Daarnaast is uit gesprekken met de opdrachtgever gebleken dat een deel van de bedrijfsgegevens handmatig wordt berekend buiten Exact Online om. Hierdoor bestaat het risico op menselijke fouten, waardoor niet altijd zeker is of de berekende cijfers een correct beeld geven van de bedrijfsprestaties.

Ook bij het presenteren van bedrijfsresultaten aan bijvoorbeeld potentiële investeerders levert dit problemen op. Het verzamelen van de juiste informatie kost tijd en uitgebreide tabellen uit Exact Online bieden onvoldoende overzicht om belangrijke resultaten op een duidelijke en professionele manier te presenteren.

Het centrale probleem is dat bedrijfsinformatie niet snel en overzichtelijk genoeg beschikbaar is en dat handmatige berekeningen risico's voor de betrouwbaarheid met zich meebrengen. Dit leidt tot onnodig tijdverlies en bemoeilijkt het analyseren en presenteren van bedrijfsresultaten.


## Introduction

Why do we need smarter traffic lights? Traffic jams are a real problem in cities. They are not only annoying and stressful for people, but they also increase air pollution. Poorly timed traffic lights can also create dangerous situations. Traditional traffic lights follow a fixed schedule and struggle to adapt to real-time conditions.

A smart traffic light uses real-time data and makes decisions based on what its environment demands. Traditional lights work on fixed schedules, which can cause traffic jams or waste green-light time when no one is waiting. In contrast, smart traffic lights adapt to traffic demands. For example, if a long queue is detected, the system can extend the green light. If a pedestrian is detected, it can activate a safe crossing phase.

---

## Main Question

What are smart traffic lights and what sensors do we need?

---

## Sub-questions

1. What are normal traffic lights?  
2. What are smart traffic lights?  
3. What sensors are used in smart traffic lights?  

---

## 1. Normal Traffic Lights

One of the most common problems in traffic is congestion. Traffic jams cause delays, stress, and increased pollution. The longer cars are waiting, the more fuel they use and the more pollution they produce.

Traffic lights are a relatively simple and low-cost solution to guide traffic. A traffic light consists of three lights: red, orange (yellow), and green.  
- Green: vehicles may proceed  
- Orange: prepare to stop  
- Red: stop  

![crossroad](../assets/treffic/traf1.png)  
<sup><sub>Image 1. A 4-lane intersection without movement directions.</sub></sup>

At an intersection, vehicles can go left, right, or straight. These movements are grouped into phases.

![crossroad+movement](../assets/treffic/traf2.png)  
<sup><sub>Image 2. A 4-lane intersection with movement directions.</sub></sup>

These movements are controlled in phases.

![phases](../assets/treffic/traf3.png)  
<sup><sub>Image 3. Ring-and-barrier diagram showing traffic phases.</sub></sup>

Each phase has fixed timing for green, orange, and red lights. This fixed timing is inefficient because it cannot adapt to real-time traffic conditions.

---

## 2. Smart Traffic Lights

Now that we understand traditional traffic lights, we can look at smart traffic lights.

A “smart” system can sense its environment, collect data, and respond automatically. A smart traffic light uses sensors and a microcontroller to adjust its behavior based on real-time conditions.

For example:
- Detecting vehicles waiting at an intersection  
- Detecting pedestrians  
- Adjusting green-light duration dynamically  

Smart traffic lights improve traffic flow and safety by reacting to actual conditions instead of following a fixed schedule.

---

## 3. Sensors in Smart Traffic Lights

To make traffic lights smart, sensors are required. In this report, three types of sensors are analyzed.

---

## Sensors

### 1. Inductive Loop

Inductive loops are commonly used in real traffic systems. They are wires embedded in the road that create a magnetic field. When a vehicle passes over them, the field changes, and the system detects the vehicle.

**Advantages:**
- Very reliable  
- Widely used  

**Disadvantages:**
- Difficult to install  
- Requires road construction  

---

### 2. Ultrasonic Sensors

Ultrasonic sensors measure distance using sound waves. They send out a signal and measure how long it takes to return.

**Advantages:**
- Low cost  
- Easy to install  
- Good for prototypes  

**Disadvantages:**
- Less accurate than other systems  
- Limited range  

---

### 3. Camera Detection

Camera systems analyze video images to detect vehicles and traffic conditions.

**Advantages:**
- Advanced detection  
- Flexible use  

**Disadvantages:**
- Expensive  
- Sensitive to weather and lighting  

---

## Result

From this research, I learned how both traditional and smart traffic lights work. Traditional traffic lights use fixed timings, which can lead to inefficiency and unnecessary waiting.

Smart traffic lights improve this by using real-time data and sensors to adapt to traffic conditions.

I also explored different sensors, each with its own strengths and weaknesses. This helped me understand which sensors are suitable for my project.

---

## Recommendation

For this project, ultrasonic sensors are recommended.

They are:
- Affordable  
- Easy to install  
- Suitable for prototypes  

Inductive loops are more reliable but difficult to implement in a prototype. Camera systems are powerful but expensive and sensitive to environmental conditions.

Therefore, ultrasonic sensors provide the best balance between cost, simplicity, and functionality.



---

## Conclusion

In this report, the differences between traditional and smart traffic lights were analyzed. Traditional systems rely on fixed timings, which often leads to inefficient traffic flow, unnecessary waiting times, and increased air pollution.

Smart traffic lights improve this by using sensors and real-time data to adapt to their environment. By detecting vehicles and pedestrians, they can make better decisions, resulting in safer and more efficient traffic flow.

Different sensors were explored, including inductive loops, ultrasonic sensors, and camera detection. Each has its own advantages and disadvantages.

It can be concluded that smart traffic lights are a more effective solution for modern cities. They improve traffic flow, reduce waiting times, and help reduce pollution. Therefore, they are an important step toward smarter and more efficient cities.

👉 [My traffic light design](design.md)



### Sourses 
How Do Traffic Signals Work? (z.d.). YouTube. https://www.youtube.com/watch?v=DP62ogEZgkI

Rokonuzzaman, M. (2021). Title of the article. Journal Name.
https://www.sciencedirect.com/science/article/abs/pii/S014829632100847X

Editraffic. (2023). Inductive loop detector basics.
https://www.editraffic.com/wp-content/uploads/2023/07/Inductive-Loop-Detector-Basics.pdf


MaxBotix Inc. (z.d.). How ultrasonic sensors work.
https://maxbotix.com/blogs/blog/how-ultrasonic-sensors-work

Jackwin Safety. (z.d.). What are the cameras on top of traffic lights?
https://jackwinsafety.com/what-are-the-cameras-on-top-of-traffic-lights/

chatGPT


## Bronnen

Damen, R. (2026, 30 april). Hoe werkt Exact Online? Kosten, modules & tips (2026). Virtual Computing. Geraadpleegd op 29 oktober 2026, van https://virtualcomputing.nl/inzichten/hoe-werkt-exact-online

## versie beheer 
|versie |datum | gedaan|
|---|---|-----|
|0.1 |29-10-2026|opzet gemaakt|
|0.11|30-10-2026| -voorwoord -samenvatting|
|||
