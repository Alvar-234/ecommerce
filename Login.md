# Ventana de Login

## Descripción

La ventana de **Login** es la primera interfaz que ven los usuarios al iniciar la aplicación. Su propósito es autenticar a los usuarios y permitirles acceder al sistema según su rol (administrador o usuario normal).

## Características Principales

1. **Campos de Entrada:**
   - **Usuario:** Campo de texto para ingresar el nombre de usuario.
   - **Contraseña:** Campo de texto para ingresar la contraseña (oculta con caracteres de seguridad).

2. **Botones:**
   - **Iniciar Sesión:** Valida las credenciales del usuario y lo redirige a la vista correspondiente (Admin o User).
   - **Salir:** Cierra la aplicación.

3. **Validación de Credenciales:**
   - Las credenciales se verifican contra la base de datos.
   - Si las credenciales son incorrectas, se muestra un mensaje de error.

4. **Diseño:**
   - Interfaz limpia y minimalista.
   - Colores y estilos consistentes con el tema de la aplicación.

## Flujo de la Ventana

1. **Inicio de la Aplicación:**
   - La ventana de Login se abre automáticamente al iniciar la aplicación.

2. **Ingreso de Credenciales:**
   - El usuario ingresa su nombre de usuario y contraseña.

3. **Validación:**
   - Al hacer clic en **Iniciar Sesión**, el sistema verifica las credenciales en la base de datos.
   - Si las credenciales son válidas, el usuario es redirigido a la vista correspondiente:
     - **Admin View:** Si el usuario es un administrador.
     - **User View:** Si el usuario es un usuario normal.
   - Si las credenciales son incorrectas, se muestra un mensaje de error.

4. **Cierre de la Aplicación:**
   - Si el usuario hace clic en **Salir**, la aplicación se cierra.

## Código Relacionado

### Archivo FXML (`login.fxml`)
```xml
<AnchorPane fx:id="loginPane" prefHeight="400" prefWidth="600" xmlns="http://javafx.com/javafx/8" xmlns:fx="http://javafx.com/fxml/1" fx:controller="com.idar.how2javafx.controllers.LoginController">
   <children>
      <Label layoutX="250" layoutY="100" text="Iniciar Sesión" style="-fx-font-size: 24px; -fx-font-weight: bold;" />
      <Label layoutX="150" layoutY="150" text="Usuario:" />
      <TextField fx:id="usernameField" layoutX="250" layoutY="150" promptText="Ingrese su usuario" />
      <Label layoutX="150" layoutY="200" text="Contraseña:" />
      <PasswordField fx:id="passwordField" layoutX="250" layoutY="200" promptText="Ingrese su contraseña" />
      <Button fx:id="loginButton" layoutX="250" layoutY="250" text="Iniciar Sesión" onAction="#handleLogin" />
      <Button fx:id="exitButton" layoutX="350" layoutY="250" text="Salir" onAction="#handleExit" />
   </children>
</AnchorPane>
