# Diagrama UML - Clase Celular

```mermaid
classDiagram
    class Celular {
        - String nroTel
        - String duenio
        - int espacio
        - int ram
        - int nroApp
        + Celular(String nroTel, String duenio, int espacio, int ram, int nroApp)
        + aumentarApps() void
        + reducirEspacio() void
        + mostrar() void
        + main(String[] args) void
    }
