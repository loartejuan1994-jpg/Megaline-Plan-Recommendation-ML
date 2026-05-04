 # 🤖 Sistema de Recomendación de Planes Megaline

## 📋 Descripción
Proyecto de Machine Learning que recomienda el plan correcto 
(Smart o Ultra) a los clientes de Megaline, basándose en su 
comportamiento de uso mensual.

## 🎯 Objetivo
Desarrollar un modelo de clasificación que analice el comportamiento 
de los clientes y recomiende automáticamente el plan más adecuado, 
superando un umbral mínimo de exactitud del 75%.

## 📊 Dataset
- **3,214 registros** de comportamiento mensual de clientes
- **Variables:** llamadas, minutos, mensajes y MB consumidos
- **Objetivo:** plan actual del cliente (Smart=0 / Ultra=1)

## 🔧 Modelos Evaluados
| Modelo | Exactitud |
|---|---|
| Bosque Aleatorio | 79.94% ✅ |
| Árbol de Decisión | 77.45% |
| Regresión Logística | 72.94% |

## 🏆 Resultado Final
- **Modelo seleccionado:** Random Forest (Bosque Aleatorio)
- **Hiperparámetros óptimos:** n_estimators=150, max_depth=10 (GridSearchCV)
- **Exactitud final:** 79.78% en conjunto de prueba
- **ROC-AUC:** 80.03%

## 📌 Variables más importantes
- `mb_used` → 35.49% ← la más determinante
- `minutes` → 22.69%
- `messages` → 22.00%
- `calls` → 19.82%

## 🛠️ Tecnologías utilizadas
- Python
- Pandas
- Scikit-learn
- Matplotlib / Seaborn
- Jupyter Notebook

## 📁 Archivos
- `Project_10_Sistema_de_Recomendación_de_Planes_Megaline.ipynb` → Proyecto completo
- `users_behavior.csv` → Dataset
