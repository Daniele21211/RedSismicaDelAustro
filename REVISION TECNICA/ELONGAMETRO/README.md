# Elongómetro – Revisión Técnica de Diseño (Ítem 30)

Este directorio contiene la documentación técnica asociada a la revisión del diseño electrónico
(esquemático y PCB) del módulo Elongómetro del proyecto RSA.

## Alcance de la revisión
La revisión se realizó sobre los archivos de diseño desarrollados en KiCad e incluyó:
- Análisis de arquitectura electrónica y conectividad.
- Verificación frente a las Especificaciones Técnicas Generales y Particulares del ítem 30.
- Evaluación de criterios básicos de compatibilidad electromagnética (EMC).
- Revisión de interfaces de comunicación (RS485, USB para flasheo).
- Revisión de elementos de diagnóstico (LEDs, test pins).
- Análisis crítico del sistema de medición basado en galgas extensométricas.

## Aspectos críticos identificados
- La función crítica del equipo corresponde al conjunto micromecánico y a la medición de galgas extensométricas en configuración de puente de Wheatstone.
- No se evidencia de forma explícita el cierre del puente de Wheatstone mediante resistencias de precisión en la tarjeta, ni se documenta la configuración real del puente (¼, ½ o completo).
- No se definen deformaciones máximas admisibles del elemento mecánico sensible (lámina metálica flexionada).
- No se documentan pruebas experimentales de capacidad de medición (carga–deformación, linealidad, histéresis, repetibilidad).
- No se evidencian mediciones ni compensaciones ambientales completas (temperatura, presión u otras).
- Se establece la necesidad de operación en ambiente controlado y cerrado, con compensación térmica activa.
- No se evidencia el uso de conectores M12 ni la configuración completa del bus RS485 (terminación y polarización seleccionables).
- No se evidencia protección ESD dedicada para el puerto USB.

## Documentos incluidos
- Nota técnica de revisión del diseño.
- Recomendaciones Técnicas EMC.

## Alcance y limitaciones
La documentación contenida en este directorio corresponde exclusivamente a una revisión técnica
de diseño. No constituye aprobación, aceptación técnica ni validación funcional del equipo.
No existen evidencias de:
- pruebas de laboratorio,
- ensayos con prototipos físicos,
- operación del sistema completo integrando hardware, firmware y software.

En ausencia de dichas evidencias, el diseño debe considerarse como una propuesta técnica en etapa de revisión.
