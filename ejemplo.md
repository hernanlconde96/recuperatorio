# diagrama uml - videojuego

```mermaid
classDiagram
    class Videojuego {
        - nombre : String
        - plataforma : String
        - cantidadJugadores : int
        + Videojuego()
        + Videojuego(nombre : String)
        + Videojuego(nombre : String, plataforma : String, cantidadJugadores : int)
        + agregarJugadores() void
        + agregarJugadores(cantidad : int) void
        + mostrarInfo() void
    }
