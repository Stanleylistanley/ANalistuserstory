# Sprint review 3 - verslag


Tijdens Sprint review 3 hebben we met het team de voortgang van het project besproken met Harm.
We hebben hierbij feedback en mogelijke uitbreidingen besproken. Ook hebben we feedback verzameld op zowel de frontend als backend van de applicatie.
De review heeft ons een goed beeld gegeven wat er nog aangepast moet worden en wat al goed is.

# Review met Product Owner

## Positieve punten
Er werd aangegeven dat de applicatie er al heel goed uit ziet en de meeste functionaliteiten al werkend zijn.
Ook gaf Harm zelf aan dat hij merkte dat de applicatie sneller was geworden vooral bij het laden van de producten, omdat dat bij sprint 2 nog erg sloom was.
Wij fetchen nu namelijk op minder producten, waardoor het iets sneller is. Daarnaast werd het design van de categorieën en gebruikers gedeelte goed ontvangen.

## Feedback en aandachtspunten
Ook kwamen er kleine opmerkingen over de navigatie en duidelijkheid van sommige onderdelen.
- Na het inloggen moet de gebruiker direct naar de productenpagina worden gestuurd. De productenoverzicht is de landingspagina.
- Locatie “LA6” is duidelijk zichtbaar, maar locaties zoals “55,6” zijn minder begrijpelijk. Als mogelijke oplossing werd een popup met een foto of een duidelijker overzicht van de lade genoemd.
- Er is geen documentatie over hoe de applicatie werkt, een soort overdrachtsdocument.
- Bij de productenoverzicht missen er eurotekens.

Bij het laten zien van de wireframe van de producten toevoegen pagina zijn er ook een paar aantekeningen gemaakt.
- Categorie was in de wireframe een input field. Suggestie van harm was om een dropdown te gerbuiken met de huidige categorieën.
- Informatie veld voor de extra info kan groter.
- Validatie velden
- 0,01 en 0,10 zijn gratis om mee te nemen.


## Extra suggesties
- Boodschappenlijst, zodat je zo min mogelijk lades hoeft te openen
- Commentaar, review van een gebruiker.
- Betalingsmethode met de QR code.
- Bakje leeg met qr code.
- Locaties generenen.


## Sprint planning voor sprint 4
Voor sprint 4 zijn de volgende werkzaamheden gepland. Deze zijn gevormd uit de aantekeningen.
•	Producten beheren ( Toevoegen, aanpassen, verwijderen)

•	Meldingen in het meldingenoverzicht kunnen opgelost worden

•	Design van gebruiker bewerken en profiel paginas update 

•	Profielpagina koppelen met login

•	Je kunt bepaalde functionaliteiten zien doormiddel van je rol

•	Productenpagina detail de locaties moeten duidelijker. (dropdown met foto)

•	Project op Azure deployen 

•	Filter en searchbar een shared component maken

•	Features mappen aanpassen frontend

•	Documentatie frontend , checklist naar eigenpagina, overdrachtsdocument

•	Testen: JUnit test, axe test


## Code review

### Algemene punten

**Voor op productie:**
- Localhost heeft nu al een hele hoge miliseconde, komt omdat er nogsteeds veel producten worden gefetched
- Filters en paginering serverside en niet clientside
- fetchen op 7 producten, zodat de miliseconde minder wordt.



**Lades code review**
Ladefunctionaliteit

Voor de lades werden de volgende technische verbeterpunten besproken:

- Binnen de backend moet meer gewerkt worden volgens een resource-oriented architecture.
- Het gebruik van een lijst met integers in de controller werd als onduidelijk gezien.
- drawerId hoort logischerwijs thuis in de DrawerController in plaats van de ProductController.
- Controllers moeten werken met DTO’s in plaats van domeinobjecten.
- Exceptions horen bij voorkeur in de presentation-laag.( maar voor nu niet erg)


**Frontend**

- Een Organism-component hoort geen service calls (async/await) uit te voeren.
- Service calls moeten buiten de feature branch/componenten gehouden worden.



## Team & samenwerking en planning

**Afstemmingen**
- Daily standups blijven houden in discord
- Taken zo snel mogelijk afmaken
  
**Werkhouding**
- Elkaar verantwoordelijk houden voor voortgang.
- Meer tijd en inzet tonen per teamlid.
- Actief bijdragen aan het gezamenlijke resultaat.

## Conclusie

De sprint review liet zien dat het project duidelijke vooruitgang boekt, vooral op het gebied van snelheid, design en functionaliteiten. 
Tegelijkertijd zijn er nog meerdere verbeterpunten op het gebied van gebruiksvriendelijkheid, architectuur en performance.
De feedback uit deze review wordt meegenomen in de volgende sprint om de applicatie verder te professionaliseren.






