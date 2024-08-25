# Análisis de Datos de Taxis en Chicago

Este proyecto aplica técnicas de análisis de datos para examinar los viajes en taxi en Chicago, entender las preferencias de los pasajeros y evaluar el impacto del clima en la duración de los viajes.

## Descripción del Proyecto

Como analista para Zuber, una nueva empresa de viajes compartidos en Chicago, se ha realizado un análisis exhaustivo de los datos de viajes en taxi. El objetivo es identificar patrones y probar una hipótesis sobre cómo el clima afecta la duración de los viajes.

## Descripción de los Datos

La base de datos incluye las siguientes tablas:

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

1. **Análisis del Clima**:
   - Se descargaron y analizaron los datos meteorológicos de noviembre de 2017 desde [este enlace](https://practicum-content.s3.us-west-1.amazonaws.com/data-analyst-eng/moved_chicago_weather_2017.html).

2. **Análisis Exploratorio de Datos**:
   - Número de viajes en taxi para cada empresa del 15 al 16 de noviembre de 2017.
   - Cantidad de viajes para empresas con "Yellow" o "Blue" en el nombre del 1 al 7 de noviembre de 2017.
   - Comparación de las dos empresas de taxis más populares y agrupación de otras empresas bajo "Other".

3. **Prueba de Hipótesis**:
   - Identificación de los barrios de O'Hare y Loop.
   - Clasificación de condiciones meteorológicas en "Bad" o "Good".
   - Análisis de duración de viajes entre Loop y O'Hare en sábados lluviosos.

4. **Análisis Exploratorio de Datos en Python**:
   - Importación y análisis de los archivos CSV proporcionados:
     - `project_sql_result_01.csv`: Datos de viajes por empresa.
     - `project_sql_result_04.csv`: Datos sobre los barrios y promedio de viajes.
   - Visualización de datos y gráficos.

5. **Prueba de Hipótesis en Python**:
   - Evaluación de la duración promedio de los viajes entre Loop y O'Hare en sábados lluviosos utilizando `project_sql_result_07.csv`.

## Archivos

- `project_sql_result_01.csv`: Resultados del análisis de viajes por empresa.
- `project_sql_result_04.csv`: Datos sobre los barrios y el promedio de viajes.
- `project_sql_result_07.csv`: Datos sobre la duración de los viajes desde Loop hasta O'Hare en sábados lluviosos.



