# Ventana de Admin (Vista de Administrador)

## Descripción

La ventana de **Admin** es la interfaz principal para los administradores del sistema. Permite gestionar completamente el catálogo de plantas, incluyendo agregar, editar y eliminar plantas. Además, los administradores pueden gestionar usuarios y sus roles. Esta vista proporciona funcionalidades avanzadas que no están disponibles para los usuarios normales.

## Características Principales

1. **Gestión de Plantas:**
   - **Agregar Plantas:** Permite registrar nuevas plantas con detalles como nombre, nombre científico, familia, época de floración, hábitat, descripción y una imagen.
   - **Editar Plantas:** Permite modificar la información de las plantas existentes.
   - **Eliminar Plantas:** Marca las plantas como eliminadas (borrado lógico) en lugar de eliminarlas físicamente de la base de datos.
   - **Tabla de Plantas:** Muestra una tabla con todas las plantas, incluyendo su estado (activa o eliminada).

2. **Gestión de Usuarios:**
   - **Agregar Usuarios:** Permite registrar nuevos usuarios con un nombre, contraseña y rol.
   - **Editar Usuarios:** Permite cambiar el nombre, contraseña o rol de un usuario existente.
   - **Eliminar Usuarios:** Elimina usuarios de la base de datos.

3. **Buscador:**
   - Permite buscar plantas por nombre en la tabla.

4. **Botones:**
   - **Atrás:** Cierra la sesión y regresa a la ventana de Login.
   - **Usuarios:** Redirige a la vista de gestión de usuarios.

## Flujo de la Ventana

1. **Acceso a la Vista:**
   - El administrador accede a esta ventana después de iniciar sesión correctamente.

2. **Carga de Datos:**
   - Al abrirse la ventana, se cargan las plantas y los usuarios desde la base de datos y se muestran en las tablas correspondientes.

3. **Gestión de Plantas:**
   - **Agregar:** El administrador completa el formulario y hace clic en "Agregar" para registrar una nueva planta.
   - **Editar:** Selecciona una planta de la tabla, modifica los campos y hace clic en "Modificar".
   - **Eliminar:** Selecciona una planta de la tabla y hace clic en "Eliminar".

4. **Gestión de Usuarios:**
   - **Agregar:** Completa el formulario de usuario y hace clic en "Agregar".
   - **Editar:** Selecciona un usuario de la tabla, modifica los campos y hace clic en "Modificar".
   - **Eliminar:** Selecciona un usuario de la tabla y hace clic en "Eliminar".

5. **Cierre de Sesión:**
   - Al hacer clic en **Atrás**, el administrador es redirigido a la ventana de Login.
