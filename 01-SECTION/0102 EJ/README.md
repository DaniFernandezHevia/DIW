# SECTION 01: Ejemplo 02. 
## Etiqueta para para aplicar al box-sizing a toda la pagina
1. .box
Cuando queremos darle el mismo diseño a todos los box-sizing que usamos en la pagina, basta con 
primero crearlos haciendo un div.box y tabulando poniendo el texto dentro en este caso lorem20 y 
por las veces que queramos en este (*4).
```
    <div class="box">Lorem ipsum ...</div>
    <div class="box">Lorem ipsum ...</div>
    <div class="box">Lorem ipsum ...</div>
    <div class="box">Lorem ipsum ...</div>

```
Ahora trabajaremos sobre el css, con el siguiente codigo:
```
*, *::before, *::after, *:before, *:after {
    box-sizing: border-box;
}

.box{
    width: 25%;
    background-color: salmon;
    color: white;
    border: 1px solid blue; 
    float: left;
}
```