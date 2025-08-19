# Telecom-X-2da-parte
Claro, Miqueas. Aquí tenés una versión adaptada para el `README.md` de GitHub, con un tono más claro, estructurado y contextualizado para un repositorio público. Incluye el nombre del proyecto, su pertenencia al programa ONE Oracle Next Education junto a Alura Latam, y está optimizado para que cualquier visitante entienda rápidamente el propósito y alcance del trabajo:

---

# 📊 Telecom X Parte 2 — Análisis de Cancelación de Clientes (Churn)

Este proyecto forma parte del programa **ONE Oracle Next Education** en colaboración con **Alura Latam**, y documenta el análisis completo de cancelación de clientes en una empresa de telecomunicaciones. El objetivo principal es identificar los factores que influyen en el abandono del servicio (`Churn`) y construir modelos predictivos que permitan anticipar este comportamiento.

---

## 🚀 Objetivos del Proyecto

- Detectar patrones asociados a la cancelación de clientes.
- Construir modelos de clasificación que predigan el churn con alta precisión.
- Proponer estrategias de retención basadas en los hallazgos del análisis.

---

## 🧪 Metodología Aplicada

### 1. **Importación y Carga de Datos**
- Se utilizó `pandas` para cargar el dataset desde una URL pública.

### 2. **Limpieza y Preprocesamiento**
- Eliminación de columnas irrelevantes (`customerID`, `gender`).
- Unificación de valores como `"No internet service"` a `"No"` en variables categóricas.
- Aplicación de One-Hot Encoding para convertir variables categóricas en numéricas.
- Eliminación de registros con valores nulos en `Charges.Total`.

### 3. **Análisis Exploratorio**
- Visualización de relaciones entre variables clave (`tenure`, `Charges.Total`) y la variable objetivo (`Churn_Yes`) mediante boxplots y stripplots.

### 4. **Análisis de Correlación**
- Generación de un heatmap para identificar variables con alta correlación con la cancelación.

### 5. **Multicolinealidad**
- Cálculo del VIF (Variance Inflation Factor) para detectar redundancias entre variables.
- Eliminación de variables con VIF elevado para mejorar la estabilidad del modelo.

### 6. **Balanceo de Clases**
- Aplicación de SMOTE (Synthetic Minority Over-sampling Technique) para equilibrar la proporción entre clientes que cancelan y los que no.

### 7. **Modelado Predictivo**
- División del dataset en conjuntos de entrenamiento y prueba.
- Escalado de variables numéricas con `StandardScaler`.
- Entrenamiento de dos modelos: **Regresión Logística** y **Random Forest**.

### 8. **Evaluación de Modelos**
- Métricas utilizadas: Exactitud, ROC AUC, Matriz de Confusión y Reporte de Clasificación.
- Visualización comparativa mediante curvas ROC.

### 9. **Factores Clave y Estrategias de Retención**
- Identificación de variables más influyentes: tipo de contrato, tiempo de permanencia (`tenure`), método de pago, servicios adicionales.
- Propuestas de retención: incentivos para contratos largos, mejora de servicios de fibra óptica, promoción de soporte técnico y seguridad online.

---

## 📁 Estructura del Repositorio

- `Telecom__X_2da_parte.ipynb`: Notebook principal con todo el análisis.
- `telecomx.csv`: Dataset utilizado.
- `README.md`: Documento explicativo del proyecto.

---

## 📌 Conclusión

Este proyecto demuestra cómo aplicar técnicas de ciencia de datos para abordar problemas reales de negocio. Los modelos desarrollados permiten identificar clientes en riesgo de cancelación y orientar estrategias de fidelización más efectivas.

---

¿Querés que lo traduzca al inglés para hacerlo bilingüe o que agregue una sección de instalación y ejecución para usuarios que quieran replicarlo en Colab?
