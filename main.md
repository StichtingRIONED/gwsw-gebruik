# GWSW Gebruik

<style>
  .symbolSmall{width:20px;height:20px;margin-right:1em;vertical-align:middle}
  .symbol{width:30px;height:30px;margin-right:1em;vertical-align:middle}
</style>

Stichting RIONED is initiatiefnemer en eigenaar van dit GitHub-project, Eric Oosterom is de verantwoordelijk projectmanager. 

Vragen over deze website en het GWSW kunt u stellen via gwsw@rioned.org. 

In het GegevensWoordenboek Stedelijk Water (GWSW) worden alle objecten en gegevens van objecten, hun onderlinge relaties en de beheeractiviteiten in de riolering eenduidig gedefinieerd en vastgelegd. Dit zodat de gegevensuitwisseling eenvoudiger gaat en dat er daardoor beter beheer mogelijk is. Het GWSW geeft ons vakgebied een gezamenlijke digitale taal. 
Hieronder leggen we uit hoe je kan instappen in het GWSW, zodat je de voordelen van de standaard kan gaan gebruiken.

De inhoudsopgave aan de linkerkant van de website kan gebruikt worden als leeswijzer en ter navigatie over de pagina.


# Aanleiding

Deze pagina is in het leven geroepen om riooldatabeheerders te ondersteunen in het gebruik van het GegevensWoordenboek Stedelijk Water (GWSW). Dit willen we doen door middel van een laagdrempelig stappenplan.
Het GWSW komt ingewikkeld over en is dat ook op sommige vlakken. Als je onder de motorkap van een auto kijkt, dan komt dat ook ingewikkeld over. Het is echter niet nodig om precies te begrijpen hoe een auto helemaal werkt, om toch goed en veilig de auto te kunnen besturen. Zo werkt het ook met het GWSW.

Op de site van Stichting RIONED staat de ['waarom'](https://www.riool.net/applicaties/gegevenswoordenboek-stedelijk-water/waarom-gwsw-) beschreven. In de volgende paragraaf staat de 'hoe' van het GWSW toegelicht. De rest van de website richt zich op de 'wat' van het GWSW: Op welke manier kan een riooldatabeheerder het GWSW in haar of 
zijn dagelijke praktijk (op operationeel niveau) gebruiken. Dit proberen we te doen aan de hand van instructies per rioolobject te geven in de vorm van filmpjes, figuren of teksten. 
Hiervoor is de samenwerking met de onderstaande leveranciers van beheersoftware gezocht:

*Logo's van meewerkende leveranciers worden hier ingevoegd*


# Hoe werkt het GWSW
## Algemeen

Het GegevensWoordenboek Stedelijk Water is niets meer dan gezamenlijke afspraken over de taal, de verbanden tussen en de uitwisseling van gegevens die iets te maken hebben met het domein Stedelijk Water. Stichting RIONED heeft dit onderverdeeld in Model, Gegevens en Toepassingen.

Het Model staat op [data.gwsw.nl](https://data.gwsw.nl/) en bestaat uit:
-	Woordenboek (Ontologie): Hoe noemen we ‘iets’?
-	Datastructuur (Datamodel): Hoe zijn de verbanden of relaties tussen die ‘iets-en’?

De Gegevens staan op de GWSW-server en bestaan uit:
-	Data-omgeving per organisatie
-	In die data-omgeving staan de gegevens van die organisatie opgeslagen conform het GWSW-model

De Toepassingen (applicaties) staan op [apps.gwsw.nl](https://apps.gwsw.nl/) en bestaan uit:
-	Apps voor het uploaden van gegevens naar de GWSW-server
-	Apps voor het controleren van gegevens op de GWSW-server
-	Apps voor het opvragen van gegevens vanaf de GWSW-server

## Illustratief voorbeeld – Een distributiecentrum
Denk bij het GWSW aan een logistiek distributiecentrum van een bedrijf zoals Coolblue of BOL. Het distributiecentrum is zo ingericht dat het een logische en (daardoor) efficiënte opslag van producten is. Elk product heeft zijn eigen plek. En die plek is daar, omdat:
1)	Het een logische plek is in relatie tot ‘buur’-producten. Zo staat het witgoed en de bijbehorende aansluitslangen bij elkaar.
2)	De bereikbaarheid aansluit op de vraag van de consument. ‘Hardlopers’ zullen normaliter voor in de hal staan. Producten die zelden besteld worden, zullen verder in de hal staan.

De indeling van een distributiecentrum (Figuur 1) is een analogie van het GWSW-datamodel.

<img src="media/figuur1_unsplash.jpg" style="width:100%;height:50%" />

*Figuur 1 Voorbeeld van een distributiecentrum (foto door Ruchindra Gunasekara op Unsplash)*

Op de GWSW-server staat er per organisatie een ‘GWSW-conform distributiecentrum’ klaar. Dit ‘distributiecentrum’ kan worden gevuld met gegevens uit het Stedelijk Water-domein. Als deze gegevens in de stellingen van het distributiecentrum zijn opgeslagen, dan kunnen ze worden gecontroleerd (denk aan een voorraadcontrole) en weer worden uitgeleverd (denk aan een bestelling uitleveren).

## Gegevens uitwisselen via de GWSW-server
Om gebruik te kunnen maken van de voordelen van het GWSW moeten de gegevens vanuit het beheerpakket (gele blokjes aan de linkerkant) op de GWSW-server (grote grijze blok in het midden) komen te staan in de data-omgeving (het ‘distributiecentrum’) van de betreffende organisatie (blauwe cilinder). Vanuit daar kunnen de gegevens worden opgevraagd voor gebruik in externe applicaties (Figuur 2).

<img src="media/figuur2_GWSWserver.jpg" style="width:100%;height:50%" />

*Figuur 2 Beheerapplicaties (links) met de verschillende datasets (gele blokken), de GWSW-server (grijze blok in het midden) met toepassingen (GWSW Apps) en gegevensopslag (GWSW Data) in een data-omgeving per organisatie (blauwe cilinders) en externe applicaties (rechts) die gebruik maken van de gegevens op de GWSW-server*

Met GWSW Apps kunnen gegevens worden geüpload naar de GWSW-server, worden gecontroleerd en worden opgevraagd vanaf de GWSW-server.

## Gegevens uploaden naar de GWSW-server
Vanuit het beheerpakket van de gemeente wordt een uitwisselformaat geëxporteerd. Dit is een zogenoemd [GWSW-OroX bestand](https://apps.gwsw.nl/doc/GWSW.orox%20Opbouw%20dataset.pdf) en heeft als bestandsextentie *.ttl*. Dit uitwisselbestand kan via de upload-functionaliteit op [apps.gwsw.nl](https://apps.gwsw.nl/) in de data-omgeving van de betreffende gemeente op de GWSW-server worden gezet. Hiervoor is de naam van de data-omgeving en een wachtwoord (sleutel) nodig. Deze sleutel kan worden opgevraagd via gwsw@rioned.org.

De gegevens uit de kernregistratie van een waterschap worden via het GegevensKnooppunt Waterschappen naar de GWSW-server geüpload. 

## Gegevens controleren op de GWSW-server
De gegevens die in de data-omgeving op de GWSW-server staan kunnen worden gecontroleerd op basiskwaliteit en mate waarin deze voldoen aan de GWSW-standaard. Dit wordt gedaan met behulp van de toepassing [Nulmeting](https://apps.gwsw.nl/item_validate). 

Omdat voor het lezen van het resultatenbestand technische kennis van het GWSW nodig is, kan je hiervoor het beste een [GWSW-adviseur inschakelen](https://www.riool.net/applicaties/gegevenswoordenboek-stedelijk-water-gwsw/gwsw-ondersteuning-beschikbaar).

## Gegevens opvragen van de GWSW-server
De gegevens die in de data-omgeving op de GWSW-server staan kunnen worden opgevraagd voor gebruik in externe applicaties/programma’s. 
Voor het maken van hydraulische berekeningen kunnen de gegevens in [.hydx formaat worden gedownload](https://apps.gwsw.nl/item_hydxdownload). Voor andere toepassingen kunnen er diverse [Geo-formaten](https://apps.gwsw.nl/item_geo) voor verschillende thema’s worden gedownload of ontsloten.

## GWSW is in ontwikkeling
Het is goed te beseffen dat het GWSW in ontwikkeling is, voor zowel het woordenboek, het datamodel en de uitwisseling. Met elke nieuwe versie komen er nieuwe mogelijkheden voor het gebruik van de gegevens, dus ook nieuwe definities en nieuwe relaties. [De huidige versie is 1.6.1](https://www.riool.net/applicaties/gegevenswoordenboek-stedelijk-water-gwsw/huidige-versie-gwsw-en-planning/deze-gwsw-eisen-stelt-u-bij-aanschaf-van-nieuwe-software).

De adoptie van het GWSW is een groeipad voor Stichting RIONED, de leveranciers van beheer- en rekenpakketten en de gebruikers. Dit heeft logischerwijs ook gevolgen voor het gebruik.

### Randvoorwaarden
Om het gegevensbeheer, -uitwisseling en -gebruik goed aan te laten sluiten op het GWSW zijn er een aantal randvoorwaarden (met verantwoordelijkheid) van toepassing.
1)	Het beheerpakket moet in staat zijn om de gegevens op te slaan conform het GWSW (Leverancier beheerpakket) 
2)	Het beheerpakket moet gevuld zijn met gegevens die qua inhoud aansluiten op het GWSW (Riooldatabeheerder) 
3)	Het beheerpakket moet in staat zijn om de gegevens te exporteren conform het GWSW (Leverancier beheerpakket) 
4)	De GWSW-server moet in staat zijn om een correct bestand te kunnen importeren, opslaan en publiceren (Stichting RIONED) 
5)	Externe applicaties moeten in staat zijn om op basis van een export vanaf de GWSW-server de gegevens toe te passen (Leverancier externe applicatie)

Omdat het doel van voorliggende website is om riooldatabeheerders te ondersteunen in het gebruik van het GWSW, zijn de punten over het beheerpakket (punt 1 en 3) en het gegevensbeheer (punt 2) het meest relevant. Deze worden in de volgende paragraaf van de website nader toegelicht. Punt 4 en 5 worden door de leveranciers en Stichting RIONED opgepakt.


