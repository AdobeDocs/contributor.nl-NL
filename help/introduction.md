---
title: Handleiding voor contribuanten voor Adobe-documentatie
seo-title: Overzicht van de Contribute-handleiding voor de technische documentatie van Adobe Experience Cloud
description: In de handleiding wordt beschreven hoe u suggesties en toevoegingen kunt toevoegen aan de documentatiesite van Adobe.
seo-description: In de handleiding wordt beschreven hoe u een bijdrage kunt leveren aan de technische documentatie van [!UICONTROL Adobe Experience Cloud].
translation-type: tm+mt
source-git-commit: 46674c112935a2a98a12210db92129a1bc475c46
workflow-type: tm+mt
source-wordcount: '840'
ht-degree: 0%

---


# Overzicht van de handleiding van de medewerker voor Adobe-documentatie

## Wat is collectieve documentatie

In 2019 gaat alle technische documentatie en de inhoud voor Adobe Experience Cloud over naar een nieuw platform, gebaseerd op open-sourcefontages, met gebruik van de oplossingen Github, Markdown en Adobe Experience Cloud, waaronder Adobe Experience Manager, Analytics, Launch en Target.

Dit open-sourcemodel verbetert de kwaliteit van de inhoud en de communicatie tussen klanten, documentatieteams en productteams. Op elke pagina kunt u nu het nut van inhoud beoordelen, problemen met het logbestand bekijken en zelfs inhoudssuggesties leveren als Git pull-aanvragen (PR&#39;s). De documentatieteams van Adobe houden dagelijks toezicht op de bijdragen en problemen en brengen waar nodig updates, aanpassingen en aanpassingen aan.

## Werken met collectieve documentatie

Als gebruiker van dit materiaal - ongeacht of u een werknemer, partner, klant of zelfs potentiële klanten bent - hebt u de keus om aan deze documentatie op verscheidene eenvoudige manieren bij te dragen;

* beoordelen of de pagina nuttig is
* een uitgave tegen een specifieke pagina registreren
* Breng zelfs een snelle bewerking door aan het ontwerpen van gehele artikelen, compleet met elementen en codevoorbeelden

In deze handleiding wordt alles beschreven wat u moet weten om te communiceren met en bij te dragen aan deze materiaalset.

<!--
> [!IMPORTANT]
> All repositories that publish to docs.adobe.com have adopted the [Adobe Open Source Code of Conduct](../code-of-conduct.md) or the [.NET Foundation Code of Conduct](https://dotnetfoundation.org/code-of-conduct). For more information, see the [Contributing](../contributing.md) article.
>
> Minor corrections or clarifications to documentation and code examples in public repositories are covered by the [Adobe Documentation Terms of Use](https://www.adobe.com/legal/terms.html). New or significant changes generate a comment in the pull request, asking you to submit an online Contribution License Agreement (CLA) if you are not an employee of Adobe. We need you to complete the online form before we can review or accept your pull request.
-->

## Snelle bewerkingen uitvoeren op bestaande documenten

Het maken van snelle bewerkingen is een goede manier om kleine fouten en omissies in documenten te corrigeren. Als in een artikel een bewerkknop wordt weergegeven zoals hieronder wordt weergegeven, kunt u een snelle correctie zelf uitvoeren. Wanneer u het document bewerkt, verzendt u een pull-verzoek (PR) om de correctie/suggestie naar ons te verzenden en kunnen we de suggestie doorlichten, goedkeuren en publiceren.

1. Onderteken, indien acceptabel, de licentieovereenkomst voor [contribuanten (CLA)](http://opensource.adobe.com/cla.html) .

   U hoeft slechts één keer een Adobe CLA te verzenden.
1. Klik **`Edit this page`** op de juiste kolom om naar het prijsonderdrukkbrondossier op GitHub te gaan.
1. Klik op het potloodpictogram om het artikel te bewerken.

   >[!NOTE]
   >
   >Als het potloodpictogram grijs uit is, moet u login aan uw rekening GitHub, of een nieuwe rekening tot stand brengen.

   ![Locatie van het potloodpictogram](assets/edit-icon.png)

1. Breng de gewenste wijzigingen aan in de webeditor. U kunt op het tabblad Wijzigingen **** voorvertoning klikken om de opmaak van de wijziging te controleren.
1. Blader naar de onderkant van de pagina nadat u de wijziging(en) hebt aangebracht. Voer een titel en beschrijving in voor uw PR en klik op Bestandswijziging **voorstellen** zoals in de volgende afbeelding wordt getoond:

   ![voorstellen, wijziging](assets/submit-pull-request.png)

   >[!NOTE]
   >
   >Als u een foutbericht krijgt over het ondertekenen van een licentieovereenkomst voor contribuanten (CLA), klikt u op **Details** om de licentieovereenkomst te openen. Onderteken de overeenkomst, indien acceptabel. Vervolgens sluit u het verzoek en opent u het verzoek en gaat u verder.

Dat is alles wat er aan te pas komt. Bedankt! De leden van het documentatieteam zullen uw trekkrachtverzoek herzien en samenvoegen.

## Een probleem aanmelden

Een andere gemakkelijke manier om ons op de hoogte te brengen van een probleem met een stuk inhoud is om een probleem te registreren.

1. Als er een probleem optreedt met inhoud, klikt u rechtsonder op een pagina op de `Log an Issue` koppeling. Zie onderstaande afbeelding:

   ![](assets/git_log_issue.png)

   >[!NOTE]
   >
   >U zult aan login aan uw rekening moeten GitHub, of een nieuwe rekening creëren, om een kwestie te registreren.

   Als u op deze koppeling klikt, kunt u een snel ticket bij ons aanmelden via de interface van Github Issue.

1. De URL van de pagina met de uitgave wordt automatisch ingevuld in het beschrijvingsveld. Vul de titel in, schrijf een korte beschrijving van de uitgave en klik vervolgens op *Nieuwe uitgave* verzenden.

   ![](assets/git_issue_example.png)

Als u een uitgave indient, wordt het inhoudsteam voor deze pagina direct op de hoogte gebracht van wie de actie kan ondernemen. Als we de inhoud hebben bijgewerkt, geven we dit via de interface Github Issues door en sturen we u een e-mail wanneer deze wordt bijgewerkt of gesloten.

## GitHub-machtigingen begrijpen

De GitHub die UI uitgeeft past aan uw bewaarplaatstoestemmingen aan. De voorgaande afbeeldingen zijn accuraat voor contribuanten die geen schrijfmachtigingen hebben voor de doelopslagplaats. GitHub leidt automatisch tot een vork van de doelbewaarplaats in uw rekening. Als u toegang tot de doelbewaarplaats hebt schrijven, leidt GitHub tot een nieuwe tak in de doelrepo.

Adobe gebruikt trekkingsverzoeken voor alle wijzigingen, zelfs voor contribuanten die schrijftoegang hebben. De meeste opslagplaatsen hebben de `master` tak beschermd zodat de updates als trekkingsverzoeken moeten worden voorgelegd.

De bewerkervaring in de browser is het meest geschikt voor kleine of niet-frequente wijzigingen. Als u een grote bijdrage levert of geavanceerde Git-functies gebruikt, raden we u aan de repo te [forken en lokaal](setup/full-workflow.md)te werken.

## Feedback geven

Als de oplossing zo groot is als die van Adobe, is de documentatie altijd een werk in uitvoering. Als u fouten ontdekt, registreer een kwestie, als u suggesties op materiaal hebt te vertellen gelieve ons. Vertel ons welke informatie u zocht. Laat ons weten of u niet kon vinden wat u nodig had, of als u moeite had om uw taak te voltooien, gelieve ons te vertellen hoe wij u kunnen helpen onze oplossingen leren.

Dank van het Collaborative Documentation team en alle schrijvers en inhoudsproducenten in de [!UICONTROL Adobe Experience Cloud].
