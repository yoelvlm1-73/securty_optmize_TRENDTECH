# Proceso actual

## 1. BPMN de práctica<br>

![BPMN de práctica](../assets/BPMN_practica.png)<br>

Declaración de IA:<br>
Claude Sonnet 5.5 (Anthropic) – 23/10/2026 – prompt registrado en docs/11-uso-ia.md<br>

## 2. El proceso elegido<br>

Nombre del proceso: Fabricación, transporte e instalación de puertas de seguridad<br>

Carriles (responsables): Cliente; Gerencia y ventas; Producción; Transporte e instalación<br>

Fuente (contacto, cargo y fecha): Orlando Morales, gerente general de Multy Security (lo conoce Yoel Morales) – [23/10/2026]<br>

## 3. Pasos del proceso <br>

| # | Paso (verbo + objeto) | Responsable |<br>
|---|---|---|
| 1 | Contactar a Multy Security | Cliente |<br>
| 2 | Atender al cliente y cotizar | Gerencia y ventas |<br>
| 3 | Generar la orden de producción | Gerencia y ventas |<br>
| 4 | Solicitar piezas metálicas al proveedor | Producción |<br>
| 5 | Recibir e inspeccionar las piezas | Producción |<br>
| 6 | Devolver al proveedor y pedir corrección | Producción |<br>
| 7 | Fabricar la puerta (corte, soldadura y acabado) | Producción |<br>
| 8 | Transportar la puerta al sitio del cliente | Transporte e instalación |<br>
| 9 | Instalar la puerta | Transporte e instalación |<br>
| 10 | Corregir la instalación | Transporte e instalación |<br>
| 11 | Entregar y firmar acta de entrega | Transporte e instalación |<br>
| 12 | Recibir y aprobar la entrega | Cliente |<br>

Decisión: ¿Cliente acepta la cotización? Sí: Generar la orden de producción (paso 3). No: Venta no concretada (fin del proceso).<br>

Decisión: ¿Piezas conformes? Sí: Fabricar la puerta (paso 7). No: Devolver al proveedor y pedir corrección (paso 6), y se vuelve a Solicitar piezas metálicas al proveedor (paso 4).<br>

Decisión: ¿Instalación conforme? Sí: Entregar y firmar acta de entrega (paso 11). No: Corregir la instalación (paso 10), y se vuelve a Instalar la puerta (paso 9).<br>

## 4. Diagrama BPMN<br>

![BPMN proceso actual](../assets/BPMN_proceso_actuall.drawio)<br>


## 5. Puntos críticos<br>

| PC | Qué pasa (se demora, se repite o se pierde) | Evidencia (dato o frase del contacto, con fecha) |<br>
|---|---|---|
| PC1 | Se repite: cuando las piezas del proveedor no son conformes, se devuelven y se vuelven a solicitar (pasos 4 a 6) | [evidencia – dd/mm/aaaa] | <br>
| PC2 | Se repite: cuando la instalación no es conforme, se corrige y se instala de nuevo (pasos 9 y 10) | [evidencia – dd/mm/aaaa] |<br>

## 6. Uso de IA<br>

| Herramienta y versión | Fecha | Prompt |<br>
|---|---|---|
| Claude Sonnet 5.5 | 23/10/2026 | Dame el md de la planeación del proyecto según la guía (Paso 5, 03.proceso_actual.md), usando solo el BPMN de Multy Security como proceso actual |<br>
