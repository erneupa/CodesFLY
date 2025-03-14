# Modificar contenido.

## ¿En qué consiste?.
Este escript consiste en que cuando yo tengo un texto que ya se ha quedado anticuado, podramos cambiarlo desde nuestro programa directamente.

## Manual.
Este script servirá para el archivo [index3.html](https://github.com/erneupa/CodesFLY/blob/main/index3.html).

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
document.querySelector(".equipo__texto").textContent = "Nuestra empresa ofrece soluciones innovadoras para impulsar tu crecimiento. Nos enfocamos en calidad, compromiso y satisfacción del cliente.";
```

### Explicación.
```document.querySelector(".equipo__texto"):``` Selecciona el primer elemento que tiene la clase equipo__texto en el DOM (normalmente un <p> o cualquier otro tipo de elemento). Este método devuelve una referencia a ese elemento.

```.textContent = "Nuestra empresa ofrece soluciones innovadoras para impulsar tu crecimiento. Nos enfocamos en calidad, compromiso y satisfacción del cliente.";``` Modifica el contenido de texto del elemento seleccionado. El texto actual será reemplazado por el nuevo texto proporcionado, en este caso, "Nuestra empresa ofrece soluciones innovadoras para impulsar tu crecimiento. Nos enfocamos en calidad, compromiso y satisfacción del cliente."

## Antes de ejecutarlo.
![9](/js/Explicaciones/assets/9.png)

## Despues de ejecutarlo.
![10](/js/Explicaciones/assets/10.png)
