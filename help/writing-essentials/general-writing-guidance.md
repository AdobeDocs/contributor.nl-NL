---
lastModified: 2018-06-28T00:00:00Z
title: Richtlijnen voor ontwerpstijl voor externe medewerkers
description: Leer meer over creatie en redactionele richtlijnen voor externe medewerkers aan Experience League.
exl-id: 874f88d7-18ad-4ac8-bfa3-737255652bbc
source-git-commit: 03d46c9ffb664824f9526f781d776069d486f271
workflow-type: tm+mt
source-wordcount: '2203'
ht-degree: 0%

---

# Richtlijnen voor ontwerpstijl voor externe medewerkers{#guidelines}

Deze pagina bevat redactionele richtlijnen voor externe auteurs die inhoud maken of bestaande inhoud op het Experience League bijwerken. Voordat u begint, moet u controleren of:

* Krijg vertrouwd met [ Markdown ](markdown.md) authoring
* Spelling en grammatica in uw artikelen controleren
* Gebruik een vriendelijke toon, een consistente presentatie en eenvoudige zinnen om computervertaling te verbeteren
* Volg [ best-practices ](#writing-tips) en redactionele normen op deze pagina

## Richtlijnen voor stijl{#style-guidelines}

Houd rekening met het volgende wanneer u documentatie schrijft.

* **schrijven beknopt**: Verspil geen woorden. Laat zinnen kort en beknopt zijn. Houd uw artikel geconcentreerd. Beperk het aantal notities tot een minimum.
* **concentreert zich op het publiek en het doel**: Alvorens u begint te schrijven, bepaal duidelijk wie de klant is en welke taak hij of zij probeert om te verwezenlijken. Schrijf uw artikel om die klant te helpen die taak te doen.
* **voorbeelden van het Gebruik**: Verstrek voorbeelden om concepten te verklaren.
* **organiseer uw inhoud**: Creeer secties om instructies in handelbaardere groepen stappen te verdelen. Gebruik een schermafbeelding wanneer u deze helderder maakt.

## Aanbevolen werkwijzen voor technisch schrijven{#writing-tips}

Technisch schrijven, met name voor softwaredocumentatie, is een gespecialiseerde bedrijfstak. Zelfs wordt de meest productieve novelist flustered wanneer het proberen van technisch schrijven-niet omdat het materiaal complex of technisch is, maar omdat het niet gemakkelijk is makend complexe, technische informatie _eenvoudig_. Uw inhoud kan alleen succesvol zijn als deze structureel consistent, scannbaar, herbruikbaar en zonder structuur- en syntaxisfouten door de publicatiepijplijn loopt.

In de volgende secties worden algemene problemen beschreven waarvoor nieuwe schrijvers moeten uitkijken:

### Koppen niet van elkaar gescheiden door tekst (dubbele koppen){#double-headings}

Als u twee koppen hebt zonder tekst die ze scheidt, voegt u ontbrekende tekst toe (om de tweede onderwerpkop in te voeren). U kunt ook een van de koppen verwijderen. Het tweede is waarschijnlijk overbodig.

Bijvoorbeeld, _het Overzicht_ dient geen doel hier:

![ Dubbele rubrieken ](assets/headings-double.png)

* Ook, als uw tweede rubriek _Overzicht_ toevallig is, is het waarschijnlijk onnodig. Uw H1 en eerste paragraaf dienen als conceptueel overzicht over het onderwerp van het artikel.

* Op dezelfde manier, voor SEO doeleinden, zijn de stand-alone rubrieken zoals _Overzicht_ en _Inleiding_ niet nuttig door zich. Geef het product of de functie die u wilt introduceren een naam. (Voorbeeld: _Overzicht van de rapporten van de Uitval_)

### Inconsistente kruisverwijzingskoppen{#maps}

Gebruik _Meer informatie_ rubrieken voor verwijzingslijsten (of kaarten). Voorbeeld:

![ Lijst van de Verwijzing van de Kruisverwijzing ](assets/headings-more-info.png)

**Begeleiding voor verwijzingslijsten**

* Een lijst met opsommingstekens gebruiken voor de kruisverwijzingen
* Cursief gebruiken voor de formele namen van hulplijnen of paginanamen (wanneer u geen koppelingstekst gebruikt)
* Geen punctuatie toepassen op de kop (of op een kop)
* Nummers in koppen voorkomen

### Verkeerd overeenkomend inhoudsopgave-item, broodkruimel en paginanaam{#toc}

Omdat we het inhoudsopgavebestand (inhoudsopgave) handmatig beheren, zijn deze problemen eenvoudig te verhelpen. Zorg ervoor dat de inhoudsopgave-vermelding overeenkomt met de paginanaam (H1). Zorg er ook voor dat deze veel overeenkomt met de breadcrumb.

**Begeleiding op TOCs en lijsten**

* Mogelijk moet u het inhoudsopgave-item verkorten, maar dit moet duidelijk betrekking hebben op de paginanaam en de broodkruimel.
* Broodkruimels worden uit de metagegevens van de titel gehaald, zodat ze kunnen verschillen (voor SEO-doeleinden).

### Aanhalingstekens in plaats van cursief{#quotes}

Het is moeilijk om te weerstaan aan het toevoegen van citaten rond een woord of uitdrukking. Aanhalingstekens zijn echter bedoeld voor het citeren van spraak en worden bijna nooit gebruikt in de productdocumentatie.

**Begeleiding op aanhalingstekens**

* Cursief werkt meestal beter dan aanhalingstekens (voor foutberichten, unieke of vreemde woorden enzovoort).
* Gebruik Vet en UICONTROL voor interface-elementen.

### Procedures{#steps}

Het schrijven van een procedure (het _taak_ inhoudstype) is geen talent dat wij met worden geboren. Het opbouwen van een leesbare, duidelijke procedure verloopt in de praktijk.

**Begeleiding voor stappen**

* Een procedure is een reeks stappen. Een stap is een kort, genummerd, _enig-zin_ bevel.
* Begin elke stap of met een werkwoord of _aan_ infinitief (om de lezer aan het doel, zoals in te richten, _om binnen ondertekend te blijven, laat **binnen ondertekend blijven toe**_). Als een stap een specifiek doel binnen de algemene procedure heeft, vermeld het doel vóór de actie.
* Als u informatie over de stap (een inhoudstype genoemd _stapinfo_ hebt, voeg het na de stap (ingesprongen met de stap) of na de activa (een het schermschot, video, of een lijst van interfacebeschrijvingen) toe.
* Als uw stap twee acties (zoals heeft, _selecteer dit, toen dat_), het als enige, korte zin schrijven.
* Beperk uw taak tot ongeveer zeven tot tien stappen. Als u meer dan tien stappen in één taak creeert, zult u het in twee taken waarschijnlijk moeten breken. Gebruik hier je beste oordeel.
* Gebruik in de productdocumentatie geen koppen als stappen. (Uitzondering hieronder voor zelfstudies.)
* Voor zelfstudies met meerdere pagina&#39;s kunnen koppen als stappen worden toegestaan. Nochtans, maak geen aantal hen. Eerder, spreid uit _Stap 1:_, _Stap 2:_, etc.

**procedure van het Voorbeeld**

Hier volgt een goed gestructureerde procedure voor aanmelden bij Adobe:

Aanmelden bij Adobe:

1. Voor `Adobe.com`, uitgezochte **Experience Cloud**.
1. Selecteer **Sign-in**.
1. Selecteer **Persoonlijke Rekening**.
1. Om binnen ondertekend te blijven, uitgezochte **blijven aangemeld**.
1. Typ uw naam en wachtwoord.
1. Selecteer **Sign-in**.

### Parallelle lijsten{#lists}

Met parallelle constructie voor lijsten kunt u gemakkelijk lezen en scannen. Lijsten bevatten een inhoudsopgave (inhoudsopgave), opsommingstekens (niet-geordende) lijsten of genummerde lijsten.

Voorbeeld-inhoudsopgave met parallelle items:

![ Parallelle TOC ](assets/parallel-toc.png)

De voorafgaande inhoudsopgave is een goed voorbeeld omdat:

* Conceptuele bovenliggende items zijn &#39;nos&#39; of &#39;zelfstandig naamwoord&#39;
* Procedures (taken) zijn actieve werkwoorden (geen gerondes)
* Alle items gebruiken hoofdlettergebruik voor zinnen

## Metagegevens voor titel en beschrijving{#metadata}

_Titel_ en _beschrijvings_ meta-gegevens zijn belangrijk voor SEO, inhoudsontdekking, en de scores van de inhoudskwaliteit op Experience League.

Hier volgen voorbeelden van titels en beschrijvingen:

**Beschrijvingen voor concepteartikelen**

* _leer over segmenten in Adobe Analytics. Krijg hulp bij het vormen van het paneel van de Segmentatie in een werkruimte._
* _vind hulp bij het gebruiken van segmenten in een rapport van de Mening van de Pagina in Adobe Analytics._

**Beschrijvingen voor procedure/taakartikelen**

* _leer hoe te om een segment in Adobe Analytics tot stand te brengen._
* _creeer een segment in Adobe Analytics. Leer hoe te om, een rapport te selecteren te vormen en in werking te stellen dat op het segment wordt gebaseerd u creeert._

Het object dat u gebruikt, is afhankelijk van de grootte en het bereik van het artikel.

**Titel voor een concepteartikel**

* _Segmenten in de rapporten van de Mening van de Pagina_

**Titel voor een procedure/taakartikel**

* _creeer een segment voor een rapport van de Mening van de Pagina_

(Vergeet niet dat de verticale streep en de productnaam automatisch aan titels worden toegevoegd.)

## Manieren om de helderheid te verbeteren (en Acrolinx-scores){#tips}

Hier volgen eenvoudige manieren om het ontwerp, de helderheid en de leesbaarheid van inhoud te verbeteren. Deze helpen ook de scores in de Acrolinx-stijl en de CQI-scores op de ExL verbeteren.

| Richtlijnen | Info |
|---|---|
| Actieve stem gebruiken | De passieve stem van de verandering in actieve stem |
| Huidige spanningen gebruiken | **Zwakke:** *de Campagne v8 zal in Juni vrijgeven.* <p>**Sterk:** *de versies van de Campagne v8 in Juni.*<p>De huidige spanningen zijn altijd beter leesbaar voor klanten. |
| Vermijd zwakke, onnodige adverbare | *Zeer*, *extreem*, *ongelooflijk*... <p>Adverbs zijn extra woorden die geen significante betekenis toevoegen als u sterke en nauwkeurige woorden, clausules, en adjectieven gebruikt. |
| De sterke werkwoorden van het gebruik voor titels en [ ingangen TOC ](#using-toc) | Voorbeelden:<p>**Zwakke:** *de verwezenlijking en het beheer van het Rand* <p>**Sterk:** *creeer en beheer eigenschappen* |
| De zin [ kapitalisatie van het gebruik ](https://docs.microsoft.com/en-us/style-guide/capitalization) | In twijfel, kapitaliseer niet. Gebruik in koppen hoofdletters in de stijl van de zin. Plaats de juiste nummers in hoofdletters en het eerste woord na een dubbele punt. In procedures, pas kapitalisatie aan die u in de interface ziet. |
| Lees deze kleine tips voor meer duidelijkheid | <ul><li>Vermijd *om* (het voegt geen betekenis toe). Al u nodig is *aan.*</li><li>Vermijd *Gebruik.* Het klinkt misschien technisch, maar dat is het niet. *gebruik* middelen *om goed gebruik van, vooral van iets te maken dat niet bedoeld voor het doel was maar* zal dienen.</li><li>Geen puntkomma&#39;s: gebruik in plaats daarvan een punt en begin een nieuwe zin. Halfdubbele punten zorgen voor onnodige complexiteit.</li><li>Dubbele punten: gebruik dubbele punten om een lijst te introduceren. Gebruik spaarzaam dubbele punten binnen zinnen. Plaats het eerste woord na een dubbele punt in een zin met een hoofdletter.</li><li>Gebruik de komma van Oxford (drie komma&#39;s in een lijst).</li><li>De lengte van de zin moet minder dan 39 woorden zijn.</li><li>Navigatie: het gebruik _gaat_ of _navigeren aan_.</li><li>Gebruik geen onbewerkte URL-tekst (gebruiksvriendelijke koppelingstekst), tenzij het weergeven van het pad belangrijke informatie is.</li></ul> |
| Spellingcontrole gebruiken in VSC | Installeer de Controle van de Spellingcontrole van de Code (uitbreiding) in de Code van Visual Studio. |
| De verandering _klikt_ aan _gaat_ of _uitgezocht_ | _klik_ is een apparaat-specifiek woord (met toegankelijkheidskwesties), en de trend moet zich van het bewegen. Hier volgen enkele suggesties voor het wijzigen van de code:<ul><li>Navigatie: _ga naar Dossier > Druk_.</li><li>Het klikken: _Uitgezochte Dossier > Druk_ of _Uitgezochte O.K._. </li></ul>Zie [ beschrijvend interactie met UI ](https://docs.microsoft.com/en-us/style-guide/procedures-instructions/describing-interactions-with-ui) voor meer ideeën over de beste woordkeus in diverse situaties. |
| Acrolinx uitvoeren in VSC | Acrolinx controleert op problemen met stijl en grammatica. Het controleert URLs, terminologie, spelling, en meer. Het helpt u uw helderheid te verbeteren en verbetert vertaling op de inhoud van het Experience League. |

{style="table-layout:auto"}

Nog een paar beste praktijken en bronnen:

* [ Scannable inhoud ](https://docs.microsoft.com/en-us/style-guide/scannable-content/): De lezers van de hulp vinden wat zij snel nodig hebben, of erkennen enkel zo snel wanneer zij niet waar zij moeten zijn. Het schrijven om het scannen te vergemakkelijken kan u helpen.
* **Aantallen:** in lichaamstekst, spelt gehele aantallen van nul tot negen, en gebruiksaantallen voor 10 of groter. Zie [ Aantallen ](https://docs.microsoft.com/en-us/style-guide/numbers).
* Schrijf zoals je spreekt, projectvriendelijkheid en kom snel tot het punt.

Zie [ Hoogste 10 het Schrijven Tips ](https://docs.microsoft.com/en-us/style-guide/top-10-tips-style-voice) in de [ Gids van de Stijl Microsoft® ](https://docs.microsoft.com/en-us/style-guide/welcome/) voor meer informatie.

## Alt-tekst{#alt-text}

Voeg betekenisvolle alternatieve tekst toe aan uw elementen (afbeeldingen). Houd rekening met alternatieve tekst die overeenkomt met:

* De doelklanten kunnen (taak of conceptennaam) verwezenlijken
* De functie of pagina die u weergeeft
* De pictogramnaam die u weergeeft

Google beschouwt de alt-text in SEO-resultaten.

## Lokalisatie - DNL en UICONTROL{#localization}

U hoeft zich geen zorgen te maken of uw product gelokaliseerd is of welke talen ExL gebruikt. U kunt de kwaliteit van de lokalisatie echter verbeteren door waar nodig de volgende twee markeringen voor markeringen (vereist) toe te passen:

* `DNL`

  DNL middelen _lokaliseren niet_. U gebruikt deze alleen voor productnamen van gedeponeerde Adoben, die allemaal in het Engels moeten blijven staan.

  Syntaxisvoorbeelden: `[!DNL Adobe Campaign]` of `[!DNL Workfront]`

  DNL is niet bedoeld voor bestandsnamen of URL&#39;s.

* `UICONTROL`

  UICONTROL wijst op een interfacecontrole (zoals een optie, gebied, lusje, pagina, groep opties, of eigenschapnaam in UI).

  Voorbeeld van syntaxis: `Select **[!UICONTROL Project]**, then select **[!UICONTROL Save]**.`

>[!IMPORTANT]
>
>U moet deze labels toepassen voordat u de inhoud lokaliseert.

### Adobe in productnamen gebruiken{#product-names}

Voor collectieve identiteit, omvatten wij gewoonlijk _Adobe_ in de eerste verwijzing van een product op het hulplijnniveau. Afhankelijk van de ruimte, kunt u Adobe in een rubriek laten vallen, maar dan zou de eerste verwijzing in het lichaamskopie de volledige naam moeten omvatten. Bepaalde producten, zoals _Adobe Audition_ en _Adobe Premiere Pro_, vereisen het gebruik van Adobe op eerste of meest prominente verwijzing in elk stuk van onderpand omdat het deel van de wettelijke, gemerkte naam uitmaakt.

## Eerste alinea{#firstparas}

In de eerste alinea moet het onderwerp worden gedefinieerd en moet worden beschreven wat de lezer leert van het lezen van het artikel.

Voorbeeld eerste alinea (concept):

_publiek is inzamelingen van bezoekers (een lijst van bezoekers IDs). De publieksservice van Adobe beheert de vertaling van bezoekersgegevens in publiekssegmentatie. Als dusdanig, is het creëren van en het leiden van publiek gelijkaardig aan het creëren van en het gebruiken van segmenten, met de toegevoegde capaciteit om het publiekssegment aan het Experience Cloud te delen._

Voorbeeld van de eerste alinea (taak):

_creeer de bron van het klantenattribuut (CSV en FIN dossiers) en upload de gegevens. U kunt de gegevensbron activeren wanneer u klaar bent. Nadat de gegevensbron actief is, deel de attributengegevens aan Analytics en Doel._

### SEO-tips voor eerste alinea&#39;s{#seo}

* Neem zoektermen op in de eerste alinea.
* Gebruik termen die door lezers worden gebruikt.
* Synoniemen en, indien nodig, eerder gebruik van termen opnemen. Bijvoorbeeld, &quot;de Dienst van identiteitskaart van het Experience Cloud (ECID), die eerder als _bezoekersidentiteitskaart_ of als acroniemen zoals MID, MCVID wordt bekend, verstrekt een universele, blijvende identiteitskaart die bezoekers identificeert.&quot;
* SEO-termen opnemen in koppelingen.
* Plaats geen essentiële termen in complexe tabellen. Complexe tabellen leveren geen betrouwbare zoekresultaten op. Tekst in afbeeldingen wordt niet doorzocht. Bijschriften worden doorzocht.

## Kapitalisatie{#capitalization}

* Bij de stijl van de Adobe wordt voor alle titels, koppen, subkoppen en pagina-navigatie-elementen gebruikgemaakt van een hoofdlettergebruik in de stijl van een zin.
* Alle woorden zijn in kleine letters behalve het eerste woord en de juiste nummers, zoals de namen van merken, oplossingen en services.
* Identiek aan het hoofdlettergebruik in de productnamen van gereedschappen, opties, menu-items, dialoogvensters en velden.

## Inhoudsopgave{#using-toc}

De `TOC.md` is uw inhoudsopgave. Elke gids zou één moeten hebben.

**Redactionele begeleiding voor een TOC**

* Hoofdlettergebruik: gebruik altijd het hoofdlettergebruik van zinnen voor elk item (behalve voor acroniemen). Hiermee kunt u alleen formele productnamen of interface-elementen (pagina&#39;s, tabbladen, velden, opties, enzovoort) in hoofdletters weergeven. Komt overeen met de interface wanneer u ernaar verwijst.
* Vormgeving en parallellisme: gebruik het dwingende werkwoord en vermijd omslagen. Inhoudsopgave&#39;s zijn lijsten, dus probeer lijsten het grootste deel van de tijd parallel te houden. Er zijn uitzonderingen die soms niet kunnen worden vermeden. Gebruik voor conceptuele pagina&#39;s fonts en zelfstandig naamwoorden. Gebruik werkwoorden voor taken.

**begeleiding van de Syntaxis**

* Een sectiekop (bovenliggend item) in de inhoudsopgave kan geen koppeling zijn, maar heeft geen pagina met inhoud. Het moet een anker zoals `{#processing-rules}` bevatten.
* U moet de juiste syntaxis gebruiken voor koppen van inhoudsopgavesecties (bijvoorbeeld `+ Processing rules {#processing-rules}` ) en koppelingen naar inhoudsopgaveartikelen (bijvoorbeeld `+ [Article name](article.md)` ).
* Items van inhoudsopgaveartikelen kunnen een verkorte versie van de titel van het artikel zijn. Volg de normen voor het schrijven van overzichten, concepten, en taken in dit document.
* Voeg hetzelfde bestand niet meerdere keren toe aan een inhoudsopgave (of aan meerdere inhoudsopgaven). Dat leidt tot oneven gedrag.
* Als uw repo meerdere gebruikershandleidingen bevat, moeten de mappen met gebruikershandleidingen zich op hetzelfde niveau bevinden, zoals de submappen in de map `help` . Elke map met gebruikershandleidingen moet een inhoudsopgavebestand hebben. Geen nestende gebruikershandleidingen.

## Vet en cursief{#bold}

* Gebruik vette tekst alleen voor interface-elementen waarop u in een procedure klikt (en met UICONTROL).
* Gebruik cursief voor accenten of wanneer een woord zonder accolade door elkaar haalt. Bijvoorbeeld, een buitenlands woord, of wanneer u een woord beschrijft of een termijn bepaalt.
