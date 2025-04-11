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
  - Migrado a KiCad v7.0 para mejor compatibilidad

> :bulb: **Acceso a archivos originales**: Contactar a [@monti3](https://github.com/monti3)

