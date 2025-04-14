# RP2350-Board

## Hardware Overview

### Microcontroladores
- **RP2350B**: MCU principal con USB nativo
- **RP2040-Zero**: Utilizado exclusivamente para debug 

### Alimentación y Comunicación
- **USB-C Principal (Alimentación)**:
  - Conectado directamente al RP2350B
  - Proporciona 5V regulados internamente a 3.3V

- **USB-C Secundario (Comunicación UART)**:
  - Conectado a puente UART-USB (CH340E)
  - Permite comunicación serial para depuración
  - Compatible con 3.3V (nivel lógico del RP2350B)

---

## Esquemático y PCB
- **Herramienta de diseño**:
  - Diseño inicial en EasyEDA
 
## ¿Como importarlo a KiCad? 
  - En el menu de KiCad, seleccionamos Archivo > Importar proyecto ajeno a KiCad > Proyecto EasyEDA (JLCEDA) Pro
   <p align="center">
  <img src="images/image.png" alt="Descripción de la imagen" width="600"/>
</p>

  - **Importante: para importarlo correctamente, se debe usar KiCad 9, ya que en versiones anteriores hay bugs no fixeados**


> :bulb: **Este proyecto esta basado mayormente en** [este archvo](https://datasheets.raspberrypi.com/rp2350/hardware-design-with-rp2350.pdf)
> :accessibility:: **Acceso a archivos originales**: Contactar a [@monti3](https://github.com/monti3)

