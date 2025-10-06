classDiagram
    direction BT
    class Negocio {
        #String nombre
        #String dueño
        #double capital
        +Negocio(String nombre, String dueño, double capital)
    }

    class Panaderia {
        -double precioPan
        -String panadero
        -double precioEmpanada
        +Panaderia(String nombre, String dueño, double capital, double precioPan, String panadero, double precioEmpanada)
        +void mostrar() void
    }

    class Peluqueria {
        -double precioCorte
        -double precioTinte
        -String ayudante
        +Peluqueria(String nombre, String dueño, double capital, double precioCorte, double precioTinte, String ayudante)
        +void mostrar() void
    }

    class Salteneria {
        -double precioSaltena
        -String ayudante
        -double precioRefresco
        +Salteneria(String nombre, String dueño, double capital, double precioSaltena, String ayudante, double precioRefresco)
        +void mostrar() void
    }

    Negocio <|-- Panaderia
    Negocio <|-- Peluqueria
    Negocio <|-- Salteneria
