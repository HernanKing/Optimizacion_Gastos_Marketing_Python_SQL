# Análisis de Datos para Optimización de Gastos de Marketing (Showz)

## Descripción del Proyecto
Este proyecto de análisis de negocio, realizado como parte de mis prácticas de Data Analytics, se enfoca en optimizar los gastos de marketing para Showz, una empresa de venta de entradas de eventos. A través del análisis de registros de visitas, pedidos y costos de marketing, busco entender el comportamiento del cliente, su rentabilidad y la eficacia de las inversiones en marketing.

## Problema de Negocio / Objetivo
Showz necesita optimizar sus inversiones en marketing para maximizar el retorno. Los objetivos clave del análisis fueron:
1.  Comprender a fondo cómo los clientes utilizan el servicio (frecuencia, duración de sesión, retorno).
2.  Identificar cuándo los clientes realizan su primera compra y cuántos pedidos hacen a lo largo del tiempo.
3.  Calcular la rentabilidad de cada cliente (`LTV - Lifetime Value`).
4.  Determinar el costo de adquisición de clientes (`CAC`) por fuente de marketing y evaluar la rentabilidad de la inversión en marketing (`ROMI`).
5.  Proporcionar recomendaciones estratégicas para los expertos de marketing sobre dónde invertir su presupuesto.

## Conjunto de Datos
El análisis se basó en tres conjuntos de datos clave:
* **`visits_log_us.csv`**: Registros del servidor sobre las visitas al sitio web (UID, Device, Start Ts, End Ts, Source Id).
* **`orders_log_us.csv`**: Datos sobre los pedidos realizados (UID, Buy Ts, Revenue).
* **`costs_us.csv`**: Estadísticas de gastos de marketing (source_id, dt, costs).

## Herramientas y Tecnologías Utilizadas
* **Python:** Lenguaje principal para el análisis, manipulación, cálculo de métricas y visualización de datos.
    * `pandas`: Indispensable para la carga, limpieza y transformación de los DataFrames.
    * `numpy`: Para operaciones numéricas.
    * `matplotlib` / `seaborn`: Para la creación de gráficos y visualizaciones que ilustran las tendencias y métricas clave.
* **SQL (Conceptos):** Aplicación de lógica de bases de datos para combinar y estructurar los datos de múltiples fuentes antes o durante el análisis en Python.
* **Jupyter Notebook:** Entorno de desarrollo para un análisis interactivo y la presentación de resultados.

## Metodología
1.  **Preparación de Datos:** Carga de los datasets, inspección de tipos de datos, limpieza y optimización para el análisis.
2.  **Cálculo de Métricas Clave (KPIs):**
    * **Visitas:** Usuarios diarios/semanales/mensuales, sesiones por día, duración de sesión, tasa de retorno de usuarios.
    * **Ventas:** Tiempo hasta la primera compra (conversión), número de pedidos, tamaño promedio de compra, Lifetime Value (LTV).
    * **Marketing:** Gasto total, Costo de Adquisición de Cliente (CAC) por fuente, y Retorno de Inversión en Marketing (ROMI).
3.  **Análisis Comparativo y Tendencias:**
    * Visualización de cómo las métricas difieren por tipo de dispositivo y fuente de adquisición.
    * Análisis de la evolución de las métricas a lo largo del tiempo.
4.  **Conclusiones y Recomendaciones Estratégicas:**
    * Síntesis de los hallazgos clave.
    * Propuestas fundamentadas sobre las fuentes de marketing más rentables y dónde concentrar futuras inversiones.

## Resultados y Conclusiones (Ejemplos, adapta con tus hallazgos reales)
* Se observó que la `Source ID X` es la fuente de adquisición de clientes con el **ROMI más alto**, indicando una inversión muy rentable.
* La mayoría de los usuarios realizan su primera compra en los primeros 7 días después de su primera sesión, siendo los `dispositivos móviles` un factor clave en las conversiones rápidas.
* El **LTV promedio** de los clientes provenientes de la `Source ID Y` es significativamente mayor, justificando una mayor inversión en este canal a largo plazo.
* Se recomienda redirigir un X% del presupuesto de marketing a la `Source ID Z` debido a su alto potencial de rentabilidad, priorizando la optimización de campañas para dispositivos [móviles/escritorio].

*<img width="1178" height="705" alt="image" src="https://github.com/user-attachments/assets/191550ef-c213-4406-955f-db26b2f90ca2" />



