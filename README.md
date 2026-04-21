<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=8B0000&height=220&section=header&animation=twinkling" width="100%"/>

<img src="https://capsule-render.vercel.app/api?type=rect&color=8B0000&height=80&text=Análisis+de+Congestión+en+TransMilenio&fontSize=32&fontColor=ffffff" width="100%"/>

<img src="https://capsule-render.vercel.app/api?type=rect&color=B22222&height=50&text=Movilidad+urbana+basada+en+datos&fontSize=20&fontColor=ffffff" width="100%"/>

<br/>

<img src="https://bogota.gov.co/sites/default/files/2025-12/transmilenio-presenta-ruta-y-mejoras-en-servicios-diciembre-bogota.jpg" width="90%" style="border-radius:14px;"/>

<br/><br/>

<img src="https://img.shields.io/badge/Proyecto-TransMilenio-red?style=for-the-badge"/>
<img src="https://img.shields.io/badge/Ruta-FJ23-darkred?style=for-the-badge"/>
<img src="https://img.shields.io/badge/Estado-En%20desarrollo-orange?style=for-the-badge"/>

<br/><br/>

> *Optimizar el transporte es optimizar la vida urbana.*

<br/>

<p style="font-size:16px;">
<b>Valeria Colmenares Moreno</b> · 
<b>Miguel Colmenares Rodríguez</b> · 
<b>María Gabriela Martín Avila</b> · 
<b>Sebastián David Moreno Bustos</b>
</p>

</div>

---

<div align="center">

<img src="https://readme-typing-svg.demolab.com?font=Montserrat&size=26&pause=1000&color=8B0000&center=true&vCenter=true&width=700&lines=Problema" />

</div>

Las estaciones **Las Aguas** y **Museo del Oro** dependen exclusivamente de la ruta **FJ23**, lo que genera un sistema vulnerable ante fallas operativas y picos de demanda.

<p align="center">
  <img src="https://media.istockphoto.com/id/1331658886/es/foto/bus-p%C3%BAblico-en-una-estaci%C3%B3n-de-pasajeros-de-la-ciudad-de-bogot%C3%A1.jpg?s=612x612&w=0&k=20&c=9WV-Vi-CrL_mf7o1fNVB6xOtox62P2sRE6tdUvu8aGo=" width="65%" style="border-radius:12px;">
</p>

En horas pico, la demanda supera la capacidad del sistema, generando congestión, aumento en tiempos de espera y saturación del servicio.

---

<div align="center">

<img src="https://readme-typing-svg.demolab.com?font=Montserrat&size=26&pause=1000&color=8B0000&center=true&vCenter=true&width=700&lines=Pregunta+de+investigación" />

</div>

<div align="center">
<i>¿En qué momentos del día la oferta del sistema es insuficiente frente a la demanda real?</i>
</div>

---

<div align="center">

<img src="https://readme-typing-svg.demolab.com?font=Montserrat&size=26&pause=1000&color=8B0000&center=true&vCenter=true&width=700&lines=Información+requerida" />

</div>

<div align="center">

<table>
<tr>
<th>Tipo</th>
<th>Variable</th>
<th>Descripción</th>
</tr>

<tr>
<td><b>Principal</b></td>
<td>Validaciones</td>
<td>Registros de ingreso de pasajeros durante el día</td>
</tr>

<tr>
<td><b>Principal</b></td>
<td>Flujo horario</td>
<td>Cantidad de usuarios por franja horaria</td>
</tr>

<tr>
<td><b>Principal</b></td>
<td>Frecuencia</td>
<td>Número de buses de la ruta FJ23</td>
</tr>

<tr>
<td><b>Complementario</b></td>
<td>Carril único</td>
<td>Impacto en la operación</td>
</tr>

<tr>
<td><b>Complementario</b></td>
<td>Regularidad</td>
<td>Consistencia del servicio</td>
</tr>

<tr>
<td><b>Complementario</b></td>
<td>Factores externos</td>
<td>Condiciones que afectan la movilidad</td>
</tr>

</table>

</div>

---

<div align="center">

<img src="https://readme-typing-svg.demolab.com?font=Montserrat&size=26&pause=1000&color=8B0000&center=true&vCenter=true&width=700&lines=Relación+del+sistema" />

</div>

```mermaid
flowchart LR
A[Demanda] --> B[Estaciones]
B --> C[Ruta FJ23]
C --> D[Frecuencia]
D --> E[Capacidad]
E --> F[Congestión]
