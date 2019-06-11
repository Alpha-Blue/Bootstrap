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
      <li class="nav-item">
        <a class="nav-link disabled" href="#">Disabled</a>
      </li>
      <li class="nav-item dropdown">
        <a class="nav-link dropdown-toggle" href="#" id="dropdown01" data-toggle="dropdown" aria-haspopup="true" aria-               expanded="false">Dropdown</a>
        <div class="dropdown-menu" aria-labelledby="dropdown01">
          <a class="dropdown-item" href="#">Action</a>
          <a class="dropdown-item" href="#">Another action</a>
          <a class="dropdown-item" href="#">Something else here</a>
        </div>
      </li>
    </ul>
    <form class="form-inline my-2 my-lg-0">
      <input class="form-control mr-sm-2" type="text" placeholder="Search" aria-label="Search">
      <button class="btn btn-outline-success my-2 my-sm-0" type="submit">Search</button>
    </form>
  </div>
</nav>
```

