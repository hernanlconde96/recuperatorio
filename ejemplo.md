# diagrama uml - sistema de personas

```mermaid
classDiagram
    class Persona {
        # nombre : String
        # paterno : String
        # materno : String
        # edad : int
        + persona(nombre : String, paterno : String, materno : String, edad : int)
        + mostrar() : void
        + getEdad() : int
    }

    class Docente {
        - sueldo : double
        - regProfesional : String
        + docente(nombre : String, paterno : String, materno : String, edad : int, sueldo : double, regProfesional : String)
        + mostrar() : void
    }

    class Estudiante {
        - ru : String
        - matricula : String
        + estudiante(nombre : String, paterno : String, materno : String, edad : int, ru : String, matricula : String)
        + mostrar() : void
        + modificarEdad(nuevaEdad : int) : void
    }

    persona <|-- docente
    persona <|-- estudiante
