# Instalando MySql:

Instalo servidor 8.0 desde linea de comandos: sudo apt install mysql-server-8.0
Bajo de internet el paquete .deb y lo instalo con el comando: sudo apt install ./mysql-workbench-community_8.038-1ubuntu24.04_amd64.deb

No me deja usar el usuario root, parece que está restringido por razones de seguridad que pueda conectarse por tcp/ip. Pero si puedo entrar a administrar mysql desde el terminal con el comando:  sudo mysql -u root      \q para salir

Después de charlar un rato con ChatGPT, creo un usuario admin con todos los privilegios, que solo se puede conectar desde el localhost:

sudo mysql -u root
CREATE USER 'admin'@'localhost' IDENTIFIED BY 'mipassword';
GRANT ALL PRIVILEGES ON *.* TO 'admin'@'localhost' WITH GRANT OPTION;
FLUSH PRIVILEGES;
\q

Ahora ya me deja entrar y crear bases de datos ...

# Configurando un usuario para peticiones de prueba Mysql.

Para evitar que se produzcan cambios en la estructura de la base de datos, 
el usuario solo podra realizar operaciones CRUD, pero no de administración.

```
CREATE USER 'app_user'@'localhost' IDENTIFIED BY 'password_app';
GRANT SELECT, INSERT, UPDATE, DELETE ON mi_base_datos.* TO 'app_user'@'localhost';
FLUSH PRIVILEGES; 
```


