### 📝 Análisis de Datos de Vinos de Argentina e Italia

## 📋 Descripción del Proyecto
Este proyecto de Data Science tiene como objetivo analizar un conjunto de datos sobre vinos de Argentina e Italia. La finalidad es responder preguntas clave relacionadas con las características, precios y puntuaciones de los vinos, identificando patrones que puedan ser útiles para la industria vitivinícola o para los amantes del vino.

## 🎯 Motivación y Audiencia
La motivación detrás de este proyecto es explorar las diferencias y similitudes en las características de los vinos de dos de las regiones vitivinícolas más importantes del mundo. La audiencia principal incluye:

- Profesionales del sector vitivinícola interesados en tendencias de mercado.
- Consumidores de vino que desean conocer más sobre las opciones disponibles.
- Analistas de datos interesados en la aplicación de técnicas de análisis en la industria alimentaria.

## 🔍 Preguntas e Hipótesis

**Preguntas clave:**
- ¿Cuáles son las variedades de uva más populares en Argentina e Italia?
- ¿Qué provincias producen los vinos mejor puntuados?
- ¿Existe una relación entre el precio y la puntuación de los vinos?
- ¿Cómo se distribuyen los precios en ambas regiones?

**Hipótesis a validar:**
- Las variedades de uva más populares son Malbec en Argentina y Sangiovese en Italia.
- Los vinos más caros tienden a obtener mejores puntuaciones.
- Mendoza y Toscana producen los vinos con las puntuaciones más altas.
- Los precios de los vinos italianos son más variables que los argentinos.

## 📊 Metodología
1. **Adquisición de datos:** Se utilizaron bases de datos públicas para obtener la información sobre vinos.
2. **Limpieza y transformación:**
   - Manejo de valores nulos.
   - Eliminación de columnas irrelevantes.
3. **Análisis exploratorio de datos (EDA):**
   - Estadísticas descriptivas.
   - Visualizaciones como gráficos de barra, dispersión y distribuciones.
4. **Entrenamiento de Modelos de Machine Learning:**
   - Modelos evaluados: Regresión Lineal, Random Forest, Gradient Boosting, XGBoost y LightGBM.
   - Se encontró que **LightGBM optimizado** es el mejor modelo.
5. **Interpretación de Resultados:**
   - Análisis de importancia de características.
   - Evaluación de predicciones y distribución de errores.

## 🛠️ Ingeniería de Atributos
- **Codificación de Variables Categóricas:** Se aplicó Label Encoding a `province`, `variety` y `winery`.
- **Normalización de Variables Numéricas:** Se utilizó StandardScaler para normalizar `price`.
- **Manejo de Valores Nulos:** Se completaron valores faltantes en `price`, `points`, `designation`, `province`, `variety` y `winery`.

## 🤖 Modelos de Machine Learning
- **Regresión Lineal:** Modelo base, con bajo desempeño.
- **Random Forest:** R² de 0.5085 tras optimización.
- **Gradient Boosting:** R² de 0.4625.
- **XGBoost:** R² de 0.5053.
- **LightGBM:** Mejor modelo con **R² de 0.5146** y **MSE de 3.94**.

## 🔍 Gráficos Claves
- **Distribución de Puntuaciones:** Histograma con KDE para visualizar las calificaciones más comunes.
- **Relación Precio-Puntuación:** Scatter plot con tendencia positiva pero no estrictamente lineal.
- **Importancia de Características:** Gráfico de barras mostrando los atributos más influyentes.
- **Predicciones vs. Valores Reales:** Scatter plot para evaluar la precisión del modelo.
- **Distribución de Errores:** Histograma para analizar sesgos o sobreajuste.

## 🌟 Conclusiones
- **LightGBM optimizado es el mejor modelo** con un **R² de 0.5146**.
- **Las variables clave en la predicción son `price`, `province` y `variety`**.
- **Los precios de los vinos italianos tienen mayor variabilidad que los argentinos**.
- **Se pueden mejorar los modelos incluyendo más atributos, como clima o tipo de suelo**.

## 💪 Contribuciones
📅 Se aceptan sugerencias y contribuciones para mejorar el análisis.

