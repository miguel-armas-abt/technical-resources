# INSTALACIÓN MYSQL
- [Descargar](https://dev.mysql.com/downloads/mysql/) `Windows (x86, 64-bit), ZIP Archive` y reservar los binarios.
- **Ruta sugerida**: `C:\dev-environment\mysql\mysql-8.2.0`

Ingresar a los binarios e instalar:
```
cd bin
mysqld --initialize
mysqld --install "mysql80"
```

Inciar el servidor:
```
net start mysql80
```

Inciar sesión con el password por defecto:
```
mysql -u root
```

Cambiar de password:
```
ALTER USER 'root'@'localhost' IDENTIFIED BY 'qwerty';
```

Detener el servidor:
```
net stop mysql80
```

Inciar sesión con el password creado:
```
mysql -u root -p"qwerty"
```
