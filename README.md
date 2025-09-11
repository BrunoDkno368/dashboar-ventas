Continuando con los proyectos en Power bi para el portfolio en este caso vamos a evaluar un dashboard de ventas creados por Chatgpt que consta de 2 tablas con datos aleatorios de unas 200 filas.
[ventas_doble_tabla.xlsx](https://github.com/user-attachments/files/22098125/ventas_doble_tabla.xlsx)

Tabla:
--------------
La primera tabla es llamada “ventas” contiene registros aleatorios en columnas  Fecha, ID_Producto, Cantidad, Tipo_Venta, Metodo_Pago, Descuento_%.

La segunda tabla, llamadas "productos" contiene las siguientes columnas ID_Producto, Producto, Categoria, Precio_Compra, Precio_Venta

Proceso:
---------
Explorado los datos verificamos que no contienen datos en blanco, sin errores, ni outliers procedemos a cargarlo en power bi

Una vez que los datos estan cargado procedemos a combinar las tablas de "venta" y "productos" mediante el campo ID_Producto

visualizaciones:
-------------
La logica de negocio nos pide ciertas visualizaciones

1 Total de ventas

2 Ganancias

3 Ganancias porcentuales

4 Producto mas vendido

5 Categoria mas vendida

6 Top 5 de productos mas vendidos

7 Tipo de venta

8 Evolucion mensual de las ventas

9 Evolucion Diaria

10 Tipo de pago

11 Ventas por categoria

Dentro de los segmentadores nos solicitan

1 Metodo de pago

2 Tipo de venta

3 Año

4 Meses

-------------
Teniendo en claro lo que debemos visualizar creamos una imagen en power point para poder organizar el lienzo en power bi para la organizacion obtenemos lo siguiente
![Presentación1](https://github.com/user-attachments/assets/5d032db9-6d31-4a9e-91ad-e984e88d36f7)

-----------------

A continuacion preparamos los datos para realizar las visualizaciones, creamos una nueva tabla para poder organizar las medidas DAX

Usando DAX creamos nuevas medidas como

1 Ganancia

2 Ganancia %

3 Valor total de compras

4 Valor total de ventas

---------------------------

Creamos las visualizaciones 

![dashboardventas](https://github.com/user-attachments/assets/700a8052-dee3-43e1-a157-cd6d4bb5efce)

----------------------
Del grafico obtenemos lo siguiente 
-------
Segmentadores


1 Segmentador llamado "Tipo de venta" que contiene la opcion online o presencial 

2 Segmentador llamado "Metodo de pago" tiene las opciones Efectivo, Mercadopago, Tarjeta de Credito, Tarjeta de Debito, Transferencia

3 Segmentador llamado "Año" que tiene los años 2022, 2023, 2024, 2025

4 Segmentador llamado "Meses" que tiene los meses del año solo con las 3 primeras letras del mes de Enero a Diciembre

-------------------
Tarjetas


1 Ventas totalas que nos nuestra el total de ventas realizadas 

2 Ganancias totales que nos muestra la ganancias 

3 Ganancias % que nos nuestra el porcentaje de ganancia 

----------------------
Grafico de barras



1 Evolucion mensual, obtenemos por año la evolucion de las ventas mes a mes

2 Top 5 de los productos mas vendidos, nos muestras los productos mas vendido en precio de venta

------------
Grafico de Area


1 Evolucion diaria nos muestra dia a dia como evolucionan las ventas

------------
Grafico Circular



1 Metodo de pago, nos muestra el metodo de pago Efectivo, Mercadopago, Tarjeta de Credito, Tarjeta de Debito, Transferencia

2 Tipo de venta, si la venta fue on line o presencial

-----------------------
Treemap



1 Mediante las categorias se hace la comparacion de la cantidad de ventas

--------------------------------------------

Tarjeta de varias filas con filtrado top N superior

1 El producto mas vendido con la cantidad vendida en dinero

2 La categoria ms vendida 
   


