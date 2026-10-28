# Analisis-ConnectaTel
# 📊 Análisis de Comportamiento de Clientes - ConnectaTel

## 🎯 Objetivo del Proyecto
Analizar el comportamiento de consumo de servicios móviles (llamadas y mensajes) de los clientes de ConnectaTel en Latinoamérica. El propósito es identificar patrones de uso, detectar valores atípicos (outliers) y segmentar a los clientes para proponer estrategias de retención y optimización de la oferta comercial.

## 📂 Datasets Utilizados
- `plans.csv`: Catálogo de planes con sus precios y beneficios.
- `users_latam.csv`: Información demográfica de los clientes, fecha de registro y plan contratado.
- `usage.csv`: Registro detallado de la actividad (llamadas y mensajes) con sus respectivas duraciones/longitudes.

## 🛠️ Herramientas
- Python, Pandas, NumPy, Matplotlib, Seaborn.
- Entorno: Jupyter Notebook / Google Colab.

## 📋 Etapas del Análisis
1. **Auditoría de Calidad:** Revisión de nulos, detección de sentinels (`-999`, `?`) y validación de rangos de fechas.
2. **Limpieza de Datos:** Imputación de mediana en edad (excluyendo sentinels), manejo de fechas imposibles y validación de nulos estructurales (MAR) en el uso.
3. **Feature Engineering:** Creación de un perfil único por usuario (`user_profile`) agregando métricas de consumo total.
4. **Análisis Estadístico y Visual:** Histogramas por plan y boxplots para identificar la distribución y outliers de consumo.
5. **Cuantificación de Outliers:** Cálculo formal de límites IQR, conteo y porcentaje de valores atípicos, con decisión de negocio de conservarlos.
6. **Segmentación:** Clasificación de clientes por grupos de edad (Joven, Adulto, Adulto Mayor) y nivel de uso (Bajo, Medio, Alto).
7. **Insights de Negocio:** Extracción de conclusiones accionables y hipótesis comerciales.

## 🚀 Cómo ejecutar este proyecto
1. Clona este repositorio o descarga el archivo `.ipynb`.
2. Abre el notebook en [Google Colab](https://colab.research.google.com/) o en tu entorno local de Jupyter.
3. Asegúrate de que los archivos CSV estén en una carpeta llamada `/datasets/` o ajusta las rutas en la celda de carga de datos.
4. Ejecuta todas las celdas en orden (`Runtime` > `Run all`).

## 👤 Autor
Andres Felipe
