# Modificación del título.

## ¿En qué consiste?.
Este script seleccionará en este caso un título y le cambiaremos la fuente.

## Código.
```
let titulo = document.getElementById("titulo"); 
titulo.style.fontFamily = "Georgia, serif";

```

### Explicación.
```let titulo = document.getElementById("titulo");``` Aquí estamos buscando un elemento en el HTML que tenga el id="titulo". El método getElementById nos da una referencia a ese elemento, por lo que ahora podemos manipularlo. Lo guardamos en la variable titulo para usarlo más adelante.

```titulo.style.fontFamily = "Georgia, serif";``` Ahora accedemos a los estilos de ese elemento. titulo.style nos permite cambiar las propiedades CSS directamente desde JavaScript. En este caso, estamos modificando la propiedad fontFamily para que el texto dentro del elemento se vea con la fuente Georgia. Si Georgia no está disponible en el dispositivo, se utilizará una fuente serif genérica.

## Antes de ejecutarlo.
![1](/assets/1.png)
