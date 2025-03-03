# Aplicación de Gestión de Plantas Funcionalidades y Base de Datos

Esta es una aplicación JavaFX para gestionar información sobre plantas. Permite a los usuarios ver una lista de plantas, seleccionar una planta para ver sus detalles (nombre, nombre científico, familia, época de floración, hábitat, descripción e imagen), y cambiar entre diferentes vistas (como la vista de inicio de sesión y la vista de usuario).

---

## Funcionalidades

### 1. **Lista de Plantas**
   - Muestra una lista de plantas disponibles en la base de datos.
   - Los usuarios pueden seleccionar una planta para ver sus detalles.

### 2. **Detalles de la Planta**
   - Muestra información detallada sobre la planta seleccionada, incluyendo:
     - Nombre
     - Nombre científico
     - Familia
     - Época de floración
     - Hábitat
     - Descripción
     - Imagen

### 3. **Carga de Imágenes**
   - Las imágenes de las plantas se cargan desde la carpeta `src/main/resources/images/plantas/`.
   - Las rutas de las imágenes se almacenan en la base de datos como rutas relativas.

### 4. **Navegación entre Vistas**
   - Los usuarios pueden cambiar entre la vista de inicio de sesión y la vista de usuario.
   - Botones como "Atrás" y "Login" permiten la navegación entre las vistas.

---

## Base de Datos

### Estructura de la Tabla `planta`

La base de datos contiene una tabla llamada `planta` con la siguiente estructura:

| Columna           | Tipo de Dato       | Descripción                                      |
|-------------------|--------------------|--------------------------------------------------|
| `id_planta`       | `INT`              | Identificador único de la planta (clave primaria). |
| `nombre`          | `VARCHAR(100)`     | Nombre común de la planta.                       |
| `nombre_cientifico` | `VARCHAR(100)`     | Nombre científico de la planta.                  |
| `familia`         | `VARCHAR(100)`     | Familia a la que pertenece la planta.            |
| `epoca_floracion` | `VARCHAR(100)`     | Época del año en que florece la planta.          |
| `habitat`         | `VARCHAR(100)`     | Hábitat natural de la planta.                    |
| `descripcion`     | `VARCHAR(250)`     | Descripción breve de la planta.                  |
| `imagen_ruta`     | `VARCHAR(255)`     | Ruta relativa de la imagen de la planta.         |
| `is_deleted`      | `BOOLEAN`          | Indica si la planta ha sido eliminada (soft delete). |

### Ejemplo de Datos

La tabla `planta` puede contener registros como los siguientes:

| id_planta | nombre    | nombre_cientifico     | familia        | epoca_floracion | habitat                   | descripcion                                                                 | imagen_ruta           |
|-----------|-----------|-----------------------|----------------|-----------------|---------------------------|-----------------------------------------------------------------------------|-----------------------|
| 1         | Rosa      | Rosa spp.             | Rosaceae       | Primavera       | Jardines y zonas templadas | Planta ornamental conocida por sus flores coloridas y fragantes.            | images/plantas/Rosa.jpg |
| 2         | Lirio     | Lilium spp.           | Liliaceae      | Verano          | Jardines y zonas templadas | Planta ornamental conocida por sus flores grandes, vistosas y fragantes.    | images/plantas/Lirio.jpg |
| 3         | Girasol   | Helianthus annuus     | Asteraceae     | Verano          | Campos y jardines          | Planta conocida por sus grandes flores amarillas que siguen el movimiento del sol. | images/plantas/Girasol.jpg |
| 4         | Tulipán   | Tulipa spp.           | Liliaceae      | Primavera       | Jardines y zonas templadas | Planta ornamental con flores en forma de copa y colores variados.           | images/plantas/Tulipan.jpg |
| 5         | Orquídea  | Orchidaceae           | Orchidaceae    | Todo el año     | Selvas y zonas tropicales  | Planta exótica conocida por sus flores de formas y colores únicos.           | images/plantas/Orquidea.jpg |

---
