# Array-de-4-dimensiones
Recorrer Array de 4 Dimensiones y Mostrarlo en el DOM

Este proyecto es una pequeña demo en JavaScript donde se recorre un array de cuatro dimensiones y se muestran todos sus elementos en el DOM mediante tarjetas generadas dinámicamente.

Además, cada tarjeta puede eliminarse con un clic, gracias a un sistema de delegación de eventos.

Funcionalidades:

Recorrido completo de un array 4D usando forEach anidados.

Creación dinámica de elementos HTML (article).

Maquetación con CSS Grid.

Animación de hover (aumento y sombra).

Eliminación de tarjetas al hacer clic (event delegation).

Código claro, limpio y sin librerías externas.

Tecnologías usadas:

HTML5

CSS3

JavaScript Vanilla (sin frameworks)

Cómo funciona?

Se define un array con cuatro niveles de profundidad, mezclando números y letras.

Se recorren todos los niveles con bucles forEach.

Cada valor final se convierte en una tarjeta <article>.

Las tarjetas se agregan al contenedor <main>.

El clic sobre una tarjeta la elimina, usando un único listener en el contenedor.
contenedor_padre.addEventListener("click", (e) => {
    if (e.target.tagName === "ARTICLE") {
        contenedor_padre.removeChild(e.target);
    }
});

