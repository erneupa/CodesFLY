# Crear producto.

## ¿En qué consiste?.
Este escript consiste en crear un nuevo producto con el mismo estilo que los demás y añadirlo al contenedor.

## Manual.
Este script servirá para el archivo [index2.html](https://github.com/erneupa/CodesFLY/blob/main/index2.html).

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
let contenedor = document.querySelector(".subscripciones");
let nuevoProducto = document.querySelector(".subscripciones__producto").cloneNode(true);

nuevoProducto.querySelector(".producto__imagen").src = "assets/dazn.jpg";
nuevoProducto.querySelector(".producto__titulo").textContent = "NUEVO PRODUCTO";
nuevoProducto.querySelector(".producto__info").textContent = "Este es un nuevo producto.";
nuevoProducto.querySelector(".producto__precio").textContent = "50,00€";

contenedor.appendChild(nuevoProducto);

```

### Explicación.
```let contenedor = document.querySelector(".subscripciones");``` Aquí estamos seleccionando el contenedor que tiene la clase .subscripciones. document.querySelector() devuelve el primer elemento que coincide con el selector CSS dado, en este caso, un contenedor de productos.

```let nuevoProducto = document.querySelector(".subscripciones__producto").cloneNode(true);``` En esta línea, seleccionamos un producto dentro del contenedor que tiene la clase .subscripciones__producto. Usamos cloneNode(true) para clonar este producto, incluyendo también sus elementos hijos (por eso pasamos el parámetro true). Esto crea una copia exacta del producto original.

```nuevoProducto.querySelector(".producto__imagen").src = "assets/dazn.jpg";``` Aquí cambiamos la fuente de la imagen del nuevo producto a "assets/dazn.jpg". querySelector(".producto__imagen") selecciona la imagen dentro del producto clonado y luego se cambia su atributo src para apuntar a la nueva imagen.

```nuevoProducto.querySelector(".producto__titulo").textContent = "NUEVO PRODUCTO";``` Se cambia el texto del título del producto clonado a "NUEVO PRODUCTO".

```nuevoProducto.querySelector(".producto__info").textContent = "Este es un nuevo producto.";``` Se cambia la descripción del producto clonado a "Este es un nuevo producto.".

```nuevoProducto.querySelector(".producto__precio").textContent = "50,00€";``` Finalmente, se cambia el precio del producto clonado a "50,00€".

```contenedor.appendChild(nuevoProducto);``` Después de haber modificado el producto clonado, lo agregamos al contenedor original de productos utilizando appendChild(). Esto coloca el nuevo producto al final de la lista de productos.

## Antes de ejecutarlo.
![5](/js/Explicaciones/assets/5.png)

## Despues de ejecutarlo.
![6](/js/Explicaciones/assets/6.png)
