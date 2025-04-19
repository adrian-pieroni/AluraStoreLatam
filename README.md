# Análisis de Datos de Ventas de Tiendas

Este repositorio contiene el análisis realizado sobre los datos de ventas de cuatro tiendas diferentes. El objetivo principal fue comprender el rendimiento de cada tienda en diversos aspectos clave del negocio, con el fin de proporcionar una recomendación informada sobre una posible decisión de venta.

## Contenido

1.  [Descripción del Proyecto](#descripción-del-proyecto)
2.  [Objetivos](#objetivos)
3.  [Conjunto de Datos](#conjunto-de-datos)
4.  [Metodología](#metodología)
5.  [Hallazgos Clave](#hallazgos-clave)
    * [Ingresos Totales de las Tiendas](#ingresos-totales-de-las-tiendas)
    * [Categorías de Productos Más y Menos Vendidas](#categorías-de-productos-más-y-menos-vendidas)
    * [Calificaciones Promedio de los Clientes por Tienda](#calificaciones-promedio-de-los-clientes-por-tienda)
    * [Productos Más y Menos Vendidos](#productos-más-y-menos-vendidos)
    * [Costo de Envío Promedio por Tienda](#costo-de-envío-promedio-por-tienda)
6.  [Recomendación](#recomendación)
7.  [Visualizaciones](#visualizaciones)
8.  [Cómo Ejecutar el Código](#cómo-ejecutar-el-código)
9.  [Librerías Utilizadas](#librerías-utilizadas)
10. [Autor](#autor)

## 1. Descripción del Proyecto

Este proyecto consistió en el análisis de datos de ventas de cuatro tiendas para identificar patrones, tendencias y diferencias en su rendimiento. Se exploraron diversos factores, incluyendo ingresos, popularidad de productos y categorías, satisfacción del cliente (a través de calificaciones), costos de envío y distribución geográfica de las ventas. El análisis culminó en una recomendación sobre a qué tienda podría ser estratégico considerar vender.

## 2. Objetivos

Los principales objetivos de este análisis fueron:

* Calcular los ingresos totales de cada tienda.
* Identificar las categorías de productos más y menos vendidas en cada tienda.
* Determinar la calificación promedio de los clientes para cada tienda.
* Identificar los productos individuales más y menos vendidos en cada tienda.
* Calcular el costo de envío promedio para cada tienda.
* Mapear geográficamente las ventas para analizar la distribución regional.
* Sintetizar los hallazgos para proporcionar una recomendación informada.

## 3. Conjunto de Datos

El conjunto de datos utilizado para este análisis consistió en cuatro archivos CSV, cada uno correspondiente a una tienda diferente. Los datos incluyeron información sobre:

* Fecha de compra
* Vendedor
* Lugar de compra
* Calificación del cliente
* Método de pago
* Cantidad de cuotas
* Latitud y longitud de la compra
* Producto vendido
* Categoría del producto
* Precio del producto
* Costo de envío

Los archivos fueron cargados directamente desde URLs proporcionadas.

## 4. Metodología

El análisis se llevó a cabo utilizando la biblioteca de Python `pandas` para la manipulación y el análisis de datos. Se realizaron las siguientes etapas:

1.  **Carga y Unión de Datos:** Los datos de las cuatro tiendas se cargaron en DataFrames de pandas y se unieron en un único DataFrame para facilitar el análisis global. Se añadió una columna para identificar la tienda de origen de cada venta.
2.  **Análisis de Ingresos:** Se calculó la facturación total (asumiendo que el precio representa el ingreso por venta) para cada tienda.
3.  **Análisis de Categorías:** Se identificaron las categorías de productos más y menos vendidas en cada tienda mediante el conteo de las ventas por categoría.
4.  **Análisis de Calificaciones:** Se calculó la calificación promedio de los clientes para cada tienda.
5.  **Análisis de Productos:** Se determinaron los productos individuales con mayor y menor número de ventas en cada tienda.
6.  **Análisis de Costos de Envío:** Se calculó el costo de envío promedio para cada tienda.
7.  **Análisis Geográfico:** Se utilizaron las coordenadas de latitud y longitud para visualizar la distribución de las ventas mediante gráficos de dispersión y un mapa de calor aproximado. Opcionalmente, se exploró la creación de un mapa interactivo con `folium`.
8.  **Síntesis y Recomendación:** Finalmente, se integraron todos los hallazgos para formular una recomendación sobre a qué tienda considerar vender, justificando la decisión con base en el análisis realizado.

## 5. Hallazgos Clave

A continuación, se resumen los principales hallazgos del análisis:

### Ingresos Totales de las Tiendas

[**INSERTA AQUÍ UNA BREVE DESCRIPCIÓN DEL GRÁFICO DE BARRAS DE FACTURACIÓN POR TIENDA Y LAS CONCLUSIONES PRINCIPALES (EJ: La Tienda 4 generó los mayores ingresos, mientras que la Tienda 1 tuvo la menor facturación.)**]

### Categorías de Productos Más y Menos Vendidas

[**INSERTA AQUÍ UNA BREVE DESCRIPCIÓN DEL GRÁFICO DE BARRAS DE VENTAS POR CATEGORÍA Y LAS CONCLUSIONES PRINCIPALES PARA CADA TIENDA (EJ: En la Tienda 3, la categoría 'Electrodomésticos' fue la más vendida, mientras que 'Libros' tuvo menos ventas.)**]

### Calificaciones Promedio de los Clientes por Tienda

[**INSERTA AQUÍ UNA BREVE DESCRIPCIÓN DEL GRÁFICO DE BARRAS DE CALIFICACIONES PROMEDIO Y LAS CONCLUSIONES PRINCIPALES (EJ: La Tienda 2 tuvo la calificación promedio ligeramente más alta, lo que sugiere una mayor satisfacción del cliente.)**]

### Productos Más y Menos Vendidos

[**INSERTA AQUÍ UNA TABLA O LISTA RESUMIENDO EL PRODUCTO MÁS Y MENOS VENDIDO PARA CADA TIENDA (EJ:
| Tienda    | Producto Más Vendido | Producto Menos Vendido |
|-----------|----------------------|-----------------------|
| Tienda 1  | ...                  | ...                   |
| Tienda 2  | ...                  | ...                   |
| ...       | ...                  | ...                   |
)**]

### Costo de Envío Promedio por Tienda

[**INSERTA AQUÍ UNA BREVE DESCRIPCIÓN DEL GRÁFICO DE BARRAS DE COSTO DE ENVÍO PROMEDIO Y LAS CONCLUSIONES PRINCIPALES (EJ: El costo de envío promedio fue más alto en la Tienda 3 y más bajo en la Tienda 1.)**]

### Distribución Geográfica de Ventas

[**INSERTA AQUÍ UNA BREVE DESCRIPCIÓN DEL GRÁFICO DE DISPERSIÓN O MAPA DE CALOR DE LAS VENTAS GEOGRÁFICAS Y LAS CONCLUSIONES PRINCIPALES (EJ: Se observó una mayor concentración de ventas en la región central, con una distribución específica para cada tienda.)**]

## 6. Recomendación

[**INSERTA AQUÍ LA RECOMENDACIÓN CLAVE SOBRE A QUÉ TIENDA CONSIDERAR VENDER (EJ: Basándonos en el análisis integral, se recomienda considerar la venta de la Tienda 1.)**]

Esta recomendación se basa en [**JUSTIFICA AQUÍ TU DECISIÓN, RESUMIENDO LOS PUNTOS CLAVE DEL ANÁLISIS QUE RESPALDAN TU ELECCIÓN. REFERENCIA LOS HALLAZGOS DE INGRESOS, RENDIMIENTO DE PRODUCTOS, SATISFACCIÓN DEL CLIENTE Y COSTOS DE ENVÍO.**]

## 7. Visualizaciones

Los siguientes gráficos fueron generados durante el análisis para visualizar los datos y respaldar las conclusiones:

* **Facturación por Tienda:** [**INSERTA AQUÍ LA FORMA DE MOSTRAR EL GRÁFICO (SI ES UN ARCHIVO, REFERENCIA LA RUTA: `images/facturacion_tiendas.png`)**]
* **Cantidad de Ventas por Categoría en Cada Tienda:** [**INSERTA AQUÍ LA FORMA DE MOSTRAR EL GRÁFICO**]
* **Calificación Promedio de Clientes por Tienda:** [**INSERTA AQUÍ LA FORMA DE MOSTRAR EL GRÁFICO**]
* **Costo de Envío Promedio por Tienda:** [**INSERTA AQUÍ LA FORMA DE MOSTRAR EL GRÁFICO**]
* **Distribución Geográfica de Ventas por Tienda:** [**INSERTA AQUÍ LA FORMA DE MOSTRAR EL GRÁFICO**]
* **(Opcional) Mapa de Calor de Densidad de Ventas:** [**INSERTA AQUÍ LA FORMA DE MOSTRAR EL GRÁFICO**]

**(Nota: Si estás trabajando en un entorno que renderiza Markdown con soporte para mostrar imágenes, puedes incluir las rutas a los archivos de imagen de tus gráficos. Si estás en Colab, podrías considerar guardar los gráficos y referenciarlos aquí o incluso incrustar el código de generación si es breve.)**

## 8. Cómo Ejecutar el Código

El código para realizar este análisis se encuentra en un notebook de Google Colab. Para ejecutar el análisis completo:

1.  Abrir el notebook en Google Colab.
2.  Ejecutar las celdas de código en secuencia. El notebook cargará los datos, realizará el análisis y generará las visualizaciones.

https://colab.research.google.com/github/adrian-pieroni/AluraStoreLatam/blob/main/AluraStoreLatam.ipynb#scrollTo=XFLJRziEUJYU

## 9. Librerías Utilizadas

Las siguientes librerías de Python fueron utilizadas para este análisis:

* `pandas`: Para la manipulación y análisis de datos.
* `matplotlib.pyplot`: Para la creación de gráficos básicos.
* `seaborn`: Para la creación de gráficos estadísticos más avanzados.
* `(Opcional) folium`: Para la generación de mapas interactivos (si se utilizó).

## 10. Autor

[**Adrián Pieroni**]
