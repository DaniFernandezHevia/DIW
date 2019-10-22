# Z-INDEX
- La propiedad **z-index** determina el nivel de pila de un elemento HTML. El "nivel de pila" se refiere a la posición del element en el eje Z
- Solo es valida esta propiedad con la propiedad **position** establecida, si es necesario puedo poner **position: relative** sin establecerle coordenadas ya que el elemento se queda en su sitio.

- Tenemos 5 tarjetas:
´´´
@for $i from 2 through 5 {
    .card:nth-child(#{$i}) {
        position: absolute;
        left: 8rem * ($i - 1);
        top: 5rem * ($i - 1);
        @if ($i == $zi) {
            z-index: 1;
        }
    }
´´´
Con scss, con el codigo anterior, hacemos que cada carta que va pasando de la 1 a la 5 va tomando diferentes valores debido a el codigo scss que hemos puesto.
