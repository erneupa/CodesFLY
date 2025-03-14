# Modificación del título.

## ¿En qué consiste?.
Este script seleccionará en este caso un título y le cambiaremos la fuente.

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

Para poder ejecutarlo, tendremos que descomentar el código q  ue queramos revisar.

## Código.
```
let titulo = document.getElementById("titulo"); 
titulo.style.fontFamily = "Georgia, serif";

```

### Explicación.
```let titulo = document.getElementById("titulo");``` Aquí estamos buscando un elemento en el HTML que tenga el id="titulo". El método getElementById nos da una referencia a ese elemento, por lo que ahora podemos manipularlo. Lo guardamos en la variable titulo para usarlo más adelante.

```titulo.style.fontFamily = "Georgia, serif";``` Ahora accedemos a los estilos de ese elemento. titulo.style nos permite cambiar las propiedades CSS directamente desde JavaScript. En este caso, estamos modificando la propiedad fontFamily para que el texto dentro del elemento se vea con la fuente Georgia. Si Georgia no está disponible en el dispositivo, se utilizará una fuente serif genérica.

## Antes de ejecutarlo.
![1](/js/Explicaciones/assets/1.png)

## Despues de ejecutarlo.
![2](/js/Explicaciones/assets/2.png)
