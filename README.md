# 🧪 A/B Testing y Priorización de Hipótesis – Análisis en E-commerce

Este proyecto analiza un conjunto de hipótesis de negocio y evalúa una prueba A/B en una tienda online.

El objetivo es priorizar iniciativas de crecimiento utilizando los frameworks ICE y RICE, y posteriormente validar su impacto mediante análisis estadístico de un experimento A/B.

## 🎯 Objetivos

- Priorizar hipótesis de negocio utilizando los frameworks ICE y RICE
- Comparar los resultados de priorización entre ambos métodos
- Analizar el desempeño de una prueba A/B
- Evaluar la significancia estadística entre los grupos
- Generar recomendaciones basadas en datos

## 📂 Dataset

El análisis se basa en tres conjuntos de datos:

### Hipótesis
- Reach (alcance)
- Impact (impacto)
- Confidence (confianza)
- Effort (esfuerzo)

### Órdenes
- transactionId
- visitorId
- revenue
- grupo (A/B)

### Visitas
- fecha
- grupo
- número de visitas

## 🛠️ Herramientas y Tecnologías

- Python
- Pandas
- NumPy
- Matplotlib / Seaborn
- SciPy / Statsmodels
- Jupyter Notebook

## 📊 Metodología

### 1. Priorización de hipótesis
- Aplicación del framework ICE
- Aplicación del framework RICE
- Comparación de resultados entre ambos enfoques

### 2. Análisis de la prueba A/B
- Preprocesamiento de datos
- Análisis de ingresos acumulados
- Análisis de tasa de conversión
- Análisis del valor promedio de pedido
- Detección de valores atípicos (percentiles 95 y 99)
- Pruebas de hipótesis (datos crudos y filtrados)

## 📈 Métricas clave

- Tasa de conversión (Conversion Rate)
- Valor promedio de pedido (AOV)
- Ingresos (Revenue)
- Significancia estadística (p-value)

## 🔍 Resultados e Insights

- La escala es mayor en RICE, así mismo su valor siempre es mayor que ice. Ambas métricas priorizan las hipótesis 7, 2, 0, 6 y 8 entre los primeros lugares.
- Se identificaron diferencias entre los grupos mediante pruebas estadísticas
- Los valores atípicos influyen significativamente en los resultados, por lo que se analizaron escenarios con y sin filtrado

Decisión final:
- A través del análisis pudimos observar que hay diferencias estadísticas entre la tasa de conversión, siendo más alta en del tratamiento B (p value  < 5%) incluso eliminando los datos atípicos. El gráfico de conversión acumulada pareciera indicar una estabilidad, sin embargo, los gráficos asociados al tamaño promedio de la compra (acumulado) nos indican crecimiento, y aún no se han estabilizado. En cuanto al análisis estadístico, el tamaño de la prueba no parece presentar diferencias estadísticas. Considero que la prueba puede tomar un tiempo adicional para buscar la estabilidad en las tasas de conversión y de esta forma adoptar la estrategia que represente mayores compradores e ingresos.
