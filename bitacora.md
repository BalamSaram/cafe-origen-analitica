# Día 1
## Errores observados

Al ejecutar node src/explorar.js en la terminal se puede observar varios datos correspondientes al arreglo de datos. Algunos de ellos contienen errores, como por ejemplo, las ciudades, donde se puede observar que el cuarto quinto elemento en el arreglo de ciudades inicia con minúscula. Otros errores, pueden ser observados directamente en el arreglo de datos, como la venta con id 8, cuya cantidad de venta es 0, por lo cual no es válida, con ello, también invalida al cliente C06.

|Problema|Decisión|
|:---|:---|
|Venta 8 cantidad 0|No se cuenta en el registro|
|Ciudades con minúsculas| Normalizar el dato antes del análisis|
|clientes repetidos| Es válido|

### Diccionario de datos

|Propiedad|Tipo|Significado|
|:---|:---|:---|
|`id`|Entero|Identifica cada una de las ventas. Debe ser único|
|`fecha`|texto|Guarda el dato del día en que se registró la venta|
|`cliente`|texto|Código asignado a cada cliente. Puede aparecer varias veces|
|`producto`|texto|Nombre de los items vendidos|
|`ciudad`|texto|Corresponde al sitio donde se realizó la venta. Requiere normalizar|
|`cantidad`|entero|corresponde a las unidades vendidas. No puede ser un valor cero o negativo.|
|`precio`|entero|Corresponde al precio unitario de venta, en COP.|