# Módulo de medición de termocupla – Revisión técnica EMC

Este directorio contiene la documentación técnica asociada a la revisión del diseño electrónico
(esquemático y PCB) del módulo de medición de termocupla embebida en presa.

# Alcance de la revisión

La revisión se realizó sobre la versión más reciente del diseño desarrollado en KiCad e incluyó:

- Análisis del esquemático y del PCB desde el punto de vista de compatibilidad electromagnética (EMC).

- Contraste contra las Recomendaciones Técnicas EMC – versión 1 emitidas previamente.
- Verificación técnica frente a las Especificaciones Técnicas Particulares del ítem 67 (parte dos).
- Revisión de aspectos de robustez asociados a:
	- Cable largo de termocupla (>10 m).
	- Operación en batería de plomo-ácido y control de carga.
	- Interfaz RS485 de campo.
	- Puntos de prueba, LEDs indicadores y flasheo del ESP32 vía USB.

# Contenido del directorio
## Recomendaciones Técnicas EMC – Termocupla Presa v1
	Bajado del coomit correspondiente para tenerlo como referencia.
## Recomendaciones Técnicas EMC – Termocupla Presa v2
	Documento que recoge observaciones y recomendaciones de diseño orientadas a mejorar la robustez EMC del módulo.
	No constituye validación funcional ni certificación normativa.
## Nota Técnica – Revisión Diseño Termocupla
	Documento técnico–administrativo que contrasta el estado del diseño frente a recomendaciones previas y especificaciones contractuales, como respaldo para la 	toma de decisiones por parte de la administración.
## Archivos de diseño KiCad
	Esquemático y PCB analizados en la revisión.

# Consideraciones importantes
Esta revisión se basa exclusivamente en documentación de diseño electrónico.
No se han realizado pruebas de laboratorio, ensayos EMC, validaciones funcionales ni revisión de firmware.
Las observaciones y recomendaciones no implican aprobación del diseño ni liberación para fabricación o instalación.
El diseño está pensado para operar en entornos con alto riesgo de ruido e inducciones, por lo que las protecciones EMC y la arquitectura de tierras son críticas.

# Uso esperado del repositorio
Este repositorio sirve como registro técnico de revisión, permitiendo:
- Trazabilidad de observaciones y recomendaciones a lo largo de las distintas versiones del diseño.
- Comunicación clara entre diseñador, contratista y administración del contrato.
- Soporte documental para decisiones técnicas y administrativas.

