# Análisis cuantitativo integral de seguridad digital

## 1. Descripción del proyecto

Este repositorio contiene el desarrollo del análisis cuantitativo integral de respuestas sobre seguridad digital. El trabajo comprende procedimientos de exploración y análisis estadístico, así como la aplicación y evaluación comparativa de modelos de aprendizaje automático para estudiar los factores asociados con la victimización digital.

## 2. Fuente de información

El análisis utiliza el dataset `SurveyResponses_DigitalSecurityAroundTheWorld.csv`, compuesto por 12.351 registros y 248 variables.

Como documentación complementaria se dispone de:

- `problema-analitico-rector.md`: documento que establece el problema analítico que orienta el estudio.
- `DataMap_DigitalSecurityAroundTheWorld.pdf`: documento de referencia para comprender las variables y las preguntas del instrumento.

La utilización y redistribución de los datos y documentos originales está sujeta a las condiciones establecidas por sus autores.

## 3. Organización del repositorio

```text
Analisis_seguridad_digital_Fase_2/
│
├── README.md
├── LICENSE
├── requirements.txt
│
├── data/
│   └── README.md
│
└── notebooks/
    ├── Analisis_Cuantitativo_Fase2_AdrianaNoguera.ipynb
    └── README.md
```

- `notebooks/`: contiene el notebook principal con el desarrollo del análisis.
- `data/`: contiene las instrucciones y documentación relacionada con los datos.
- `requirements.txt`: especifica las dependencias y versiones de las librerías.
- `LICENSE`: establece las condiciones de uso del código.

## 4. Instrucciones de ejecución

1. Clonar o descargar este repositorio.
2. Instalar Python y Jupyter Notebook.
3. Instalar las dependencias mediante:

```bash
pip install -r requirements.txt
```

4. Obtener el dataset original de acuerdo con las instrucciones y condiciones de acceso documentadas en la carpeta `data/`.
5. Ubicar el archivo CSV en la ruta de datos configurada en el notebook.
6. Abrir `notebooks/Analisis_Cuantitativo_Fase2_AdrianaNoguera.ipynb`.
7. Ejecutar las celdas en orden.

## 5. Dependencias

El análisis utiliza las siguientes librerías de Python:

- pandas 3.0.3
- numpy 2.4.6
- matplotlib 3.11.0
- seaborn 0.13.2
- scipy 1.18.0
- statsmodels 0.14.6
- scikit-learn 1.9.0
- jupyter 1.1.1

Las versiones se encuentran especificadas en `requirements.txt`.

## 6. Metodología de análisis

El desarrollo comprende el análisis exploratorio de los datos, la construcción de una variable objetivo de victimización digital, la preparación de los datos y la aplicación de tres modelos de clasificación:

- Regresión logística.
- Random Forest.
- Gradient Boosting.

La evaluación contempla métricas de clasificación, validación cruzada y procedimientos estadísticos para comparar el desempeño de los modelos.

## 7. Resultados principales

En el conjunto de prueba, Gradient Boosting obtuvo el mayor valor de F1-score (0.7995), seguido de Random Forest (0.7626) y regresión logística (0.7134).

Las comparaciones mediante bootstrap pareado mostraron diferencias en F1-score entre los tres modelos, con intervalos de confianza del 95 % que no incluyeron el cero.

## 8. Limitaciones

Los resultados deben interpretarse considerando la presencia de registros incompletos, el carácter autorreportado de la información, el desequilibrio en la distribución de la variable objetivo y la ausencia de validación externa. Los modelos permiten identificar patrones predictivos, pero no establecer relaciones causales.

## 9. Autoría y licencia

**Autora:** Adriana del Pilar Noguera Torres  
**Proyecto:** Análisis cuantitativo integral – Fase 2  
**Entorno:** Python – Jupyter Notebook  
**Licencia del código:** MIT.

La licencia MIT se aplica al código desarrollado para este proyecto y no modifica las condiciones de uso del dataset ni de los documentos originales.

## 10. Repositorio

**Repositorio público:** [Analisis_seguridad_digital_Fase_2](https://github.com/AdriNoguera/Analisis_seguridad_digital_Fase_2)
