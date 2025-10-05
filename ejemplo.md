# Diagrama UML - Clase MP4

```mermaid
classDiagram
    class MP4 {
        - String marca
        - float capacidadGb
        - List~Dict~ canciones
        - List~Dict~ videos
        + MP4(String marca, float capacidadGb)
        + espacio_usado() float
        + espacio_disponible() float
        + borrar_cancion(criterio, valor) void
        + __add__(cancion) str
        + __sub__(video) str
        + __str__() str
    }
