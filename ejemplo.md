
**Leyenda:**
- `-` = atributo privado/protegido
- `+` = método público
- `△` = herencia

## Descripción de Clases

### Clase Base: Vehiculo
**Atributos:**
- `conductor` (String) - Nombre del conductor
- `placa` (String) - Placa del vehículo
- `id` (int) - Identificador único

**Métodos:**
- `mostrarDatos()` - Muestra placa y conductor
- `cambiarConductor(String)` - Cambia el conductor

### Subclases:

#### Bus
**Atributos propios:**
- `capacidad` (int) - Número de pasajeros
- `sindicato` (String) - Sindicato al que pertenece

#### Auto
**Atributos propios:**
- `caballosFuerza` (int) - Potencia del motor
- `descapotable` (boolean) - Si es descapotable

#### Moto
**Atributos propios:**
- `cilindrada` (int) - Cilindrada del motor
- `casco` (boolean) - Si incluye casco

## Relaciones
- **Herencia**: Bus, Auto y Moto heredan de Vehiculo
- **Jerarquía**: Estructura de herencia simple
- **Especialización**: Cada subclase añade atributos específicos
