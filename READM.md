## proyecto-ranking-cafe
# Ranking de países latinoamericanos por calidad de café
### Rol: Junior Data Analyst

## 📊 Dashboard Interactivo

## Fase de consulta:

Una importadora de café quiere saber qué países de América Latina producen consistentemente el café mejor calificado para priorizar sus compras. Los datos son reseñas reales de 1,340 cafés evaluados por catadores profesionales en el año 2018. Se plantearon las siguientes preguntas para encontar la solución adecuada a este problema de negocio:

1. ¿Qué países de LATAM producen el café mejor calificado?

2. ¿Cuántas muestras tienen cada uno?

3. ¿Qué atributo (aroma, acidez, balance) tiene más peso en la calificación final?

## Objetivo del análisis:
Analizar los datos sobre reseñas de café para identificar el país latinoamericano con mejor calificación y el atributo más destacado sobre el café. 

## Proceso de análisis:

## 1. Preparación

### *Datos utilizados*

Para este análisis se usaron dos datasets abiertos del sitio web kaggle.com. Un solo CSV, manejable en Excel sin necesidad de combinar archivos.

### *Información de los datasets*

Los datos de este proyecto fueron tomados del Coffee Quality Institute que evalúa cafés de todo el mundo con catadores entrenados. Este dataset tiene 1,340 reseñas de granos Arabica y Robusta con calificaciones en aroma, sabor, acidez, balance y más. Los países muestreados son: Colombia, México, Guatemala, Brasil, Honduras, Perú, El Salvador y Costa Rica.

### *Organización de los datasets*

La base de datos incluye diversa información sobre la producción, el procesamiento y la evaluación sensorial del café. También contiene datos sobre la genética del café, los tipos de suelo y otros factores que pueden influir en la calidad del café en un solo arvhivo .csv de Excel. Dentro del dataset existe una columna nombrada como *"Total Cup Points"* y es la suma de las 10 atributos tomados en cuenta para calificar el café indicadas anteriormente (aroma, flavor, aftertaste, acidity, body, entre otros).

## 2. Staging

### *Análisis exploratorio de los datasets en Excel/Power Query*

1. Revisión de valores duplicados, filas o columnas vacías y encabezados estandarizados.
   
2. Normalización de la columna de "Altitud" que se encuentra con rangos y dividirla en 3 columnas diferentes ("Altitud inferior", "Altitud superior" y "Promedio de altitud").
   
3. Reemplazar y estandarizar las variaciones de los nombres de los países. 

## 3. Intermediate

1. De la base de datos se autofiltró la columna de *"Country of origin"* para que solo queden los países latinoamericanos evaluados.

2. Se creó una nueva tabla con las columnas: *"Country of origin"*, *"Promedio de Total Cup Points"* y *"Cantidad de muestra"*.

3. Se copiaron los países en otra hoja de cálculo y luego se eliminaron los duplicados para que no se repitan y queden en una columna los 10 países evaluados.

4. Se usó la función *"PROMEDIO.SI"* para encontrar el promedio de la columna *Total Cup Points*, que es el total de los 10 atributos  (aroma, flavor, aftertaste, acidity, body, entre otros) encuestados para decidir la calificación final de la muestra de café.

5. Se usó la función *CONTAR.SI* para encontrar el número de muestras de café evaluadas por país.

6. Se creo una nueva tabla para evaluar que atributo tiene mayor influencia en el resultado final *Total Cup Points* con la función *PROMEDIO.SI* del café con la mejor calificación.

## Conclusiones:

- El país latinoamericano con mejor calificación es Guatemala con un promedio de 84,3.
- La cantidad de muestras varia dependiendo del pais y se encuentran en un rango de 2-21. Guatemala contó con 21 muestras evaluadas por los catadores de café.
- El atributo con mayor peso o influencia dentro de la calificación final es de *SABOR* con un promedio de 7,88 , seguido por *AROMA* con 7,7. Los demás atributos (*ACIDEZ* y *BALANCE*) tienen el mismo peso dentro de la calificación.

## Insight:

- Guatemala representa sin duda una gran alternativa para la compra de café debido a sus varias fincas que lo producen, asegurando stock ilimitado constante conservando la alta calidad del mismo.
  
- Se recomienda tener en cuenta a Colombia como una alternativa de compra ya que tiene también representa mantener una alta calidad de café de diversas fincas (19 en total), lo cual en temporadas de escasez o plagas ayudaría a mantener el stock sin afectar las ventas.
  

