#Angular Material

####FLEX
Agregue el flex atributo al elemento secundario de un diseño, y se doblará (estiramiento) para rellenar el área disponible.
```html
<div layout="row">
  <div flex>
    [flex]
  </div>
  <div flex>
    [flex]
  </div>
  <div flex hide-sm>
    [flex]
  </div>
</div>
```

####FLEX = 'valor'
El atributo flex puede tener un valor entero de 0-100. El elemento se extenderá al porcentaje de espacio disponible que coincida con el valor. El valor de flex está limitado a 33, 66, y múltiplos de cinco. Por ejemplo: flex = "5", flex = "20", flex = "33" , flex = "50", flex = "66", flex = "75", .... 
```html
<div layout="row" layout-wrap>
  <div flex="33">
    [flex="33"]
  </div>
  <div flex="55">
    [flex="55"]
  </div>
  <div flex>
    [flex]
  </div>
  <div flex="66">
    [flex="66"]
  </div>
  <div flex>
    [flex]
  </div>
</div>
```

####FLEX OFFSET (margin)
#
**offset**	Elemento Conjuntos compensado.
#
**offset-sm**	Elemento Conjuntos compensado en dispositivos menos de 600px de ancho.
#
**offset-gt-sm**	Compensado en los dispositivos de más de 600px de ancho elemento Sets.
#
**offset-md**	Establece compensado en dispositivos entre 600px y 960px de ancho elemento.
#
**offset-gt-md**	Compensado en los dispositivos de más de 960px de ancho elemento Sets.
#
**offset-lg**	Establece compensado en dispositivos entre 960px y 1200px de ancho elemento.
#
**offset-gt-lg**	Compensado en los dispositivos de más de 1200px de ancho elemento Sets.
```html
<div layout="row">
  <div flex offset="33">
    [flex offset="33"]
  </div>
  <div flex>
    [flex]
  </div>
</div>
```
#
#


####FLEX ORDER
**flex-order**	Establece orden de los elementos.
#
**flex-order-sm**	Establece orden de los elementos en los dispositivos menos de 600px de ancho.
#
**flex-order-gt-sm**	Establece orden de los elementos en los dispositivos de más de 600px de ancho.
#
**flex-order-md**	Establece orden de los elementos en los dispositivos entre 600px y 960px de ancho.
#
**flex-order-gt-md**	Establece orden de los elementos en los dispositivos de más de 960px de ancho.
#
**flex-order-lg**	Establece orden de los elementos en los dispositivos entre 960px y 1200px de ancho.
#
**flex-order-gt-lg**	Establece orden de los elementos en los dispositivos de más de 1200px de ancho.
```html
<div layout="row" layout-margin>
  <div flex flex-order="3">
    [flex-order="3"]
  </div>
  <div flex flex-order="2">
    [flex-order="2"]
  </div>
  <div flex flex-order="1">
    [flex-order="1"]
  </div>
</div>
```
#
#
#

####BASIC HTML
```html
<html ng-app >
	<head>
	    <title>Angular Material Design</title>
	    <meta name="viewport" content="width=device-width, initial-scale=1, maximum-scale=1, user-scalable=no">

	    <!-- lib angular -->
	    <script src="https://ajax.googleapis.com/ajax/libs/angularjs/1.4.5/angular.min.js"></script>

	     <!-- Angular Material CSS now available via Google CDN; version 0.10 used here -->
    	<link rel="stylesheet" href="https://ajax.googleapis.com/ajax/libs/angular_material/0.10.0/angular-material.min.css">

  	</head>
  	
  	<body ng-app="app">


		  <!-- Angular Material Dependencies -->
	    <script src="https://ajax.googleapis.com/ajax/libs/angularjs/1.3.15/angular.min.js"></script>
	    <script src="https://ajax.googleapis.com/ajax/libs/angularjs/1.3.15/angular-animate.min.js"></script>
	    <script src="https://ajax.googleapis.com/ajax/libs/angularjs/1.3.15/angular-aria.min.js"></script>

	    <!-- Angular Material Javascript now available via Google CDN; version 0.10 used here -->
	    <script src="https://ajax.googleapis.com/ajax/libs/angular_material/0.10.0/angular-material.min.js"></script>

	</body>
</html>
```
