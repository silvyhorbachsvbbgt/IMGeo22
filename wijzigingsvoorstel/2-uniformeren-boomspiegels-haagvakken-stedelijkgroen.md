Uniformeren
===========

Boomspiegels, haagvakken en uitsparingen stedelijk groen in wegdelen
--------------------------------------------------------------------

### Huidige situatie en probleem

Voor uitsparingen van stedelijk groen in wegdelen die kleiner zijn dan 5
vierkante meter geldt in de BGT geen verplichting om deze objecten als
BegroeidTerreindeel op te nemen. Wel mogen deze objecten optioneel in IMGeo
worden opgenomen. Nu blijkt dat bijna alle bronhouders uitsparingen van
stedelijk groen kleiner dan 5 meter opnemen in de BGT.

Daarnaast kent IMGeo een type ‘boomspiegel’ bij Weginrichtingselement met de
definitie ‘Het stuk grond rondom de stam van een boom dat van boven toegankelijk
is voor lucht en water.’ Deze objecten zijn optioneel en kunnen met punt- of
vlakgeometrie worden afgebakend. Een boomspiegel met vlakgeometrie is
niet-opdelend en vanuit BOR-afnemers en BGT-bronhouders is de wens geuit om de
boomspiegels opdelend te laten zijn.

De informatie over stukken grond rondom een de stam van een boom kunnen in IMGeo
nu in twee objectklassen worden opgenomen, en bronhouders doen dit (ook binnen
hun eigen bestand) verschillend. Dit is niet consistent en niet-uniform.
Gebruikers van de BGT vragen om een uniforme kaart om landelijke analyses te
kunnen uitvoeren.

In IMGeo kan optioneel een haag als VegetatieObject met lijn- of vlakgeometrie
worden opgenomen. Een haag met vlakgeometrie is niet-opdelend, en er bestaat
onduidelijkheid en interpretatieverschil onder bronhouders welk terreinobject
onder een haag moet worden opgenomen: IMGeo voorziet nu niet in een
fysiek-voorkomen ‘haagvak’ om een terreindeel aan te duiden dat onder een haag
ligt. Bronhouders vragen nu om advies aan Geonovum met als reactie om een
BegroeidTerreindeel met fysiek-voorkomen ‘groenvoorziening’ op te nemen, echter
dit is nergens in model of werkafspraak nu vastgelegd. Dit is niet consistent en
niet-uniform.

### Oplossing en nut

Om meer uniformiteit en consistentie in de afbakening van boomspiegels,
haagvakken en ander (klein) stedelijk groen te bereiken worden de volgende
wijzigingen voorgesteld:

-   De inwinregel dat uitsparingen van klein stedelijk groen in wegdelen die
    kleiner dan 5 m2 zijn wordt geschrapt.

-   Het type ‘boomspiegel’ bij Weginrichtingselement komt te vervallen.

-   Aan ‘groenvoorziening’ van BegroeidTerreindeel worden de nadere typeringen
    ‘haagvak’ en ‘boomspiegel’ toegevoegd.

De wijzigingen leveren de volgende voordelen op:

-   Door dat boomspiegels als groenvoorziening bij BegroeidTerreindeel mee doen
    in de opdelende BGT-laag, kunnen voor beheer openbare ruimte betere
    berekeningen worden gedaan op het areaal. Dit leidt tot kostenbesparingen
    voor beheer en onderhoud. Bijvoorbeeld bij de aanbesteding van het opnieuw
    leggen van de tegels van een troittoir, omdat de vierkante meters
    boomspiegel automatisch niet worden meegerekend in het aantal vierkante
    meters tegels van het voetpad.

-   Door dat boomspiegels consistent en uniform als groenvoorziening van
    begroeidterreindeel worden opgenomen, kunnen betere landelijke analyses
    worden uitgevoerd. Dit leidt tot beter resultaten in onderzoek en beleid.
    Bijvoorbeeld bij de uitvoering van de impactanalyse wateroverlast en
    overstromingen wordt het afwaterend vermogen over alle (on)begroeid
    terreindelen berekend en worden niet de boomspiegels bij
    weginrichtingselement vergeten.

-   Door de keuze-/interpretatieruimte voor afbakening en classificatie van
    haagvakken en boomspiegels in te perken, kunnen bestekken worden
    geüniformeerd en kunnen bronhouders beter samenwerken in de inwinning en
    bijhouding van de BGT.

### Impact en implementatie

De impact van dit voorstel is relatief laag: (bijna) alle gegevens zijn
ingewonnen en beschikbaar en de software aanpassing blijft beperkt tot
uitbreiden en laten vervallen van classificaties. Voor de implementatie wordt
eerst de software en daarna de data aangepast.

De **software** van bronhouders en (BOR-)gebruikers dient eerst te worden
aangepast zodanig dat ‘haagvak’ en ‘boomspiegel’ als groenvoorziening bij
BegroeidTerreindeel kan worden geleverd en/of ontvangen. In de
(overgangs)periode dat niet alle bronhouders en gebruikers over zijn op de
nieuwe versie van IMGeo zal een centrale voorziening heen-en-weer vertalen
tussen de oude en nieuwe classificaties. Na de overgangsperiode worden oude
classificaties niet meer geaccepteerd in de BGT, en mag bronhoudersoftware
boomspiegels als Weginrichtingselement niet kunnen leveren.

Na het aanpassen van de software wordt aan bronhouders gevraagd om met
terugwerkende kracht alle **boomspiegels** om te zetten van
Weginrichtingselement naar BegroeidTerreindeel.

<http://85.214.237.242/test/imgeo22/?categorie=vervallen-boomspiegel>

De boomspiegels worden eventueel van punt- naar vlakgeometrie omgezet, en
krijgen een nieuwe identificatie, omdat deze bij een andere objectklasse worden
opgenomen

*Samenvatting implementatie boomspiegels.*

| \<icon1B\>                                  | \<icon2A\>          | \<icon3A\>                                 | \<icon4A\>                             | \<icon5\>                                 |   |   |   |   |   |
|---------------------------------------------|---------------------|--------------------------------------------|----------------------------------------|-------------------------------------------|---|---|---|---|---|
| Software aanpassen op nieuwe classificaties | Centraal signaleren | Data decentraal aanpassen door bronhouders | Data omzetten met terugwerkende kracht | Doorlo6\>ptijd implementatie van 1,5 jaar |   |   |   |   |   |

Na het aanpassen van de software wordt aan bronhouders gevraagd om met
terugwerkende kracht de **haagvakken** zijnde terreindelen onder een
vegetatieobject ‘haag’ om te zetten naar BegroeidTerreindeel met
fysiek-voorkomen ‘groenvoorziening’ en optioneel het plus-fysiekvoorkomen
‘haagvak’.

<http://85.214.237.242/test/imgeo22/?categorie>=

Terreindelen die niet als BegroeidTerreindeel zijn opgenomen krijgen daarmee
mogelijk een nieuwe identificatie, omdat deze bij een andere objectklasse worden
opgenomen.

*Samenvatting implementatie haagvakken*

| \<icon1B\>                                  | \<icon2A\>          | \<icon3B\>                                 | \<icon4A\>                             | \<icon6\>                               |   |   |   |   |   |
|---------------------------------------------|---------------------|--------------------------------------------|----------------------------------------|-----------------------------------------|---|---|---|---|---|
| Software aanpassen op nieuwe classificaties | Centraal signaleren | Data decentraal aanpassen door bronhouders | Data omzetten met terugwerkende kracht | Doorlooptijd implementatie van 1,5 jaar |   |   |   |   |   |

Voor uitsparingen van **stedelijk groen in wegdelen kleiner dan 5m2** is de
verwachting dat deze (bijna) allemaal zijn opgenomen als
BegroeidTerreindeel:groenvoorziening of als Weginrichtingselement:boomspiegel.
Zeker na het omzetten van boomspiegels naar BegroeidTerreindeel:groenvoorziening
moet een volledig beeld van alle kleine uitsparingen in stedelijk groen
beschikbaar zijn. Aan bronhouders wordt niet gevraagd om ook actief

<http://85.214.237.242/test/imgeo22/?categorie=stedelijkgroen>

*Samenvatting implementatie stedelijk groen*

| \<icon1A\>       | \<icon2A\>                             | \<icon3B\>                                 | \<icon4B\>                                    | \<icon56\>                            |   |   |   |   |   |
|------------------|----------------------------------------|--------------------------------------------|-----------------------------------------------|---------------------------------------|---|---|---|---|---|
| Software voldoet | Data inwinnen via reguliere bijhouding | Data decentraal aanpassen door bronhouders | Data aanpassen na signalering of terugmelding | Doorlooptijd implementatie van 2 jaar |   |   |   |   |   |

\<icon1A\>

![Approved Window icon](media/51e255cf9ca735d13ce814cb4190537d.png)

Software voldoet

\<icon1B\>

![Code Window icon](media/4c12d0aee36ab140454736d3cbca9f4c.png)

Software aanpassen op nieuwe classificaties

\<icon2A\>

![Data Search icon](media/3e7a602ebe38c76776a8a0eba4e83990.png)

Centraal signaleren

\<icon2B\>

![Tripod 2 icon](media/d90734a4417d5c260354cbcc065fe438.png)

Data inwinnen via reguliere bijhouding

\<icon3A\>

![Edit Map icon](media/d67b761a11e02641c4b79438ac558c58.png)

Data decentraal aanpassen door bronhouders

\<icon3B\>

![Data Refresh icon](media/bcc6db15c559764f2caf8f68d454efe0.png)

Data central converteren

\<icon4A\>

![Forward icon](media/9cd5ddd8e03eb4a08f10fa67032369fc.png)

Data aanpassen met terugwerkende kracht

\<icon4B\>

![Forward icon](media/9cd5ddd8e03eb4a08f10fa67032369fc.png)

Data aanpassen na signalering of terugmelding

\<icon5A\>

![Timer icon](media/35627a5d92e005a53a25950ea2b9207e.png)

![Euro Sign 2 icon](media/88000ee2a4a6f611856e2315cc841b76.png)

Tijd/Geld

\<icon6A\>

![Sand watch 2 icon](media/597a9db0358ca2af752b262a0bb08569.png)

Doorlooptijd
