# Colimadores

## Descripción general
Esta carpeta contiene el diseño de las tarjetas electrónicas de los **Colimadores**, desarrolladas para el sistema de la Red Sísmica del Austro.

El diseño electrónico se ha realizado utilizando **KiCad** y contempla los archivos necesarios para análisis, revisión técnica, fabricación y ensamblaje del PCB.

Existen dos variantes de diseño:
- **Colimador fijo**
- **Colimador móvil**

---

## Contenido de la carpeta

### Colimador fijo
Contiene el diseño electrónico correspondiente al colimador de instalación fija.

- **Archivos_KiCad**
  - `.kicad_pro`: archivo principal del proyecto
  - `.kicad_sch`: esquemáticos eléctricos
  - `.kicad_pcb`: diseño de la placa PCB
- **BOM (Bill of Materials)**
  - Listado de componentes electrónicos
- **Gerbers**
  - Archivos de fabricación del PCB
- **Esquemático**
  - Archivos PDF de conexiones
- **PCB**
  - Fotografías de la PCB (top y bottom)

---

### Colimador móvil
Contiene el diseño electrónico correspondiente al colimador de instalación móvil.

- **Archivos_KiCad**
  - `.kicad_pro`: archivo principal del proyecto
  - `.kicad_sch`: esquemáticos eléctricos
  - `.kicad_pcb`: diseño de la placa PCB
- **BOM (Bill of Materials)**
  - Listado de componentes electrónicos
- **Gerbers**
  - Archivos de fabricación del PCB
- **Esquemático**
  - Archivos PDF de conexiones
- **PCB**
  - Fotografías de la PCB (top y bottom)

---

## Versiones
Las versiones de cada diseño se organizan en subcarpetas identificadas por revisión (v1, v2, etc.).  
La **última versión válida para revisión técnica** en ambos casos es la **v2**.

---

## Nota para revisión
Para efectos de revisión técnica, se deberán considerar **únicamente** los archivos fuente generados en **KiCad** (`.kicad_pro`, `.kicad_sch`, `.kicad_pcb`) correspondientes a cada variante.

Los archivos PDF, imágenes y Gerbers se consideran derivados y no forman parte de la revisión del diseño electrónico.
