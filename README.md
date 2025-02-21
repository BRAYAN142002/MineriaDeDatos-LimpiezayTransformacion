# 📊 Limpieza y Transformación de Datos – Google Colab  

Este repositorio contiene unos **Notebook en Google Colab** donde se realiza un proceso detallado de **limpieza y transformación de datos** antes de su uso en minería de datos. La calidad de los datos es clave para garantizar un análisis preciso y modelos efectivos.  

---

## ✨ Objetivos  

✅ Identificar y manejar valores nulos y atípicos para evitar sesgos en el análisis.  
✅ Corregir errores en los datos como formatos incorrectos o valores inconsistentes.  
✅ Estandarizar y transformar variables para mejorar la coherencia del dataset.  
✅ Aplicar técnicas de codificación (**One-Hot Encoding, Label Encoding**) si es necesario.  
✅ Detectar y eliminar datos duplicados para evitar redundancias.  
✅ Verificar la distribución de los datos y ajustar si es necesario (**log transform, Box-Cox**).  
✅ **Generar la vista minable**, es decir, el dataset listo para su uso en minería de datos.  

---

## 🛠️ Tecnologías utilizadas  

- **Python** (pandas, numpy, seaborn, matplotlib, scikit-learn)  
- **Google Colab**  

---

## 📌 Pasos realizados en el Notebook  

### 📥 1. Carga de datos  
- Se carga el dataset desde su fuente original (**CSV**).  
- Se revisa la estructura de los datos y se convierten a un formato adecuado.  

### 🔎 2. Análisis exploratorio inicial (EDA)  
- **Resumen estadístico** de las variables numéricas y categóricas.  
- **Revisión de datos faltantes** y su impacto en el análisis.  
- **Identificación de valores inconsistentes o erróneos**.  

### ⚠️ 3. Manejo de valores nulos  
- **Estrategias de imputación**:  
  - Para variables numéricas: **media, mediana o interpolación**.  
  - Para variables categóricas: **moda o categoría "desconocida"**.  
- Eliminación de filas o columnas si el porcentaje de valores nulos es alto.  

### 📉 4. Detección y tratamiento de valores atípicos  
- Uso de técnicas como el **rango intercuartílico (IQR)** y **z-score**.  
- Opciones: **eliminación, transformación o reemplazo por valores ajustados**.  

### 🔄 5. Corrección de datos erróneos  
- **Conversión de tipos de datos** (ej. strings a fechas, enteros a flotantes).  
- **Normalización de formatos** (ej. fechas, texto en minúsculas, eliminación de espacios).  

### 🏷️ 6. Transformaciones necesarias  
- **One-Hot Encoding** para variables categóricas.  
- **Label Encoding** si es adecuado para modelos específicos.  
- **Mapeo de valores** para categorías con errores ortográficos o formatos diferentes.  

### 📊 7. Verificación y reducción de dimensionalidad  
- Eliminación de **columnas irrelevantes o redundantes**.  
- Análisis de **correlación** para evitar multicolinealidad.  
- Aplicación de **PCA (opcional)** para reducir dimensiones si el dataset es grande.  

### 🔀 8. Manejo de datos duplicados  
- **Identificación y eliminación** de filas duplicadas para evitar sesgos.  

### 🔧 9. Ajuste de la distribución de datos (si es necesario)  
- **Transformación logarítmica** para datos sesgados positivamente.  
- **Box-Cox transformation** para normalizar distribuciones.  

### 📤 10. Generación de la vista minable  
- **Exportación del dataset limpio** en un nuevo archivo listo para el análisis.  
