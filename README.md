<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=8B0000&height=220&section=header&animation=twinkling" width="100%"/>

<img src="https://capsule-render.vercel.app/api?type=rect&color=8B0000&height=80&text=Análisis+de+Congestión+en+TransMilenio&fontSize=32&fontColor=ffffff" width="100%"/>

<br/>

<img src="https://media.istockphoto.com/id/1331658886/es/foto/bus-p%C3%BAblico-en-una-estaci%C3%B3n-de-pasajeros-de-la-ciudad-de-bogot%C3%A1.jpg?s=612x612&w=0&k=20&c=9WV-Vi-CrL_mf7o1fNVB6xOtox62P2sRE6tdUvu8aGo=" width="70%" style="border-radius:15px;"/>

<br/><br/>

<img src="https://bogota.gov.co/sites/default/files/2025-12/transmilenio-presenta-ruta-y-mejoras-en-servicios-diciembre-bogota.jpg" width="85%" style="border-radius:15px;"/>

<br/><br/>

<p>
<b>Valeria Colmenares Moreno</b> · 
<b>Miguel Colmenares Rodríguez</b> · 
<b>María Gabriela Martín Avila</b> · 
<b>Sebastián David Moreno Bustos</b>
</p>

<br/>

> *Un sistema de transporte no falla de repente… se va saturando poco a poco hasta que colapsa.*

</div>

---

## 🚨 ¿Qué está pasando realmente?

Las estaciones **Las Aguas** y **Museo del Oro** dependen únicamente de la ruta **FJ23**.

Eso, en la práctica, significa algo simple pero crítico:  
si esa ruta falla, **no hay plan B**.

---

### 📉 Lo que se observa en el día a día

- En horas pico → acumulación masiva de personas  
- En horas valle → la demanda sigue siendo alta  
- Los tiempos de espera → aumentan constantemente  
- La operación → no logra adaptarse a la demanda  

No es solo congestión… es **falta de capacidad de respuesta del sistema**.

---

## 🎯 El punto clave del proyecto

No se trata solo de describir el problema, sino de responder esto:


Porque ahí es donde realmente se puede intervenir.

---

## 📊 Qué datos necesitamos

Para entender lo que pasa, no basta con observar. Hay que medir.

### Datos principales
- Validaciones de pasajeros durante el día  
- Flujo por horas  
- Frecuencia de buses  

### Datos que complementan
- Operación en carril único  
- Regularidad del servicio  
- Condiciones externas del sistema  

---

## ⚙️ Cómo se analiza

```mermaid
flowchart LR
A[Pasajeros] --> B[Estaciones]
B --> C[Ruta FJ23]
C --> D[Frecuencia]
D --> E[Capacidad]
E --> F[Congestión]
