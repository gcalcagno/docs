#METEOR JS

####Crear Proyecto
```
$ meteor create MiProyecto 
```
####Ejecutar Proyecto
```
$ cd /MiProyecto
$ meteor
```

####Se generan 3 archivos
```
MiBiblioteca.css
MiBiblioteca.js
MiBiblioteca.html
```

#### Crear categorias 
1) Crear colección en nuestro archivo MiBiblioteca.js (en la primer línea de nuestro archivo)
```js
  favoritos = new Meteor.Collection ("Favoritos");
```

2)Crear categorías con Mongo DB desde la consola del navegador
```
favoritos.insert({Category:"Videos", items:{Nombre: "La Revolución Francesa", Formato:"mp4", Localizacion: "youtube"}});
favoritos.insert({Category:"Libros", items:{Nombre: "Piratas del Caribe", Formato:"digital", Localizacion: "dropbox"}});
//testeamos si se creo correctamente
favoritos.findOne({Category: "Libros"});
```
