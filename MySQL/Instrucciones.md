#Instrucciones para configurar la base de datos 

1.- Instalar MySQL Server
    - `sudo apt update`
    - `sudo apt install mysql-Server`

2.- Entrar a MySQL en la terminal
    - `sudo mysql`

3.- Crear una nueva base de datos
    - `CREATE DATABASE detectorsintomas;`

4.- Seleccionar la base de datos
    - `use detectorsintomas;`

5.- Crear una tabla llamada registro que contenga todos los campos necesarios
    - `CREATE TABLE registro (id INT(6) UNSIGNED AUTO_INCREMENT PRIMARY KEY, fecha TIMESTAMP DEFAULT CURRENT_TIMESTAMP, nombre CHAR (248) NOT NULL, correo CHAR (248) NOT NULL, temp FLOAT(4,2) NOT NULL, bpm INT(1) UNSIGNED NOT NULL, sp02 INT(1) UNSIGNED NOT NULL, protodiagnostico CHAR (248) NOT NULL);`

6.- Crear un nuevo usuario de MySQL
- `CREATE USER 'newuser'@'localhost' IDENTIFIED BY 'password';`
- `GRANT ALL PRIVILEGES ON *.* TO 'hugohugo'@'localhost';`




Para salir de los comandos de MySQL, usar el comando exit;