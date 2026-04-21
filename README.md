# Análisis de Congestión en TransMilenio

<p align="center">
  <strong>Valeria Colmenares Moreno</strong> · 
  <strong>Miguel Colmenares Rodríguez</strong> · 
  <strong>María Gabriela Martín Avila</strong> · 
  <strong>Sebastián David Moreno Bustos</strong>
</p>

---

## 1. Problema

Las estaciones **Las Aguas** y **Museo del Oro** dependen exclusivamente de la ruta **FJ23**, lo que genera un sistema vulnerable y poco flexible ante cambios en la demanda o fallas operativas.

<p align="center">
  <img src="https://media.istockphoto.com/id/1331658886/es/foto/bus-p%C3%BAblico-en-una-estaci%C3%B3n-de-pasajeros-de-la-ciudad-de-bogot%C3%A1.jpg?s=612x612&w=0&k=20&c=9WV-Vi-CrL_mf7o1fNVB6xOtox62P2sRE6tdUvu8aGo=" width="65%" style="border-radius:10px;">
</p>

En horas pico, la demanda supera la capacidad del sistema, generando:

- congestión de pasajeros  
- aumento en los tiempos de espera  
- saturación de la operación  

Además, incluso en horas valle, la afluencia se mantiene alta, lo que indica un problema estructural y no puntual.

---

## 2. Pregunta de investigación

> ¿En qué momentos del día la oferta del sistema es insuficiente frente a la demanda real?

---

## 3. Información necesaria

Para responder esta pregunta, se requiere recolectar y analizar:

### Datos principales
- Validaciones de pasajeros durante el día  
- Flujo por franja horaria  
- Frecuencia de buses (ruta FJ23)  

<p align="center">
  <img src="https://bogota.gov.co/sites/default/files/2025-12/transmilenio-presenta-ruta-y-mejoras-en-servicios-diciembre-bogota.jpg" width="70%" style="border-radius:10px;">
</p>

### Datos complementarios
- Impacto del carril único  
- Regularidad del servicio  
- Condiciones externas que afectan la operación  

---

## 4. Enfoque del análisis

El problema se entiende como una relación entre la demanda de pasajeros y la capacidad del sistema.

```mermaid
flowchart LR
A[Demanda] --> B[Estaciones]
B --> C[Ruta FJ23]
C --> D[Frecuencia]
D --> E[Capacidad]
E --> F[Congestión]
