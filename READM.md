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

La base de datos incluye diversa información sobre la producción, el procesamiento y la evaluación sensorial del café. También contiene datos sobre la genética del café, los tipos de suelo y otros factores que pueden influir en la calidad del café en un solo arvhivo .csv de Excel. Dentro del dataset existe una columna nombrada como "Total Cup Points" y es la suma de las 10 atributos tomadas en cuenta para calificar el café indicadas anteriormente (aroma, flavor, aftertaste, acidity, body, entre otros).

## 2. Staging

### *Análisis exploratorio de los datasets en Excel/Power Query*

1. Revisión de valores duplicados, filas o columnas vacías y encabezados estandarizados.
   
2. Normalización de la columna de "Altitud" que se encuentra con rangos y dividirla en 3 columnas diferentes ("Altitud inferior", "Altitud superior" y "Promedio de altitud").
   
3. Reemplazar y estandarizar las variaciones de los nombres de los países. 






