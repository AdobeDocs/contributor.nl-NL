---
title: GitHub-bijdrageworkflow voor grote wijzigingen
description: Leer hoe u kunt bijdragen aan de documentatie van Adobe op Experience League.
exl-id: ad467ad4-abd2-4166-8659-e29c48d268ec
source-git-commit: 90122796acee9214ba96360eb7b5ff5c321a4bd6
workflow-type: tm+mt
source-wordcount: '944'
ht-degree: 0%

---

# GitHub-bijdrageworkflow voor grote wijzigingen

<!--
>[!IMPORTANT]
>All repositories that publish to docs.adobe.com have adopted the [Adobe Open Source Code of Conduct](../../code-of-conduct.md) or the [.NET Foundation Code of Conduct](https://dotnetfoundation.org/code-of-conduct). For more information, see the [Contributing](../../contributing.md) article.
>
> Minor corrections or clarifications to documentation and code examples in public repositories are covered by the [Adobe Documentation Terms of Use](https://www.adobe.com/legal/terms.html). New or significant changes generate a comment in the pull request, asking you to submit an online Contribution License Agreement (CLA) if you are not an employee of Adobe. We need you to complete the online form before we can review or accept your pull request.
--->

## Overzicht

Deze workflow is geschikt voor een medewerker die een grote wijziging moet aanbrengen of die regelmatig een bijdrage levert aan een opslagplaats. De frequente contribuanten hebben typisch aan de gang zijnde (lang lopende) veranderingen, die door veelvoudige bouwstijl/bevestiging/het opvoeren cycli gaan of veelvoudige dagen overspannen alvorens trekverzoek aftekenen en samenvoegen.

### Terminologie

Alvorens u begint, herzien sommige termijnen Git/GitHub die in dit werkschema worden gebruikt.

| Naam | Beschrijving |
|-----------|-------------|
| vork | Normaal gebruikt als naamwoord, wanneer het verwijzen naar een exemplaar van een belangrijkste bewaarplaats GitHub. In de praktijk is een vork gewoon een andere opslagplaats. Maar het is speciaal in die zin dat GitHub een verbinding in twee richtingen terug naar de hoofd/ouderbewaarplaats handhaaft. Het wordt soms gebruikt als werkwoord, zoals in &quot;U moet eerst de gegevensopslagplaats vorken.&quot; |
| extern | Een benoemde verbinding met een externe opslagplaats, zoals de &quot;oorspronkelijke&quot; of &quot;upstream&quot; externe opslagplaats. Git verwijst hiernaar als externe bestanden omdat deze worden gebruikt om te verwijzen naar een opslagplaats die op een andere computer wordt gehost. In dit werkschema, is ver altijd een bewaarplaats GitHub. |
| oorsprong | De naam die is toegewezen aan de verbinding tussen uw lokale opslagplaats en de opslagplaats waaruit deze is gekloond. In deze workflow staat de oorsprong voor de verbinding met uw vork. Het wordt soms gebruikt als een moniker voor de oorspronkelijke repository zelf, zoals in &quot;Herinner me om uw veranderingen in oorsprong te duwen.&quot; |
| upstream | Net als de oorspronkelijke externe server is upstream een benoemde verbinding met een andere repository. In deze workflow vertegenwoordigt upstream de verbinding tussen uw lokale opslagplaats en de hoofdopslagplaats, waaruit uw vork is gemaakt. Het wordt soms gebruikt als moniker voor de stroomopwaartse bewaarplaats zelf, zoals in &quot;Herinner me om de veranderingen van upstream terug te trekken.&quot; |

Als u met de concepten Git en GitHub zoals een bewaarplaats of tak onbekend bent, gelieve eerst te herzien [Git- en GitHub-basisbegrippen](git-fundamentals.md).

## Workflow

>[!IMPORTANT]
> Als u dit nog niet hebt gedaan, moet u de stappen in het dialoogvenster [Instellen](github-signup.md) sectie.

In deze workflow worden wijzigingen doorgevoerd in een herhalingscyclus. Beginnend van de lokale bewaarplaats van uw apparaat, stromen zij terug naar uw vork GitHub, in de belangrijkste bewaarplaats GitHub, en terug plaatselijk terug aangezien u veranderingen van andere contribuanten opneemt.

### GitHub-stroom gebruiken

Herstellen vanaf [Git- en GitHub-basisbegrippen](git-fundamentals.md) dat een Git-opslagplaats een hoofdvertakking bevat, plus eventuele extra werk-in-uitvoering vertakkingen die niet in hoofd zijn geïntegreerd. Wanneer u een reeks logisch verwante veranderingen introduceert, is het beste praktijken om tot een *werktak* om uw wijzigingen te beheren via de workflow. Wij verwijzen hier naar het als werkende tak omdat het een werkruimte is om veranderingen te herhalen/te verfijnen, tot zij terug in de belangrijkste tak kunnen worden geïntegreerd.

Door gerelateerde wijzigingen in een specifieke vertakking te isoleren, kunt u deze wijzigingen onafhankelijk beheren en introduceren en kunt u ze op een specifieke releasetijd in de publicatiecyclus toepassen. Afhankelijk van het type werk dat u doet, kunt u in feite eenvoudig met verschillende werkvertakkingen in uw opslagplaats belanden. Het is niet ongebruikelijk om aan veelvoudige takken tezelfdertijd te werken, elk die een verschillend project vertegenwoordigen.

>[!NOTE]
>
>Wijzigingen aanbrengen in de hoofdvertakking *is geen goede praktijk*. Veronderstel dat u de belangrijkste tak gebruikt om een reeks veranderingen voor een vastgestelde eigenschapversie voor te stellen. U voltooit de wijzigingen en wacht op de release ervan. Ondertussen hebt u een dringend verzoek om iets te repareren, dus brengt u de wijziging aan in een bestand in de hoofdvertakking en publiceert u de wijziging. In dit voorbeeld publiceert u per ongeluk beide oplossingen *en* de wijzigingen die u op een bepaalde datum voor release hebt gebruikt.

De volgende stap bestaat uit het maken van een nieuwe werkende vertakking in uw lokale opslagplaats om de voorgestelde wijzigingen vast te leggen. Elke client is anders, dus raadpleeg de Help voor uw voorkeursclient. U kunt een overzicht van het proces in de GitHub Gids op zien [GitHub-stroom](https://guides.github.com/introduction/flow/).

## Verwerking van aanvraag volledig uitvoeren

U kunt voorgestelde wijzigingen verzenden door deze te bundelen in een nieuw pull-verzoek (PR) dat wordt toegevoegd aan de PR-wachtrij van de doelopslagplaats. Een trektrekkingsverzoek laat het samenwerkingsmodel van GitHub toe, door te vragen om de veranderingen van uw werkende tak worden getrokken en in een andere tak worden samengevoegd. In de meeste gevallen is die andere vertakking de standaard/hoofdvertakking in de hoofdopslagplaats.

### Validatie

Alvorens uw trekkingsverzoek in zijn bestemmingstak kan worden samengevoegd, zou het door één of meerdere processen van de PR bevestiging kunnen moeten overgaan. Validatieprocessen kunnen variëren afhankelijk van het bereik van voorgestelde wijzigingen en de regels van de gegevensopslagruimte van bestemming. Nadat uw pull-verzoek is verzonden, kunt u verwachten dat de inhoud wordt gecontroleerd en, indien van toepassing, wordt samengevoegd in de hoofdopslagplaats.

### Reviseren en aftekenen

Nadat alle PR-verwerking is voltooid, moet u de resultaten controleren (PR-opmerkingen, voorbeeld-URL&#39;s, enz.) om te bepalen of extra veranderingen in zijn dossiers worden vereist alvorens u voor het samenvoegen ondertekent. Als een PR-controleur uw intrekkingsverzoek heeft beoordeeld, kunnen deze ook feedback geven via opmerkingen als er nog onopgeloste problemen/vragen zijn die moeten worden opgelost voordat ze worden samengevoegd.

Wanneer de trekkingsaanvraag emissievrij is en afgemeld, worden uw wijzigingen weer samengevoegd in de bovenliggende vertakking en wordt de trekkingsaanvraag gesloten.

### Publiceren

Vergeet niet dat uw pull-verzoek moet worden samengevoegd met een PR-controleur voordat de wijzigingen kunnen worden opgenomen in de volgende geplande publicatiereeks. Een volledige aanvraag wordt doorgaans in de volgorde van indiening beoordeeld of samengevoegd. Als voor uw pull-verzoek samenvoeging voor een specifieke publicatiereeks is vereist, moet u vooraf met uw PR-controleur werken om ervoor te zorgen dat samenvoegen plaatsvindt voordat de publicatie wordt uitgevoerd.
