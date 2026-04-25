# Experimento-A-B-en-p-gina-de-inicio

📊 Proyecto: Optimización de Conversión mediante A/B Testing

📝 Descripción del ProyectoEste proyecto analiza los resultados de un experimento A/B realizado para evaluar dos versiones de una landing page (Versión A vs. Versión B). El objetivo principal es determinar qué versión maximiza tanto la tasa de conversión como el valor económico (ticket promedio) por usuario.

Además, se realizó un análisis segmentado por fuente de tráfico y tipo de usuario para identificar patrones de comportamiento que ayuden a optimizar la estrategia de marketing.

🛠️ Tecnologías Utilizadas
   * Python (Pandas, NumPy)
   * Estadística: Scipy (T-test de Welch, Z-test, Chi-cuadrado, Prueba de Levene)
   * Visualización: Matplotlib, Seaborn
 

📈 Metodología y Resultados

1. Calidad de Datos (Data Cleaning)

Se validó la integridad de 40,000 registros, confirmando:

  * 0% de valores nulos y duplicados.
  * Consistencia lógica: No existen gastos registrados sin una conversión marcada.
  * Temporalidad: Datos continuos sin sesgos por interrupciones técnicas.

2. Análisis del Gasto Promedio (Valor Económico)
 * Hipótesis: Comparar si la Página B genera mayores ingresos que la A.
 * Prueba de Levene: Valor p < 0.05 (Varianzas heterogéneas).
 * Prueba T de Welch: Valor p = 3.62e-21.
 * Resultado: La Página B incrementó el gasto promedio de $61.09 a $68.75, una diferencia estadísticamente significativa.

3. Tasa de Conversión (Eficiencia)
 * Hipótesis: Evaluar si la Página B convierte más visitantes en clientes.
 * Prueba Z de Proporciones: Valor p = 0.0000.
 * Resultado: La Página B es superior, logrando una tasa de conversión significativamente más alta que la versión de control.

4. Análisis de Segmentación (Fuentes y Usuarios)
 * Fuente de Tráfico: Se encontró una asociación significativa ($\chi^2$, p=0.0341). Los canales de Email y Ads son los más efectivos.
 * Tipo de Usuario: No se encontró asociación significativa ($\chi^2$, p=0.4736). La página convierte por igual a usuarios nuevos y recurrentes.

💡 Conclusiones y Recomendaciones
  * Implementación: Se recomienda migrar al 100% a la Página B debido a su superioridad en volumen y valor de ventas.
  * Estrategia de Marketing: Priorizar la inversión en Email Marketing, ya que atrae usuarios con mayor probabilidad de conversión.
  * Escalabilidad: Mantener esfuerzos en adquisición de tráfico nuevo, dado que responden con la misma efectividad que los usuarios recurrentes.
