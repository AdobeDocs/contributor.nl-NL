---
title: Markering gebruiken voor het schrijven van documentatie
description: Leer de grondbeginselen van Markdown authoring. Zoek naar informatie voor de taal Markering die wordt gebruikt voor het schrijven van artikelen.
exl-id: 3e5726e2-139e-4e44-ae5b-8a3ae4782faf
source-git-commit: fff920c9e98ca821a4180157174c2a2ee1b84cb8
workflow-type: tm+mt
source-wordcount: '1340'
ht-degree: 0%

---

# Hoe wordt Markdown gebruikt voor het schrijven van technische documentatie

De technische documentatieartikelen van de Adobe worden geschreven in een lichtgewichtprijsverhogingstaal genoemd [ Markdown ](https://daringfireball.net/projects/markdown/), die zowel gemakkelijk te lezen en gemakkelijk is te leren.

Aangezien wij de inhoud van Docs van de Adobe in GitHub opslaan, kan het een versie van Markering gebruiken genoemd [ GitHub Gearomatiseerde Prijsverhoging (GFM) ](https://help.github.com/categories/writing-on-github/), die extra functionaliteit voor gemeenschappelijke het formatteren behoeften verstrekt. Bovendien heeft de Adobe Markdown op een aantal manieren uitgebreid om bepaalde aan Help gerelateerde functies zoals notities, tips en ingesloten video&#39;s te ondersteunen.

## Grondbeginselen van markeringen

In de volgende secties worden de grondbeginselen van het ontwerpen in Markdown beschreven.

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

Om tekst als **vette letters** te formatteren, sluit u het in twee asterisks in. Om tekst als *cursief* te formatteren, sluit u het in één enkele asterisk in:

```markdown
   This text is **bold**.
   This text is *italic*.
   This text is both ***bold and italic***.
```

Als u opmaaktekens voor opmaak wilt negeren, gebruikt u \ vóór het teken:

```markdown
This is not \*italicized\* type.
```

### Genummerde lijsten en lijsten met opsommingstekens

Als u genummerde lijsten wilt maken, begint u met een regel met `1.` of `1)` , maar gebruikt u niet beide indelingen in dezelfde lijst. U hoeft de getallen niet op te geven. GitHub doet dat voor jou.

```markdown
1. This is step 1.
1. This is the next step.
1. This is yet another step, the third.
```

Weergegeven:

1. Dit is stap 1.
1. Dit is de volgende stap.
1. Dit is nog een stap, de derde.

Als u opsommingstekens wilt maken, begint u met een regel met \* of - of +, maar combineert u de indelingen niet in dezelfde lijst. (Gebruik in hetzelfde document geen opsommingstekens, zoals \* en \+.)

```markdown
* First item in an unordered list.
* Another item.
* Here we go again.
```

Weergegeven:

* Eerste item in een ongeordende lijst.
* Nog een item.
* Hier gaan we  opnieuw.

U kunt lijsten binnen lijsten ook insluiten en inhoud tussen lijstpunten toevoegen.

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

   ![ scherm ](assets/no-localize/adobe_standard_logo.png)

1. Zorg ervoor dat uw tabel er zo uitziet:

   | Hallo | Wereld |
   |---|---|
   | Hoe | Ben je dat? |

1. Dit is de vierde stap.

   >[!NOTE]
   >
   >Dit is een opmerking  tekst.

1. Doe nog een stap.

### Tabellen

Tabellen maken geen deel uit van de kernspecificatie Markering, maar de Adobe ondersteunt ze in zekere mate. Markering ondersteunt geen lijsten met meerdere regels in cellen. U kunt het beste voorkomen dat meerdere regels in tabellen worden gebruikt. U kunt tabellen maken door het verticale streepje (|) te gebruiken om kolommen en rijen te definiëren. Bij deze optie wordt de kolomkop gemaakt, bij elke kolom worden de leidingen van elkaar gescheiden. Neem een lege regel voor de tabel op, zodat deze correct wordt weergegeven.

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

* GitHub [ organiseert informatie met lijsten ](https://help.github.com/articles/organizing-information-with-tables/)
* De [&#128279;](https://www.tablesgenerator.com/markdown_tables) Web-app van de Generator van de Lijsten van de Vermindering 
* [ zet de lijsten van HTML in Markering ](https://jmalarcon.github.io/markdowntables/) om

### Koppelingen

De syntaxis voor de markering van een inline-koppeling bestaat uit het `[link text]` -gedeelte. Dit is de tekst die aan hyperlinks wordt gekoppeld, gevolgd door het `(file-name.md)` -gedeelte. Dit is de URL of de bestandsnaam waarnaar wordt gekoppeld:

`[link text](file-name.md)`

```markdown
[Adobe](https://www.adobe.com)
```

Weergegeven:

[ Adobe ](https://www.adobe.com)

Gebruik relatieve koppelingen voor koppelingen naar artikelen (kruisverwijzingen) in de opslagplaats. U kunt alle relatieve koppelingsoperanden gebruiken, zoals ./ (huidige map), ../ (één map terug) en ../../ (twee mappen terug).

```markdown
See [Overview example article](../../overview.md)
```

Voor meer informatie bij het verbinden, zie het [ 1&rbrace; artikel van Verbindingen &lbrace;van deze gids voor het verbinden van syntaxis.](linking.md)

### Afbeeldingen

```markdown
![Adobe Logo](assets/no-localize/adobe_standard_logo.png "Hover text")
```

Weergegeven:

![ het Logo van de Adobe ](assets/no-localize/adobe_standard_logo.png " Hover tekst ")

### Codeblokken

Markering ondersteunt de plaatsing van codeblokken, zowel inline in een zin als als een apart &#39;afgezonderd&#39; blok tussen zinnen. Voor details, zie {de inheemse steun van 0} Markering voor codeblokken [&#128279;](https://daringfireball.net/projects/markdown/syntax#precode)

Gebruik backtikken (`` ` ``) om inline-codestijlen in een alinea te maken. Om een specifiek multi-line codeblok tot stand te brengen, voeg drie achtertikken (` ` `` `) vóór en na het codeblok (genoemd een &quot;omheind codeblok&quot;in Markdown en enkel een &quot;codeblok&quot;component in AEM) toe. Voor afgezonderde codeblokken voegt u de codetaal toe na de eerste set backtikken, zodat de syntaxis van de code correct wordt gemarkeerd met Markering. Voorbeeld: ` `` `javascript`

Voorbeelden:

```markdown
This is `inline code` within a paragraph of text.
```

Weergegeven:

Dit is `inline code` in een alinea met tekst.

Dit is een afgezonderd codeblok:

```javascript
function test() {
 console.log("notice the blank line before this function?");
```

## Extensies voor aangepaste markeringen

Artikelen in Adoben maken gebruik van de standaardopmaak voor de meeste artikelen, zoals alinea&#39;s, koppelingen, lijsten en koppen. Voor een rijkere opmaak kunnen artikelen uitgebreide opmaakfuncties gebruiken, zoals:

* Notitieblokken
* Ingesloten video&#39;s
* Tags voor omzetting
* Componenteigenschappen, zoals een andere kop-id toewijzen aan een kop en een afbeeldingsgrootte opgeven

Gebruik het blokcitaat van de Prijsverhoging ( >) aan het begin van elke lijn om een uitgebreide component, zoals een nota samen te voegen.

Enkele gebruikelijke opmaakelementen, zoals koppen en codeblokken, bevatten uitgebreide eigenschappen. Als u de standaardeigenschappen moet wijzigen, voegt u de parameters tussen de franse accolades /{ /} toe na de component. Uitgebreide eigenschappen worden in context beschreven.

### Notitieblokken

U kunt uit deze typen notitieblokken kiezen om de aandacht op specifieke inhoud te vestigen:

* `[!NOTE]`
* `[!TIP]`
* `[!IMPORTANT]`
* `[!CAUTION]`
* `[!WARNING]`
* `[ !ADMINISTRATION]`
* `[!AVAILABILITY]`
* `[!PREREQUISITES]`
* `[!ERROR]`
* `[ !ADMINISTRATION]`
* `[!INFO]`
* `[!SUCCESS]`

Over het algemeen moeten notenblokken spaarzaam worden gebruikt omdat ze verstorend kunnen zijn. Hoewel ze ook ondersteuning bieden voor codeblokken, afbeeldingen, lijsten en koppelingen, kunt u proberen om de notitieblokken eenvoudig en eenvoudig te houden.


```markdown
>[!NOTE]
>
>This is a standard NOTE block.
```

```markdown
>[!TIP]
>
>This is a standard TIP.
```

```markdown
>[!IMPORTANT]
>
>This is an IMPORTANT note.
```

Weergegeven:

![ Gegenereerde nota&#39;s ](assets/notes-rendered.png)

### Video&#39;s

Ingesloten video&#39;s worden niet native gerenderd in Markdown, maar u kunt deze extensie Markdown gebruiken.

```markdown
>[!VIDEO](https://video.tv.adobe.com/v/29770/?quality=12)
```

Weergegeven:

>[!VIDEO](https://video.tv.adobe.com/v/29770/?quality=12)

### Meer als dit

De component &quot;Meer als dit&quot; in AEM wordt aan het einde van een artikel weergegeven. Gerelateerde koppelingen worden weergegeven. Als het artikel wordt gerenderd, kan het dezelfde opmaak krijgen als niveau 2-koppen (##) zonder dat het aan de miniinhoudsopgave wordt toegevoegd.

![ morelikethis syntax ](assets/more-like-this-syntax.png)

Weergegeven:

>[!MORELIKETHIS]
>
>* [ Artikel  1 ](https://helpx.adobe.com/nl/support/analytics.html)
>* [ Artikel  2 ](https://helpx.adobe.com/nl/support/audience-manager.html)

### UICONTROL en DNL

Al onze Help-inhoud voor Markdown is gelokaliseerd met behulp van in eerste instantie automatische vertaling. Als de hulp nooit is gelokaliseerd, dan houden wij de machinevertaling. Als de Help-inhoud echter in het verleden is gelokaliseerd, fungeert de door de computer vertaalde inhoud als plaatsaanduiding tijdens het vertalen van de inhoud.

**&grave;&grave;**

Tijdens het vertalen van computers worden items die zijn getagd met &grave;&grave; gecontroleerd op basis van een lokalisatiedatabase voor de juiste vertaling. Als de UI niet gelokaliseerd is, zal deze markering het systeem toestaan om de verwijzing UI in het Engels voor die bepaalde taal (d.w.z. te verlaten. Analytische verwijzingen in het Italiaans).

**broninhoud van het Voorbeeld:**

![ tekst van de steekproefcontrole ](assets/sample-uicontrol.png)

<!--
**Source:**

```markdown
1. Go to the **[!UICONTROL Run Process]** screen.
1. Choose **[!UICONTROL File] > [!UICONTROL Print] > [!UICONTROL Print All]** to print all the files on your server.
1. The [!UICONTROL Processing Rules] dialog box appears.
```

>[!NOTE]
>
>Of the two tagging options, this is the most crucial to deliver high quality and is mandatory.
-->

**``**

In de regel gebruiken we een lijst &#39;Niet vertalen&#39; om de machinevertalingsprogramma&#39;s te vertellen wat ze in het Engels moeten houden. De meest voorkomende items zijn de lange namen van oplossingen, zoals &quot;Adobe Analytics&quot;, &quot;Adobe Campaign&quot; en &quot;Adobe Target&quot;. Er kunnen zich echter gevallen voordoen waarin de motor gedwongen moet worden het Engels te gebruiken, omdat de term in kwestie op een specifieke of algemene manier kan worden gebruikt. Dit zou het meest voor de hand liggende geval zijn: korte namen voor oplossingen zoals &quot;Analytics&quot;, &quot;Campaign&quot;, &quot;Target&quot; enz. Het zou voor een machine moeilijk zijn om te begrijpen dat dit oplossingsnamen en geen algemene termen zijn. De tag kan ook worden gebruikt voor namen/functies van derden die altijd in het Engels overblijven of voor kortere tekstgedeelten zoals woordgroepen of zinnen die in het Engels moeten blijven staan.

**broninhoud van het Voorbeeld:**

![ steekproef dnl- tekst ](assets/sample-dnl.png)

<!--
**Source:**

```markdown
* With [!DNL Target], you can create A/B tests to find the optimal 
* Adobe Analytics is a powerful solution to collect analytics on your site. [!DNL Analytics] can also help you with reporting to easily digest that data.
```
-->

## Gotchas en probleemoplossing

### Alt-tekst

Alt-tekst met onderstrepingstekens wordt niet correct gerenderd. In plaats van dit bijvoorbeeld te gebruiken:

```markdown
![Settings_Step_2](/assets/settings_step_2.png)
```

We raden u aan afbreekstreepjes (-) te gebruiken in plaats van onderstrepingstekens (_) in bestandsnamen.

```markdown
![Settings-Step-2](/assets/settings-step-2.png)
```

### Apostroffen en aanhalingstekens

Als u tekst kopieert naar een Markeringen-editor, kan de tekst &#39;slimme&#39; (gekrulde) apostroffen of aanhalingstekens bevatten. Deze moeten worden gecodeerd of gewijzigd in standaardapostroffen of aanhalingstekens. Anders krijgt u oneven tekens zoals deze wanneer het bestand wordt gepubliceerd: Itâ€™s

Hier volgen de coderingen voor de &quot;slimme&quot; versies van deze leestekens:

* Linkeraanhalingsteken (openen): `&#8220;`
* Rechteraanhalingsteken (sluiten): `&#8221;`
* Rechteraanhalingsteken (sluiten) of apostrof: `&#8217;`
* Eén enkel aanhalingsteken links (openen) (zelden gebruikt): `&#8216;`

### Hoekhaken

Als u punthaken in tekst (geen code) in uw dossier-bijvoorbeeld gebruikt om placeholder te wijzen-moet u de punthaken manueel coderen. Anders denkt Markdown dat ze een HTML-tag moeten zijn.

Codeer `<script name>` bijvoorbeeld als `&lt;script name&gt;`

### Ampersanden in titels

Ampersands (&amp;) zijn niet toegestaan in titels. Gebruik in plaats hiervan &#39;en&#39; of gebruik de `&amp;` -codering.

## Zie ook

### Markeringsmiddelen

* [ Inleiding aan Markering ](https://daringfireball.net/projects/markdown/syntax)
* [ Grondbeginselen van de Prijsverlaging van GitHub ](https://help.github.com/articles/markdown-basics/)
