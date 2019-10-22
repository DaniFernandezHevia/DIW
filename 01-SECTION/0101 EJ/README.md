# SECCION 01: Ejemplo 01. Ejemplos de bordes.
## Usando border-box 
1. Ejemplo donde introducimos un padding y un border, por lo que, además del ancho de 20rem,
le pondremos un padding de 5rm que se sumará a su ancho y un border que actuará de igual manera.
- Codigo:
```
div{
    
    width: 20rem;
    height: 20rem;
    background-color: salmon; 
    padding: 5rem;
    border: 20px solid blue;    
}
```
2. Ahora usamos el  [box-sizing: border-box;] con esta etiqueta lo que hacemos al añadir el padding,
es que en vez de aumentar la caja, lo que hará es actuar hacia dentro y no aumentar las medidas de la 
caja.

- Codigo:
``` 
div{
    box-sizing: border-box;
    width: 20rem;
    height: 20rem;
    background-color: salmon; 
    padding: 5rem;
    border: 20px solid blue; 
}
```
Además con la etiqueta [overflow: auto;], introducimos una barra de scroll, en el caso de que el 
texto introducido no nos entre al completo en nuestra caja. También podemos usar el overflow con 
hidden para ocultar el texto que no entre en la caja.

