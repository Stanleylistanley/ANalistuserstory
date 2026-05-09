# Visie-scope voor sprint 4

## Inleiding
In dit visie-scope/analyse document ga ik de huidige situatie, behoeften en verbeterkansen van het project Turing lab beschrijven.
Het document vormt de basis voor de ontwikkeling van de bestaande website van onze opdrachtgever Harm.

In de loop van dit project zijn er veel nieuwe knelpunten en kansen ontstaan, waardoor het essentieel is om te bepalen welke functionele eisen en wensen in dit traject centraal zullen staan.
Omdat er in het begin van dit project al een visie scope is opgesteld, zal ik in dit document starten met een kleine samenvatting van de belangrijkste onderdelen die niet door de tijd zijn veranderd.

## Inhoudsopgave
- Organisatorische context
- Aanleiding
- Bedrijfsprocessen en probleemstelling
   - Huidige situatie
   - Gewenste situatie
-Knelpunten en Kansen
- Verwachte resultaat
- Conclusie

## Organisatorische context
Dit project wordt uitgevoerd binnen de Hogeschool Utrecht. Op de campus bevindt zich een interne materialenwinkel (Het Turing Lab) waar studenten elketronische producten kunnen verkrijgen voor hardware- en softwareprojecten binnen opleidingem zoals ICT, open-ICT, werktuigbouwkunde en elektrotechniek.

De materialenwinkel wordt beheerd door de opdrachtgever/ docent Harm. De opdrachtgever is verantwoordelijk voor de inkoop en het beheer van de voorraad. Harm is zelf Technische informatica docent. Daarnaast helpen er ook studenten als medewerkers met dagelijkse werkzaamheden.

De kernactiviteit van deze organisatie is het beschikbaar stellen van elektronische materialen aan studenten voor onderwijs- en projectdoeleinden. Hierbij gaat het om meer dan 800 elektronische onderdelen die regelmatig worden gebruikt binnen onderwijsprojecten.

In dit project zijn de opdrachtgever (docent en beheerder van de Turing Lab), studentmedewerkers die met de voorraad werken en de studenten die gebruikmaken van de producten van de materialenwinkel direct betrokken.

## Aanleiding
Het Turing Lab is een plek binnen de ICT-opleiding van Hogeschool Utrecht waar studenten werken aan projecten met hardware en software. In dit lab is er een webshop met ongeveer 833 elektronische producten die studenten kunnen gebruiken. Per jaar zijn er meer dan 1500 transacties.

De webshop is op dit moment een simpele HTML-pagina die gemaakt wordt met een Python-script. Dit werkt, maar er is geen goed systeem om de voorraad bij te houden. Studenten kunnen producten pakken zonder dat dit ergens wordt bijgehouden. Daardoor is het niet duidelijk hoeveel producten er nog zijn.

Dit zorgt voor problemen. Producten kunnen ineens op zijn zonder dat iemand het merkt. Ook is er geen overzicht van welke producten opnieuw besteld moeten worden. Daarnaast hangt het systeem sterk af van één persoon, wat een risico is.

Dit heeft gevolgen voor zowel studenten als beheerders. Studenten weten niet of een product beschikbaar is, en beheerders hebben geen duidelijk overzicht van de voorraad. Hierdoor is het moeilijk om de voorraad goed te beheren.

Een belangrijke voorwaarde is dat de huidige manier van werken niet veel mag veranderen en dat er geen extra handelingen bijkomen voor gebruikers. Daarom is er behoefte aan een ICT-oplossing die helpt om beter inzicht te krijgen in de voorraad, zonder het proces ingewikkelder te maken.

De aanleiding voor dit project is dus dat er nu geen duidelijk en actueel overzicht van de voorraad is, en dat dit verbeterd moet worden op een eenvoudige manier die past bij de huidige werkwijze van het Turing Lab.

## Bedrijfsprocessen en probleemstelling
Om de probleemstelling te odnerhalen is het belangrijk om de huidige en gewenste situaite in kaart te brengen en de visie te begrijpen. Voor deze analyse ga ik kijken naar het proces van het beheren van producten. Hierbij hebben we gekeken naar het huidige proces van harm en is er geconstateerd dat Harm al zijn producten via de code zelf beheert. Dat er onhandig en inefficiënt is.


### Huidige situatie
Huidige proces tussen Harm, directeur en systeem:
<img width="791" height="491" alt="image" src="https://github.com/user-attachments/assets/2e47233c-4190-4a7a-8834-26df6b8db095" />
De huidige webshop van het Turing Lab bestaat uit een eenvoudige HTML-pagina die wordt gegenereerd met behulp van een python-script. 
De website geeft studenten de mogelijkheid om producten te bekijken, maar het bevat verder geen andere functionaliteiten.

Wanneer de beheerder prodcuten wil toevoegen, aanpassen of verwijderen, moet dit handmatig via de code worden uitgevoerd. Dit is erg inefficiënt en onhandig. Er is dus geen centrale beheeromgeving waar producten eenvoudig beheerd kunnen worden. Het huidige systeem is ook erg afhankelijk van Harm, omdat alleen hij weet hoe de website in elkaar zit.

### Gewenste situatie
Voor het Toevoegen van producten:
<img width="1387" height="470" alt="image" src="https://github.com/user-attachments/assets/77daa643-ccb1-425d-9f9c-ab6f4d89e41e" />

Voor het bewerken en verwijderen van producten:
<img width="1572" height="292" alt="image" src="https://github.com/user-attachments/assets/8a94a915-9269-4467-a261-7d6c07bfaae9" />


In de gewenste situatie beschikt de website over een beheeromgeving waarin producten eenvoudig via de applicatie beheerd kunnen worden. De beheerder moet de producten kunnen toevoegen, aanpassen en verwijderen zonder wijzigingen direct in de code uit te voeren.

Door middel van een formulier kan de beheerder productinformatie zoals naam, prijs, categorie, locatie en afbeeldingen beheren. Hierdoor wordt het beheer efficiënter, minder foutgevoelig en beter beheerbaar. 


## Verwachte resultaat Sprint 4
Voor sprint 4 is het belangrijkste doel om de functionaliteit van het beheren van producten toe te voegen

## Conclusie

