# Diagrama UML - Clases Pasajero y Crucero

```mermaid
classDiagram
    class Pasajero {
        - String nombre
        - int edad
        - String genero
        - int nroHabitacion
        - double costoPasaje
        + Pasajero(String nombre, int edad, String genero, int nroHabitacion, double costoPasaje)
        + mostrarDatos() String
        + mostrarNombre() String
        + getGenero() String
        + getCostoPasaje() double
    }

    class Crucero {
        - String nombre
        - String paisOrigen
        - String paisDestino
        - ArrayList~Pasajero~ pasajeros
        + Crucero(String nombre, String paisOrigen, String paisDestino)
        + agregarPasajero(Pasajero p) void
        + mostrarInfo() String
        + mostrarNombre() String
        + compararCostoTotal(Crucero other) String
        + compararCantidadPasajeros(Crucero other) String
        + contarGenero() String
    }

    Crucero "1" --> "*" Pasajero : tiene >
