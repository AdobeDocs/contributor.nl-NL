---
lastModified: 2018-06-28T00:00:00Z
title: Hoe te om Markdown voor het schrijven van documentatie te gebruiken
seo-title: Hoe te om Markdown voor het schrijven van Adobe documentatie te gebruiken
description: dit artikel bevat de grondbeginselen en referentiegegevens van de opmaaktaal die wordt gebruikt voor het schrijven van artikelen .
seo-description: dit artikel bevat de grondbeginselen en referentiegegevens van de opmaaktaal die wordt gebruikt voor het schrijven van artikelen voor Adobe - documentatie .
translation-type: tm+mt
source-git-commit: 27ba164070996d192c84493d83232484d2badb28
workflow-type: tm+mt
source-wordcount: '1329'
ht-degree: 1%

---


# Hoe te om Markdown voor het schrijven van technische documentatie te gebruiken

De artikelen in de technische documentatie van Adobe zijn geschreven in een lichte opmaaktaal die [Markdown](https://daringfireball.net/projects/markdown/)wordt genoemd, zowel gemakkelijk te lezen als gemakkelijk te leren.

Aangezien wij de inhoud van Docs van Adobe in GitHub opslaan, kan het een versie van Markering gebruiken genoemd [GitHub Gearomatiseerde Prijsverhoging (GFM)](https://help.github.com/categories/writing-on-github/), die extra functionaliteit voor gemeenschappelijke het formatteren behoeften verstrekt. Bovendien heeft Adobe Markdown op een aantal manieren uitgebreid om bepaalde aan Help gerelateerde functies zoals notities, tips en ingesloten video&#39;s te ondersteunen.

## Grondbeginselen van markeringen

### Koppen

Als u een kop wilt maken, gebruikt u een hash-teken (#) aan het begin van een regel:

```
   # This is level 1 (article title)
   ## This is level 2
   ### This is level 3
   #### This is level 4
   ##### This is level 5
```

### Standaardtekst

Een alinea vereist geen speciale syntaxis in Markdown.

Als u tekst wilt opmaken als **vet**, plaatst u de tekst in twee sterretjes. Als u tekst wilt opmaken als *cursief*, plaatst u de tekst in één sterretje:

```markdown
    This text is **bold**.
    This text is *italic*.
    This text is both ***bold and italic***.
```

<!--
To format superscript (H<sub>2</sub>O) and subscript (e=mc<sup>2</sup>) text:

```markdown
This is subscript H<sub>2</sub>O and superscript e=mc<sup>2</sup>.
```
-->

Als u opmaaktekens voor opmaak wilt negeren, gebruikt u \ vóór het teken:

```markdown
This is not \*italicized\* type.
```

### Genummerde lijsten en lijsten met opsommingstekens

Als u genummerde lijsten wilt maken, begint u met een regel met `1.` of `1)`, maar gebruikt u niet beide indelingen in dezelfde lijst. U hoeft de getallen niet op te geven. GitHub doet dat voor jou.

```markdown
1. This is step 1.
1. This is the next step.
1. This is yet another step, the third.
```

Weergegeven:

1. Dit is stap 1.
1. Dit is de volgende stap.
1. Dit is nog een stap, de derde.

<!-- markdownlint-disable MD037 -->
Als u opsommingstekens wilt maken, begint u met een regel met \* of - of +, maar combineert u de indelingen niet in dezelfde lijst. (Gebruik in hetzelfde document geen opsommingstekens, zoals \* en \+.)
<!-- markdownlint-disable MD037 -->

```markdown
* First item in an unordered list.
* Another item.
* Here we go again.
```

Weergegeven:

* Eerste item in een ongeordende lijst.
* Nog een item.
* Hier gaan we weer.

U kunt ook lijsten insluiten in lijsten en inhoud toevoegen tussen lijstitems.

```markdown
1. Set up your table and code blocks.
1. Perform this step.

   ![screen](assets/no-localize/adobe_standard_logo.png)
1. Make sure that your table looks like this: 

   | Hello | World |
   |---|---|
   | How | are you? |  
1. This is the fourth step.

   >[!NOTE]
   >
   >This is note text.

1. Do another step.
```

Weergegeven:

1. Stel uw tabel- en codeblokken in.
1. Voer deze stap uit.

   ![scherm](assets/no-localize/adobe_standard_logo.png)
1. Zorg ervoor dat uw tabel er zo uitziet:

   | Hallo | Wereld |
   |---|---|
   | Hoe | Ben je dat? |
1. Dit is de vierde stap.

   >[!NOTE]
   >
   >Dit is notitietekst.

1. Doe nog een stap.

### Tabellen

Tabellen maken geen deel uit van de kernspecificatie Markering, maar Adobe ondersteunt ze tot op zekere hoogte. Markering ondersteunt geen lijsten met meerdere regels in cellen. U kunt het beste voorkomen dat meerdere regels in tabellen worden gebruikt. U kunt tabellen maken door het verticale streepje (|) te gebruiken om kolommen en rijen te definiëren. Bij deze optie wordt de kolomkop gemaakt, bij elke kolom worden de leidingen van elkaar gescheiden. Neem een lege regel voor de tabel op, zodat deze correct wordt weergegeven.

```markdown
| Header | Another header | Yet another header |
|--- |--- |--- |
| row 1 | column 2 | column 3 |
| row 2 | row 2 column 2 | row 2 column 3 |
```

Weergegeven:

| Koptekst | Een andere header | Nog een kop |
|--- |--- |--- |
| rij 1 | kolom 2 | kolom 3 |
| rij 2 | rij 2 kolom 2 | rij 2 kolom 3 |

Eenvoudige tabellen werken naar behoren in Markering. Tabellen die meerdere alinea&#39;s of lijsten in een cel bevatten, zijn echter moeilijk te gebruiken. Voor dergelijke inhoud raden we u aan een andere indeling te gebruiken, zoals koppen en tekst.

Zie voor meer informatie over het maken van tabellen:

* GitHub [organiseert informatie met lijsten](https://help.github.com/articles/organizing-information-with-tables/)
* De webapp [Markdown Tables Generator](https://www.tablesgenerator.com/markdown_tables)
* [HTML-tabellen converteren naar Markering](https://jmalarcon.github.io/markdowntables/)

### Koppelingen

De syntaxis van de Prijsondering voor een gealigneerde verbinding bestaat uit het `[link text]` gedeelte, dat de tekst is die hyperlinked zal zijn, door het `(file-name.md)` gedeelte wordt gevolgd, dat URL of dossiernaam is die met wordt verbonden:

`[link text](file-name.md)`

```markdown
[Adobe](https://www.adobe.com)
```

Weergegeven:

[Adobe](https://www.adobe.com)

Gebruik relatieve koppelingen voor koppelingen naar artikelen (kruisverwijzingen) in de opslagplaats. U kunt alle relatieve koppelingsoperanden gebruiken, zoals ./ (huidige map), ../ (één map terug) en ../../ (twee directory&#39;s terug).

```markdown
See [Overview example article](../../overview.md)
```

Raadpleeg het artikel [Koppelingen](linking.md) in deze handleiding voor koppelingen naar syntaxis voor meer informatie over koppelingen.

### Afbeeldingen

```markdown
![Adobe Logo](assets/no-localize/adobe_standard_logo.png "Hover text")
```

Weergegeven:

![Adobe-](assets/no-localize/adobe_standard_logo.png "LogoHover-tekst")

### Codeblokken

Markering ondersteunt de plaatsing van codeblokken, zowel inline in een zin als als een apart &#39;afgezonderd&#39; blok tussen zinnen. Zie de native ondersteuning van [Markdown voor codeblokken voor meer informatie](https://daringfireball.net/projects/markdown/syntax#precode)

Gebruik backtikken ( \`) om inline-codestijlen in een alinea te maken. Als u een specifiek codeblok met meerdere regels wilt maken, voegt u drie backtikken (\`\&#39;\&#39;) toe vóór en na het codeblok (een &quot;afgezonderd codeblok&quot; in Markdown genoemd en alleen een &quot;codeblok&quot;-component in AEM). Voor afgezonderde codeblokken voegt u de codetaal toe na de eerste set backtikken, zodat de syntaxis van de code correct wordt gemarkeerd met Markering. Voorbeeld: \`\`\\javascript

Voorbeelden:

```markdown
This is `inline code` within a paragraph of text.
```

Weergegeven:

Dit bevindt zich `inline code` in een alinea met tekst.

Dit is een afgezonderd codeblok:

```markdown
\```javascript
function test() {
 console.log("notice the blank line before this function?");
\```
```

Weergegeven:

```javascript
function test() {
 console.log("notice the blank line before this function?");
```

### Definitielijsten

Een definitielijst is een extensie Markdown die de component Definitielijst in AEM ondersteunt. Een definitielijst bestaat uit een term en de bijbehorende definitie.

<!--

```markdown
Frog
: An amphibious green creature. Likes flies.

Cat
: A less amphibious creature than frogs.
```

Displayed:

Frog
: An amphibious green creature. Likes flies.

Cat
: A less amphibious creature than frogs.
--->

#### Opmerkingen en opmerkingen

Opmerkingen (opmerkingen) worden niet weergegeven in de voor het publiek toegankelijke Help-artikelen. Opmerkingen worden echter wel weergegeven in de openbare opmaakbestanden die gebruikers kunnen zien en bewerken.

## Extensies voor aangepaste markeringen

Adobe-artikelen gebruiken standaardmarkeringen voor de meeste artikelopmaak, zoals alinea&#39;s, koppelingen, lijsten en koppen. Voor een rijkere opmaak kunnen artikelen uitgebreide opmaakfuncties gebruiken, zoals:

* Notitieblokken
* Ingesloten video&#39;s
* Niet lokaliseren
* Componenteigenschappen, zoals een andere kop-id toewijzen aan een kop

Gebruik het blokcitaat van de Prijsverhoging ( >) aan het begin van elke lijn om een uitgebreide component, zoals een nota samen te voegen. Als u subcomponenten binnen componenten moet gebruiken, voeg een extra niveau van blokcitaten (> >) voor die subcomponentensectie toe. Een NOTITIE in een DONOTLOCALIZE-sectie moet bijvoorbeeld beginnen met > >.

Enkele gebruikelijke opmaakelementen, zoals koppen en codeblokken, bevatten uitgebreide eigenschappen. Als u de standaardeigenschappen moet wijzigen, voegt u de parameters tussen de franse accolades /{ /} toe na de component. Uitgebreide eigenschappen worden in context beschreven.

### Notitieblokken

U kunt uit vier typen notitieblokken kiezen om de aandacht op specifieke inhoud te vestigen:

* `[!NOTE]`
* `[!CAUTION]`
* `[!TIP]`
* `[!IMPORTANT]`

Over het algemeen moeten notenblokken spaarzaam worden gebruikt omdat ze verstorend kunnen zijn. Hoewel ze ook ondersteuning bieden voor codeblokken, afbeeldingen, lijsten en koppelingen, kunt u proberen om de notitieblokken eenvoudig en eenvoudig te houden.


```markdown
>[!NOTE]
>
>This is a standard NOTE block.
```

Weergegeven:

>[!NOTE]
>
>Dit is een standaardblok van de NOOT.

```markdown
>[!TIP]
>
>This is a standard tip.
```

Weergegeven:

>[!TIP]
>
>Dit is een standaardtip.

### Video&#39;s

Ingesloten video&#39;s worden niet native gerenderd in Markdown, maar u kunt deze extensie Markdown gebruiken.

```markdown
>[!VIDEO](https://www.youtube.com/watch?v=A0EcD2AxvJE)
```

Weergegeven:

>[!VIDEO](https://www.youtube.com/watch?v=A0EcD2AxvJE)

### Meer als dit

De component &quot;Meer als dit&quot; in AEM wordt aan het einde van een artikel weergegeven. Gerelateerde koppelingen worden weergegeven. Als het artikel wordt gerenderd, kan het dezelfde opmaak krijgen als niveau 2-koppen (##) zonder dat het aan de miniinhoudsopgave wordt toegevoegd.

```markdown
>[!MORELIKETHIS]
>* [Article 1](https://helpx.adobe.com/support/analytics.html)
>* [Article 2](https://helpx.adobe.com/support/audience-manager.html)
```

Weergegeven:

>[!MORELIKETHIS]
>* [Artikel 1](https://helpx.adobe.com/nl/support/analytics.html)
>* [Artikel 2](https://helpx.adobe.com/nl/support/audience-manager.html)


### DNL - Niet lokaliseren - en UICONTROL

In sommige gevallen moeten bepaalde delen van de inhoud in een artikel alleen in het Engels worden gemarkeerd.
Woorden, woordgroepen en andere elementen moeten in onze vertaalsystemen worden gedeclareerd en zorgen voor de mogelijkheid om een gecontroleerde lexicon te beheren.

Voor woorden of uitdrukkingen die niet zouden moeten worden gelokaliseerd, gebruik de `[!DNL]` uitbreiding om het woord of de sectie te verpakken.

Voor elementen in de gebruikersinterface en menu&#39;s van een oplossing, gebruiken wij de `` uitbreiding.

**Voorbeeld:**

In [!DNL Adobe Target] kunt u uw tests direct op een [!DNL Target]toegelaten pagina tot stand brengen.

**Bron:**

```markdown
In [!DNL Adobe Target] you can create your tests directly on a [!DNL Target]-enabled page.
```

**Voorbeeld**

Gebruik de [!UICONTROL Visual Experience Composer] insteekmodule [!DNL Target] om de test rechtstreeks op een pagina te maken.

**Bron:**

```markdown
Use the [!UICONTROL Visual Experience Composer] in [!DNL Target] to create your test directly on a page.
```

## Gotchas en probleemoplossing

### Alt-tekst

Alt-tekst met onderstrepingstekens wordt niet correct gerenderd. In plaats van dit bijvoorbeeld te gebruiken:

```markdown
![Settings_Step_2](/assets/settings_step_2.png)
```

U kunt het beste afbreekstreepjes (-) gebruiken in plaats van onderstrepingstekens (_) in bestandsnamen.

```markdown
![Settings-Step-2](/assets/settings-step-2.png)
```

### Apostroffen en aanhalingstekens

Als u tekst kopieert naar een Markeringen-editor, kan de tekst &#39;slimme&#39; (gekrulde) apostroffen of aanhalingstekens bevatten. Deze moeten worden gecodeerd of gewijzigd in standaardapostroffen of aanhalingstekens. Anders krijgt u oneven tekens zoals deze wanneer het bestand wordt gepubliceerd: Itâ€™s

Hier volgen de coderingen voor de &quot;slimme&quot; versies van deze leestekens:

* Aanhalingsteken links (openen): `&#8220;`
* Rechteraanhalingsteken (sluiten): `&#8221;`
* Recht (sluiten) enkel aanhalingsteken of apostrof: `&#8217;`
* Eén enkel aanhalingsteken links (openen) (zelden gebruikt): `&#8216;`

### Hoekhaken

Als u punthaken in tekst (geen code) in uw dossier-bijvoorbeeld gebruikt om placeholder te wijzen-moet u de punthaken manueel coderen. Anders denkt Markdown dat het een HTML-tag moet zijn.

Coderen `<script name>` als `&lt;script name&gt;`

### Ampersanden in titels

Ampersands (&amp;) zijn niet toegestaan in titels. Gebruik in plaats hiervan &#39;en&#39; of gebruik de `&amp;` codering.

## Zie ook

### Markeringsmiddelen

* [Inleiding tot afwaardering](https://daringfireball.net/projects/markdown/syntax)
* [De Grondbeginselen van de Verkoop van GitHub](https://help.github.com/articles/markdown-basics/)
