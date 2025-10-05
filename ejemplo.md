# diagrama uml - sistema de personas

```mermaid
classDiagram
    class persona {
        # nombre : String
        # paterno : String
        # materno : String
        # edad : int
        + persona(nombre : String, paterno : String, materno : String, edad : int)
        + mostrar() : void
        + getEdad() : int
    }

    class docente {
        - sueldo : double
        - regProfesional : String
        + docente(nombre : String, paterno : String, materno : String, edad : int, sueldo : double, regProfesional : String)
        + mostrar() : void
    }

    class estudiante {
        - ru : String
        - matricula : String
        + estudiante(nombre : String, paterno : String, materno : String, edad : int, ru : String, matricula : String)
        + mostrar() : void
        + modificarEdad(nuevaEdad : int) : void
    }

    persona <|-- docente
    persona <|-- estudiante
