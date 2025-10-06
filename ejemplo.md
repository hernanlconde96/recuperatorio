classDiagram
    direction BT
    class Negocio {
        #String nombre
        #String dueño
        #double capital
        +Negocio(String nombre, String dueño, double capital)
        +String getNombre()
        +void setNombre(String nombre)
        +String getDueño()
        +void setDueño(String dueño)
        +double getCapital()
        +void setCapital(double capital)
    }

    class Panaderia {
        -double precioPan
        -String panadero
        -double precioEmpanada
        +Panaderia(String nombre, String dueño, double capital, double precioPan, String panadero, double precioEmpanada)
        +void mostrar() void
        +double getPrecioPan()
        +void setPrecioPan(double precioPan)
        +String getPanadero()
        +void setPanadero(String panadero)
        +double getPrecioEmpanada()
        +void setPrecioEmpanada(double precioEmpanada)
    }

    class Peluqueria {
        -double precioCorte
        -double precioTinte
        -String ayudante
        +Peluqueria(String nombre, String dueño, double capital, double precioCorte, double precioTinte, String ayudante)
        +void mostrar() void
        +double getPrecioCorte()
        +void setPrecioCorte(double precioCorte)
        +double getPrecioTinte()
        +void setPrecioTinte(double precioTinte)
        +String getAyudante()
        +void setAyudante(String ayudante)
    }

    class Salteneria {
        -double precioSaltena
        -String ayudante
        -double precioRefresco
        +Salteneria(String nombre, String dueño, double capital, double precioSaltena, String ayudante, double precioRefresco)
        +void mostrar() void
        +double getPrecioSaltena()
        +void setPrecioSaltena(double precioSaltena)
        +String getAyudante()
        +void setAyudante(String ayudante)
        +double getPrecioRefresco()
        +void setPrecioRefresco(double precioRefresco)
    }

    Negocio <|-- Panaderia
    Negocio <|-- Peluqueria
    Negocio <|-- Salteneria
    
