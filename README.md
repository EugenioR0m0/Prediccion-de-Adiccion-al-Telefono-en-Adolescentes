# Predicción de Adicción al Teléfono en Adolescentes 

Este proyecto utiliza el dataset [**Teen Phone Addiction and Lifestyle Survey**](https://www.kaggle.com/datasets/khushikyad001/teen-phone-addiction-and-lifestyle-survey/data) de Kaggle con el objetivo de **analizar y predecir el nivel de adicción al teléfono en adolescentes** a partir de factores relacionados con su estilo de vida, rendimiento académico y salud mental.

## Objetivo 
- Predecir la variable **`Addiction_Level`** mediante modelos de regresión.
- Identificar los factores que más influyen en la adicción (ej. horas de uso diario, horas de sueño, tiempo en redes sociales).
- Evaluar el desempeño de modelos lineales y no lineales para determinar cuál ofrece mayor precisión y generalización.

## Metodología 
1. **Exploración y limpieza de datos**
   - Eliminación de variables irrelevantes.
   - Conversión de variables categóricas a numéricas (one-hot encoding).
   - Detección y eliminación de outliers con el método de Tukey (IQR).
   - Revisión de valores nulos e imputación preventiva.

2. **Selección de características**
   - Uso de **LassoCV** para reducir colinealidad y conservar solo variables relevantes.

3. **Modelado**
   - **Regresión lineal múltiple** para interpretar efectos directos.
   - **Regresión polinomial (grado 2)** para capturar relaciones no lineales.

4. **Evaluación**
   - Validación con **train/test split**.
   - Métricas de desempeño: **R²** y **RMSE**.
   - Gráficas de residuos y valores reales vs predichos.

5. **Inferencia estadística**
   - Estimación de coeficientes con intervalos de confianza al 95%.
   - Identificación de variables estadísticamente significativas.

## Resultados 
- El **modelo lineal múltiple** explicó alrededor del **70% de la variabilidad** en `Addiction_Level`.
- El **modelo polinomial grado 2** alcanzó un **R² ≈ 0.96** y **RMSE ≈ 0.26**, mostrando gran precisión y buena capacidad de generalización.
- Principales hallazgos:
  - **Mayor uso diario, tiempo en redes sociales y gaming incrementan la adicción.**
  - **Más horas de sueño actúan como un factor protector.**

## Conclusión 
El proyecto demuestra que es posible predecir con alta precisión la adicción al teléfono en adolescentes y, al mismo tiempo, identificar los hábitos más determinantes. Estos resultados pueden ser útiles para diseñar **estrategias de prevención y concientización** sobre el uso responsable de la tecnología en jóvenes.

# Predicción de Adicción al Teléfono en Adolescentes

Este proyecto utiliza el dataset [Teen Phone Addiction and Lifestyle Survey](https://www.kaggle.com/datasets/khushikyad001/teen-phone-addiction-and-lifestyle-survey/data) con el objetivo de analizar y predecir el nivel de adicción al teléfono en adolescentes a partir de factores relacionados con su estilo de vida, rendimiento académico y salud mental.

## Objetivo
- Predecir la variable `Addiction_Level` mediante modelos de regresión.
- Identificar los factores que más influyen en la adicción (ej. horas de uso diario, horas de sueño, tiempo en redes sociales).
- Evaluar el desempeño de modelos lineales y no lineales para determinar cuál ofrece mayor precisión y generalización.

## Metodología
1. Exploración y limpieza de datos
   - Eliminación de variables irrelevantes.
   - Conversión de variables categóricas a numéricas (one-hot encoding).
   - Detección y eliminación de outliers con el método de Tukey (IQR).
   - Revisión de valores nulos e imputación preventiva.

2. Selección de características
   - Uso de LassoCV para reducir colinealidad y conservar solo variables relevantes.

3. Modelado
   - Regresión lineal múltiple para interpretar efectos directos.
   - Regresión polinomial (grado 2) para capturar relaciones no lineales.

4. Evaluación
   - Validación con train/test split.
   - Métricas de desempeño: R² y RMSE.
   - Gráficas de residuos y valores reales vs predichos.

5. Inferencia estadística
   - Estimación de coeficientes con intervalos de confianza al 95%.
   - Identificación de variables estadísticamente significativas.

## Resultados
- El modelo lineal múltiple explicó alrededor del 70% de la variabilidad en `Addiction_Level`.
- El modelo polinomial grado 2 alcanzó un R² ≈ 0.96 y RMSE ≈ 0.26, mostrando gran precisión y buena capacidad de generalización.
- Principales hallazgos:
  - Mayor uso diario, tiempo en redes sociales y gaming incrementan la adicción.
  - Más horas de sueño actúan como un factor protector.

## Conclusión
El proyecto demuestra que es posible predecir con alta precisión la adicción al teléfono en adolescentes y, al mismo tiempo, identificar los hábitos más determinantes. Estos resultados pueden ser útiles para diseñar estrategias de prevención y concientización sobre el uso responsable de la tecnología en jóvenes.

## Archivos del repositorio
- [Prediccion_Adiccion_Telefono.ipynb](Prediccion_Adiccion_Telefono.ipynb) - Notebook con el código, gráficas y explicaciones.
- [Prediccion_Adiccion_Telefono.html](Prediccion_Adiccion_Telefono.html) - Versión exportada del notebook en formato HTML para visualizar sin ejecutar código.
- [teen_phone_addiction_dataset.csv](teen_phone_addiction_dataset.csv) - Base de datos original utilizada para el análisis.
