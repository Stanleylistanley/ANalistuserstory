# Analist Stanley - ontwerp voor sprint 4

## Inleiding
Dit ontwerp vertaalt de knelpunt en wensen van de beheerder naar concrete systeemfuncties, user stories, acceptatiecriteria en technische modellen. 
Het project Turing Lab is gevormd door onze opdrachtgever Harm. Hierbij wilt hij zijn huidige website efficienter maken en overzichtelijker voor de gebruiker.
De huidige website bestaat nu alleen uit een simpele links naar producten. Wij willen hier een systeem omheen bouwen om het efficienter te maken.
Na de analyse van de huidige website zijn er een aantal punten uitgekomen waar wij aan kunnen werken. Waaronder dat Harm handmatig in de code zelf producten beheert.
Dit is erg onhandig en inefficiënt.

Om dit knelpunt op te lossen, richt dit ontwerp zich op het knelpunt:
- De beheerder kan momenteel niet beheren via de applicatie, omdat er geen functionaliteit is om producten toe te voegen, aan te passen of te verwijderen. Hierdoor moeten wijzigingen handmatig via de code worden uitgevoerd, wat inefficiënt en foutgeboelig is.

Het doel is om een pagina op de website zelf te ontwikkelen waarbij Harm producten zelf kan beheren zonder in de code te hoeven duiken.

Relatie tot code: In onze huidige situatie hebben we al alle producten van Harm in ons database gestopt. hierbij moeten we dus nog een CRUD features bij toevoegen, zodat we vanuit de frontend data kunnen opslaan in de backend. De uitbreidingen die in dit ontwerp/analyse beschreven staan, bouwen voort op onze bestaande structuur.

## Knelpunt

## Producten toevoegen
Als beheerder wil ik nieuwe producten kunnen toevoegen via de applicatie, zodat de productcatalogus actueel blijft.

### Acceptatiecriteria
- [ ] Basisinformatie heeft
      - Naam
      - Prijs
      - Categorie 
      - Plaats(locatie)
      **Deze zijn verplicht**
- [ ] Categorie Bestaat uit Main/sub. Bijv Components/Resistors
- [ ] Bij locatie moet een shortcode worden ingevuld die automatisch
- [ ] Er is een "product opslaan" en "annuleer" knop
- [ ] Product wordt succesvol in de database opgeslagen
- [ ] na het succesvol opslaan toont er een bevestinging popup
- [ ] Product is daarna zichtbaar via de API(GET/products)
- [ ] Er zijn foutmeldingen bij ongeldige invoer. bijvoorbeeld bij categorie en locatie.

### Definition of ready (DoR)
- [ ] User story is duidelijk beschreven
- [ ] Acceptatie criteria zijn opgesteld
- [ ] Wireframe is opgesteld en gecheckt door team
- [ ] Benodigde velden zijn duidelijk
- [ ] Benodigde Backend requirements zijn bekend

### Definition of done (DoD)
- [ ] Beheerder kan succesvol een product toevoegen via applicatie
- [ ] Validatie werkt correct
- [ ] Product wordt in database opgeslagen
- [ ] product is zichtbaar via API
- [ ] Functionaliteit is getest



### Scenarios

Scenario 1 - Succesvol product toevoegen
- **Gegeven** de beheerder vult alle verplichte velden correct in
- **Wanneer** de beheerder op "Product opslaan" klikt
- **Dan** wordt het product opgeslagen in de database
- **En** verschijnt het product in het producten overzicht

Scenario 2 - Verplichte velden ontbreken
- **Gegeven** de beheerder laat verplichte velden leeg
- **Wanneer** de beheerder probeert op te slaan
- **Dan** krijgt de beheerder foutmeldingen
- **En** Wordt het product niet opgeslagen


### Use Case

Titel: Product toevoegen
Doel: Beheerder kan via de applicatie producten toevoegen aan het systeem zonder in de code te hoeven duiken.
Actor: Beheerder

Precondities:
- Beheerder is ingelogd
- Beheerder wilt een product toevoegen

Stappen:
- Beheerder opent de "producten toevoegen" pagina via de knop bij de productenoverzicht
- Beheerder vult de minimale verplichte velden in
- Beheerder vult de optionele velden in zo nodig
- Beheerder klikt op "product opslaan"
- Systeem valideert invoer
- Systeem slaat product op in database
- Systeem toont bevestiging

Alternatieve paden:
- Invoer ongeldig -> foutmelding -> terug naar formulier

Postcondities: Het product is succesvol opgeslagen in de database en is zichtbaar in het producten overzicht.


### Domeinmodel
### Toestandsdiagram
<img width="615" height="641" alt="image" src="https://github.com/user-attachments/assets/bdcf90df-4889-4de0-b27a-211f304daef1" />

Koppeling met user story
- Nieuw -> valideren -> opgeslagen = product succesvol toegevoegd
- Valideren -> Fout -> Nieuw = Validatie van invoer

Toestandstabel
| Toestand | Betekenis | Conditie | 
|----------|-----------|----------|
|   nieuw       | formulier is ingevuld en klaar om een nieuw product te zijn       |     invoer nog niet gevalideerd     |
|  valideren        |   Systeem controleert invoer        |    Opslaan actie is uitgevoerd      |
|  Fout        |  invoer is ongeldig         |    foute invoer van bijv. lege naam      |
| Opgeslagen         |   product is succesvol opgeslagen        |    Product staat in database      |



### wireframe
<img width="1048" height="483" alt="image" src="https://github.com/user-attachments/assets/eb5b38d0-3ad0-46c8-a37f-caca6a548467" />





### Product aanpassen
Als beheerder wil ik bestaande producten kunnen aanpassen, zodat ik fouten kan corrigeren of informatie kan bijwerken

### Producten verwijderen
Als beheerder wil ik producten kunnen verwijderen, zodat verouderde of niet op voorraad producten niet meer zichtbaar zijn.


