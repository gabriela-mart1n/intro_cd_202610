<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=8B0000&height=220&section=header&animation=twinkling" width="100%"/>

<img src="https://capsule-render.vercel.app/api?type=rect&color=8B0000&height=80&text=Análisis+de+Congestión+en+TransMilenio&fontSize=32&fontColor=ffffff" width="100%"/>

<img src="https://capsule-render.vercel.app/api?type=rect&color=B22222&height=50&text=Movilidad+urbana+basada+en+datos&fontSize=20&fontColor=ffffff" width="100%"/>

<br/>

[![Typing SVG](https://readme-typing-svg.demolab.com?font=Montserrat&size=22&pause=1000&color=FF4C4C&center=true&vCenter=true&width=1000&lines=Analizando+la+congestión+en+Bogotá;Datos+que+optimizan+transporte;Soluciones+reales+con+ciencia+de+datos)](https://git.io/typing-svg)

<br/>

<img src="https://media.istockphoto.com/id/1331658886/es/foto/bus-p%C3%BAblico-en-una-estaci%C3%B3n-de-pasajeros-de-la-ciudad-de-bogot%C3%A1.jpg?s=612x612&w=0&k=20&c=9WV-Vi-CrL_mf7o1fNVB6xOtox62P2sRE6tdUvu8aGo=" width="70%" style="border-radius:12px;"/>

<br/><br/>

<p>
<b>Valeria Colmenares Moreno</b> · 
<b>Miguel Colmenares Rodríguez</b> · 
<b>María Gabriela Martín Avila</b> · 
<b>Sebastián David Moreno Bustos</b>
</p>

</div>

---

## 🚨 Problema

Las estaciones **Las Aguas** y **Museo del Oro** dependen únicamente de la ruta **FJ23**, lo que genera un sistema vulnerable ante fallas operativas y picos de demanda.

En horas pico, la capacidad del sistema es superada, provocando:

- congestión de pasajeros  
- aumento en tiempos de espera  
- saturación del servicio  

---

## 📉 Contexto del sistema

<p align="center">
  <img src="https://bogota.gov.co/sites/default/files/2025-12/transmilenio-presenta-ruta-y-mejoras-en-servicios-diciembre-bogota.jpg" width="75%" style="border-radius:12px;">
</p>

Incluso en horas valle, la afluencia sigue siendo alta, lo que indica que el problema no es ocasional, sino estructural.

---

## 🎯 Pregunta clave

> ¿En qué momentos del día la oferta del sistema es insuficiente frente a la demanda real?

---

## 📊 Información requerida

### Datos principales
- Validaciones de pasajeros  
- Flujo por franja horaria  
- Frecuencia de buses  

### Datos complementarios
- Carril único  
- Regularidad del servicio  
- Factores externos  

---

## ⚙️ Relación del sistema

```mermaid
flowchart LR
A[Demanda] --> B[Estaciones]
B --> C[Ruta FJ23]
C --> D[Frecuencia]
D --> E[Capacidad]
E --> F[Congestión]
