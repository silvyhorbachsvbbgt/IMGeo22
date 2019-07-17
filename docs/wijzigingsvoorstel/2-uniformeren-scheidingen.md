Uniformeren hekken, muren en andere typen scheidingen
=====================================================

### Huidige situatie en probleem

In de BGT worden scheidingen alleen vastgelegd als ze bepaalde minimum
afmetingen hebben, die per type scheiding verschillen (zie BGT
gegevenscatalogus).

In IMGeo kunnen scheidingen, die kleiner dan het BGT minimum zijn, worden
opgenomen als objecttype ‘overige scheiding’. Deze kent dezelfde typen
scheiding. De populatie van Overige Scheiding bestaat uit:

-   Scheidingen die niet voldoen aan de BGT minimummaat;

-   Scheidingen in terrein met fysiek voorkomen ‘erf’ die niet aan de
    straatzijde gelegen zijn.

De opname van een hek, muur of ander type scheiding wordt dus bepaald op basis
van minimale afmetingen of de ligging in de openbare ruimte. Een hek wordt als
Scheiding opgenomen als dit hek minimaal 10 meter lang én minimaal 1 meter hoog
is. Een muur wordt als Scheiding opgenomen als deze muur minimaal 1 meter lang
én minimaal 30 centimeter breed is.

Nu blijkt dat bijna alle bronhouders hekken en muren kleiner dan de minimale
afmetingen in de BGT opnemen als Scheiding. Dit is niet consistent en
niet-uniform.

[http://85.214.237.242/test/imgeo22/?categorie=hekmuurkorter10m\#](http://85.214.237.242/test/imgeo22/?categorie=hekmuurkorter10m)

Bronhouders en softwareleveranciers van bronhouders hebben gevraagd om het
onderscheid tussen Scheiding en OverigeScheiding te laten vervallen om de
bijhouding van de BGT te vereenvoudigen.

### Oplossing en nut

Om meer uniformiteit en consistentie in de afbakening van scheidingen te
bereiken worden de volgende wijzigingen voorgesteld:

-   De objectklasse OverigeScheiding komt te vervallen. Alle hekken, muren en
    andere typen scheidingen worden opgenomen als Scheiding.

-   In de BGT catalogus wordt beschreven welke hekken, muren en andere typen
    scheidingen aangeleverd *moeten* worden:

    -   Elke scheiding in terrein met fysiek voorkomen ‘erf’ die aan de
        straatzijde gelegen zijn.

    -   Elk hek langer dan 10 meter en hoger dan 1 meter.

    -   Elke muur langer dan 1 meter en breder dan 30 centimeter.

    -   Elke kademuur, damwand, geluidscherm en walbescherming.

-   In de IMGeo catalogus wordt beschreven welke hekken, muren en andere type
    scheidingen aangeleverd *mogen* worden.

    -   Elke scheiding in terrein met fysiek voorkomen ‘erf’ die niet aan de
        straatzijde gelegen zijn.

    -   Elke scheiding kleiner dan de minimale BGT-afmetingen.

-   De eisen voor opname van een scheiding met lijn- of vlakgeometrie blijven
    ongewijzigd:

-   Een BGT-muur of kademuur breder dan 30 centimeter *moet* met vlakgeometrie
    worden afgebakend; smaller dan 30 centimeter met lijngeometrie.

-   Een muur of kademuur smaller dan 30 centimeter *mag* met vlakgeometrie
    worden afgebakend.

-   Andere typen scheidingen hebben alleen lijngeometrie in IMGeo.

De wijzigingen leveren de volgende voordelen op:

-   De bijhouding van scheidingen door bronhouders wordt vereenvoudigd omdat
    alle scheidingen onder dezelfde objectklasse vallen. Dit scheelt op de
    bijhoudingskosten van de BGT.

-   Er kunnen betere landelijke analyses worden uitgevoerd omdat de gegevens van
    scheidingen op één plek (objectklasse) in de BGT\|IMGeo dataset beschikbaar
    zijn. Dit leidt tot beter resultaten in onderzoek en beleid.

-   Door de keuze-/interpretatieruimte voor afbakening en classificatie van
    scheiding in te perken, kunnen bestekken worden geüniformeerd en kunnen
    bronhouders beter samenwerken in de inwinning en bijhouding van de BGT.

-   De werkafspraak OverigScheiding als gevolg van een fout/inconsistentie in de
    modellering van IMGeo (OverigeScheiding heeft geen bgt-type) wordt opgelost.
    Software wordt consistenter en dus eenvoudiger te beheren.

### Impact en implementatie

De impact van dit voorstel is relatief laag: (bijna) alle gegevens zijn
ingewonnen en beschikbaar en de software aanpassing blijft beperkt tot het laten
vervallen van een objectklasse. Voor de implementatie wordt eerst de data en
daarna de software aangepast.

Aan bronhouders gevraagd om met terugwerkende kracht alle hekken, muren en
andere typen scheidingen die ondergebracht zijn in de objectklasse
OverigeScheiding om te zetten naar Scheiding.

<http://85.214.237.242/test/imgeo22/?categorie=vervallen-overigescheiding>

Hekken, muren en andere typen scheidingen die worden omgezet naar Scheiding
krijgen een nieuwe identificatie, omdat deze bij een andere objectklasse worden
opgenomen.

*Samenvatting implementatie hekken, muren en andere typen scheidingen.*

| \<icon1A\>       | \<icon2A\>          | \<icon3A\>                                 | \<icon4A\>                             | \<icon5\>                                 |   |   |   |   |   |
|------------------|---------------------|--------------------------------------------|----------------------------------------|-------------------------------------------|---|---|---|---|---|
| Software voldoet | Centraal signaleren | Data decentraal aanpassen door bronhouders | Data omzetten met terugwerkende kracht | Doorlo6\>ptijd implementatie van 1,5 jaar |   |   |   |   |   |

\<icon1A\>

![Approved Window icon](media/51e255cf9ca735d13ce814cb4190537d.png)

Approved Window icon

Software voldoet

\<icon1B\>

![Code Window icon](media/4c12d0aee36ab140454736d3cbca9f4c.png)

Code Window icon

Software aanpassen op nieuwe classificaties

\<icon2A\>

![Data Search icon](media/3e7a602ebe38c76776a8a0eba4e83990.png)

Data Search icon

Centraal signaleren

\<icon2B\>

![Tripod 2 icon](media/d90734a4417d5c260354cbcc065fe438.png)

Tripod 2 icon

Data inwinnen via reguliere bijhouding

\<icon3A\>

![Edit Map icon](media/d67b761a11e02641c4b79438ac558c58.png)

Edit Map icon

Data decentraal aanpassen door bronhouders

\<icon3B\>

![Data Refresh icon](media/bcc6db15c559764f2caf8f68d454efe0.png)

Data Refresh icon

Data centraal converteren

\<icon4A\>

![Rewind icon](media/8c9b26622bcbc8c510f1a06c3d4e391b.png)

Rewind icon

Data aanpassen met terugwerkende kracht

\<icon4B\>

![Forward icon](media/9cd5ddd8e03eb4a08f10fa67032369fc.png)

Forward icon

Data aanpassen na signalering of terugmelding

\<icon5A\>

![Timer icon](media/35627a5d92e005a53a25950ea2b9207e.png)

Timer icon

![Euro Sign 2 icon](media/88000ee2a4a6f611856e2315cc841b76.png)

Euro Sign 2 icon

Tijd/Geld

\<icon6A\>

![Sand watch 2 icon](media/597a9db0358ca2af752b262a0bb08569.png)

Sand watch 2 icon

Doorlooptijd
