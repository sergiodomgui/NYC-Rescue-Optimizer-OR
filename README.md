# NYC-Rescue-Optimizer 

Este proyecto implementa un modelo de programación lineal para la optimización y asignación de vehículos de emergencia en los distintos distritos de la ciudad de Nueva York, utilizando datos reales de incidentes y distancias.

## Descripción

El objetivo principal es maximizar la eficiencia de la cobertura basándose en la población de los barrios y la cercanía a las estaciones de bomberos. El modelo resuelve la asignación de 5 tipos de vehículos en 218 estaciones, considerando turnos de trabajo y restricciones de capacidad.

## Tecnologías utilizadas

* **Python 3.10+**
* **Google OR-Tools**: Empleando solvers como **CBC** y **SCIP** para la resolución de problemas de optimización lineal y entera.
* **Pandas & NumPy**: Para el manejo de estructuras de datos.
* **Matplotlib**: Para la visualización de resultados y comparación de rendimiento entre solvers.

## Estructura de Datos

El sistema consume datos dinámicos desde repositorios externos en formato JSON:
* `incidentes2019.json`: Histórico de incidentes.
* `estaciones.json`: Información y capacidad de las estaciones.
* `barrios.json`: Población y datos demográficos por NTA (Neighborhood Tabulation Areas).
* `distancias_estaciones_barrios.json`: Matrices de distancias calculadas.
