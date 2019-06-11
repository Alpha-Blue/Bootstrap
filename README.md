# Bootstrap
This is a small tutorial I made on Bootstrap. I had to make this for my final schoolproject. (Hence why it's in dutch)

## Wat is Bootstap?

Bootstrap is een HTML, CSS, Javascript en jQuery library. Met Bootstrap kun je simpel en snel responsive websites maken. Dit door het gebruik van build-in classes. Bootstrap wordt wereldwijd gebruikt voor websites. Het is gratis en binnen 5 minuten te installeren op je website. 

## Hoe installeer je Bootstrap?

Aller eerst maak je natuurlijk een project folder. Dit kan lokaal of via FTP op je website online. Hierin maak je eerst een HTML bestand aan. Daarna een CSS folder, een Javascript folder en een folder voor al je foto's genaamd IMG. In de HTML file zet je om te beginnen het volgende:
```HTML
<!DOCTYPE html>
<html lang="en">
<head>

  <title>Bootstrap Tutorial Sample Page</title>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">

</head>
<body>


</body>
</html>
```
Hierna plak je de volgende link in de __head__ sectie. Zorg ervoor dat wanneer je custom CSS toevoegd, deze __ONDER__ de <link> tag komt van Bootstrap. Bootstap moet altijd als eerste ingeladen worden.
```HTML
<link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.3.1/css/bootstrap.min.css" integrity="sha384-ggOyR0iXCbMQv3Xipma34MD+dH/1fQ784/j6cY/iJTQUOhcWr7x9JvoRxT2MZw1T" crossorigin="anonymous">  
```
Als dit gelukt is, plak je de volgende <script> tags helemaal onderaan de body. Dus net boven de afsluiting van de __body__.
```HTML
<script src="https://code.jquery.com/jquery-3.3.1.slim.min.js" integrity="sha384-q8i/X+965DzO0rT7abK41JStQIAqVgRVzpbzo5smXKp4YfRvH+8abtTE1Pi6jizo" crossorigin="anonymous"></script>
<script src="https://cdnjs.cloudflare.com/ajax/libs/popper.js/1.14.7/umd/popper.min.js" integrity="sha384-UO2eT0CpHqdSJQ6hJty5KVphtPhzWj9WO1clHTMGa3JDZwrnQq4sF86dIHNDz0W1" crossorigin="anonymous"></script>
<script src="https://stackpath.bootstrapcdn.com/bootstrap/4.3.1/js/bootstrap.min.js" integrity="sha384-JjSmVgyd0p3pXB1rRibZUAYoIIy6OrQ6VrjIEaFf/nJGzIxFDsf4x0xIM+B07jRM" crossorigin="anonymous"></script>
```  
Nu heb je je standaard Bootstrap bestanden ingeladen. Hoe maak je er nu het beste gebruik van?
  
## Hoe gebruik je Bootstrap?

Laten we beginnen met de navigatie bar.
Plak het volgende stukje code in de __body__ tag:
```HTML
<nav class="navbar navbar-expand-md navbar-dark fixed-top bg-dark">
  <a class="navbar-brand" href="#">Navbar</a>
  <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarsExampleDefault" aria-controls="navbarsExampleDefault" aria-expanded="false" aria-label="Toggle navigation">
    <span class="navbar-toggler-icon"></span>
  </button>

  <div class="collapse navbar-collapse" id="navbarsExampleDefault">
    <ul class="navbar-nav mr-auto">
      <li class="nav-item active">
        <a class="nav-link" href="#">Home <span class="sr-only">(current)</span></a>
      </li>
      <li class="nav-item">
        <a class="nav-link" href="#">Link</a>
      </li>
    </ul>
  </div>
</nav>
```
Hieronder wat de verschillende classes betekenen:
#### 1. navbar

Dit is de standaard navigatiebar class van Bootstrap. Bij iedere Bootstrap navigatiebar moet je deze gebruiken wil het fatsoenlijk functioneren. 

#### 2. navbar-expand-md

Deze class heeft verschillende groottes. (sm, small. md, medium. lg, large. xl, extra large) Dit bepaald wanneer het responsive menu tevoorschijn komt. Dus wanneer het "hamburger" menu tevoorschijn komt zoals dat genoemd wordt.

#### 3. navbar-dark

Dit is de kleur van de teskt in het menu (de nav-links). Je hebt ook bijvoorbeeld navbar-light voor een witte kleur.

#### 4. fixed-top

Deze zorgt er simpelweg voor dat de navbar fixed wordt. Dus dat als je naar beneden scrolled op de pagina, de navbar meegaat. Items met position fixed, zitten dus vast aan een bepaalde positie zelfs al wordt er gescrolled.

#### 5. bg-dark

Deze zorgt ervoor dat de navbar een donkere achtergrondkleur krijgt. Dit kan bijvoorbeeld ook zijn bg-light. Dan krijgt de navbar een lichte achtergrond.

#### 6. navbar-brand

Dit is simpelweg je logo in het begin van je navbar.

#### 7. navbar-toggler

Dit is de knop in het responsive menu. (het hamburger menu waar we het eerder over hadden) Door deze class weet bootstrap dat dat de knop is.

#### 8. navbar-toggler-icon

Dit is het icon wat je gebruikt. (bijvoorbeeld dus de hamburger.)

#### 9. navbar-collapse, collapse

Deze twee zorgen er simpelweg voor dat er een menu opent zodra je op de __navbar-toggler-icon__ klikt, en dat zodra je nog een keer klikt hij ook weer sluit.

#### 10. navbar-nav

Dit is gewoon een standaard class voor de UL van een menu.

#### 11. mr-auto 

Deze zorgt ervoor dat alle menu items aan de rechterkant van het menu uitlijnen.

#### 12. nav-item

Dit is een class die je aan iedere li tag geeft in je code. Zo weet bootstrap dat het een navigatie item is.

#### 13. Active

Deze zet je op het menu item wat op dat moment de juiste pagina is. Zit je bijvoorbeeld op de over ons pagina, dan zet je de class active ook op het menu item over ons.

#### 14. nav-link

Dit is de a tag in de li. Dit zorgt ervoor dat het ook echt een link is. Deze heeft natuurlijk ook een Bootstrap class nodig.

Dit is een van de vele voorbeelden waarbij Bootstrap gebruikt wordt. In het algemeen is het gewoon super handig bij het maken van een responsive website. Ik denk dat als iemand de documentatie van Bootstrap zelf erbij pakt, je al een heel eind komt. Daar staat in detail uitgelegd wat iedere class doet en hoe je het kunt gebruiken met voorbeelden. Toen ik net begon met Bootstrap, heb ik ook de documantatie gebruikt. Heb hierdoor nooit vast gezeten met Bootstrap.

[Vind de documentatie hier](https://getbootstrap.com/docs/4.3/getting-started/introduction/)


