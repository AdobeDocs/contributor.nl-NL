---
title: Handleiding voor contribuanten voor Adobe-documentatie
seo-title: Contributor guide overview for Adobe Experience Cloud technical documentation
description: In de handleiding wordt beschreven hoe u suggesties en toevoegingen kunt toevoegen aan de documentatiesite Adobe.
seo-description: The guide describes how you can contribute to the [!UICONTROL Adobe Experience Cloud] technical documentation.
exl-id: 1294d0c6-897e-49c0-bf27-fd7d122f1fc8
source-git-commit: 5a9bbe0663a1efa8a683e892a42faed18f072e8a
workflow-type: tm+mt
source-wordcount: '819'
ht-degree: 0%

---

# Medewerkershandleiding voor Adobe-documentatie

In deze handleiding wordt beschreven hoe u een bijdrage kunt leveren aan de Adobe Enterprise Help op het Experience League.

## Wat is samenwerkingsdocumentatie?

De technische documentatie en enablement inhoud voor Adobe Experience Cloud en andere producten van de Onderneming van Adobe zijn gebaseerd op open bronprincipes die de oplossingen GitHub, Markdown, en van Adobe Experience Cloud gebruiken.

Dit open-sourcemodel verbetert de kwaliteit van de inhoud en de communicatie tussen klanten, documentatieteams en productteams. Op elke pagina kunt u nu het nut van inhoud beoordelen, problemen met het logbestand bekijken en zelfs inhoudssuggesties leveren als Git pull-aanvragen (PR&#39;s). De documentatieteams van de Adobe houden dagelijks toezicht op de bijdragen en problemen en voeren zo nodig updates, bijstellingen en aanpassingen uit.

## Werken met documentatie voor samenwerken

Als gebruiker van dit materiaal - ongeacht of u een werknemer, partner, klant of zelfs potentiële klanten bent - hebt u de keus om aan deze documentatie op verscheidene eenvoudige manieren bij te dragen;

* De bruikbaarheid van de pagina beoordelen
* Een probleem op een specifieke pagina vastleggen
* Breng snel wijzigingen aan in het ontwerpen van volledige artikelen, compleet met elementen en codevoorbeelden.

In deze handleiding wordt alles beschreven wat u moet weten om te communiceren met en bij te dragen aan deze materiaalset.

<!--
>[!IMPORTANT]
>All repositories that publish to docs.adobe.com have adopted the [Adobe Open Source Code of Conduct](../code-of-conduct.md) or the [.NET Foundation Code of Conduct](https://dotnetfoundation.org/code-of-conduct). For more information, see the [Contributing](../contributing.md) article.
>
> Minor corrections or clarifications to documentation and code examples in public repositories are covered by the [Adobe Documentation Terms of Use](https://www.adobe.com/legal/terms.html). New or significant changes generate a comment in the pull request, asking you to submit an online Contribution License Agreement (CLA) if you are not an employee of Adobe. We need you to complete the online form before we can review or accept your pull request.
-->

## Snelle bewerkingen uitvoeren op bestaande documenten

Het maken van snelle bewerkingen is een goede manier om kleine fouten en omissies in documenten te corrigeren. Als in een artikel een bewerkknop wordt weergegeven zoals hieronder wordt weergegeven, kunt u een snelle correctie zelf uitvoeren. Wanneer u het document bewerkt, verzendt u een pull-verzoek (PR) om de correctie/suggestie naar ons te verzenden en kunnen we de suggestie doorlichten, goedkeuren en publiceren.

1. Onderteken de [Licentieovereenkomst voor contribuanten (CLA)](http://opensource.adobe.com/cla.html) indien aanvaardbaar.

   U hoeft slechts één keer een Adobe CLA in te dienen.
1. Klik op de knop **`Edit this page`** pictogram in de juiste kolom om naar het van de prijsverhogingsbron dossier op GitHub te gaan.

   ![Dit paginapictogram bewerken](/help/assets/git_edit.png)

1. Klik op het potloodpictogram om het artikel te bewerken.

   >[!NOTE]
   >
   >Als het potloodpictogram grijs uit is, moet u login aan uw rekening GitHub, of een nieuwe rekening tot stand brengen.

   ![Locatie van het potloodpictogram](assets/edit-icon.png)

1. Breng de gewenste wijzigingen aan in de webeditor. U kunt op de knop **Wijzigingen voorvertonen** om de opmaak van de wijziging te controleren.
1. Blader naar de onderkant van de pagina nadat u de wijziging(en) hebt aangebracht. Voer een titel en beschrijving in voor je PR en klik op **Bestand wijzigen voorstellen** zoals weergegeven in de volgende afbeelding:

   ![voorstellen, wijziging](assets/submit-pull-request.png)

   >[!NOTE]
   >
   >Als u een foutbericht krijgt over het ondertekenen van een licentieovereenkomst voor contribuanten (CLA), klikt u op **Details** de licentieovereenkomst te openen. Onderteken de overeenkomst, indien acceptabel. Vervolgens sluit u het verzoek en opent u het verzoek en gaat u verder.

Dat is alles wat er aan te pas komt. Bedankt! De leden van het documentatieteam zullen uw trekkrachtverzoek herzien en samenvoegen.

## Een probleem aanmelden

Een andere gemakkelijke manier om ons op de hoogte te brengen van een probleem met een stuk inhoud is om een probleem te registreren.

1. Als u een probleem met een stuk inhoud ziet, klikt u op de knop **`Log an Issue`** in de rechterkolom.

   ![](assets/git_log_issue.png)

   >[!NOTE]
   >
   >U zult aan login aan uw rekening GitHub moeten, of een nieuwe rekening creëren, om een kwestie te registreren.

   Als u op deze koppeling klikt, kunt u een snel ticket bij ons aanmelden via de interface van Github Issue.

1. De URL van de pagina met de uitgave wordt automatisch ingevuld in het beschrijvingsveld. Vul de titel in, schrijf een korte beschrijving van de kwestie, en klik dan *Nieuwe uitgave verzenden*.

   ![](assets/git_issue_example.png)

Als u een uitgave indient, wordt het inhoudsteam voor deze pagina direct op de hoogte gebracht van wie de actie kan ondernemen. Als we de inhoud hebben bijgewerkt, geven we dit via de interface Github Issues door en sturen we u een e-mail wanneer deze wordt bijgewerkt of gesloten.

## GitHub-machtigingen begrijpen

De GitHub die UI uitgeeft past aan uw bewaarplaatstoestemmingen aan. De voorgaande afbeeldingen zijn accuraat voor contribuanten die geen schrijfmachtigingen hebben voor de doelopslagplaats. GitHub leidt automatisch tot een vork van de doelbewaarplaats in uw rekening. Als u toegang tot de doelbewaarplaats hebt schrijven, leidt GitHub tot een nieuwe tak in de doelrepo.

Adobe gebruikt trekkingsverzoeken voor alle veranderingen, zelfs voor contribuanten die schrijftoegang hebben. De meeste opslagplaatsen hebben de `master` vertakking beveiligd zodat updates moeten worden ingediend als pull-aanvragen.

De bewerkervaring in de browser is het meest geschikt voor kleine of niet-frequente wijzigingen. Als u een grote bijdrage levert of geavanceerde Git-functies gebruikt, raden we u aan [forceer de repo en werk lokaal](setup/full-workflow.md).

## Feedback geven

Met een oplossing die zo groot als Adobe wordt geplaatst, is de documentatie altijd een werk lopend. Als u fouten ontdekt, registreer een kwestie, als u suggesties op materiaal hebt te vertellen gelieve ons. Vertel ons welke informatie u zocht. Laat ons weten of u niet kon vinden wat u nodig had, of als u moeite had om uw taak te voltooien, gelieve ons te vertellen hoe wij u kunnen helpen onze oplossingen leren.

Dank van het Collaborative Documentation team en alle schrijvers en inhoudsproducenten in het [!UICONTROL Adobe Experience Cloud].
