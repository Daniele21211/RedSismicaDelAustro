# Colimadores – Revisión Técnica

Este directorio contiene la documentación técnica asociada a la revisión del diseño electrónico (esquemático y PCB) de los módulos colimador fijo y colimador móvil del sistema RSA.

## Alcance de la revisión

La revisión se realizó sobre las versiones entregadas del diseño desarrolladas en KiCad e incluyó:

-  Análisis de cierre eléctrico y conectividad.

-  Revisión frente a las Especificaciones Técnicas Generales y Particulares de los ítems correspondientes (ítem 64 – colimador móvil, ítem 65 – colimador fijo).

-  Evaluación de criterios básicos de compatibilidad electromagnética (EMC).

-  Identificación de riesgos de diseño, definiciones técnicas pendientes y faltantes de implementación.

La revisión se basa exclusivamente en los archivos de diseño disponibles. No se dispone de evidencia de pruebas en prototipos reales, ensayos de laboratorio ni pruebas en campo.

## Documentos incluidos
-  Recomendaciones técnicas de las dos tarjetas bajadas desde el commit correspondiente a su emisión en el repsitorio.

-  Nota Técnica – Colimador móvil V2

-  Recomendaciones Técnicas EMC – Colimador móvil V2

-  Nota Técnica – Colimador fijo V2

-  Recomendaciones Técnicas EMC – Colimador fijo V2

## Observaciones relevantes

Entre los principales aspectos identificados en la revisión de los colimadores se encuentran:

-  Definición incompleta del sistema de accionamiento del actuador lineal en el colimador móvil (driver de potencia externo y su integración EMC).

-  Falta de definición formal del sistema de realimentación de posición (encoder), incluyendo tipo, resolución y montaje mecánico.

-  Manejo EMC incompleto de interfaces de campo (RS485, sensor óptico cableado).

-  Puntos de prueba insuficientes para verificación integral del PCBA.

-  Protección ESD/transitorios no documentada de forma integral en todas las interfaces.

-  Conectores industriales (M8/M12) considerados parte del conjunto chasis–arnés y no del PCBA, requiriendo documentación adicional del sistema completo.

## Estado del diseño

Los diseños de los colimadores no se consideran aptos para liberación, fabricación ni aceptación contractual en su estado actual. Las observaciones indicadas deben ser atendidas y evidenciadas en una nueva versión del diseño.

