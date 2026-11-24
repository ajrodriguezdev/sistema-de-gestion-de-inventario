# 📦 Sistema de Gestión de Inventario

<p align="center">
  <img src="https://img.shields.io/badge/Java-17%2B-orange?style=for-the-badge&logo=openjdk&logoColor=white"/>
  <img src="https://img.shields.io/badge/Spring_Boot-Backend-6DB33F?style=for-the-badge&logo=springboot&logoColor=white"/>
  <img src="https://img.shields.io/badge/MySQL-Database-4479A1?style=for-the-badge&logo=mysql&logoColor=white"/>
  <img src="https://img.shields.io/badge/Maven-Build-C71A36?style=for-the-badge&logo=apachemaven&logoColor=white"/>
</p>

<p align="center">
  Aplicación backend para administrar productos, existencias, ventas y movimientos de inventario mediante servicios REST.
</p>

---

## 📌 Descripción del proyecto

El Sistema de Gestión de Inventario es una aplicación diseñada para facilitar el control y administración de productos dentro de un negocio.

Su objetivo es centralizar la información de los productos, controlar las entradas y salidas de mercancía, registrar ventas y mantener actualizadas las existencias disponibles.

La solución estará desarrollada con Java y Spring Boot, utilizando MySQL como sistema de gestión de bases de datos.

## 🎯 Objetivos

- Administrar el catálogo de productos.
- Controlar las entradas y salidas de inventario.
- Registrar movimientos de mercancía.
- Gestionar ventas y actualizar existencias.
- Identificar productos con bajo stock.
- Implementar reglas de negocio para evitar inconsistencias.
- Diseñar una estructura backend escalable y mantenible.

## ⚙️ Funcionalidades

| Funcionalidad | Descripción | Estado |
|---|---|---|
| Gestión de productos | Crear, consultar, actualizar y eliminar productos | 📋 Pendiente |
| Categorías | Clasificar productos por categorías | 📋 Pendiente |
| Control de existencias | Consultar cantidades disponibles | 📋 Pendiente |
| Entradas de inventario | Registrar ingreso de mercancía | 📋 Pendiente |
| Salidas de inventario | Registrar retiros de productos | 📋 Pendiente |
| Gestión de ventas | Registrar ventas y descontar existencias | 📋 Pendiente |
| Alertas de stock | Identificar productos con existencias bajas | 📋 Pendiente |
| Historial de movimientos | Consultar operaciones realizadas | 📋 Pendiente |

## 🛠️ Tecnologías utilizadas

**Backend**
- Java
- Spring Boot
- Spring Web
- Spring Data JPA
- Hibernate

**Base de datos**
- MySQL
- SQL

**Herramientas**
- Maven
- Git y GitHub
- Postman
- IntelliJ IDEA o Visual Studio Code

## 🏗️ Arquitectura del proyecto

```text
src/
└── main/
    ├── java/com/inventario/
    │   ├── controller/
    │   ├── service/
    │   ├── repository/
    │   ├── entity/
    │   ├── dto/
    │   ├── exception/
    │   └── InventarioApplication.java
    └── resources/
        └── application.properties
```

### Responsabilidad de las capas

| Capa | Responsabilidad |
|---|---|
| Controller | Exponer los endpoints REST |
| Service | Gestionar las reglas de negocio |
| Repository | Acceder a la base de datos |
| Entity | Representar productos, ventas y movimientos |
| DTO | Gestionar los datos de entrada y salida |
| Exception | Centralizar el manejo de errores |

## 🗄️ Modelo de datos

Se contempla trabajar inicialmente con las siguientes entidades:

- **Product:** información de los productos.
- **Category:** clasificación de productos.
- **InventoryMovement:** registro de entradas y salidas.
- **Sale:** información de las ventas.
- **SaleDetail:** detalle de los productos vendidos.

Las relaciones y atributos definitivos se establecerán durante el diseño de la base de datos.

## 🔗 Endpoints proyectados

| Método | Endpoint | Descripción |
|---|---|---|
| POST | `/api/products` | Registrar producto |
| GET | `/api/products` | Consultar productos |
| GET | `/api/products/{id}` | Consultar producto por ID |
| PUT | `/api/products/{id}` | Actualizar producto |
| DELETE | `/api/products/{id}` | Eliminar producto |
| POST | `/api/inventory/entries` | Registrar entrada |
| POST | `/api/inventory/exits` | Registrar salida |
| GET | `/api/inventory/movements` | Consultar movimientos |
| POST | `/api/sales` | Registrar venta |

*Los endpoints son una propuesta inicial y podrán ajustarse durante el desarrollo.*

## 🚀 Instalación y ejecución

### Requisitos previos

- Java 17 o superior.
- Maven.
- MySQL.
- Git.

### 1. Clonar el repositorio

```bash
git clone https://github.com/ajrodriguezdev/sistema-gestion-inventario.git
```

### 2. Ingresar al proyecto

```bash
cd sistema-gestion-inventario
```

### 3. Configurar la base de datos

Crear una base de datos llamada `gestion_inventario` y configurar las credenciales en `application.properties`.

```properties
spring.datasource.url=jdbc:mysql://localhost:3306/gestion_inventario
spring.datasource.username=${DB_USERNAME}
spring.datasource.password=${DB_PASSWORD}
```

### 4. Ejecutar la aplicación

```bash
mvn spring-boot:run
```

## 🧪 Pruebas

Se utilizará Postman para verificar los endpoints, validar operaciones CRUD y comprobar el comportamiento de las reglas de negocio relacionadas con las existencias y las ventas.

## 🗺️ Roadmap

- [ ] Configuración inicial de Spring Boot.
- [ ] Diseño de la base de datos MySQL.
- [ ] Implementación de entidades y relaciones.
- [ ] Desarrollo de gestión de productos.
- [ ] Implementación de categorías.
- [ ] Control de entradas y salidas.
- [ ] Implementación de ventas.
- [ ] Validación de existencias y reglas de negocio.
- [ ] Historial de movimientos.
- [ ] Pruebas con Postman.
- [ ] Documentación de la API.

## 👩‍💻 Autora

**Andrea Rodriguez**  
Ingeniera de Sistemas | Backend Developer

- GitHub: [@ajrodriguezdev](https://github.com/ajrodriguezdev)
- LinkedIn: [Perfil profesional](https://www.linkedin.com/in/aj-rodriguez-g)

---

<p align="center">
  Desarrollado con Java, Spring Boot y MySQL.
  <br/>
  <b>Gestionando información, optimizando procesos. 💻</b>
</p>
