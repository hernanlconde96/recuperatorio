# Diagrama UML - Sistema de Negocios

```mermaid
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
```

## Descripción del Diagrama

### Clase Padre
- **Negocio**: Clase base con atributos comunes a todos los negocios

### Clases Hijas
- **Panaderia**: Especializada en productos de panadería
- **Peluqueria**: Especializada en servicios de belleza
- **Salteneria**: Especializada en venta de salteñas

### Relaciones
- Todas las clases hijas heredan de la clase `Negocio`
- Cada clase hija tiene sus propios atributos específicos
- Todas implementan el método `mostrar()` con su propia lógica
