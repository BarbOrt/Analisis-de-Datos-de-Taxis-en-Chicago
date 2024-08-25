# Análisis de Datos de Taxis en Chicago

Este proyecto aplica técnicas de análisis de datos para examinar los viajes en taxi en Chicago, entendiendo las preferencias de los pasajeros y el impacto de factores externos, como el clima, en los viajes.

## Descripción del Proyecto

Como analista para Zuber, una nueva empresa de viajes compartidos, se ha llevado a cabo un análisis detallado utilizando una base de datos de viajes en taxi en Chicago. El objetivo fue identificar patrones en los datos y probar una hipótesis sobre el impacto del clima en la duración de los viajes.

## Descripción de los Datos

La base de datos contiene las siguientes tablas:

- **neighborhoods**: Información sobre los barrios de Chicago.
  - `name`: Nombre del barrio
  - `neighborhood_id`: Código del barrio

- **cabs**: Datos sobre los taxis.
  - `cab_id`: Código del vehículo
  - `vehicle_id`: ID técnico del vehículo
  - `company_name`: Empresa propietaria del vehículo

- **trips**: Información sobre los viajes en taxi.
  - `trip_id`: Código del viaje
  - `cab_id`: Código del vehículo
  - `start_ts`: Fecha y hora de inicio del viaje
  - `end_ts`: Fecha y hora de finalización del viaje
  - `duration_seconds`: Duración del viaje en segundos
  - `distance_miles`: Distancia del viaje en millas
  - `pickup_location_id`: Código del barrio de recogida
  - `dropoff_location_id`: Código del barrio de finalización

- **weather_records**: Datos sobre el clima.
  - `record_id`: Código del registro meteorológico
  - `ts`: Fecha y hora del registro
  - `temperature`: Temperatura en el momento del registro
  - `description`: Descripción de las condiciones meteorológicas

## Pasos Realizados

### Paso 1: Análisis del Clima

Se descargaron y analizaron los datos meteorológicos de noviembre de 2017 desde el sitio web proporcionado para entender las condiciones climáticas durante el periodo de estudio.

### Paso 2: Análisis Exploratorio de Datos

1. **Número de Viajes por Empresa (15-16 Noviembre 2017)**:
   - Se determinó el número de viajes realizados por cada empresa de taxis en los días especificados.

2. **Viajes para Empresas "Yellow" o "Blue" (1-7 Noviembre 2017)**:
   - Se analizaron los viajes para las empresas de taxis que incluyen "Yellow" o "Blue" en su nombre.

3. **Comparación de Empresas Populares**:
   - Se identificaron las dos empresas de taxis más populares y se compararon con otras empresas agrupadas bajo "Other".

### Paso 3: Prueba de Hipótesis

1. **Identificación de Barrios**:
   - Se recuperaron los identificadores de los barrios de O'Hare y Loop para su análisis.

2. **Condiciones Climáticas**:
   - Se clasificaron las condiciones meteorológicas en "Bad" o "Good" en función de la descripción del clima.

3. **Duración de Viajes en Sábados Lluviosos**:
   - Se analizó si la duración de los viajes entre Loop y O'Hare cambia en sábados lluviosos.

### Paso 4: Análisis Exploratorio de Datos en Python

1. **Importación y Análisis de Datos**:
   - Se importaron los archivos CSV resultantes y se realizó un análisis para verificar los tipos de datos y los resultados.

2. **Visualización**:
   - Se crearon gráficos para visualizar la cantidad de viajes por empresa de taxis y los barrios principales por número de finalizaciones.

### Paso 5: Prueba de Hipótesis en Python

1. **Análisis Estadístico**:
   - Se realizó una prueba de hipótesis para determinar si la duración de los viajes desde Loop hasta O'Hare cambia en sábados lluviosos, con un análisis estadístico detallado.

## Conclusiones

- **Viajes por Empresa**: Se identificaron las empresas de taxis con más y menos viajes en los periodos analizados.
- **Comparación de Empresas**: Flash Cab y Taxi Affiliation Services destacaron en noviembre de 2017.
- **Impacto del Clima**: La prueba de hipótesis mostró si la duración de los viajes varía significativamente en sábados lluviosos.

## Evaluación

El proyecto cumple con los criterios de evaluación establecidos, incluyendo la recuperación de datos, creación de slices de datos, agrupamiento, unión de tablas, formulación y prueba de hipótesis, y conclusiones basadas en el análisis.

## Archivos

- `project_sql_result_01.csv`: Resultados del análisis de viajes por empresa.
- `project_sql_result_04.csv`: Datos sobre los barrios y el promedio de viajes.
- `project_sql_result_07.csv`: Datos sobre la duración de los viajes desde Loop hasta O'Hare en sábados lluviosos.


