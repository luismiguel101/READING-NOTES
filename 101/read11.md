## Preguntas y Respuestas sobre el DOM y JavaScript

### 1. ¿Qué es el DOM?
El **DOM (Document Object Model)** es una representación estructurada de un documento HTML o XML en forma de árbol. Cada nodo en este árbol representa un elemento, atributo o texto del documento, permitiendo que los lenguajes de programación, como JavaScript, interactúen con la página web.

### 2. Relación entre el DOM y JavaScript
JavaScript usa el DOM para acceder y manipular el contenido, estructura y estilos de una página web en tiempo real. A través del DOM, JavaScript puede agregar, modificar o eliminar elementos, responder a eventos y cambiar estilos de los elementos de la página.

### 3. Método para seleccionar un elemento por su ID
Para seleccionar un elemento del DOM por su ID, se usa el método `document.getElementById()`. Su sintaxis es:

```javascript
const elemento = document.getElementById("miElemento");
```

Donde `"miElemento"` es el valor del atributo `id` del elemento que queremos seleccionar.

### 4. Método para cambiar el color de fondo de un elemento
Para cambiar el color de fondo de un elemento, se utiliza la propiedad `style.backgroundColor`. Ejemplo de implementación:

```javascript
const elemento = document.getElementById("miElemento");
elemento.style.backgroundColor = "blue";
```

Esto cambiará el color de fondo del elemento con `id="miElemento"` a azul.

