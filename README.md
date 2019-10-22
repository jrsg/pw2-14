# Instrucciones

### Base de datos

* Tabla usuarios
  * id  (int, llave primaria, auto incrementable)
  * email (varchar 100)
  * password (hash, varchar 32)  
  * creacion (datetime)
  * actualizacion (datetime)
  
* Tabla propositos
  * id  (int, llave primaria, auto incrementable)
  * id_usuario (int, llave foránea)
  * proposito (varchar 150)
  * vencimiento (date)

### Aplicación

#### Directorio raíz 
* index.php - pantalla inicial
* login.php - proceso de identificación y autenticación de usuarios
* logout.php - proceso de cierre de sesión

#### Directorio usuario
* nuevo.php - formulario de registro de usuarios nuevos
* guardar.php - proceso para guardar nuevos usuarios
* perfil.php - formulario con datos del usuario
* actualizar.php - proceso de actualización de los datos del usuario

#### Directorio propósitos
* index.php - lista de propósitos registrados
* proposito.php - formulario de captura de propósitos
* guardar.php - proceso para guardar propósitos
* borrar.php - proceso para eliminar propósitos

Nota: la aplicación debe permitir a usuarios registrados y autenticados crear, actualizar y borrar sus propósitos de año nuevo.

### Diagrama

![diagrama](diagrama.png "Diagrama de flujo")
