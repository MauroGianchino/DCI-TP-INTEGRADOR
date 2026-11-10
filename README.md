## Trabajo práctico final de la asignatura DCI ##
Este repositorio contiene el trabajo práctico final para la asignatura de Diseño de Circuitos Impresos de la carrera de posgrado de FIUBA.

* Autor: Ing. Mauro Ariel Gianchino
* Título corto del trabajo: Réplica del módulo Adafruit TLV320DAC3100: DAC I2S con salida de auriculares y parlante  
* Descripción:  Réplica en KiCad del módulo Adafruit TLV320DAC3100 I2S DAC with Headphone and Speaker Out (PID 6309). El circuito recibe audio digital por I2S (BCLK, WSEL, DIN) y lo convierte, con el códec TLV320DAC3100 de Texas Instruments, en audio analógico: salida estéreo para auriculares de 16 Ω con acople AC y salida mono clase D para parlante de 4–8 Ω (hasta 2,5 W sobre 4 Ω alimentado con 5 V). Se configura por I2C, genera MCLK internamente con una PLL desde BCLK, y admite headset con micrófono (jack TRRS con detección). Se alimenta con 3–5 V y expone sus señales en dos headers. El objetivo del TP es rediseñar esquemático y PCB de forma nativa en KiCad, aplicando las pautas de la asignatura (IPC, reglas de fabricación relajadas, límites de fabricantes locales). El resultado debe ser un primer prototipo fácil de ensamblar y retrabajar.
* Cursada: OCT-NOV-DIC 2026


## Licencia de este trabajo ##
Este trabajo es una obra derivada (adaptación) del diseño de PCB del módulo *Adafruit TLV320DAC3100 I2S DAC with Headphone and Speaker Out*, publicado por Adafruit Industries en https://github.com/adafruit/Adafruit-TLV320DAC3100-I2S-DAC-PCB bajo la licencia Creative Commons Attribution-ShareAlike 3.0 Unported (CC BY-SA 3.0). El diseño original fue modificado.

Conforme a la cláusula ShareAlike, esta adaptación se distribuye bajo la misma licencia, **CC BY-SA 3.0 Unported**. El texto completo está en el archivo [license.txt](license.txt) de la raíz de este repositorio (también disponible en https://creativecommons.org/licenses/by-sa/3.0/legalcode).


## Estado del proyecto ##
- [x] Propuesta
- [ ] Esquemático
- [ ] Asociación de huellas y modelos 3D
- [ ] Posicionamiento
- [ ] Ruteo y DRC
- [ ] Documentación final (BOM, gerbers)

## Estructura del TP FINAL ##

Se propone y se pide utilizar la siguiente estructura.

* doc: Toda la información sobre el circuito, principalmente de autoría o procesamiento propio. Por ejemplo:
  * Notas de ingeniería propias.
  * Notas de aplicación propias.
  * Estudios previos, estado del arte, resumen de las investigaciones.
  * Notas con cálculos.
  * Dibujos adicionales.
  * Fotos de los prototipos.
  * Presupuestos, cotizaciones.
* info: Toda la iformación recolectada, principalmente de terceros, como por ejemplo:
  * Hojas de datos.
  * Notas de aplicación.
  * Info de productos comerciales.
  * Info en internet.
* pcb: Archivos de diseño esquemático y pcb.

Dependiendo la magnitud del proyecto, tendremos más o menos información en estos directorios. 
Revisar los README.md en cada directorio para conocer las pautas de cada uno para este TP.

NOTA: El alumno puede y debe borrar de este archivo todo lo que considere necesario, por ejemplo las aclaraciones del docente y esta misma nota.

## Obligatorios para el TP Final ##
* doc/propuesta/README.md (con textos y links, formato markdown, a imágenes que deben estar en el mismo repo. Las imágenes son las que se piden en las pautas de TP).
* info/*.pdf (Se piden solo las hojas de datos de los componentes relevantes como circuitos integrados, conectores particulares, módulos, etc. No es necesario poner hojas de pasivos, discretos comunes, conectores estándar.)
* pcb/* (Acá va el proyecto KiCad, modelos 3D, bibliotecas particulares y archivos generados como BOM, gerbers, etc.). EVITE subir al git archivos temporales de KiCad. Se recomienda usar un .gitignore adecuado.
* El alumnos es libre de agregar otras cosas, pero siempre tenga en cuenta que el repositorio es público. Evitar colocar información personal o documentación confidencial. 
