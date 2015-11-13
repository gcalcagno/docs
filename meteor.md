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
  /*para testear si se creó correctamente*/
  favoritos
```

2)Crear categorías con Mongo DB desde la consola del navegador dentro de la "Colección Favoritos"
``` js
favoritos.insert({Category:"Videos", items:{Nombre: "La Revolución Francesa", Formato:"mp4", Localizacion: "youtube"}});
favoritos.insert({Category:"Libros", items:{Nombre: "Piratas del Caribe", Formato:"digital", Localizacion: "dropbox"}});
/*Busca Categoría Libros*/
favoritos.findOne({Category: "Libros"});
/*Count de Categorías*/
favoritos.find({}).count();
```
