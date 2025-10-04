# Diagrama UML - Vehículos

```mermaid
classDiagram
    class Vehiculo {
        # conductor : String
        # placa : String
        # id : int
        + Vehiculo(conductor : String, placa : String, id : int)
        + mostrarDatos() : void
        + cambiarConductor(nuevoConductor : String) : void
    }

    class Bus {
        - capacidad : int
        - sindicato : String
        + Bus(conductor : String, placa : String, id : int, capacidad : int, sindicato : String)
    }

    class Auto {
        - caballosFuerza : int
        - descapotable : boolean
        + Auto(conductor : String, placa : String, id : int, caballosFuerza : int, descapotable : boolean)
    }

    class Moto {
        - cilindrada : int
        - casco : boolean
        + Moto(conductor : String, placa : String, id : int, cilindrada : int, casco : boolean)
    }

    Vehiculo <|-- Bus
    Vehiculo <|-- Auto
    Vehiculo <|-- Moto
