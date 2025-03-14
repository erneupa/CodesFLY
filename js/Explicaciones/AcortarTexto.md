# Acortar Texto.

## ¿En qué consiste?.
Para este script, tendremos un texto y un botón el cual pone mostrar menos, de tal forma que cuando ejecutemos nuestro programa, se acortará el texto y el botón cambiará a mostrar más.

## Manual.
Este script servirá para el archivo [index.html](https://github.com/erneupa/CodesFLY/blob/main/index.html).

El Programa cuando lo abramos, nos aparecerá tal que así:
```
/*

// -------------------------------------------------------------------------------------------------
// Modificación del título: Cambia la fuente del h1.
// -------------------------------------------------------------------------------------------------

let titulo = document.getElementById("titulo"); // Selecciona el elemento h1 con el ID "titulo"
titulo.style.fontFamily = "Georgia, serif"; // Aplica la fuente "Georgia, serif"

*/

/*----------------------------------------------------------------------------------------------------------------------------------*/

/*

// -------------------------------------------------------------------------------------------------
// Acortar el texto de un párrafo y cambiar el botón a "Mostrar más"
// -------------------------------------------------------------------------------------------------

let parrafo = document.getElementById("texto"); // Selecciona el párrafo con el ID "texto"
let boton = document.getElementById("mostrarMas"); // Selecciona el botón con el ID "mostrarMas"
let textoLargo = parrafo.textContent; // Obtiene el texto completo 

parrafo.textContent = textoLargo.substring(0, textoLargo.length / 2) + "..."; // Acorta el texto a la mitad
boton.textContent = "Mostrar más"; // Cambia el texto del botón a "Mostrar más"

*/

/*----------------------------------------------------------------------------------------------------------------------------------*/

/*

// -------------------------------------------------------------------------------------------------
// Crear un nuevo producto con el mismo estilo y añadirlo al contenedor
// -------------------------------------------------------------------------------------------------

let contenedor = document.querySelector(".subscripciones"); // Selecciona el contenedor de productos
let nuevoProducto = document.querySelector(".subscripciones__producto").cloneNode(true); // Clona un producto existente

// Modifica el contenido del nuevo producto con nueva información
nuevoProducto.querySelector(".producto__imagen").src = "assets/dazn.jpg"; // Cambia la imagen
nuevoProducto.querySelector(".producto__titulo").textContent = "NUEVO PRODUCTO"; // Cambia el título
nuevoProducto.querySelector(".producto__info").textContent = "Este es un nuevo producto."; // Cambia la descripción
nuevoProducto.querySelector(".producto__precio").textContent = "50,00€"; // Cambia el precio

contenedor.appendChild(nuevoProducto); // Agrega el nuevo producto al final de la lista

*/

/*----------------------------------------------------------------------------------------------------------------------------------*/

/*

// -------------------------------------------------------------------------------------------------
// Eliminar un producto existente de la lista (el segundo producto en este caso)
// -------------------------------------------------------------------------------------------------

let productos = document.querySelectorAll(".subscripciones__producto"); // Selecciona todos los productos

productos[1].remove(); // Elimina el segundo producto de la lista

*/

/*----------------------------------------------------------------------------------------------------------------------------------*/

/*

// -------------------------------------------------------------------------------------------------
// Modificar el contenido de la primera descripción dentro del artículo "equipo__informacion"
// -------------------------------------------------------------------------------------------------

document.querySelector(".equipo__texto").textContent = "Nuestra empresa ofrece soluciones innovadoras para impulsar tu crecimiento. Nos enfocamos en calidad, compromiso y satisfacción del cliente."; 
// Cambia el texto de la primera etiqueta <p> dentro del artículo con la clase "equipo__informacion"

*/
```

Para poder ejecutarlo, tendremos que descomentar el código que queramos revisar.

## Código.
```
let parrafo = document.getElementById("texto");
let boton = document.getElementById("mostrarMas");
let textoLargo = parrafo.textContent;

parrafo.textContent = textoLargo.substring(0, textoLargo.length / 2) + "...";
boton.textContent = "Mostrar más";

```

### Explicación.
```let parrafo = document.getElementById("texto");``` Aquí seleccionamos el párrafo que tiene el id="texto". Este método nos devuelve una referencia al elemento con ese id, y lo guardamos en la variable parrafo para poder manipularlo.

```let boton = document.getElementById("mostrarMas");``` De manera similar, seleccionamos el botón con el id="mostrarMas", lo guardamos en la variable boton para poder cambiar su contenido más tarde.

```let textoLargo = parrafo.textContent;``` Aquí, tomamos el texto completo que está dentro del párrafo seleccionado y lo almacenamos en la variable textoLargo. textContent obtiene todo el contenido de texto, excluyendo etiquetas HTML.

```parrafo.textContent = textoLargo.substring(0, textoLargo.length / 2) + "...";``` Esta línea acorta el texto del párrafo a la mitad. substring(0, textoLargo.length / 2) corta el texto desde el inicio hasta la mitad de su longitud, y luego agregamos "..." al final para indicar que el texto está incompleto.

```boton.textContent = "Mostrar más";``` Finalmente, cambiamos el texto del botón a "Mostrar más", para que el usuario sepa que puede hacer clic para ver el resto del texto.

## Antes de ejecutarlo.
![3](/js/Explicaciones/assets/1.png)

## Despues de ejecutarlo.
![4](/js/Explicaciones/assets/2.png)
