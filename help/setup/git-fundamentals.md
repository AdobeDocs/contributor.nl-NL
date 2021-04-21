---
title: De documentatie van Git en GitHub essentiële
description: Dit artikel verklaart een overzicht van Git, bewaarplaats GitHub, en hoe de inhoud wordt georganiseerd, en noemende overeenkomsten die voor de documentatie van Adobe worden gebruikt.
exl-id: 2b2ec764-4201-4bcd-802d-a034d6675793
translation-type: tm+mt
source-git-commit: 1b1678b33059f4bc8f7aff4690f1d775e6aee2d6
workflow-type: tm+mt
source-wordcount: '660'
ht-degree: 0%

---

# De documentatie van Git en GitHub essentiële

## Overzicht

Als u alleen kleine, alleen-tekst wijzigingen in artikelen wilt aanbrengen, hoeft u de details van dit artikel niet te begrijpen. In dit artikel wordt de workflow beschreven voor het uitvoeren van belangrijke bewerkingen, zoals het maken van nieuwe artikelen, het toevoegen van afbeeldingen of het doorlopend bewerken van Adobe-documentatie.

Als medewerker aan de documentatieinhoud van Adobe, kunt u met veelvoudige hulpmiddelen en processen in wisselwerking staan. U kunt parallel met andere contribuanten aan hetzelfde project werken, mogelijk dezelfde inhoud, zelfs tegelijkertijd. Dit wordt allen toegelaten door de software van Git en van GitHub.

Git is een opensource versiecontrolesysteem dat samenwerking toestaat. Meerdere contribuanten kunnen werken aan bestanden die in *repositories* leven.

GitHub is een webgebaseerde hostingservice voor Git-opslagruimten, zoals die welke worden gebruikt om [docs.adobe.com](https://docs.adobe.com)-inhoud op te slaan. Voor om het even welk project, gastheren GitHub de belangrijkste bewaarplaats, waarvan de contribuanten exemplaren voor hun eigen werk kunnen maken.

## Git

Git heeft een unieke workflow en terminologie voor bijdragen die het gedistribueerde model ondersteunen. Er is bijvoorbeeld geen bestandsvergrendeling die normaal gesproken aan uitchecken/inchecken is gekoppeld. Met Git kunnen wijzigingen nog fijner worden opgelost, waarbij bestanden per byte worden vergeleken.

Git gebruikt ook een gelaagde structuur om inhoud voor een project op te slaan en te beheren:

- *Bewaarplaats*: Dit is ook wel een  *repo* genoemd, de hoogste opslageenheid. Een gegevensopslagruimte bevat een of meer vertakkingen.
- *Vertakking*: Alle opslagruimten bevatten een standaardvertakking (doorgaans &quot;master&quot; genoemd) en een of meer vertakkingen die bestemd zijn om weer in de master vertakking te worden samengevoegd. De master vertakking fungeert als de huidige versie en bron waaruit de inhoud wordt gepubliceerd. Het is het bovenliggende element waarvan alle andere vertakkingen in de repository worden gemaakt.

Medewerkers werken met Git samen om opslagruimten op zowel het lokale niveau als het niveau van GitHub bij te werken en te manipuleren:

- Lokaal door hulpmiddelen zoals de Desktop GitHub.
- Via [www.github.com](https://www.github.com), die Git integreert om de afstemming van bijdragen te beheren die terugvloeien naar de hoofdopslagplaats.

## GitHub

Alle werkschema&#39;s beginnen en eindigen op het niveau GitHub, waar de belangrijkste bewaarplaats voor om het even welk Adobe documentatieproject wordt opgeslagen. De kopieën die contribuanten voor eigen gebruik maken, worden verspreid over meerdere computers. Deze exemplaren worden uiteindelijk in de belangrijkste bewaarplaats GitHub van het project samengebracht.

### Directoryorganisatie

De standaard/master vertakking van een project fungeert als de huidige versie van de inhoud voor het project. De inhoud in de master vertakking - en takken die van het worden gecreeerd - richt zich op de organisatie van de artikelonderwerpen. Submappen worden gebruikt voor het ordenen van inhoud en afbeeldingselementen.

Doorgaans vindt u een hoofdmap `help` van de hoofdmap van de opslagplaats. De artikelmap bevat een set submappen. Artikelen in de submappen worden opgemaakt als Markeringsbestanden die de extensie *.md* gebruiken.

Binnen de wortel van deze folder, kunt u algemene artikelen vinden die op de algemene dienst of het product betrekking hebben. En typisch, kunt u een andere reeks subdirectories dan vinden die de eigenschappen/de diensten of gemeenschappelijke scenario&#39;s aanpassen.

### Map Middelen

De gidsen van de gebruiker bevatten `/assets` subdirectories voor beelddossiers die binnen een folder van verwijzingen worden voorzien.

<!--

### Markdown file template

For convenience, the root directory of each repository typically contains a Markdown template file named `template.md`. You can use this template file as a "starter file" if you need to create a new article for submission to the repository. The file contains:

- A **metadata header** at the top of the file, delineated by two, 3-hyphen lines. It contains the various tags used for tracking information related to the article. It also includes SEO optimizations and reporting processes that Adobe uses to evaluate the performance of the content. So the metadata is important!
- Various **examples of using Markdown** to format the elements of an article.
- General **instructions on the use of Markdown extensions**, which you can use for various types of alerts.
- Examples of **embedding video** by using an iframe.
- General **instructions on the use of docs.adobe.com extensions**, which you can use for special controls such as buttons and selectors.

-->

## Pull-aanvragen

Een *pull request* verstrekt een geschikte manier voor een medewerker om een reeks veranderingen voor te stellen die op de standaardtak zullen worden toegepast. De veranderingen (die ook als *komma* worden bekend) worden opgeslagen in de tak van een contribuant, zodat kan GitHub het effect van *het samenvoegen* hen in de standaardtak eerst modelleren. Een pull-verzoek fungeert ook als een mechanisme om de contribuant feedback te geven van een build/validatieproces, de controleur van de pull-aanvraag, om mogelijke problemen of vragen op te lossen voordat de wijzigingen worden samengevoegd in de standaardvertakking.

Er zijn twee manieren om door trekpleverzoek bij te dragen, afhankelijk van de grootte van veranderingen die u wilt voorstellen. Wij zullen dit in detail later, in de [GitHub werkschema](local-repo.md) sectie van deze gids behandelen.
