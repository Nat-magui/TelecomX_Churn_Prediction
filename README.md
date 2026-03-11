# 📊 Telecom X – Predicción de Cancelación de Clientes (Churn)

## 📌 Descripción del proyecto

Este proyecto forma parte del **Challenge Telecom X – Parte 2** del programa **Oracle Next Education (ONE) en colaboración con Alura Latam**.

El objetivo del proyecto es analizar el comportamiento de los clientes de **Telecom X** y desarrollar **modelos de Machine Learning capaces de predecir la cancelación de clientes (churn)**.

La predicción del churn permite a las empresas **anticiparse a la pérdida de clientes y aplicar estrategias de retención**, mejorando la satisfacción del usuario y reduciendo el impacto económico asociado a la cancelación de servicios.

---

# 🎯 Objetivos del análisis

El proyecto busca:

* Analizar los factores que influyen en la **cancelación de clientes**
* Construir **modelos predictivos de churn**
* Comparar diferentes algoritmos de **Machine Learning**
* Identificar **variables clave que explican la cancelación**
* Proponer **estrategias de retención basadas en datos**

---

# 📂 Estructura del proyecto

```
TelecomX_Churn_Prediction/
│
├── TelecomX_Churn_Prediction.ipynb
│   Notebook principal con el análisis completo
│
├── datos_tratados.csv
│   Dataset procesado en la Parte 1 del challenge
│
└── README.md
    Documentación del proyecto
```

El análisis se desarrolla completamente dentro del **notebook**, siguiendo un pipeline de ciencia de datos.

---

# 🔎 Pipeline de análisis

El proyecto sigue las principales etapas de un flujo de **Data Science**:

## 1️⃣ Preparación de datos

* Carga del dataset tratado
* Eliminación de variables irrelevantes (customerID)
* Codificación de variables categóricas mediante **One-Hot Encoding**
* Verificación de distribución de la variable objetivo (**Churn**)

---

## 2️⃣ Análisis exploratorio

Se analizaron relaciones entre variables y churn mediante:

* matriz de **correlación**
* **boxplots**
* análisis dirigido de variables relevantes

Variables analizadas:

* tenure
* MonthlyCharges
* TotalCharges
* tipo de contrato
* método de pago

---

## 3️⃣ Modelado predictivo

Se implementaron dos modelos de clasificación:

### 🔹 Logistic Regression

Modelo lineal utilizado para clasificación binaria.

Se aplicó **normalización de datos** utilizando `StandardScaler`.

---

### 🔹 Random Forest

Modelo basado en **ensamble de árboles de decisión**, capaz de capturar relaciones no lineales entre variables.

Este modelo no requiere normalización.

---

## 4️⃣ Evaluación de modelos

Los modelos fueron evaluados utilizando:

* Accuracy
* Precision
* Recall
* F1-score
* Matriz de confusión

### Resultados principales

| Modelo              | Accuracy | Recall (Churn) |
| ------------------- | -------- | -------------- |
| Logistic Regression | ~0.81    | ~0.54          |
| Random Forest       | ~0.79    | ~0.46          |

El modelo de **Regresión Logística mostró una mejor capacidad para detectar clientes que cancelan**, lo cual es especialmente relevante en problemas de churn.

---

## 5️⃣ Importancia de variables

Se analizaron las variables más relevantes mediante **Random Forest Feature Importance**.

Variables más influyentes:

* TotalCharges
* tenure
* MonthlyCharges
* Cuentas_Diarias
* Contract_Two year
* PaymentMethod_Electronic check

Estos factores muestran que la cancelación está fuertemente relacionada con:

* antigüedad del cliente
* nivel de gasto
* condiciones contractuales

---

# 💡 Insights principales

El análisis permitió identificar varios patrones en el comportamiento de los clientes:

* Clientes con **menor antigüedad (tenure)** presentan mayor probabilidad de cancelación.
* Clientes con **cargos mensuales más altos** tienden a cancelar con mayor frecuencia.
* Los **contratos de mayor duración** reducen significativamente la probabilidad de churn.
* Factores como el **método de pago** y la **cantidad de servicios contratados** también influyen en el comportamiento del cliente.

---

# 📈 Recomendaciones estratégicas

A partir del análisis se proponen algunas estrategias para reducir la cancelación de clientes:

* Incentivar **contratos de largo plazo**
* Implementar **programas de onboarding para nuevos clientes**
* Analizar la **estructura de precios y planes**
* Utilizar el modelo predictivo para **identificar clientes con alto riesgo de churn**

Estas acciones permitirían a Telecom X **anticiparse a la cancelación y mejorar la retención de clientes**.

---

# 🧠 Tecnologías utilizadas

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn
* Google Colab

---

# 📚 Aprendizajes del proyecto

Este proyecto permitió aplicar conceptos clave de:

* análisis exploratorio de datos
* preparación de datasets
* modelos de clasificación
* evaluación de modelos
* interpretación de resultados de machine learning
* aplicación de ciencia de datos a problemas de negocio

---

# 🚀 Autor

Proyecto desarrollado por **Magalí Aldana Suárez**

Programa **Oracle Next Education (ONE) – Data Science**

---

# 🔗 Challenge

Proyecto realizado como parte del desafío:

**Telecom X – Predicción de Cancelación de Clientes (Churn)**

Programa **Oracle Next Education + Alura Latam**
