# Spinner

*¿Comó crear un spinner con html & css?*

Muchas veces es necesario integrar a nuestro código un elemento "spinner" que permita comunicar al usuario, a cerca de su petición a nuestro sitio, para hecer visible que el computador esta procesando la peticion, nuestro código debera mostrar que se esta trabajando mediante el uso de un "spinner". 

En este repositorio podemos encontrar visualizar el código base para poder generar un "spinner" con HTML y CSS sin requerir de javaScript, por lo tanto es un elemento que no ocupa mucha memoria o espacio.

El código esta dividido básicamente en dos archivos, uno de HTML, que incluye solo dos lineas y un archivo CSS con la propiedades o atributos requeridos para hacer que el spinner simule un movimiento rotatorio.

`code CSS`

```
.sppiner {
  background: linear-gradient(to right, var(--primary), var(--secondary));
  border-radius: 50%;
  height: var(--tamano);
  position: relative;
  width: var(--tamano);
  display: flex;
  justify-content: center;
  align-items: center;
  animation: spin var(--user-time) linear infinite;
}

.fondo {
  background: #00061f;
  height: var(--interno);
  width: var(--interno);
  border-radius: 50%;
}

@keyframes spin {
  0% {
    transform: rotate(0deg);
  }

  100% {
    transform: rotate(360deg);
  }
}
```