# Proyecto: Sistema de Gestión de Plantas

## Descripción del Proyecto

Este proyecto es una aplicación de escritorio desarrollada en Java utilizando JavaFX para la interfaz gráfica y MySQL como base de datos. El sistema permite gestionar un catálogo de plantas, incluyendo su información básica, imágenes y estado (activa o eliminada). Está diseñado para ser utilizado por administradores y usuarios con diferentes niveles de acceso.

## Características Principales

### 1. **Gestión de Plantas**
   - **Agregar nuevas plantas:** Permite registrar nuevas plantas con detalles como nombre, nombre científico, familia, época de floración, hábitat, descripción y una imagen.
   - **Editar plantas:** Permite modificar la información de las plantas existentes.
   - **Eliminar plantas:** Marca las plantas como eliminadas (borrado lógico) en lugar de eliminarlas físicamente de la base de datos.
   - **Buscar plantas:** Los usuarios pueden buscar plantas por nombre en la lista.

### 2. **Gestión de Usuarios**
   - **Roles de usuario:** Los usuarios pueden ser administradores o usuarios normales.
   - **Autenticación:** Los usuarios deben iniciar sesión para acceder al sistema.
   - **Cambio de contraseña:** Los usuarios pueden cambiar su contraseña.

### 3. **Interfaz Gráfica**
   - **JavaFX:** La interfaz gráfica está construida con JavaFX, lo que permite una experiencia de usuario moderna y responsive.
   - **Vistas separadas:** Diferentes paneles para agregar, editar y eliminar plantas, así como para gestionar usuarios.

### 4. **Base de Datos**
   - **MySQL:** Se utiliza MySQL para almacenar la información de las plantas y los usuarios.
   - **Procedimientos almacenados:** Algunas operaciones de la base de datos se realizan mediante procedimientos almacenados para mejorar la eficiencia.

## Estructura del Proyecto

### 1. **Carpetas Principales**
   - `src/main/java`: Contiene el código fuente de la aplicación.
     - `com.idar.how2javafx.controllers`: Controladores de las vistas.
     - `com.idar.how2javafx.objets`: Modelos de datos (por ejemplo, la clase `Planta`).
     - `lib`: Clases utilitarias para interactuar con la base de datos (`SqlLib`).
   - `src/main/resources`: Recursos como archivos FXML, imágenes y estilos CSS.
     - `scenes`: Archivos FXML para las vistas.
     - `images`: Imágenes utilizadas en la interfaz gráfica.

### 2. **Vistas**
   - **Login:** Pantalla de inicio de sesión para autenticar a los usuarios.
   - **User View:** Vista para usuarios normales, donde pueden ver la lista de plantas y sus detalles.
   - **Admin View:** Vista para administradores, con funcionalidades completas de gestión de plantas y usuarios.

### 3. **Base de Datos**
   - **Tablas:**
     - `planta`: Almacena la información de las plantas.
     - `usuario`: Almacena la información de los usuarios.
   - **Procedimientos almacenados:**
     - `AgregarPlanta`, `EliminarPlanta`, `CambiarNombrePlanta`, etc.
