# A3.1-SVM y Multiple Testing (Khan)

## Índice
1. [Dataset](./A3.1%20Khan.csv)
2. [Notebook](./A3.1%20SVM%20y%20multiple%20testing.ipynb)
3. [Reporte HTML](./A3.1%20SVM%20y%20multiple%20testing.html)
4. [README](./README.md)

---

## Descripción
Este proyecto analiza un dataset de expresión génica del estudio Khan, que contiene **83 muestras** y **2308 genes** como variables de entrada. La variable de salida tiene valores del 1 al 4, representando distintos tipos de cáncer.  

El trabajo realizado en la notebook incluye los siguientes pasos:

1. **Revisión de datos:** Se importan los datos y se verifica la ausencia de valores faltantes. Se calculan diferencias de medias entre clases, identificando los genes con mayor variación y discutiendo su posible relevancia biológica.  
2. **Pruebas estadísticas y corrección por múltiples comparaciones:** Se calculan los estadísticos t y p-values para comparar clases específicas y se aplican correcciones de Bonferroni, Holm y Benjamini-Hochberg para identificar genes con expresión significativamente distinta entre clases.  
3. **Análisis de varianza (ANOVA):** Se realiza ANOVA para comparar la expresión de genes entre las 4 clases, evaluando qué genes presentan diferencias significativas de manera global.  
4. **Modelos SVM:** Se separan los datos en conjuntos de entrenamiento y prueba, y se entrenan **SVM con kernel lineal, polinómico (orden 3) y RBF**. La selección de características se basa en los genes previamente identificados como relevantes, con el fin de reducir tiempo de cómputo.  
5. **Evaluación de desempeño:** Se calculan métricas de desempeño para los tres modelos y se comparan sus resultados, analizando la capacidad de clasificación de cada kernel y posibles indicios de sobreajuste.  

Se utilizan las librerías: **pandas, numpy, matplotlib, seaborn, scikit-learn, scipy y statsmodels**.
