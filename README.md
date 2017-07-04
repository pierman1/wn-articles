# WN-articles

-----

## 1. Waarom Javascript?

Javascript is overal. JavaScript is de enige script-taal op aarde die gebruikt word voor het bouwen van applicaties op elk platform wat je kan verzinnen! Tegenwoordig bevatten huishoudelijke objecten steeds meer JavaScript programmeer werk (Internet of Things). Om nog maar niet te spreken over web-applicaties, desktopapplicaties, TV applicaties, noem maar op, je kan het maken met Javascript.

Op het gebied van de browser, heeft Javascript geen enkele concurrentie. Als je een goeie website wil maken heb je javascript nodig! De software industrie is constant in ontwikkeling. Veel talen die eerst ‘cutting edge’ waren een aantal jaar geleden zijn nu verouderd of overtollig geworden. Er valt een hele boel te kiezen voor developers als je kijkt naar functional, object-georiënteerd scripting talen. Omdat dit allemaal zo snel veranderd is het een hele boel werk om ‘up to date’ te blijven. Je moet op de hoogte blijven van alle nieuwe programmeer talen. Zoals je kan voorstellen is dit een onmogelijke taak. Doordat er steeds nieuwe talen komen betekend het niet dat het programmeer wereldje gigantisch aan het veranderen is keer op keer. Er zijn een aantal talen waar programmeurs voor gekozen hebben om mee door te werken voor lange tijd, en deze zullen daarom ook niet zomaar verdwijnen. Eén van deze talen is Javascript. Deze taal blijft de afgelopen jaren steeds boven aan staan in het programmeer wereldje. Maar waarom?

Javascript werd een hele tijd geleden veel bekritiseerd en niet serieus genomen. Sommigen noemden het geen echte programmeer taal (terwijl het steeds veel gebruikt werd).

**Wat is JavaScript?**

Kortom is Javascript een programmeer taal voor het maken van interactieve websites, web-apps etc. binnen de browser. Hier komen we straks nog op terug.

**Toekomst van Javascript**

In plaats van te vragen: “Wat is de toekomst van JavaScript?” is het goeie om te zeggen juist Javascript is de toekomst!Door Javascript zijn er frameworks beschikbaar gemaakt zoals node.js, jQuery (een libary), JSON(JavaScript Object Notation) MongoDB en ES6 transpilers, dit maakt het een belangrijke taal voor developers en zorgt ervoor dat het zijn relevantie behoudt.
Nu node.js gebruikt kan worden voor het serverside programmeren met JavaScript, is het een taal geworden die inzetbaar is voor alles.

Javascript is niet een taal van komen en gaan. Javascript gaat blijven. Het is onmogelijk dat het opeens overgenomen word door een andere taal op de korte duur. Ook zal Javascript niet de enige taal zijn in de programmeurs wereld, maar dat gaat af en toe wel zo lijken. In de browser zul je er niet aan ontkomen en de browser domineert inmiddels vrijwel alles dat de client doet. En nu gaat ook de serverside er aan geloven door JavaScript te omarmen met tools als Node.js. Kortom, omdat er al zoveel gebaseerd is op Javascript zou men het hoogstwaarschijnlijk altijd blijven gebruiken!

- http://computerworld.nl/development/83981-12-voorspellingen-over-de-toekomst-van-programmeren
- https://dzone.com/articles/why-javascript-and-will

----------

## 2. GitHub & Git-workflow

Github is de grootste internet ‘version control repository’ en Internet hosting service van de wereld. Ook functioneert Github als een soort social media platform voor developers. Github is een systeem wat is gemaakt op Git. Git zelf is een version control system voor developers. Het verschil zit hem in dat Github een ‘web-based graphical interface’ heeft en Git niet, daarnaast is Github ook een community.
Waarom gebruiken we GitHub?

**Code reviewen**

Github zorgt ervoor dat je je code makkelijk kan delen met andere developers. Zo kan je veel van elkaar leren en elkaar helpen bij het verbeteren van code. We kunnen zogenaamde ‘issues’ aanmaken op iemands werk waar de desbetreffende persoon (of team) weer over na kan denken. Zo kunnen we via GitHub elkaar helpen met innovatief en goeie code te schrijven, en zo goeie producten/projecten te maken.

Github is een repository. Dit betekend dat al jou werkt word getoond aan het publiek. Hierdoor is GitHub een community waar iedereen wereldwijd zijn projecten aan elkaar toont. Daarom is het gelijk ook een platform om jezelf te tonen aan het developers wereldje. Net als met google drive kan je samen werken aan de zelfde code door het version management systeem, worden aanpassingen die in het verleden gedaan is niet kwijtgeraakt, na elke iteratie.
Repositiories

Een repository is de omgeving waar je project in zit. Dit bevat alle code, bestanden, afbeeldingen etcetera. Een repository wordt vaak gebruikt voor het samen werken aan een project iedereen kan zijn aanpassingen doen aan de code, mits hij of zij als ‘collaborator’ (medewerker) wordt beschouwd. Zo kan men gezamenlijk werken aan één mappen structuur en de zelfde code.  
Git branches

Er zijn veel bestaande modellen waar mee gewerkt word. Hieronder ga ik een workflow bespreken, er bestaan heel veel verschillende workflows en meningen over hoe dit moet. Dit is hoe ik mijn laatste project gewerkt heb.

De centrale repo bestaat uit twee hoofd branches:

- master
- develop

De master branch is de plek waar de nieuwe versies van je product op komen te staan (production release). Zie de afbeelding hiernaast. Wij beschouwen origin/master als de belangrijkste tak waar de broncode van HEAD altijd in een productie-ready staat is.

De develop branch word gebruikt om op te developpen alle commits worden gemerged met de develop, op het moment als develop op een stabiel punt is gekomen en klaar is om in productie te worden genomen, dan kunnen alle aanpassingen gemerged worden in master.

Zo zorgen we ervoor dat elke keer als er iets gemerged word in master, dat dat een nieuwe productie release is. Omdat we zo zorgen dat master altijd klaar is voor productie dan kunnen we met gebruik van een Git hook script automatisch de coden builden en uitzetten op productie servers elke keer als er wat gecommit word op de master.

Naast de hoofd branches, heeft het development model een heel aantal andere branches om te zorgen dat je goed kwan produceren met meerdere teamgenoten, Het verschil met de hoofd branches is dat deze niet voor altijd bestaan, maar verwijderd worden na verloop van tijd.

**Feature branches**

Feature branches worden gebruikt om nieuwe features in uit te werken. In de branch word de nieuwe feature gebouwd, op het moment als deze goed is kan hij gemerged worden met develop Moet een branch zijn van develop en moet ook gemerged worden met develop.

Een klein voorbeeld van het maken van een feature branch:

Vanuit de develop branch gaan we een nieuwe feature branch aanmaken.

<code>$ git checkout -b feature/my feature<br>
Switched to a new branch “myfeature”</code>

**Pull requests**

Een pull request maak je om anderen te laten weten dat je een repository gepushed hebt. Als een pull request aangevraagd is kunnen andere teamleden deze checken en reviewen en follow-up commits toevoegen. Als de pull request compleet is kan deze gemergd worden met een andere branch of met de master.
Issues

Issues kan je inschieten voor bugs en ontbrekende features. Aan deze issue kan je een label hangen, hoe belangrijk is de issue? Wat voor probleem is het? En wie gaat hem oplossen. Dit is een efficiënte manier om te zorgen dat alle opmerkingen meegenomen worden in het eindproduct.

Er valt veel te lezen over verschillende technieken van het werken met GitHub en Git. Wat in ieder geval zo is, is dat het ons helpt bij het structureren en controleren van ons werk. Zo kunnen we overzichtelijk zien wat we gedaan hebben, enzo hier altijd naar terug grijpen. Ook is het mogelijk om met meerdere mensen aan de zelfde code te werken. Kortom, een handige tool die we allen moeten gebruiken!

## 3. Maintainable CSS

Het schrijven van CSS styles is belangrijk voor de visuele kant van een project/product. Soms word hier weinig tijd aan besteed, met als nadeel dat je langer doet over het onderhoud. Andere steken hier meer tijd in, waardoor je later weer sneller dingen kunt aanpassen.

https://maintainablecss.com/

### Hergebruik

DRY, (don’t repeat yourself, of wel niet in herhaling vallen). De kunst is om zo weinig mogelijk dingen te herhalen. Maar hoe hergebruiken we nou een stijl regel?

### ID’s
Semantisch is het gebruik van ID’s alleen relevant als een element maar één enkele keer voorkomt. Classes gebruiken we als er meerdere instanties voorkomen. ID’s hebben de overhand als het gaat over het overschrijven van een style.

**Voorbeeld:**

#### HTML
`<div id=“module” class=“module-override”>`

### CSS

`#module {
  color: red;
}`

`.module-override {
    color: blue;
}`


In dit geval gaat de module rood blijven, omdat de ID voor de class gaat. Om dit te voorkomen en er toch voor te zorgen dat hij de kleur: blue krijgt, gebruiken we classes:

### HTML
`<div class=“module module-override”>`

### CSS
`#module {
    color: red;
}`

`.module-override {
    color: blue;
}`

Nu heeft het element de kleur: blue.

Als je ID’s gebruikt, gebruik deze dan om de het gedrag van de browser te beïnvloeden. Bijvoorbeeld menu anchors. Maar probeer ze niet te gebruiken voor het stijlen.

### Conventies

Er zijn veel verschillende manier van hoe mensen CSS schrijven, dit noemen we code conventies. Een manier van Maintainable CSS schrijven gaat als volgt:

`.<naam-module>[-<component>][-<state>] {}`

`/* Module container */
.searchResults {}`

`/* Component */
.searchResults-heading {}`

`/* State */
.searchResults-isLoading {}`


Notes:

- component and state are both delimited by a dash
- names are written with lowerCamelCase
- selectors are prefixed with the module name

Niet alle elementen hoeven een class te krijgen. Je zou kunnen schrijven .searchResults p als je dat wil. Soms moet dit ook in het geval van het gebruik van markdown. Maar wees ervan bewust dat je als je een module die een p bevat gebruikt dat de styles inherit zullen zijn en dat de styles hiervan overschreven moeten worden.

Modules
Een goed voorbeeld van css modules staat omschreven op maintainablecss.com
Daar vergelijken ze een  oude met een onafhankelijke ‘unit’. Dus je hebt een woonkamer met daarin verschillende ‘units’ (modules). Bijvoorbeeld de bank, de televisie een stoel een tafel. Deze units bij elkaar vormen een woonkamer. Maar als je een van deze units weg haalt blijven de andere nogsteeds werken. Haal je de tv weg dan kan je nog steeds op de bank zitten.

In een website geld het zelfde, we hebben bijvoorbeeld de header, een formulier een artikel een producten lijst, een navigatie en een artikel. Deze onderdelen kunnen allemaal gezien worden als verschillende modules.

### Wat is een component?

Een module bestaat uit componenten. Zonder componenten is een module incompleet of gebroken. Een module is een herbruikbaar stuk HTML en CSS. Voordat we elementen kunnen bundelen in een module moeten we eerst begrijpen wat het is en welke verschillende use cases er kunnen voordoen.

Bijvoorbeeld bestaat een tafel uit 4 poten en een tafel blad. Als je 1 van deze zaken weg haalt is de functionaliteit ook weg. Een module in het web werkt hetzelfde als 1 van de componenten weg is dan werkt de module niet meer.

```
<div class="basket">
  <h1 class="basket-title">Your basket</h1>
  <div class="basket-item">
      <h3 class="basket-productTitle">Product title</h3>
      <form>
          <input type="submit" class="basket-removeButton" value="Remove">
      </form>
  </div>
</div>```

**And the CSS would be:**

```
.basket {}
.basket-title {}
.basket-item {}
.basket-productTitle {}
.basket-removeButton {}```

### States & modifiers

Vaak komen er veel onderdelen voor in de userinterface, de onderdelen komen vaak overeen. Daarom is het handig om een state mee tegeven. Bijvoorbeeld voor een button, die groen moet zijn als hij actief is en rood als hij niet actief is. Daarom geven we hem de 'state' active mee.

```<div class ="btn btn-active" >```

Btn is is in de geval de main class, vervolgens word er ook de class btn-active aan toegevoegd.

Modifiers gebruiken we om zaken met de zelfde stijlregels, maar met een klein duidelijk verschil net even iets anders te stijlen

### Conclusie

Kortom, er komt veel bij kijken bij het schrijven van goed onderhoudbare CSS. Ook hier is niet één manier die het best is, maar je moet vinden wat er bij je past. De kunst is het op delen van je code in verschillende elementen (modules), en zo veel mogelijk onafhankelijke CSS te schrijven. Hiermee kun je ervoor zorgen dat je geen problemen gaat ervaren bij het herschrijven van je CSS, of als je een stuk weg wilt doen omdat je het niet meer nodig denk te hebben.

Interessant om je in te verdiepen:

- BEM methode

### Bronnen:

- https://medium.com/simple-human/how-to-write-scalable-modular-and-maintainable-css-8411e491939f
- https://maintainablecss.com/

--------

## 4. Minor Everythings Web

De afgelopen maanden heb ik me bezig gehouden met de minor Web Development, onderdeel van de opleiding Communicatie & Multimedia Design op de Hoge school van Amsterdam. Het was een hele intensieve tijd waarin ik een hele boel geleerd heb. Voordat ik met deze minor begon dacht ik dat ik een aardig beeld had van het web, dit was niet het geval. Ik heb een boel nieuwe technieken geleerd, het schrijven van ES6 Javascript, structureren van code en het aanpakken van moeilijke vraagstukken.

We zijn begonnen met het maken van een ‘web application from scratch’. Ook het schrijven van innovatieve CSS code was erg nuttig. Heel veel dingen die je vaak met Javascript oplost kunnen gewoon in  CSS. Na deze introductie werd het steeds interessanter. Van de verschillende browsers en hoe zij omgaan met stukken code, tot ‘Internet of Things’ waar we met gebruik van een NodeMCU data kunnen sturen naar een server. Ook het werken met socket verbindingen en het Real time web gedeelte was erg leerzaam. Al met al veel geleerd maar wat hierna?

Waar zie ik mezelf werken? Wil ik freelancen of wil ik in een groot bedrijf werken? Of wil ik mijn eigen bedrijf beginnen met het maken van applicaties en websites? In de meesterproef heb ik in een team van 5 mensen 5 weken samengewerkt aan 2 verschillende producten. In deze 5 weken hebben we twee goedwerkende producten weten te realiseren. We zijn ook genomineerd om mee te doen aan de Golden Dot awards en uitgenodigd om te spreken op de Young Talent day. Dit heeft dus goed uitgepakt, een klein hecht team wat alles doet. Van design tot de code. Mij lijkt het erg leuk om zo te werken, met alle verschillende beroepsrollen die dicht met elkaar samen werken.

Maar hoe blijf je nou geïnspireerd en gemotiveerd om vernieuwend te blijven? In grote bedrijven heb je altijd de senior developers met veel ervaring. Als je dit zelf het hebt, ga je dan genoeg hebben aan meetups en workshops? De kracht zit het in je constant blijven ontwikkelen. De techniek veranderd, dus jij moet veranderen. Volgend school jaar moet ik nog een afstudeerproject doen, en ik denk deze te gaan doen bij een groot bedrijf om te kijken hoe dat gaat. En hopelijk heb ik hierna een dusdanig beeld van waar ik wil werken en hoe ik wil werken. De minor Everythings Web heeft me veel geleerd maar ook laten zien dat je altijd moet blijven leren, hiermee moet je rekening houden wat betreft het kiezen van een baan.  Gelukkig heb ik nog even!

---------

## 5. Wat is node.js?

JavaScript draait normaal gesproken binnen in je browser. Door middel van de V8 engine van Google kan je computer dit ook draaien. Je kan hierdoor heel veel verschillende dingen doen, die normaal gesproken gedaan werden met PHP, en dergelijken. Welkom bij Node.js server-side Javascript! Iedereen kent Javascript wel, een scripting taal die wordt gebruikt voor het maken van interactieve websites.

Wat deze V8 engine doet is eigenlijk machine-code (Een computerprogrammeertaal die bestaat uit binaire instructies die een computer direct kan reageren.) genereren uit Javascript code waardoor je applicaties kunt bouwen met deze engine. Node.js maakt dus gebruik van de engine en heeft enkele extra’s toegevoegd in C++. Node.js is een back-end variant van de Javsacript zoals wij het kennen, voor de front end van websites.

In vacatures zie je vaak staan dat ze opzoek zijn naar een developer met node.js skills, dit wil vaak zeggen dat je kan werken met het concatenating en bundelen van files, en het aan maken en schrijven van nieuwe tasks server side. Als er gezocht word naar een Node.js engineer gaat het meer over het neerzetten van een webserver.

### Hoe werkt het?

### NPM modules

NPM (Node Package Manager) word automatisch meegeleverd wanneer Node.js is geinstalleerd. NPM bestaat uit een command line client die samen werkt met een extern register. Hiermee kan je JavaScript-modules gebruiken en die beschikbaar zijn op in het register.

Een NPM package is eigenlijk een stuk code wat developers hebben geschreven om een bepaald probleem op te lossen, bijvoorbeeld een script voor het bundelen van verschillende files. Deze module is weer te gebruiken door andere developers. Als je gebruikt maakt van dit soort modules is het makkelijk om via npm te checken of er updates zijn, en kan je gemakkelijk deze updates installeren.

Een package is een directory met daarin één of meer bestanden, hierbij komt ook een “package.json” bestand met daarin de metadata over deze packages. De applicaties, zoals websites, zijn afhankelijk van tientallen van dit soort packages. Deze packages zijn als het ware de bouwblokken waarmee je een grootte, custom oplossing kan bouwen. NPM is dus een manier om code te hergebruiken van andere developers, en zo ook een manier om je code te delen, daarnaast is het makkelijk gemaakt om je versies te beheren van code.

### Event driven programmeren

Dit gaat over de core van node.js. Het gaat niet om het feit dat het server side javascript is. Het is een single threaded server die reageert op callbacks en die nooit de main thread in de weg zit.

Een traditionele Webserver werkt zo:

- De request voor de blog posts komt binnen
- Er word een aanvraag gedaan bij de database om de artikelen op te halen
- De html word opgebouwd met daarin de artikelen
- Dit word naar de client gestuurd.

Wat dit betreft werkt Node.js niet anders. Onder de motorkap zit het verschil. Op het moment als de db wordt aangeroepen om de artikelen te op te halen (laten we zeggen dat dit 100ms duurt). Is de hele tread is aan het wachten op de response van de db. Dit noemen we IO heavy (input/output). Op het moment als de server de HTML aan het bouwen is van de response van de db. Dit is sneller, ongeveer 10ms, maar dit is CPU intensief.

Node.js maakt gebruik van een single, event driven thread. In plaats van dat er elke keer een nieuwe tread word gecreëerd bij elke request, word er gebruik gemaakt van één enkele thread voor elke request. Bijvoorbeeld: Op het moment als je een call maakt naar een database inplaats van dat dit alles blokt totdat het gereturned is, kan je gelijk een nieuwe callback functie aanroepen als de callback klaar is.

Het verschil zit hem dus niet in node.js zelf maar in de code die jij hebt geschreven die anders gebruikt word.

- https://dzone.com/articles/quick-introduction-how-nodejs
- https://nodejs.org/en/

-------

## 6. Webpack vs. Browserify vs. npm-scripts vs. gulp

Webpack en browserify doen ongeveer hetzelfde, het bundelen van modules om zo gebruikt te kunnen worden in een browser. Bijvoorbeeld de Node module is een feature, deze bestaat niet in de browser en ES6 modules zijn nog helemaal niet geïmplementeerd door browsers. Dit is de reden dat we dingen bundelen. Webpack is een bundler terwijl gulp een task runner is. Zo zou je dus verwachten dat deze tools samen gebruikt worden. Inplaats van dat is er een groeiende trend om Webpack te gebruiken in plaats van Gulp.

### Npm scripts
Met NPM scripts heb je direct toegang tot alle NPM-packages, die constant aan het groeien is. Je hebt geen abstractielaag nodig om dit te beheersen dus als je met een groot team werkt en op veel verschillende projecten lijkt npm-scripts een mooie oplossing te zijn. De taken en configuraties zijn makkelijk samen te voegen en uitwisselbaar.

### Webpack
Webpack is meer van een conventioneel instrument. Het heeft een aantal aannames van je workflow en je project setup. Er is veel over Webpack te vinden, en veel configuraties (setups), waar je zo mee aan de slag kant. Het tweaken hiervan is iets minder makkelijk. Verder een prachtige tool voor van alles, denk hierbij aan bundelen, transpillen, linten etc.


### Grunt / Gulp
Deze taskrunners zijn een beetje de midden weg tussen Webpack en npm scripts. De configuratie setup is veel eenvoudiger, en als je al bekend bent met het ene of het andere, is het best makkelijk om een setup aan te passen en snel aan de slag te gaan.

### Overzicht

**Npm scripts**: zeer grote projecten of veel projecten die gemeenschappelijke taken delen. Veel ontwikkelaars dragen bij aan deze projecten met verschillende achtergronden. Bedrijven die werken aan verschillende projecten.

**Webpack**: als je een complexe Front end apllicatie gaat bouwen, met veel niet code gerelateerde zaken. Zoals CSS, afbeeldingen, fonts, SVG's. Dan is Webpack precies wat je nodig hebt.

**Grunt / Gulp**: relatief eenvoudige of minder eenvoudige projecten. Voor teams die een gedeelde kennis hebben voor één van deze taskrunners. Voor unique projecten.

Het is dus niet zo dat het één beter is dan het ander, maar vooral waarom je het gebruikt en of het het waard is om er veel moeite en tijd in te steken. Aan de hand hiervan kan je kiezen voor een taskrunner of een complete setup met Webpack.

- https://medium.com/@justusromijn/my-50-cents-about-the-webpack-vs-gulp-vs-grunt-vs-npm-scripts-discussion-b45c32dbe5f2
- http://blog.andrewray.me/webpack-when-to-use-and-why/
- https://webpack.github.io/
