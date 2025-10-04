
## Descripción de Clases

### Clase Base: Vehiculo
**Atributos:**
- `conductor` (String)
- `placa` (String)
- `id` (int)

**Métodos:**
- `mostrarDatos()`
- `cambiarConductor(String)`

### Subclases:

#### Bus (hereda de Vehiculo)
**Atributos propios:**
- `capacidad` (int)
- `sindicato` (String)

#### Auto (hereda de Vehiculo)
**Atributos propios:**
- `caballosFuerza` (int)
- `descapotable` (boolean)

#### Moto (hereda de Vehiculo)
**Atributos propios:**
- `cilindrada` (int)
- `casco` (boolean)

## Relaciones
- **Herencia**: Bus, Auto y Moto heredan de Vehiculo
- **Jerarquía**: Estructura de herencia simple
