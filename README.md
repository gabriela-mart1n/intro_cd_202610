<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=8B0000&height=220&section=header&animation=twinkling" width="100%"/>

<img src="https://capsule-render.vercel.app/api?type=rect&color=8B0000&height=80&text=Análisis+de+Congestión+en+TransMilenio&fontSize=32&fontColor=ffffff" width="100%"/>

<img src="https://capsule-render.vercel.app/api?type=rect&color=B22222&height=50&text=Movilidad+urbana+basada+en+datos&fontSize=20&fontColor=ffffff" width="100%"/>

<br/>

<img src="https://bogota.gov.co/sites/default/files/2025-12/transmilenio-presenta-ruta-y-mejoras-en-servicios-diciembre-bogota.jpg" width="90%" style="border-radius:14px;"/>

<br/><br/>

<p style="font-size:16px;">
<b>Valeria Colmenares Moreno</b> · 
<b>Miguel Colmenares Rodríguez</b> · 
<b>María Gabriela Martín Avila</b> · 
<b>Sebastián David Moreno Bustos</b>
</p>

</div>

---

<h2 style="color:#8B0000; font-family:Georgia;">Problema</h2>

Las estaciones **Las Aguas** y **Museo del Oro** dependen exclusivamente de la ruta **FJ23**, lo que genera un sistema vulnerable ante fallas operativas y picos de demanda.

<p align="center">
  <img src="https://media.istockphoto.com/id/1331658886/es/foto/bus-p%C3%BAblico-en-una-estaci%C3%B3n-de-pasajeros-de-la-ciudad-de-bogot%C3%A1.jpg?s=612x612&w=0&k=20&c=9WV-Vi-CrL_mf7o1fNVB6xOtox62P2sRE6tdUvu8aGo=" width="65%" style="border-radius:12px;">
</p>

En horas pico, la demanda supera la capacidad del sistema, generando congestión, aumento en tiempos de espera y saturación del servicio. Incluso en horas valle, la afluencia se mantiene alta, lo que evidencia un problema estructural.

---

<h2 style="color:#8B0000; font-family:Georgia;">Pregunta de investigación</h2>

<div align="center">

<i>¿En qué momentos del día la oferta del sistema es insuficiente frente a la demanda real?</i>

</div>

---

<h2 style="color:#8B0000; font-family:Georgia;">Información requerida</h2>

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
<td>Impacto en la operación del sistema</td>
</tr>

<tr>
<td><b>Complementario</b></td>
<td>Regularidad</td>
<td>Consistencia en los tiempos de llegada</td>
</tr>

<tr>
<td><b>Complementario</b></td>
<td>Factores externos</td>
<td>Condiciones que afectan la movilidad</td>
</tr>

</table>

</div>

---

<h2 style="color:#8B0000; font-family:Georgia;">Relación del sistema</h2>

```mermaid
flowchart LR
A[Demanda] --> B[Estaciones]
B --> C[Ruta FJ23]
C --> D[Frecuencia]
D --> E[Capacidad]
E --> F[Congestión]
