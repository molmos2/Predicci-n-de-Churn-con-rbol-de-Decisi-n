# Prediccion-de-Churn-con-Arbol-de-Decision
Predecir si un cliente abandonará el servicio (churn) en función de sus ingresos, edad y antigüedad.
## 📊 Análisis Exploratorio de Datos (EDA)
- Visualizamos la distribución de edad, ingresos, meses como cliente.
- Exploramos correlaciones.
- Detectamos que ingresos bajos tienden a estar asociados al churn.

---

## 🏗️ Modelado Predictivo
Modelo: Árbol de Decisión (`DecisionTreeClassifier`)
- Variables: Edad, Ingresos, Meses como cliente
- Accuracy: 100% en el dataset de prueba.
- Regla principal aprendida: **Ingresos <= 1950 ➔ mayor probabilidad de churn.**

---

## 🔮 Predicción de Nuevo Cliente
### Datos del cliente:
- Edad: 30 años
- Ingresos: 1800 €
- Meses como cliente: 3

### Resultado de la predicción:
El modelo predice que **este cliente abandonará (Churn = 1)**.

---

## 📈 Interpretación del Árbol
El modelo ha aprendido que:
- Clientes con **ingresos bajos (≤ 1950)** tienen alta probabilidad de marcharse.
- Clientes con **ingresos altos (> 1950)** tienen alta probabilidad de quedarse.
