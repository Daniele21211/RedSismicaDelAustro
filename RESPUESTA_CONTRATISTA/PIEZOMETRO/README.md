\# Piezómetro – Documentación de Hardware (V2 / V3) y Correcciones (Versión Final)



Este directorio consolida la evidencia y entregables del \*\*Módulo Piezómetro\*\* (hardware KiCad), incluyendo paquetes ZIP y el registro de correcciones propuestas para la \*\*versión final\*\*.



> \*\*Nota importante (bloqueante):\*\*  

> Antes de realizar \*\*cualquier reajuste\*\* o modificación adicional para la versión final, se deben \*\*probar las tarjetas de la versión V2\*\* (ya disponibles en \*\*Cuenca\*\*) y documentar resultados.  

> Las correcciones listadas en este README se consideran \*\*propuestas / pendientes de validación\*\* hasta completar dichas pruebas.



---



\## Estructura y archivos relevantes



\- `Piezometro\_v3.zip`  

&nbsp; Paquete de proyecto \*\*KiCad 9.0\*\* correspondiente a \*\*V3\*\* (borrador de versión final / iteración reciente).



\- \*(Opcional / si aplica)\* V2: archivos o referencias de la versión anterior para contraste (BOM, Gerbers, esquemáticos, etc.).



---



\## Estado actual del proyecto



\- \*\*V2 (tarjetas físicas):\*\* Disponibles en \*\*Cuenca\*\*.  

&nbsp; \*\*Pendiente:\*\* ejecución de pruebas funcionales y registro de resultados.

\- \*\*V3 (KiCad 9.0):\*\* Empaquetada en ZIP.  

&nbsp; \*\*Importante:\*\* no se considera “final” hasta validar V2 y cerrar acciones de corrección.



---



\## Pruebas obligatorias en V2 (Cuenca) antes de cambios finales



Registrar evidencias (fotos, capturas de consola, mediciones, checklist firmado) para:



1\. \*\*Alimentación\*\*

&nbsp;  - Encendido estable, consumos esperados, ausencia de sobrecalentamiento.

&nbsp;  - Pruebas con las fuentes previstas (según requerimientos del sistema).



2\. \*\*Programación / Firmware\*\*

&nbsp;  - Carga y ejecución de firmware.

&nbsp;  - Arranque consistente y logs básicos (si aplica).



3\. \*\*Indicadores y salidas\*\*

&nbsp;  - LEDs de estado.

&nbsp;  - Activación de relés / salidas (si aplica) y verificación con carga real o simulada.



4\. \*\*Comunicación\*\*

&nbsp;  - Enumeración/OTG-Serial (si aplica al diseño).

&nbsp;  - Pruebas de transmisión/recepción básicas con herramienta de monitoreo.



5\. \*\*Ruido / estabilidad\*\*

&nbsp;  - Comportamiento estable durante operación continua (mínimo 30–60 min).

&nbsp;  - Observaciones sobre ruido, resets, caídas de comunicación, etc.



> \*\*Resultado esperado:\*\*  

> Con V2 validada, se define con evidencia cuáles correcciones se aplican realmente a la versión final.



---



\## Correcciones propuestas para la versión final (pendientes de validación con V2)



A continuación se listan correcciones detectadas en revisión de diseño y/o recomendaciones técnicas.  

\*\*Estas acciones NO deben aplicarse todavía\*\* hasta concluir las pruebas de V2.



\### A) Tierra / Planos / EMC (pendiente de confirmación con mediciones)

\- \*\*Unión controlada AGND–GND en “punto único”\*\* usando \*\*NET-TIE / 0 Ω\*\* (referencia: reemplazo de unión directa por elemento controlado; por ejemplo, “cambiar L3 por NET-TIE / 0 Ω” cuando aplique).

\- \*\*Mantener separación por zonas\*\* (analógica/digital/potencia) y confirmar que el retorno de corriente no atraviesa áreas sensibles.

\- Revisión de “masa tipo jaula”/blindaje y su referencia a GND (si aplica a gabinete o perímetro de cobre).



\### B) Ruteo y retorno de corriente

\- Validar rutas de retorno (especialmente señales rápidas o conmutadas).

\- Evitar cortes innecesarios en plano GND debajo de trazas críticas.



\### C) Protección y robustez

\- Verificación de protecciones ESD/TVS en interfaces externas (según conectores y ambiente de uso).

\- Revisión de filtros/RC/terminaciones donde corresponda.



\### D) Ajustes de manufactura / DFM

\- Revisión de clearances, anchos de pista, vías térmicas y puntos de test.

\- Verificación de serigrafía y referencias para ensamblaje.



> \*\*Importante:\*\*  

> Cada corrección debe tener \*\*criterio de aceptación\*\* y quedar registrada como:  

> (1) problema observado en V2 / evidencia, (2) cambio propuesto, (3) resultado esperado, (4) verificación posterior en V3/final.



---



\## Control de cambios (recomendado)



Usar este formato cuando se apruebe una corrección (después de V2):



\- \*\*ID:\*\* PZ-FIX-XX  

\- \*\*Descripción:\*\* …  

\- \*\*Motivo:\*\* hallazgo en pruebas V2 / recomendación técnica  

\- \*\*Impacto:\*\* esquemático / PCB / BOM / firmware  

\- \*\*Evidencia:\*\* enlace/archivo/captura  

\- \*\*Estado:\*\* Propuesto / Aprobado / Implementado / Verificado



---



\## Cómo actualizar este directorio



1\. Añadir/actualizar ZIPs y documentos.

2\. Actualizar este README con:

&nbsp;  - resultados de pruebas V2 (Cuenca),

&nbsp;  - correcciones aprobadas,

&nbsp;  - checklist y evidencia.



---



\## Historial / notas



\- \*\*V2:\*\* tarjetas físicas en Cuenca (pendiente de pruebas).

\- \*\*V3:\*\* proyecto KiCad 9.0 empaquetado en `Piezometro\_v3.zip`.



