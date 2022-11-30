---
lastModified: 2018-06-28T00:00:00Z
title: Richtlijnen voor ontwerpstijl voor externe medewerkers
description: Leer meer over creatie en redactionele richtlijnen voor externe medewerkers aan Experience League.
exl-id: 874f88d7-18ad-4ac8-bfa3-737255652bbc
source-git-commit: 03d46c9ffb664824f9526f781d776069d486f271
workflow-type: tm+mt
source-wordcount: '2227'
ht-degree: 0%

---

# Richtlijnen voor ontwerpstijl voor externe medewerkers{#guidelines}

Deze pagina bevat redactionele richtlijnen voor externe auteurs die inhoud maken of bestaande inhoud op het Experience League bijwerken. Voordat u begint, moet u controleren of:

* Ga vertrouwd met [Markering](markdown.md) ontwerpen
* Spelling en grammatica in uw artikelen controleren
* Gebruik een vriendelijke toon, een consistente presentatie en eenvoudige zinnen om computervertaling te verbeteren
* Volg [best practices](#writing-tips) en redactionele normen op deze pagina

## Richtlijnen voor stijl{#style-guidelines}

Houd rekening met het volgende wanneer u documentatie schrijft.

* **beknopt schrijven**: Verspil geen woorden. Zorgt u voor korte en beknopte zinnen. Houd uw artikel geconcentreerd. Beperk het aantal notities tot een minimum.
* **Focus op publiek en doel**: Alvorens u begint te schrijven, bepaal duidelijk wie de klant is en welke taak hij of zij probeert te verwezenlijken. Schrijf uw artikel om die klant te helpen die taak te doen.
* **Voorbeelden gebruiken**: Geef voorbeelden om concepten uit te leggen.
* **Uw inhoud ordenen**: Maak secties om instructies op te splitsen in overzichtelijkere groepen stappen. Gebruik een schermafbeelding wanneer u deze helderder maakt.

## Aanbevolen werkwijzen voor technisch schrijven{#writing-tips}

Technisch schrijven, met name voor softwaredocumentatie, is een gespecialiseerde bedrijfstak. Zelfs wordt de meest productieve novelist gedumpt wanneer het proberen van technisch schrijven-niet omdat het materiaal complex of technisch is, maar omdat het niet gemakkelijk is makend complexe, technische informatie _eenvoudig_. Uw inhoud kan alleen succesvol zijn als deze structureel consistent, scannbaar, herbruikbaar en zonder structuur- en syntaxisfouten door de publicatiepijplijn loopt.

In de volgende secties worden algemene problemen beschreven waarvoor nieuwe schrijvers moeten uitkijken:

### Koppen niet van elkaar gescheiden door tekst (dubbele koppen){#double-headings}

Als u twee koppen hebt zonder tekst die ze scheidt, voegt u ontbrekende tekst toe (om de tweede onderwerpkop in te voeren). U kunt ook een van de koppen verwijderen. Het tweede is waarschijnlijk overbodig.

Bijvoorbeeld: _Overzicht_ heeft hier geen enkel doel:

![Dubbele koppen](assets/headings-double.png)

* En als uw tweede rubriek toevallig is _Overzicht_, het is waarschijnlijk onnodig. Uw H1 en eerste paragraaf dienen als conceptueel overzicht over het onderwerp van het artikel.

* Op dezelfde wijze, voor SEO-doeleinden, stand-alone rubrieken zoals _Overzicht_ en _Inleiding_ zijn op zich niet nuttig. Geef het product of de functie die u wilt introduceren een naam. (Voorbeeld: _Overzicht van de evaluatierapporten_)

### Inconsistente kruisverwijzingskoppen{#maps}

Gebruiken _Meer informatie_ koppen voor kruisverwijzingslijsten (of kaarten). Voorbeeld:

![Kruisverwijzingslijst](assets/headings-more-info.png)

**Richtlijnen voor kruisverwijzingslijsten**

* Een lijst met opsommingstekens gebruiken voor de kruisverwijzingen
* Cursief gebruiken voor de formele namen van hulplijnen of paginanamen (wanneer u geen koppelingstekst gebruikt)
* Geen punctuatie toepassen op de kop (of op een kop)
* Nummers in koppen voorkomen

### Verkeerd overeenkomend inhoudsopgave-item, broodkruimel en paginanaam{#toc}

Omdat we het inhoudsopgavebestand (inhoudsopgave) handmatig beheren, zijn deze problemen eenvoudig te verhelpen. Zorg ervoor dat de inhoudsopgave-vermelding overeenkomt met de paginanaam (H1). Zorg er ook voor dat deze veel overeenkomt met de breadcrumb.

**Richtlijnen voor inhoudsopgaven en lijsten**

* Mogelijk moet u het inhoudsopgave-item verkorten, maar dit moet duidelijk betrekking hebben op de paginanaam en de broodkruimel.
* Broodkruimels worden uit de metagegevens van de titel gehaald, zodat ze kunnen verschillen (voor SEO-doeleinden).

### Aanhalingstekens in plaats van cursief{#quotes}

Het is moeilijk om te weerstaan aan het toevoegen van citaten rond een woord of uitdrukking. Aanhalingstekens zijn echter bedoeld voor het citeren van spraak en worden bijna nooit gebruikt in de productdocumentatie.

**Richtsnoeren voor aanhalingstekens**

* Cursief werkt meestal beter dan aanhalingstekens (voor foutberichten, unieke of vreemde woorden enzovoort).
* Gebruik Vet en UICONTROL voor interface-elementen.

### Procedures{#steps}

Het schrijven van een procedure (de _taak_ content type ) is geen talent waarmee we geboren zijn . Het opbouwen van een leesbare, duidelijke procedure verloopt in de praktijk.

**Richtlijnen voor stappen**

* Een procedure is een reeks stappen. Een stap is een korte, genummerde stap. _in één zin_ gebruiken.
* Begin elke stap of met een werkwoord of _Naar_ oneindig (om de lezer naar het doel te leiden, zoals in, _Schakel **Aangemeld blijven**_). Als een stap een specifiek doel binnen de algemene procedure heeft, vermeld het doel vóór de actie.
* Als u informatie hebt over de stap (een inhoudstype wordt _stapinformatie_, voegt u deze toe na de stap (ingesprongen met de stap) of na het element (een schermafbeelding, video of een lijst met interfacebeschrijvingen).
* Als uw stap twee handelingen bevat (zoals _Selecteer deze_), schrijven als een enkele, korte zin.
* Beperk uw taak tot ongeveer zeven tot tien stappen. Als u meer dan tien stappen in één taak creeert, zult u het in twee taken waarschijnlijk moeten breken. Gebruik hier je beste oordeel.
* Gebruik in de productdocumentatie geen koppen als stappen. (Uitzondering hieronder voor zelfstudies.)
* Voor zelfstudies met meerdere pagina&#39;s kunnen koppen als stappen worden toegestaan. Nochtans, maak geen aantal hen. In plaats daarvan, spelling-out _Stap 1:_, _Stap 2:_, enzovoort.

**Voorbeeld**

Hier volgt een goed gestructureerde procedure voor aanmelden bij Adobe:

Aanmelden bij Adobe:

1. Aan `Adobe.com`, selecteert u **Experience Cloud**.
1. Selecteren **Aanmelden**.
1. Selecteren **Persoonlijke account**.
1. Als u aangemeld wilt blijven, selecteert u **Aangemeld blijven**.
1. Typ uw naam en wachtwoord.
1. Selecteren **Aanmelden**.

### Parallelle lijsten{#lists}

Met parallelle constructie voor lijsten kunt u gemakkelijk lezen en scannen. Lijsten bevatten een inhoudsopgave (inhoudsopgave), opsommingstekens (niet-geordende) lijsten of genummerde lijsten.

Voorbeeld-inhoudsopgave met parallelle items:

![Parallelle inhoudsopgave](assets/parallel-toc.png)

De voorafgaande inhoudsopgave is een goed voorbeeld omdat:

* Conceptuele bovenliggende items zijn &#39;nos&#39; of &#39;zelfstandig naamwoord&#39;
* Procedures (taken) zijn actieve werkwoorden (geen gerondes)
* Alle items gebruiken hoofdlettergebruik voor zinnen

## Metagegevens voor titel en beschrijving{#metadata}

_Titel_ en _beschrijving_ Metagegevens zijn belangrijk voor SEO, de ontdekking van inhoud, en de scores van de inhoudskwaliteit op Experience League.

Hier volgen voorbeelden van titels en beschrijvingen:

**Beschrijvingen voor conceptieplekken**

* _Meer informatie over segmenten in Adobe Analytics. Hulp bij het configureren van het deelvenster Segmentatie in een werkruimte._
* _Zoek hulp bij het gebruiken van segmenten in een rapport van de Mening van de Pagina in Adobe Analytics._

**Beschrijvingen voor procedure-/taakartikelen**

* _Leer hoe u een segment maakt in Adobe Analytics._
* _Maak een segment in Adobe Analytics. Leer hoe te om, een rapport te selecteren te vormen en in werking te stellen dat op het segment wordt gebaseerd u creeert._

Het object dat u gebruikt, is afhankelijk van de grootte en het bereik van het artikel.

**Titel voor een conceptobject**

* _Segmenten in paginaweergaverapporten_

**Titel van een procedure/taakartikel**

* _Een segment maken voor een rapport Paginaweergaven_

(Vergeet niet dat de verticale streep en de productnaam automatisch aan titels worden toegevoegd.)

## Manieren om de helderheid te verbeteren (en Acrolinx-scores){#tips}

Hier volgen eenvoudige manieren om het ontwerp, de helderheid en de leesbaarheid van inhoud te verbeteren. Deze helpen ook de scores in de Acrolinx-stijl en de CQI-scores op de ExL verbeteren.

| Richtlijnen | Over |
|---|---|
| Actieve stem gebruiken | De passieve stem van de verandering in actieve stem |
| Huidige spanningen gebruiken | **Zwak:** *Campaign v8 zal in juni worden uitgebracht.* <p>**Sterk:** *De release van Campaign v8 in juni.*<p>De huidige spanningen zijn altijd beter leesbaar voor klanten. |
| Vermijd zwakke, onnodige adverbare | *Zeer*, *uiterst*, *ongelooflijk*.... <p>Adverbs zijn extra woorden die geen significante betekenis toevoegen als u sterke en nauwkeurige woorden, clausules, en adjectieven gebruikt. |
| Gebruik sterke werkwoorden voor titels en [Inhoudsopgave-items](#using-toc) | Voorbeelden:<p>**Zwak:** *Treinontwikkeling en -beheer* <p>**Sterk:** *Kenmerken maken en beheren* |
| Zin gebruiken [kapitalisatie](https://docs.microsoft.com/en-us/style-guide/capitalization) | In twijfel, kapitaliseer niet. Gebruik in koppen hoofdletters in de stijl van de zin. Plaats de juiste nummers in hoofdletters en het eerste woord na een dubbele punt. In procedures, pas kapitalisatie aan die u in de interface ziet. |
| Lees deze kleine tips voor meer duidelijkheid | <ul><li>Vermijden *Om* (er wordt geen betekenis aan toegevoegd). Alles wat u nodig hebt *naar.*</li><li>Vermijden *Gebruik deze functie.* Het klinkt misschien technisch, maar dat is het niet. *Gebruiken* middelen *een goed gebruik te maken van met name iets dat niet voor het doel was bedoeld, maar dat*.</li><li>Vermijd puntkomma&#39;s: Gebruik in plaats daarvan een punt en begin een nieuwe zin. Halfdubbele punten zorgen voor onnodige complexiteit.</li><li>Dubbele punten: Gebruik dubbele punten om een lijst te introduceren. Gebruik spaarzaam dubbele punten binnen zinnen. Plaats het eerste woord na een dubbele punt in een zin met een hoofdletter.</li><li>Gebruik de komma van Oxford (drie komma&#39;s in een lijst).</li><li>De lengte van de zin moet minder dan 39 woorden zijn.</li><li>Navigatie: gebruiken _ga naar_ of _navigeren naar_.</li><li>Gebruik geen onbewerkte URL-tekst (gebruiksvriendelijke koppelingstekst), tenzij het weergeven van het pad belangrijke informatie is.</li></ul> |
| Spellingcontrole gebruiken in VSC | Installeer de Controle van de Spellingcontrole van de Code (uitbreiding) in de Code van Visual Studio. |
| Wijzigen _klikken_ tot _ga naar_ of _selecteren_ | _Klikken_ Dit is een apparaatspecifiek woord (met toegankelijkheidsproblemen) en de trend is om ervan af te stappen. Hier volgen enkele suggesties voor het wijzigen ervan:<ul><li>Navigatie: _Ga naar Bestand > Afdrukken_.</li><li>Klikken: _Selecteer Bestand > Afdrukken_ of _Selecteer OK_. </li></ul>Zie [Interacties met de gebruikersinterface beschrijven](https://docs.microsoft.com/en-us/style-guide/procedures-instructions/describing-interactions-with-ui) voor meer ideeën over de beste woordkeuze in verschillende situaties . |
| Acrolinx uitvoeren in VSC | Acrolinx controleert op problemen met stijl en grammatica. Het controleert URLs, terminologie, spelling, en meer. Het helpt u uw helderheid te verbeteren en verbetert vertaling op de inhoud van het Experience League. |

{style=&quot;table-layout:auto&quot;}

Nog een paar beste praktijken en bronnen:

* [Scannbare inhoud](https://docs.microsoft.com/en-us/style-guide/scannable-content/): Help lezers snel te vinden wat ze nodig hebben, of herkennen net zo snel als ze niet waar ze moeten zijn. Het schrijven om het scannen te vergemakkelijken kan u helpen.
* **Getallen:** In lichaamstekst, specificeer gehele aantallen van nul tot negen, en gebruik cijfers voor 10 of groter. Zie [Getallen](https://docs.microsoft.com/en-us/style-guide/numbers).
* Schrijf zoals je spreekt, projectvriendelijkheid en kom snel tot het punt.

Zie [Top 10 van schrijftips](https://docs.microsoft.com/en-us/style-guide/top-10-tips-style-voice) in de [Microsoft® Style Guide](https://docs.microsoft.com/en-us/style-guide/welcome/) voor meer informatie .

## Alt-tekst{#alt-text}

Voeg betekenisvolle alternatieve tekst toe aan uw elementen (afbeeldingen). Houd rekening met alternatieve tekst die overeenkomt met:

* De doelklanten kunnen (taak of conceptennaam) verwezenlijken
* De functie of pagina die u weergeeft
* De pictogramnaam die u weergeeft

Google beschouwt de alt-text in SEO-resultaten.

## Lokalisatie - DNL en UICONTROL{#localization}

U hoeft zich geen zorgen te maken of uw product gelokaliseerd is of welke talen ExL gebruikt. U kunt de kwaliteit van de lokalisatie echter verbeteren door waar nodig de volgende twee markeringen (vereiste markeringen) toe te passen:

* `DNL`

   DNL betekent _niet lokaliseren_. U gebruikt deze alleen voor handelsmerken van Adobe-producten, die allemaal in het Engels moeten blijven staan.

   Syntaxisvoorbeelden: `[!DNL Adobe Campaign]` of `[!DNL Workfront]`

   DNL is niet bedoeld voor bestandsnamen of URL&#39;s.

* `UICONTROL`

   UICONTROL wijst op een interfacecontrole (zoals een optie, gebied, lusje, pagina, groep opties, of eigenschapnaam in UI).

   Voorbeeld van syntaxis: `Select **[!UICONTROL Project]**, then select **[!UICONTROL Save]**.`

>[!IMPORTANT]
>
>U moet deze labels toepassen voordat u de inhoud lokaliseert.

### Adobe gebruiken in productnamen{#product-names}

Voor de bedrijfsidentiteit nemen we doorgaans _Adobe_ in de eerste referentie van een product op het niveau van de gids. Afhankelijk van de ruimte, kunt u Adobe in een rubriek laten vallen, maar dan zou de eerste verwijzing in het lichaamskopie de volledige naam moeten omvatten. Bepaalde producten, zoals _Adobe Audition_ en _Adobe Premiere Pro_, het gebruik van Adobe op eerste of belangrijkste referentie in elk stuk onderpand vereisen omdat het deel uitmaakt van de wettelijke, merknaam.

## Eerste alinea{#firstparas}

In de eerste alinea moet u het onderwerp definiëren en aangeven wat de lezer leert van het lezen van het artikel.

Voorbeeld van de eerste alinea (concept):

_Soorten publiek zijn verzamelingen bezoekers (een lijst met bezoekers-id&#39;s). Adobe beheert de vertaling van bezoekersgegevens in publiekssegmentatie. Als dusdanig, is het creëren van en het leiden van publiek gelijkaardig aan het creëren van en het gebruiken van segmenten, met de toegevoegde capaciteit om het publiekssegment aan de Experience Cloud te delen._

Voorbeeld van eerste alinea (taak):

_Maak de bron van het klantkenmerk (CSV- en FIN-bestanden) en upload de gegevens. U kunt de gegevensbron activeren wanneer u klaar bent. Nadat de gegevensbron actief is, deel de attributengegevens aan Analytics en Doel._

### SEO-tips voor eerste alinea&#39;s{#seo}

* Neem zoektermen op in de eerste alinea.
* Gebruik termen die door lezers worden gebruikt.
* Synoniemen en, indien nodig, eerder gebruik van termen opnemen. Bijvoorbeeld: &quot;De Experience Cloud ID-service (ECID), voorheen bekend als _bezoeker-id_ of als acroniemen zoals MID, MCVID, verstrekt een universele, blijvende identiteitskaart die bezoekers identificeert.&quot;
* SEO-termen opnemen in koppelingen.
* Plaats geen essentiële termen in complexe tabellen. Complexe tabellen leveren geen betrouwbare zoekresultaten op. Tekst in afbeeldingen wordt niet doorzocht. Bijschriften worden doorzocht.

## Kapitalisatie{#capitalization}

* In de stijl Adobe wordt voor alle titels, koppen, subkoppen en pagina-navigatie-elementen gebruikgemaakt van een hoofdlettergebruik in de stijl van een zin.
* Alle woorden zijn in kleine letters behalve het eerste woord en de juiste nummers, zoals de namen van merken, oplossingen en services.
* Identiek aan het hoofdlettergebruik in de productnamen van gereedschappen, opties, menu-items, dialoogvensters en velden.

## Inhoudsopgave{#using-toc}

De `TOC.md` is uw inhoudsopgave. Elke gids zou één moeten hebben.

**Redactionele richtsnoeren voor een inhoudsopgave**

* Hoofdlettergebruik: Gebruik altijd een zin-case voor elk item (zonder acroniemen). Hiermee kunt u alleen formele productnamen of interface-elementen (pagina&#39;s, tabbladen, velden, opties, enzovoort) in hoofdletters weergeven. Komt overeen met de interface wanneer u ernaar verwijst.
* Vormgeving en parallellisme: Gebruik het dwingende werkwoord en vermijd het. Inhoudsopgave&#39;s zijn lijsten, zodat lijsten meestal parallel worden gehouden. Er zijn uitzonderingen die soms niet kunnen worden vermeden. Gebruik voor conceptuele pagina&#39;s fonts en zelfstandig naamwoorden. Gebruik werkwoorden voor taken.

**Syntaxisrichtlijnen**

* Een sectiekop (bovenliggend item) in de inhoudsopgave kan geen koppeling zijn. het heeft geen pagina met inhoud. Het moet een anker bevatten, zoals `{#processing-rules}`.
* U moet de juiste syntaxis gebruiken voor de koppen van inhoudsopgavesecties (bijvoorbeeld `+ Processing rules {#processing-rules}`) en koppelingen naar inhoudsopgaveartikelen (bijvoorbeeld `+ [Article name](article.md)`).
* Items van inhoudsopgaveartikelen kunnen een verkorte versie van de titel van het artikel zijn. Volg de normen voor het schrijven van overzichten, concepten, en taken in dit document.
* Voeg hetzelfde bestand niet meerdere keren toe aan een inhoudsopgave (of aan meerdere inhoudsopgaven). Dit veroorzaakt oneven gedrag.
* Als uw repo meerdere gebruikershandleidingen bevat, moeten de directory&#39;s van de gebruikershandleiding zich op hetzelfde niveau bevinden, zoals de submappen in de `help` directory. Elke map met gebruikershandleidingen moet een inhoudsopgavebestand hebben. Geen nestende gebruikershandleidingen.

## Vet en cursief{#bold}

* Gebruik vette tekst alleen voor interface-elementen waarop u in een procedure klikt (en met UICONTROL).
* Gebruik cursief voor accenten of wanneer een woord zonder accolade door elkaar haalt. Bijvoorbeeld, een buitenlands woord, of wanneer u een woord beschrijft of een termijn bepaalt.
