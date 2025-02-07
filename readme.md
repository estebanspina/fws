# FWS (Functional Web Scripting Language) #

FWS es un proyecto de lenguaje de programación diseñado para el desarrollo web, inspirado en la sintaxis y funcionalidad de lenguajes maduros como JavaScript. Su objetivo es ofrecer un rendimiento mejorado y un enfoque en la programación funcional, permitiendo a los desarrolladores construir aplicaciones web de manera eficiente y efectiva.

## Características Clave ##

### Sintaxis Familiar ###
- La sintaxis de FWS deberá ser similar a la de JavaScript, permitiendo que los desarrolladores que ya están familiarizados con este lenguaje maduro puedan adaptarse rápidamente.
- Soporte para estructuras de control como if, for, while, y funciones de alto orden.

### Tipado Dinámico ###
- FWS implementa un sistema de tipos dinámicos, lo que permite a los desarrolladores declarar variables sin necesidad de especificar un tipo explícito. Esto proporciona una gran flexibilidad y agilidad en el desarrollo.
- Las variables pueden cambiar de tipo en tiempo de ejecución, lo que facilita la manipulación de datos de diferentes tipos sin complicaciones.

Ejemplo:

```
var x = 10;         // x es un número
x = "Hola";        // x ahora es una cadena
x = [1, 2, 3];    // x ahora es un array
```

### Enfoque en Programación Funcional ###

- FWS promueve un estilo de programación funcional, donde las funciones son ciudadanos de primera clase. Esto significa que las funciones pueden ser asignadas a variables, pasadas como argumentos y retornadas desde otras funciones.
- Soporte para funciones puras, evitando efectos secundarios y facilitando la composición de funciones.

Ejemplo:

```
// Definición de una función pura
function suma(a, b) {
    return a + b;
}

// Composición de funciones
function aplicarDoble(func, valor) {
    return func(func(valor));
}

var resultado = aplicarDoble(suma, 5)(3); // Resultado: 16
print("El resultado es: " + resultado);
```

### Ejecutable en el Navegador ###

- FWS se compilará a código máquina o a WebAssembly, permitiendo que las aplicaciones se ejecuten directamente en el navegador con un rendimiento cercano al nativo.
- Integración con tecnologías web existentes como HTML5, CSS3 y APIs del navegador.

### Manejo Asíncrono ###

- Soporte para operaciones asíncronas, incorporando promesas y async/await, facilitando el trabajo con solicitudes HTTP y otras operaciones que requieren tiempo.

### Seguridad ###

- Enfoque en la seguridad para evitar vulnerabilidades comunes, como inyecciones de código o acceso no autorizado a datos.

### Ejemplo de Código ###

```
// Definición de una función pura
function cuadrado(x) {
    return x * x;
}

// Uso de la función
var resultado = cuadrado(4);
print("El cuadrado es: " + resultado); // Salida: El cuadrado es: 16

// Uso de funciones de alto orden
function map(func, arr) {
    var resultado = [];
    for (var i = 0; i < arr.length; i++) {
        resultado[i] = func(arr[i]);
    }
    return resultado;
}

// Aplicar la función cuadrado a un array
var numeros = [1, 2, 3, 4];
var cuadrados = map(cuadrado, numeros);
print("Cuadrados: " + cuadrados); // Salida: Cuadrados: 1,4,9,16
```
