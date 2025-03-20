## 📌 Descripción del Proyecto
Este proyecto busca predecir el peso de los pollos en una empresa avícola con más de 40 años en el mercado. El objetivo es optimizar la toma de decisiones en el proceso de beneficio de las aves mediante técnicas de Machine Learning, asegurando que alcancen el peso comercial ideal.

Se utilizó la metodología **CRISP-DM** para estructurar el análisis y desarrollo del modelo, pasando por las etapas de comprensión del negocio, análisis exploratorio, preprocesamiento, modelado y evaluación.

## 📊 Dataset
El conjunto de datos fue extraído del sistema de información de la empresa avícola e incluye variables relevantes como:
- **Variables numéricas:** Peso, PesoGr, Consumo, Unidades, Edad, Temperatura, Densidad, Consumo Agua, Humedad, HorasLuz.
- **Variables categóricas:** Tipo de alimento, Sexo, Tipo de granja, Ciudad, Departamento.
- **No se encontraron valores nulos**, pero sí valores atípicos que fueron tratados en la fase de preprocesamiento.

## 🔍 Análisis de Datos
- **Análisis exploratorio:** Se estudiaron distribuciones, valores atípicos y correlaciones.
- **Selección de variables:** Se aplicaron técnicas como *Mutual Information*, *VIF*, *SelectKBest*, *LASSO* y *RFE* para identificar las variables con mayor impacto en la predicción del peso de los pollos.
- **Eliminación de valores atípicos:** Se utilizó *Z-score (±3)* para filtrar datos extremos en las variables con alta dispersión.

## 🛠️ Tecnologías Utilizadas
- **Lenguaje:** Python  
- **Bibliotecas:** Pandas, NumPy, Scikit-Learn, XGBoost, Matplotlib, Seaborn  
- **Modelos utilizados:**  
  - **XGBoost** (modelo principal de predicción)  
  - **Regresión Lineal**  
  - **Clusterización K-Means** (análisis complementario)  
- **Evaluación de modelos:** Precisión, matriz de confusión, método del codo, puntaje de silueta.

## 🔬 Metodología CRISP-DM
1. **Comprensión del negocio:** Identificar el impacto del peso de las aves en la rentabilidad de la empresa.  
2. **Comprensión de los datos:** Análisis exploratorio, identificación de correlaciones y selección de variables clave.  
3. **Preparación de los datos:** Limpieza, eliminación de valores atípicos y transformación de variables.  
4. **Modelado de los datos:** Entrenamiento de modelos supervisados y no supervisados.  
5. **Evaluación del modelo:** Comparación de métricas para seleccionar la mejor solución.  

## 📌 Resultados
- **El modelo XGBoost alcanzó una precisión del 92% en la predicción del peso de los pollos.**  
- **Se identificaron las variables clave para la predicción:** *Consumo, PesoGr, Unidades, Edad y Consumo de Agua.*  
- **El método del codo y la puntuación de silueta** fueron utilizados para evaluar la clusterización K-Means.  

## 🚀 Próximos pasos
- Implementación de un dashboard interactivo en **Power BI** para la visualización en tiempo real de los datos.  
- Optimización del modelo con técnicas de **feature engineering** y validación cruzada.  
- Exploración de modelos más avanzados como **redes neuronales**.  

## 📎 Requisitos para ejecutar el código
Para correr el código, instala las dependencias con:
```bash
pip install pandas numpy scikit-learn xgboost matplotlib seaborn
