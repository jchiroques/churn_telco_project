# Telco Customer Churn Prediction

## 📌 1. Descripción del Proyecto

Este proyecto tiene como objetivo predecir si un cliente de una compañía de telecomunicaciones abandonará el servicio (churn), utilizando técnicas de Machine Learning. El enfoque sigue la metodología CRISP-DM e incluye el flujo completo desde el entendimiento del negocio hasta el despliegue en una aplicación interactiva con Streamlit.

---

## 🎯 2. Objetivo del Negocio

Las empresas de telecomunicaciones pierden ingresos cuando un cliente se da de baja. Un modelo predictivo permite:

* Identificar clientes con alta probabilidad de churn.
* Tomar acciones preventivas.
* Reducir costos de adquisición y retención.

**Pregunta de negocio:**
¿Podemos predecir qué clientes se irán para actuar antes de que ocurra?

---

## 📊 3. Dataset

El dataset contiene información de clientes como:

* Tipo de servicios contratados
* Método de pago
* Tenencia
* Características demográficas
* Historial de facturación

Variable objetivo:

* `Churn` → cliente abandona (Sí/No)

---

## 🔍 4. Entendimiento de la Data

Antes de modelar, se analizan:

* Distribuciones de variables
* Valores faltantes
* Proporción de clases (suele estar desbalanceado)
* Relación entre variables y la variable objetivo

---

## 🧹 5. Preparación de Datos

Las principales tareas realizadas incluyen:

* Estandarización y limpieza
* Transformación de variables categóricas
* Codificación adecuada
* Manejo del desbalance en las clases
* División en entrenamiento y prueba

---

## 🤖 6. Modelamiento

Se probaron diversos modelos de clasificación, por ejemplo:

* Regresión logística
* Árboles de decisión
* Random Forest
* Gradient Boosting

Se selecciona el mejor basándose en desempeño y simplicidad de interpretación.

---

## 📈 7. Evaluación

El foco está en métricas alineadas con el negocio, como:

* Recall
* Precision
* F1-score
* Matriz de confusión
* Curva ROC AUC

El recall es crítico en este problema, ya que perder un cliente cuesta más que contactar a uno que no se irá.

---

## 🖥️ 8. Despliegue (Streamlit)

El modelo se implementó en una interfaz interactiva con Streamlit donde el evaluador puede:

* Ingresar características de un cliente
* Obtener la predicción de churn
* Visualizar métricas del modelo

---

## 📡 9. Monitoreo (Conceptual)

Se plantean acciones recomendadas para producción:

* Seguimiento de métricas en el tiempo
* Reentrenamiento periódico
* Evaluación de drift en la data

---

## 📁 10. Estructura del Proyecto

```
├── data/
│   ├── raw/
│   └── processed/
├── notebooks/
├── src/
│   ├── data_preparation.py
│   ├── train_model.py
│   ├── evaluate.py
│   └── app_streamlit.py
├── models/
├── requirements.txt
└── README.md
```

---

## 🚀 11. Cómo Ejecutar

1. Clonar el repositorio
2. Crear entorno virtual e instalar dependencias desde `requirements.txt`
3. Ejecutar exploración y entrenamiento
4. Ini
