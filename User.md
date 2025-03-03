# Ventana de User (Vista de Usuario)

## Descripción

La ventana de **User** es la interfaz principal para los usuarios normales. Permite ver la lista de plantas disponibles, buscar plantas por nombre y ver los detalles de cada planta seleccionada. Esta vista tiene funcionalidades limitadas en comparación con la vista de administrador, ya que los usuarios normales no pueden agregar, editar o eliminar plantas.

## Características Principales

1. **Lista de Plantas:**
   - Muestra una lista de plantas disponibles en la base de datos.
   - Cada planta se muestra con su nombre común.

2. **Buscador:**
   - Permite buscar plantas por nombre.
   - Filtra la lista de plantas en tiempo real según el texto ingresado.

3. **Detalles de la Planta:**
   - Al seleccionar una planta de la lista, se muestran sus detalles:
     - Nombre científico.
     - Familia.
     - Época de floración.
     - Hábitat.
     - Descripción.
     - Imagen de la planta.

4. **Botones:**
   - **Atrás:** Cierra la sesión y regresa a la ventana de Login.

## Flujo de la Ventana

1. **Acceso a la Vista:**
   - El usuario accede a esta ventana después de iniciar sesión correctamente.

2. **Carga de Datos:**
   - Al abrirse la ventana, se cargan las plantas desde la base de datos y se muestran en la lista.

3. **Búsqueda de Plantas:**
   - El usuario puede escribir en el campo de búsqueda para filtrar la lista de plantas por nombre.

4. **Selección de una Planta:**
   - Al hacer clic en una planta de la lista, se muestran sus detalles en el panel derecho.

5. **Cierre de Sesión:**
   - Al hacer clic en **Atrás**, el usuario es redirigido a la ventana de Login.
