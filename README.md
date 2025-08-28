# Proyecto de Ejemplo MySQL - SENA GFC 10

Este proyecto contiene un ejemplo de base de datos en MySQL para el curso de grado 10. Incluye scripts para la creación de la base de datos, tablas, inserción de datos y consultas básicas utilizando `INNER JOIN`.

## Archivos incluidos

- **MySQL-Ejemplo-DB.sql**: Script para crear la base de datos `SENA_GFC_10`, las tablas principales (`Citys`, `Documents`, `Persons`) y poblarlas con datos de ejemplo.
- **MySQL-Ejemplo-Query.sql**: Script con consultas SQL para obtener información de las personas, mostrando datos relacionados como ciudad y tipo de documento, usando `INNER JOIN`.
- **LICENSE**: Licencia del proyecto.

## Estructura de la Base de Datos

- **Citys**: Tabla de ciudades.
- **Documents**: Tipos de documentos de identidad.
- **Persons**: Información personal, enlazada con ciudad y tipo de documento mediante claves foráneas.

## Uso de los scripts

1. **Crear la base de datos y poblarla**
	- Ejecuta el script `MySQL-Ejemplo-DB.sql` en tu gestor de MySQL (por ejemplo, MySQL Workbench).
	- Esto creará la base de datos, las tablas y agregará datos de ejemplo.

2. **Realizar consultas**
	- Ejecuta el script `MySQL-Ejemplo-Query.sql` para ver ejemplos de consultas que unen las tablas y muestran información completa de las personas.

## Ejemplo de consulta principal

La consulta principal une las tablas `Persons`, `Citys` y `Documents` para mostrar:
- ID de la persona
- Tipo y número de documento
- Apellidos y nombres
- Fecha de nacimiento
- Dirección
- Ciudad de residencia

## Requisitos

- MySQL 5.7 o superior
- Gestor de base de datos (MySQL Workbench, DBeaver, etc.)

## ¿Cómo ejecutar los scripts?

### 1. Usando la terminal de MySQL

1. Abre la terminal de comandos (CMD o PowerShell).
2. Accede al cliente de MySQL con tu usuario y contraseña:
	```sh
	mysql -u root -p -h localhost -P 3306
	```
3. Una vez dentro, ejecuta el script de creación de la base de datos:
	```sql
	source "ruta/completa/MySQL-Ejemplo-DB.sql";
	```
4. Para ejecutar el script de consultas:
	```sql
	source "ruta/completa/MySQL-Ejemplo-Query.sql";
	```

### 2. Usando MySQL Workbench

1. Abre MySQL Workbench y conecta a tu servidor.
2. Haz clic en "File" > "Open SQL Script" y selecciona `MySQL-Ejemplo-DB.sql`.
3. Ejecuta el script con el botón "Run" (el rayo).
4. Repite el proceso para `MySQL-Ejemplo-Query.sql` para ejecutar las consultas.

### 3. Usando XAMPP (phpMyAdmin)

1. Inicia XAMPP y asegúrate que el servicio MySQL esté activo.
2. Abre phpMyAdmin desde el panel de XAMPP.
3. Selecciona la pestaña "Importar" y elige el archivo `MySQL-Ejemplo-DB.sql` para cargar la base de datos y los datos.
4. Para ejecutar consultas, ve a la pestaña "SQL", copia el contenido de `MySQL-Ejemplo-Query.sql` y ejecútalo.

---

## Autor

Andrés Felipe Gutiérrez Rivera

---

Este proyecto es solo para fines educativos y de práctica en SQL y bases de datos relacionales.