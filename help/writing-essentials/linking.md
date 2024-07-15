---
lastModified: 2018-06-28T00:00:00Z
title: Koppelingen gebruiken in documentatie
seo-title: Using links in Adobe Git/Markdown documentation
description: In dit artikel vindt u richtlijnen voor het maken van koppelingen naar inhoud en afbeeldingen.
seo-description: This article provides guidance on creating links to content and images for Adobe documentation.
exl-id: f9d61aa9-931c-4654-ab21-c6e47936954e
source-git-commit: dad1df81797e6078645449501ed0661cf4bcf3ce
workflow-type: tm+mt
source-wordcount: '319'
ht-degree: 0%

---

# Koppelingen gebruiken in documentatie

In dit artikel wordt het gebruik van hyperlinks in documentatiepagina&#39;s beschreven. Koppelingen zijn eenvoudig toe te voegen aan markering met een aantal verschillende conventies. Koppelingen wijzen gebruikers naar inhoud op dezelfde pagina, wijzen naar andere aangrenzende pagina&#39;s of wijzen naar externe sites en URL&#39;s.

>[!IMPORTANT]
>In het ideale geval moeten alle koppelingen beveiligde koppelingen zijn ( `https` vs `http` ) wanneer het doel dit ondersteunt (wat de overgrote meerderheid zou moeten doen).

## Koppeling naar URL&#39;s

De woorden die u opneemt in koppelingstekst moeten de titel zijn van de pagina waarnaar u koppelt of een specifieke, beschrijvende tekst.

**Voorbeelden:**

- `For more information, see the [overview article](https://github.com/AdobeDocs/target.en/help/overview.md).`

- `For more details, see [Adobe Legal Concerns](https://www.adobe.com/legal).`

## Koppeling maken tussen artikelen

Gebruik de volgende syntaxis voor koppelingen om een inline koppeling te maken van het ene artikel naar het andere in dezelfde repository:

- Een artikel in een map is gekoppeld aan een ander artikel in dezelfde map:

  `[link text](article-name.md)`

- Een artikel verbindt van subdirectory aan een artikel in de wortelfolder:

  `[link text](../article-name.md)`

- Een artikel verbindt van subsubdirectory met een artikel in de wortelfolder:

  `[link text](../../article-name.md)`

- Een artikel in de hoofdmap is gekoppeld aan een artikel in een submap:

  `[link text](./directory/article-name.md)`

- Een artikel in een submap is gekoppeld aan een artikel in een andere submap:

  `[link text](../directory/article-name.md)`

- Een artikel in een subsubmap is gekoppeld aan een artikel in een andere submap:

  `[link text](../../directory/article-name.md)`

## Koppeling naar ankers

U hoeft geen ankers te maken. Ze worden automatisch gegenereerd tijdens het publiceren voor alle H2-koppen. Het enige wat u moet doen is verbindingen aan H2 (##) secties tot stand brengen.

- Een koppeling maken naar een kop in hetzelfde artikel:

  `[link](#the-text-of-the-level2-section-separated-by-hyphens)`

  `[Link to anchors](#links-to-anchors)`

- Een koppeling maken naar een anker in een ander artikel in dezelfde submap:

  `[link text](article-name.md#anchor-name)`

  `[Configure your profile](overview.md#getting-started)`

- Een koppeling maken naar een anker in een andere submap voor services:

  `[link text](../directory/article-name.md#anchor-name)`

  `[Configure your profile](../overview.md#configure-your-profile)`

## Koppelen aan afbeeldingen

U kunt het beste afbeeldingen en bestanden opslaan in een map `assets` op hetzelfde niveau als het markeringsbestand dat ernaar is gekoppeld.

- Een artikel verwijst naar een afbeelding in de submap `assets` :

  `![alt text](assets/image-name.png)`

- Een artikel verwijst naar een afbeelding in de submap `assets/no-localize` :

  `![alt text](assets/no-localize/image-name.png)`
