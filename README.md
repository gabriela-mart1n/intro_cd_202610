<h1 align="center">🏠 Predicción de Precios de Vivienda en Bogotá</h1>
<h3 align="center">Caso de Estudio | Ciencia de Datos · UNIANDES</h3>

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.10+-3776AB?style=for-the-badge&logo=python&logoColor=white"/>
  <img src="https://img.shields.io/badge/Jupyter-Notebook-F37626?style=for-the-badge&logo=jupyter&logoColor=white"/>
  <img src="https://img.shields.io/badge/scikit--learn-ML-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white"/>
  <img src="https://img.shields.io/badge/Estado-Completo-28a745?style=for-the-badge"/>
</p>

[![Typing SVG](https://readme-typing-svg.demolab.com?font=Comfortaa&size=60&pause=1000&color=1E3A5F&center=true&vCenter=true&width=2000&height=120&lines=Predicci%C3%B3n+de+Precios+%F0%9F%8F%A0;Machine+Learning+Aplicado;Ciencia+de+Datos+UNIANDES)](https://git.io/typing-svg)

---

## 📌 Descripción del Problema

El mercado inmobiliario en Bogotá presenta alta variabilidad en precios según localidad, estrato, área y servicios disponibles. Este proyecto busca **predecir el precio de venta de inmuebles** utilizando técnicas de Machine Learning supervisado, con base en un dataset de propiedades reales.

> **Objetivo principal:** Construir un modelo de regresión que estime el precio de una vivienda con un error menor al 10%.

---

## 🗂️ Estructura del Proyecto
```
📦 prediccion-vivienda-bogota/
├── 📂 data/
│   ├── raw/              # Datos originales sin procesar
│   └── processed/        # Datos limpios y transformados
├── 📂 notebooks/
│   ├── 01_EDA.ipynb          # Análisis exploratorio
│   ├── 02_Preprocesamiento.ipynb
│   └── 03_Modelado.ipynb
├── 📂 src/
│   ├── features.py       # Ingeniería de variables
│   └── model.py          # Entrenamiento y evaluación
├── 📂 outputs/
│   └── modelo_final.pkl  # Modelo serializado
├── requirements.txt
└── README.md
```

---

## 📊 Dataset

<details>
<summary><b>📋 Ver descripción de las variables</b></summary><br>

| Variable | Tipo | Descripción |
|---|---|---|
| `area_m2` | Numérica | Área total en metros cuadrados |
| `habitaciones` | Entera | Número de habitaciones |
| `banos` | Entera | Número de baños |
| `estrato` | Categórica | Estrato socioeconómico (1–6) |
| `localidad` | Categórica | Localidad de Bogotá |
| `parqueadero` | Booleana | Tiene parqueadero (Sí/No) |
| `precio_cop` | Numérica | **Variable objetivo** — precio en pesos colombianos |

</details>

<details>
<summary><b>🔍 Ver estadísticas descriptivas</b></summary><br>

- **Registros totales:** 8.500 propiedades
- **Periodo:** 2022 – 2024
- **Fuente:** Portal inmobiliario hipotético
- **Valores nulos:** < 2% (imputados con mediana)
- **Precio promedio:** $420.000.000 COP
- **Rango:** $90M – $2.500M COP

</details>

---

## ⚙️ Instalación y Requisitos

### 1. Clonar el repositorio
```bash
git clone https://github.com/usuario/prediccion-vivienda-bogota.git
cd prediccion-vivienda-bogota
```

### 2. Crear entorno virtual e instalar dependencias
```bash
python -m venv venv
source venv/bin/activate        # En Windows: venv\Scripts\activate
pip install -r requirements.txt
```

### 3. Ejecutar los notebooks en orden
```bash
jupyter notebook notebooks/
```

### Dependencias principales
```
pandas==2.1.0
numpy==1.26.0
scikit-learn==1.3.0
matplotlib==3.8.0
seaborn==0.13.0
xgboost==2.0.0
joblib==1.3.2
```

---

## 🧪 Metodología
```
Datos Crudos → EDA → Limpieza → Feature Engineering → Modelado → Evaluación → Despliegue
```

1. **Análisis Exploratorio (EDA):** Distribución de precios, correlaciones, outliers
2. **Preprocesamiento:** Codificación de variables categóricas, escalado, imputación
3. **Modelos entrenados:**
   - Regresión Lineal (baseline)
   - Random Forest Regressor
   - XGBoost ⭐ *(mejor desempeño)*
4. **Validación:** Cross-validation con 5 folds, métrica principal: RMSE y R²

---

## 📈 Resultados

| Modelo | R² | RMSE (COP) |
|---|---|---|
| Regresión Lineal | 0.71 | $82.000.000 |
| Random Forest | 0.88 | $51.000.000 |
| **XGBoost** | **0.93** | **$38.000.000** |

> ✅ El modelo XGBoost logró un R² de **0.93**, superando el objetivo del proyecto.

### Variables más importantes (Feature Importance)
```
area_m2        ████████████████████  38%
estrato        ██████████████        27%
localidad      █████████             18%
habitaciones   █████                  9%
parqueadero    ████                   8%
```

---

## 🏁 Conclusiones

- El **área en m²** y el **estrato** son los factores con mayor peso en la predicción del precio.
- XGBoost superó ampliamente a la regresión lineal, capturando relaciones no lineales entre variables.
- Se recomienda reentrenar el modelo cada semestre con datos nuevos dado el dinamismo del mercado.
- Como trabajo futuro: incorporar variables de ubicación geoespacial (latitud/longitud) y cercanía a TransMilenio.

---

## 👥 Autores

<p align="center">
  <a href="https://tecnologia.uniandes.edu.co/">
    <img src="https://img.shields.io/badge/Universidad_de_los_Andes-C8102E?style=for-the-badge&logo=academia&logoColor=white"/>
  </a>
  <a href="#">
    <img src="https://img.shields.io/badge/Facultad_de_Ingeniería-1E3A5F?style=for-the-badge&logo=graduation-cap&logoColor=white"/>
  </a>
</p>

| Nombre | Rol |
|---|---|
| Nombre Apellido 1 | Modelado y evaluación |
| Nombre Apellido 2 | EDA y visualización |
| Nombre Apellido 3 | Preprocesamiento y pipeline |

---

## 📄 Licencia

Este proyecto fue desarrollado con fines académicos en el marco del curso de **Ciencia de Datos** — Universidad de los Andes, 2024.

---

<img src="https://raw.githubusercontent.com/Trilokia/Trilokia/379277808c61ef204768a61bbc5d25bc7798ccf1/bottom_header.svg" />

<p align="center">
  <i>¿Tienes preguntas sobre el proyecto? Abre un <b>Issue</b> o contáctanos directamente.</i>
</p>
