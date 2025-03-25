# Proyecto de Gestión de Inventarios para una Tienda de Barrio

## Descripción

Desarrollar un software de gestión de inventarios para una tienda de barrio utilizando el stack de *Java con Spring Boot* para el backend, *React.js* para el frontend y *MongoDB* como base de datos. El sistema debe incluir una API RESTful que permita manejar los productos en el inventario a través de las operaciones básicas de un CRUD (Crear, Leer, Actualizar, Eliminar). Además, la API debe ser desplegada en *Azure* utilizando *GitHub Actions* para automatizar el proceso de despliegue.

---

## Requisitos Funcionales

### 1. API RESTful con Spring Boot:
- *POST* /productos: Agregar un nuevo producto al inventario.
- *GET* /productos: Listar todos los productos disponibles en el inventario.
- *PUT* /productos/{id}: Actualizar la información de un producto en el inventario.
- *DELETE* /productos/{id}: Eliminar un producto del inventario.

### 2. Interfaz Gráfica en React:
- Una página principal que muestre solo los productos disponibles en el inventario (recuperados desde la API).
- La interfaz debe mostrar el nombre del producto, precio y cantidad disponible.
- La interfaz debe ser sencilla y fácil de usar para los empleados de la tienda.

### 3. Pruebas:
- Implementar pruebas unitarias para la API RESTful que verifiquen que las operaciones CRUD funcionan correctamente.

---

## Requisitos Técnicos

### 1. Backend:
- Utilizar *Java* con *Spring Boot* para crear la API RESTful.
- La base de datos será *MongoDB, por lo que se debe configurar **Spring Data MongoDB* para interactuar con la base de datos.
- La API debe permitir operaciones CRUD sobre los productos (nombre, precio, cantidad, etc.).

### 2. Frontend:
- Desarrollar la interfaz gráfica con *React.js* para visualizar los productos del inventario.
- Mostrar los productos con su nombre, precio y cantidad disponible.
- Implementar una interfaz sencilla y clara para que los empleados de la tienda puedan visualizar el inventario de forma intuitiva.

### 3. Base de Datos:
- Utilizar *MongoDB* como base de datos NoSQL para almacenar la información de los productos (nombre, precio, cantidad, etc.).
- Configurar la conexión de MongoDB en *Spring Boot* a través de *Spring Data MongoDB*.

### 4. Despliegue en Azure con GitHub Actions:
- El código de la API y el frontend deben estar almacenados en un repositorio GitHub.
- Utilizar *GitHub Actions* para automatizar el proceso de integración continua (CI) y despliegue continuo (CD) en *Azure*.
- Crear un pipeline de *GitHub Actions* que se ejecute al hacer un push a la rama principal (main o master) del repositorio.
- El pipeline debe incluir los siguientes pasos:
  - Ejecutar pruebas unitarias y de integración.
  - Empaquetar la aplicación (backend y frontend) y desplegarla automáticamente en *Azure* (Azure Web Apps o Azure Kubernetes Service, según se decida).

---

## Consideraciones

- *Validaciones:* Asegúrate de incluir validaciones en los datos de entrada para garantizar que los productos tengan los campos necesarios (nombre, precio, cantidad).
- *Interfaz de Usuario:* La interfaz gráfica debe ser responsiva y mostrar los productos de manera clara y ordenada. Debe ser fácil de usar para los empleados de la tienda.
- *Despliegue:* El despliegue debe ser automatizado mediante *GitHub Actions* y funcionar correctamente en la nube de *Azure*.
