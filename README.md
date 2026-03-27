<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0d4a2a&height=200&section=header&animation=twinkling" width="100%"/>

# Predicción de Deserción Escolar en Bogotá
### Taller 05 · Introducción a la Ciencia de Datos · Grupo 3
<br/>

[![Typing SVG](https://readme-typing-svg.demolab.com?font=Comfortaa&size=22&pause=1200&color=0d4a2a&center=true&vCenter=true&width=1000&height=60&lines=Estudiantes)](https://git.io/typing-svg)

**María Gabriela Martín Avila** ·  **Tomas Pulgarin Castañeda** ·  
**Alejandro Rojas Martínez** ·  **Emmily Rodriguez Grisales**

 **Docente:** Rodrigo Taborda

<br/>


[![Typing SVG](https://readme-typing-svg.demolab.com?font=Comfortaa&size=22&pause=1200&color=20b267&center=true&vCenter=true&width=1000&height=60&lines=Detectando+riesgo+antes+de+que+sea+tarde...;Ciencia+de+Datos+al+servicio+de+la+educaci%C3%B3n;Ciencia+de+datos+con+impacto+social+real)](https://git.io/typing-svg)


<br/>

<img src="https://img.shields.io/badge/Deserción_Escolar-Bogotá-0d4a2a?style=for-the-badge&logo=google-maps&logoColor=white"/>
<img src="https://img.shields.io/badge/Estudiantes_Analizados-42.500-1a6b3c?style=for-the-badge&logo=graduation-cap&logoColor=white"/>
<img src="https://img.shields.io/badge/Colegios_Públicos-214-20b267?style=for-the-badge&logo=school&logoColor=white"/>
<img src="https://img.shields.io/badge/Periodo-2019_al_2023-1a6b3c?style=for-the-badge&logo=calendar&logoColor=white"/>

<br/><br/>

> *"Cada estudiante que abandona el colegio representa una cadena de oportunidades perdidas. Este proyecto usa datos para romper ese ciclo."*

<br/>

---
<div align="center">
<img src="https://images.unsplash.com/photo-1580582932707-520aed937b7b?w=1200&h=300&fit=crop" width="100%" style="border-radius: 10px;"/>
</div>

## Variables a Estudiar

[![Typing SVG](https://readme-typing-svg.demolab.com?font=Comfortaa&size=22&pause=1200&color=0d4a2a&center=true&vCenter=true&width=1000&height=60&lines=Inasistencias+al+mes+📅;Promedio+académico+📊;Distancia+al+colegio+📍;Situación+laboral+💼;Estrato+socioeconómico+🏘️;Tipo+de+hogar+👨‍👩‍👧)](https://git.io/typing-svg)

| # | Variable | Descripción |
|---|---|---|
| 1 |  Inasistencias al mes | Cuántos días faltó el estudiante en el mes |
| 2 |  Promedio académico | Rendimiento general del estudiante (escala 0–5) |
| 3 |  Distancia al colegio | Qué tan lejos vive el estudiante de su institución |
| 4 |  Repitencia | Si el estudiante ha repetido algún año escolar |
| 5 |  Situación laboral | Si el estudiante trabaja además de estudiar |
| 6 |  Estrato socioeconómico | Nivel socioeconómico del hogar (1 al 6) |
| 7 |  Tipo de hogar | Con quién vive el estudiante (biparental, monoparental, etc.) |
| 8 |  Acceso a internet | Si el estudiante tiene conexión en casa |
| 9 |  Localidad | En qué zona de Bogotá vive |
| 10 |  Deserción | Verificar si el estudiante abandonó o no el colegio |
<div align="center">
 
---
 
## 🔬 Metodología
 
[![Typing SVG](https://readme-typing-svg.demolab.com?font=Comfortaa&size=22&pause=1200&color=0d4a2a&center=true&vCenter=true&width=1000&height=60&lines=¿Cómo+le+decimos+a+los+datos+que+nos+cuenten+una+historia%3F;7+pasos+para+anticipar+la+deserción+escolar+📚)](https://git.io/typing-svg)
 
> *Cada fase es un escalón. Juntas, convierten filas en una base de datos en alertas que salvan trayectorias de vida.*
 
---
 
### Fase 1 · Entendimiento del Problema 🧭
 
<img src="https://img.shields.io/badge/Etapa-Estratégica-0d4a2a?style=for-the-badge&logoColor=white"/>
 
Antes de tocar un solo dato, nos preguntamos: **¿qué queremos resolver realmente?**
 
El Ministerio de Educación necesita anticiparse — no reaccionar. Aquí definimos la pregunta central del proyecto, el tipo de solución (un modelo de clasificación), quiénes van a usar los resultados (orientadores escolares), y qué significaría que el modelo funcione bien. También establecemos el horizonte de predicción: **3 meses antes** de que ocurra la deserción.
 
```
🎯 Pregunta clave:
¿Puede un modelo de datos identificar, al inicio del período,
qué estudiante tiene riesgo de no terminar el año?
```
 
---
 
### Fase 2 · Recolección de Datos 🗄️
 
<img src="https://img.shields.io/badge/Etapa-Fundacional-1a6b3c?style=for-the-badge&logoColor=white"/>
 
Los datos vienen del **Sistema Educativo Distrital (SED)** y el **Ministerio de Educación Nacional (MEN)**. Aquí identificamos qué registros históricos tenemos disponibles y cuáles variables son relevantes para el problema.
 
Trabajamos con información de **42.500 estudiantes** de bachillerato en **214 colegios públicos** de Bogotá entre 2019 y 2023. Cada registro es una historia: cuánto faltó, cómo le fue, dónde vive, con quién vive.
 
```
📦 Fuentes principales:
   ├── SIMAT (Sistema Integrado de Matrícula)
   ├── Registros de calificaciones por período
   ├── Encuestas socioeconómicas estudiantiles
   └── Datos de geolocalización por localidad
```
 
---
 
### Fase 3 · Exploración de los Datos (EDA) 🔍
 
<img src="https://img.shields.io/badge/Etapa-Descubrimiento-20b267?style=for-the-badge&logoColor=white"/>
 
Antes de construir cualquier modelo, **escuchamos lo que los datos tienen para decir**. En esta fase hacemos preguntas, graficamos distribuciones, buscamos patrones y encontramos los primeros indicios de qué variables importan más.
 
Algunos hallazgos que esperamos descubrir:
 
| 🔎 Pregunta | 📊 Lo que buscamos |
|---|---|
| ¿Cuándo empieza a caer la asistencia? | Meses previos a la deserción |
| ¿Qué localidades concentran más casos? | Mapas de riesgo por zona |
| ¿Trabajar afecta el rendimiento? | Relación trabajo–notas–ausencias |
| ¿Qué tan desbalanceados están los datos? | % de desertores vs. no desertores |
 
> 💡 *El EDA no es un trámite. Es donde el analista aprende a ver lo que los números esconden.*
 
---
 
### Fase 4 · Preparación de los Datos ⚙️
 
<img src="https://img.shields.io/badge/Etapa-Transformación-0d4a2a?style=for-the-badge&logoColor=white"/>
 
Los datos rara vez llegan limpios. En esta fase los transformamos para que el modelo pueda entenderlos. Tratamos valores faltantes, convertimos categorías en números, normalizamos escalas y creamos **nuevas variables** que capturen señales que las originales no muestran solas.
 
Por ejemplo: un estudiante con inasistencias crecientes mes a mes es más riesgoso que uno con el mismo total distribuido uniformemente. Esa *tendencia* es una variable nueva que construimos aquí.
 
```
🛠️ Lo que hacemos en esta fase:
   ├── Limpieza de valores nulos o inconsistentes
   ├── Codificación de variables categóricas
   ├── Creación de variables derivadas (Feature Engineering)
   ├── Normalización de escalas numéricas
   └── Balanceo de clases (los desertores son minoría en los datos)
```
 
---
 
### Fase 5 · Modelado 🤖
 
<img src="https://img.shields.io/badge/Etapa-Núcleo_del_Proyecto-1a6b3c?style=for-the-badge&logoColor=white"/>
 
Aquí entrenamos el modelo que aprenderá a identificar patrones de riesgo a partir de los datos históricos. Probamos varios algoritmos de clasificación y comparamos cuál se desempeña mejor para nuestro objetivo.
 
Dado que nos importa **no perder casos reales de deserción**, priorizamos modelos con alta sensibilidad — preferiríamos alertar de más que dejar sin atención a un estudiante en riesgo.
 
| 🧠 Modelo | ¿Por qué lo probamos? |
|---|---|
| Regresión Logística | Línea base sencilla e interpretable |
| Random Forest | Robusto y maneja variables mixtas |
| Gradient Boosting | Excelente para datos desbalanceados |
| XGBoost ✅ | Mayor precisión y control del sesgo |
 
> *Elegimos el modelo como elegimos un médico: no solo el más sofisticado, sino el más confiable para este caso específico.*
 
---
 
### Fase 6 · Evaluación e Interpretabilidad 📊
 
<img src="https://img.shields.io/badge/Etapa-Validación-20b267?style=for-the-badge&logoColor=white"/>
 
Un modelo que funciona pero nadie entiende no sirve en la práctica. En esta fase medimos qué tan bien predice el modelo y, sobre todo, **explicamos por qué toma cada decisión**.
 
Usamos **SHAP** (SHapley Additive exPlanations), una técnica que permite ver cuánto aportó cada variable a la predicción de un estudiante específico. Así un orientador puede saber: *"este alumno está en riesgo principalmente porque faltó 14 días en el último mes y trabaja"*.
 
```
📏 Métricas que evaluamos:
   ├── AUC-ROC     → ¿Qué tan bien distingue entre casos?
   ├── Recall      → ¿Cuántos desertores reales detectamos?
   ├── Precisión   → ¿Cuántas alertas son correctas?
   ├── F1-Score    → Balance entre las dos anteriores
   └── Sesgo       → ¿El modelo es justo entre estratos y géneros?
```
 
---
 
### Fase 7 · Despliegue y Sistema de Alertas 🚀
 
<img src="https://img.shields.io/badge/Etapa-Impacto_Real-0d4a2a?style=for-the-badge&logoColor=white"/>
 
El modelo no vive en un notebook. Vive en manos de quienes pueden actuar. En esta última fase construimos el sistema que pone las predicciones al servicio de los orientadores escolares, de forma simple y accionable.
 
Al inicio de cada período, el sistema genera una lista priorizada por colegio con el nivel de riesgo de cada estudiante y una sugerencia de intervención: llamar al acudiente, gestionar subsidio de transporte, remitir a apoyo psicosocial.
 
| 🟢 Riesgo Bajo | 🟡 Riesgo Medio | 🔴 Riesgo Alto |
|---|---|---|
| Monitoreo mensual | Contacto con familia | Intervención inmediata |
| Seguimiento de asistencia | Apoyo académico dirigido | Orientación + subsidios |
 
```
🌐 Herramientas del sistema:
   ├── API de predicción en tiempo real
   ├── Dashboard interactivo para orientadores
   ├── Reportes automáticos por colegio
   └── Alertas semanales por correo / SMS
```
 
> *La ciencia de datos no termina cuando el modelo aprende. Termina cuando un estudiante no abandona.*
 
---
 
<br/>
 
[![Typing SVG](https://readme-typing-svg.demolab.com?font=Comfortaa&size=18&pause=1500&color=20b267&center=true&vCenter=true&width=1000&height=50&lines=Fase+1+🧭+→+Fase+2+🗄️+→+Fase+3+🔍+→+Fase+4+⚙️+→+Fase+5+🤖+→+Fase+6+📊+→+Fase+7+🚀)](https://git.io/typing-svg)
 
</div>

<br/>
<div align="center">

<br/>
<div align="center">
<br/>
<div align="center">



## 🎯 **CONCLUSIÓN** 🔥

<div align="center">
<img src="https://capsule-render.vercel.app/api?type=soft&color=20b267&height=90&section=footer&text=¡La+Ciencia+de+Datos+salva+vidas!&fontSize=30&fontColor=ffffff" width="100%"/>
</div>

<img src="https://images.unsplash.com/photo-1522202176988-66273c2fd55f?w=1200&h=400&fit=crop" width="100%" style="border-radius: 15px; box-shadow: 0 4px 12px rgba(0,0,0,0.1);"/>

**La deserción escolar no es solo un número…**  
**es el futuro de miles de jóvenes de Bogotá que se apaga.**

Este proyecto demuestra que **la Ciencia de Datos puede cambiar esa historia**.

Ya no esperamos a que el estudiante abandone el colegio.  
**Ahora lo detectamos 3 meses antes** y actuamos a tiempo.

<img src="https://images.unsplash.com/photo-1516321318423-f06f85e504b3?w=800&h=300&fit=crop" width="100%" style="border-radius: 15px; margin: 20px 0; box-shadow: 0 4px 12px rgba(0,0,0,0.1);"/>

Gracias al modelo de clasificación, los orientadores podrán recibir **alertas tempranas** y ofrecer:
- ✅ Apoyo psicosocial  
- ✅ Subsidios de transporte  
- ✅ Refuerzo académico  
- ✅ Acompañamiento familiar  

**Cada estudiante que se queda en el colegio es una victoria real de la tecnología al servicio del bien común.**

---

**Este es solo el comienzo…**  
En las próximas fases llevaremos este modelo a un **dashboard interactivo** para que **todos los colegios públicos de Bogotá** puedan usarlo **gratis y en tiempo real**.

> **"No se trata de predecir el abandono… se trata de evitarlo."**

[![Typing SVG](https://readme-typing-svg.demolab.com?font=Comfortaa&size=24&pause=800&color=20b267&center=true&vCenter=true&width=1000&height=70&lines=Ciencia+de+Datos+con+impacto+real;Anticipando+el+futuro+de+nuestros+estudiantes;¡Porque+cada+joven+cuenta!;Transformando+datos+en+oportunidades)](https://git.io/typing-svg)

**¡La Ciencia de Datos no solo analiza el mundo… lo cambia!** 🚀
