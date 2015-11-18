#METEOR JS
### PATRON MVVM
```
Meteor almacena un modelo de datos igual en el cliente y el servidor. El cliente 
almacena los cambios localmente e intenta sincronizar con el servidor, al tiempo 
que vigila los cambios que puedan llegar al servidor

```

### Crear Proyecto
```
$ meteor create MiProyecto 
```
### Ejecutar Proyecto
```
$ cd /MiProyecto
$ meteor
```


### SASS

```
1) Creamos una carpeta Client dentro de la Raíz de nuestro proyecto (Todos los archivos que estén dentro de 
esta carpeta serán compilados por Meteor)
$ cd /MiProyecto
$ mkdir client
2) Instalamos fourseven y se va a encargar de compilar todos los archivos sass
$ meteor add fourseven:scss
```

### IMAGENES Y FUENTES
```
Las Imagenes y Fuentes deben estar en la carpeta Public (si no tenemos esta carpeta la creamos dentro de 
la raíz de nuestro proyecto).
1) Creamos una carpeta public dentro de la Raíz de nuestro proyecto.
$ cd /MiProyecto
$ mkdir public
IMPORTANTE:Si colocamos la carpeta img o fuentes dentro de Client la applicación va a dar un error.
```

###Se generan 3 archivos
```
MiBiblioteca.css
MiBiblioteca.js
MiBiblioteca.html
```

### Crear categorias con MONGO DB
1) Crear colección en nuestro archivo MiBiblioteca.js (en la primer línea de nuestro archivo)
```js
  favoritos = new Meteor.Collection ("Favoritos");
  /*para testear si se creó correctamente*/
  favoritos
```

2)Crear categorías con Mongo DB desde la consola del navegador dentro de la "Colección Favoritos"
``` js
/*crea categoria con registros */
favoritos.insert({Category:"Videos", items:{Nombre: "La Revolución Francesa", Formato:"mp4", Localizacion: "youtube"}});
favoritos.insert({Category:"Libros", items:{Nombre: "Piratas del Caribe", Formato:"digital", Localizacion: "dropbox"}});

/*categoria*/
favoritos.insert({Category:"Tutoriales"});

/*Busca Categoría Libros*/
favoritos.findOne({Category: "Libros"});

/*Count de Categorías*/
favoritos.find({}).count();

/*eliminar categoria */
favoritos.remove({"_id": "F37ALy9HZqha4S2BM"});
```
