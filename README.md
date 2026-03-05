# Optimización de Last Mile: Análisis de Cumplimiento (OTIF) y Devoluciones

### Análisis de Eficiencia en Distribución y Gestión de Novedades
**Herramientas:** `Excel (Power Query)` | `Looker Studio` | `Gestión de KPIs` | `Análisis Estadístico`

---

## Objetivo del Proyecto
Identificar cuellos de botella y fugas de eficiencia en la operación de última milla mediante el análisis de 100 órdenes de pedido. El enfoque principal es la medición del cumplimiento de la promesa de entrega (**SLA**) y el impacto financiero de la logística inversa (devoluciones).

## Metodología (Data Governance)
Para garantizar la integridad del análisis, se ejecutó el siguiente flujo:
1. **Extracción y Limpieza:** Normalización de datos en Excel, estandarización de nomenclaturas de ciudades y transportadoras para eliminar duplicados.
2. **Modelado:** Creación de columnas calculadas para medir el `Tiempo de Entrega Real` vs. `Promesa de Entrega`.
3. **Visualización:** Diseño de un Dashboard Ejecutivo interactivo en **Looker Studio** para el monitoreo de indicadores críticos.

## Hallazgos Críticos (Insights de Negocio)
* **Brecha de Cumplimiento:** El **OTIF** global es del **57%**, lo que indica una oportunidad de mejora del 43% en la experiencia del cliente final.
* **Impacto de Devoluciones:** Una tasa del **23%** de retorno genera un sobrecosto logístico que debe ser mitigado mediante validación de datos en origen.
* **Anomalía Geográfica (Medellín):** Se identificó que Medellín concentra el mayor volumen de incumplimiento, sugiriendo una saturación en la red de distribución local.
* **Causas Raíz:** El **"Cliente Ausente"** y **"Fallas Logísticas"** son los principales detonantes de los retrasos.

## Propuesta de Mejora Analítica
Basado en los datos, se recomiendan las siguientes acciones:
1. **Notificaciones Proactivas:** Implementar alertas automáticas al cliente para reducir la tasa de "Cliente Ausente".
2. **Auditoría de Transportadoras:** Revisar los acuerdos de nivel de servicio (ANS) específicamente en la zona de Medellín debido al bajo desempeño detectado.

---

## Estructura del Repositorio
* **data/**: Contiene el dataset original y la base de datos normalizada (`base_limpia.csv`).
* **dashboard/**: Enlace al reporte interactivo y exportación en PDF.
* **capturas/**: Visualizaciones clave de KPIs de transportadoras y ciudades.

### Enlaces de Interés
* [Ver Dashboard Interactivo en Looker Studio](https://lookerstudio.google.com/reporting/c4186dd3-699f-47a4-9f90-34eb5d0b631e)
* [Revisar Análisis en Excel](https://docs.google.com/spreadsheets/d/1zfgc8o4R3_vumDl0f9RYY7ikEFRyiKY_3Ud3nQBkyUI/edit?usp=sharing)


**Autor** Laura M
