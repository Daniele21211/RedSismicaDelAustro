\# Termocupla – Documentación de Hardware (V2 / V3) y Correcciones (Versión Final)



Este directorio consolida la evidencia y entregables del \*\*Módulo Termocupla\*\* (hardware y documentación), incluyendo el proyecto KiCad y el informe técnico de respuesta EMC, así como el registro de correcciones propuestas para la \*\*versión final\*\*.



> \*\*Nota importante (bloqueante):\*\*  

> Antes de realizar \*\*cualquier reajuste\*\* o modificación para la versión final, se deben \*\*ejecutar pruebas sobre la tarjeta física\*\* de Termocupla.  

> La tarjeta está programada para \*\*llegar mañana sábado\*\* (según coordinación).  

> \*\*Referencia de fecha:\*\* hoy es \*\*viernes 16/01/2026\*\*, por lo que “mañana sábado” corresponde a \*\*sábado 17/01/2026\*\*.



---



\## Estructura y archivos relevantes



\- `Termocupla\_V3.zip`  

&nbsp; Proyecto de hardware (KiCad) correspondiente a \*\*V3\*\*.



\- `InformeRespuesta EMC TermocuplaV3.docx`  

&nbsp; Informe técnico de respuesta / recomendaciones EMC para \*\*Termocupla V3\*\*.



---



\## Estado actual del proyecto



\- \*\*Tarjeta física (pendiente de recepción y pruebas):\*\* llegada prevista \*\*sábado 17/01/2026\*\*.  

\- \*\*V3 (KiCad + informe):\*\* disponible en este directorio, \*\*pendiente de validación\*\* con pruebas físicas.



---



\## Pruebas obligatorias en la tarjeta física antes de cambios finales



Registrar evidencias (fotos, mediciones, capturas de pantalla, checklist) para:



1\. \*\*Alimentación\*\*

&nbsp;  - Encendido estable, consumos esperados, ausencia de sobrecalentamiento.

&nbsp;  - Verificación de tensiones principales (según diseño).



2\. \*\*Funcionamiento general\*\*

&nbsp;  - Inicialización correcta del sistema.

&nbsp;  - Verificación de estados/indicadores (si aplica).



3\. \*\*Lectura de termocupla / adquisición\*\*

&nbsp;  - Verificación de lectura válida con una fuente de referencia o condiciones controladas.

&nbsp;  - Estabilidad de la medición en operación continua (mínimo 30–60 min).



4\. \*\*Comunicación / interfaz\*\*

&nbsp;  - Enumeración y comunicación básica (según la interfaz implementada).

&nbsp;  - Registro de logs o datos transmitidos (si aplica).



5\. \*\*Robustez / ruido\*\*

&nbsp;  - Observaciones de reinicios, ruido, drift, caídas de comunicación.

&nbsp;  - Confirmación de comportamiento estable bajo condiciones normales.



> \*\*Resultado esperado:\*\*  

> Con resultados de pruebas, se define con evidencia qué correcciones se aplican realmente a la \*\*versión final\*\*.



---



\## Correcciones propuestas para la versión final (pendientes de validación)



Las siguientes acciones se consideran \*\*propuestas\*\* hasta finalizar pruebas en la tarjeta física.



\### A) EMC / Planos de tierra / retorno de corriente

\- Aplicación de recomendaciones EMC del informe `InformeRespuesta EMC TermocuplaV3.docx`.

\- Verificación de continuidad/criterio de retorno de corriente y separación de zonas si aplica.



\### B) Ruteo y layout

\- Revisión de rutas críticas y retornos.

\- Confirmación de que no existan cortes o cuellos de botella en plano GND en áreas sensibles.



\### C) Protección y robustez

\- Validación de protecciones en interfaces externas (ESD/TVS) según conectores y entorno de uso.

\- Revisión de filtros/terminaciones donde corresponda.



\### D) Manufactura / DFM

\- Clearances, anchos de pista, vías térmicas y puntos de test.

\- Serigrafía y referencias para ensamblaje.



> \*\*Importante:\*\*  

> Toda corrección aprobada debe incluir:

> 1) evidencia en pruebas, 2) cambio propuesto, 3) resultado esperado, 4) verificación posterior.



---



\## Control de cambios (recomendado)



Formato sugerido para correcciones aprobadas:



\- \*\*ID:\*\* TC-FIX-XX  

\- \*\*Descripción:\*\* …  

\- \*\*Motivo:\*\* hallazgo en pruebas / recomendación técnica  

\- \*\*Impacto:\*\* esquemático / PCB / BOM / firmware  

\- \*\*Evidencia:\*\* archivo/captura/foto  

\- \*\*Estado:\*\* Propuesto / Aprobado / Implementado / Verificado



---



\## Historial / notas



\- \*\*Recepción tarjeta:\*\* prevista para \*\*sábado 17/01/2026\*\*.

\- \*\*V3:\*\* proyecto KiCad empaquetado en `Termocupla\_V3.zip`.

\- \*\*Informe EMC:\*\* `InformeRespuesta EMC TermocuplaV3.docx`.





