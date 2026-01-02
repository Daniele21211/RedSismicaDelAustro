# Tarjeta Acelerógrafo – Revisión Técnica

Este directorio contiene la documentación técnica asociada a la revisión del diseño electrónico
(esquemático y PCB) del módulo acelerógrafo del sistema RSA.

## Alcance de la revisión
La revisión se realizó sobre la versión 2 del diseño desarrollado en KiCad e incluyó:
- Análisis de cierre eléctrico y conectividad.
- Revisión frente a las Especificaciones Técnicas Generales y Particulares del ítem (ítem 23).
- Evaluación de criterios básicos de compatibilidad electromagnética (EMC).
- Identificación de riesgos de diseño y faltantes de implementación.

La revisión se basa exclusivamente en los archivos de diseño disponibles.
No se dispone de evidencia de pruebas en prototipos reales, ensayos de laboratorio ni pruebas en campo.

## Documentos incluidos

- **Nota Técnica – Acelerógrafo V2**  
  Documento de respaldo técnico–contractual que identifica incumplimientos explícitos frente a las
  especificaciones del ítem. No constituye aprobación del diseño.

- **Recomendaciones Técnicas EMC – Acelerógrafo V2**  
  Documento técnico que presenta observaciones y sugerencias de mejora de diseño orientadas a
  robustez EMC y cumplimiento de especificaciones. No constituye validación funcional.

## Observaciones relevantes
Entre los principales aspectos identificados en la revisión se encuentran:
- Ausencia de implementación de la telemetría de operación integrada en el PCBA.
- No implementación de las dos interfaces RS485/MODBUS exigidas por especificación.
- Puntos de prueba incompletos para verificación del PCBA.
- Protección ESD/transitorios no documentada de forma integral.
- Conectores M8/M12 considerados parte del conjunto chasis–arnés y no del PCBA, requiriendo
  documentación adicional del sistema completo.

## Estado del diseño
El diseño no se considera apto para liberación, fabricación ni aceptación contractual en su estado
actual. Las observaciones indicadas deben ser atendidas y evidenciadas en una nueva versión del diseño.

---
Este repositorio se utiliza como herramienta de trazabilidad técnica del proceso de revisión.

