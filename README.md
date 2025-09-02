Continuando con los proyectos en Power bi para el portfolio en este caso vamos a hacer una visualización mediante la creación de 2 archivos creados mediante Chat gpt de unas 200 filas.
[ventas_doble_tabla.xlsx](https://github.com/user-attachments/files/22098125/ventas_doble_tabla.xlsx)


La primera hoja llamada “Ventas” contiene registros aleatorios en columnas  Fecha, ID_Producto, Cantidad, Tipo_Venta, Metodo_Pago, Descuento_%.

mientras la segunda en la hoja llamada columna contiene las siguientes columnas ID_Producto, Producto, Categoria, Precio_Compra, Precio_Venta

Proceso:

En este caso los datos llegan sin errores, sin datos en blancos ni outliers procedemos a cargarlos en Power bi , ya lo con los datos cargados vamos a combinar las tablas de Ventas y Productos mediante el campo ID_Producto
En la columna Fecha  en 3 columnas distintas, una para el día, otra para el mes  y la ultima para el año. Dentro de la columnas creadas tanto día como mes la pasamos a formato texto solo con sus 3 primeras iníciales 
Creamos nuevas columas por un lado Ganancia con una expresión DAX SUM(tabla_ventas[Valor_Total_venta]) - SUM(tabla_ventas[Valor_Total_Compra])
También creamos una columna nueva con DAX las Ganancias%  con la expresion [Ganancia] / SUM(tabla_ventas[Valor_Total_Compra]) 
De igual forma creamos 2 columnas mas una llamada Valor_Total_Compra y Valor_Total_venta
Grafico

<img width="1366" height="768" alt="imagen dashboard" src="https://github.com/user-attachments/assets/42bcf8a6-8678-4797-977f-f3172637c75c" />

El Dashboard está compuesto de diferentes gráficos como de tarjeta, circular, columnas agrupadas, de área y un treemap

En el grafico podemos visualizar tarjetas como Ventas totales, Ganancias Totales y Ganancia %

En la tarjeta Producto top podemos observar el producto mas vendido con las unidades aplicando el Filtro top N igualmente en la tarjeta Categoría top

Tenemos un grafico de barras agrupadas que nos muestra los productos mas vendidos

En uno de los gráficos circulares observamos si fueron ventas presenciales u online. En el otro grafico circular observamos el tipo de pago realizado por los clientes (tarjeta de crédito, mercado pago, tarjeta de debito, transferencia o efectivo)

En el grafico Categoría podemos observar en un treemap la cantidad que se vendieron por categoría

Con un grafico de área visualizamos la evolución por días de las ventas

En la grafica de columnas apiladas podemos distinguir las ventas por meses del año

Tenemos 4 filtros 

1 por año

2 por meses

3 por tipo de venta

4 por método de pago 

Visualizacion

mediante paint realizamos un fondo para poder organizar de mejor manera los datos a visualizar 

<img width="960" height="540" alt="fondo" src="https://github.com/user-attachments/assets/853ca920-59ed-4848-9fe0-3209a4048dfd" />
