# Diagrama UML - Sistema de Vehículos

## Estructura de Clases

```mermaid
classDiagram
    class Vehiculo {
        -String conductor
        -String placa
        -int id
        +mostrarDatos() void
        +cambiarConductor(String) void
    }

    class Bus {
        -int capacidad
        -String sindicato
    }

    class Auto {
        -int caballosFuerza
        -boolean descapotable
    }

    class Moto {
        -int cilindrada
        -boolean casco
    }

    Vehiculo <|-- Bus
    Vehiculo <|-- Auto
    Vehiculo <|-- Moto
