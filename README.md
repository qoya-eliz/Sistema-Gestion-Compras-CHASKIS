# 🚌 Sistema Web de Gestión y Compra de Pasajes Interprovinciales - "Los Chaskis"

![Estado](https://img.shields.io/badge/Estado-En_Desarrollo-yellow)
![Universidad](https://img.shields.io/badge/UTP-Ingeniería_de_Sistemas-red)
![Curso](https://img.shields.io/badge/Curso-Marcos_de_Desarrollo_Web-blue)

## 📌 Información General del Proyecto
* **Universidad:** Universidad Tecnológica del Perú (UTP)
* **Facultad:** Facultad de Ingeniería
* **Carrera:** Ingeniería de Sistemas e Informática
* **Curso:** Marcos de Desarrollo Web (100000S157)
* **Docente:** Moreno Cueva, Máximo Alberto
* **Año:** 2026

### 👥 Integrantes del Equipo
* Aguilar Vila, Angeles Abril
* Auqui Alvarez, Diego Alonso
* Chuquiruna Aguilar, Elsa Elizabeth
* Torres Arevalo, Freddy Joel

---

## 🏬 Descripción de la Empresa
**Agencia de Transportes "Los Chaskis" S.A.** es una empresa peruana dedicada al transporte interprovincial de pasajeros y carga terrestre. Su modelo operativo conecta las principales ciudades de la costa y sierra del Perú (Lima, Piura, Chiclayo, Cajamarca) garantizando altos estándares de puntualidad, seguridad vial y monitoreo de flota en tiempo real.

---

## 🎯 Objetivos del Sistema

### Objetivo General
Desarrollar e implementar un sistema web integral para mejorar la gestión de la venta de pasajes y el control de abordaje de la empresa de transporte Los Chaskis, centralizando la información operativa y proporcionando acceso controlado a clientes, administradores y supervisores.

### Objetivos Específicos
1. Diseñar una interfaz web responsiva utilizando HTML, JavaScript y Bootstrap 5 para facilitar la interacción de los usuarios y del personal operativo.
2. Desarrollar la lógica de negocio mediante Spring Boot y Spring Web para administrar usuarios, buses, asientos, rutas, viajes, pasajeros y ventas.
3. Implementar un mecanismo de autenticación y autorización con Spring Security y JWT para diferenciar accesos según los roles de Cliente, Administrador y Supervisor.
4. Diseñar e implementar una base de datos MySQL relacional optimizada para garantizar el almacenamiento transaccional y la integridad de la información.

---

## 🛠️ Stack Tecnológico

| Capa / Herramienta | Tecnología Seleccionada |
| :--- | :--- |
| **Frontend** | HTML5, CSS3, JavaScript (Vanilla/DOM), Bootstrap 5, Thymeleaf |
| **Backend** | Java 21 (LTS), Spring Boot, Spring Web, Spring Data JPA, Hibernate, Spring Validator |
| **Seguridad** | Spring Security & JWT (JSON Web Tokens) |
| **Base de Datos** | MySQL Server 8.0 (Gestionado en MySQL Workbench) |
| **Gestor de Dependencias** | Apache Maven 3.8+ / 3.9+ |
| **Entorno Recomendado** | Visual Studio Code (con *Extension Pack for Java*) |
| **Control de Versiones** | Git & GitHub |

---

## 📋 Funcionalidades Principales (Alcance)

* 🔐 **Autenticación & Roles:** Control de acceso unificado con Spring Security para *Administrador*, *Supervisor de Terminal* y *Cliente*.
* 🎟️ **Portal B2C (Cliente):** Buscador de itinerarios por origen/destino, selección interactiva de asientos en croquis (2x2), registro filiatorio de pasajeros y simulación de compra con comprobante digital.
* 🛠️ **Backoffice Administrativo:** Mantenimiento de flota de buses, maquetación de asientos, programación de rutas/horarios, gestión de usuarios y consulta de reportes analíticos.
* 🚌 **Módulo de Embarque (Supervisor):** Verificación en plataforma del manifiesto de pasajeros por bus/placa y actualización del estado de abordaje (*Pendiente*, *Abordó*, *Ausente*).
* 📄 **Gestión de Comprobantes:** Generación interna y simulación de boletas y facturas electrónicas desglosando Subtotal e IGV (18%).

---

## ⚙️ Requisitos e Instalación

### **Prerrequisitos**
* **Java Development Kit (JDK):** Versión 21 (LTS) instalada.
* **MySQL Server:** Versión 8.0 en ejecución.
* **Editor / IDE Recomendado:** Visual Studio Code (con *Extension Pack for Java*).
* **Gestor de Construcción:** Maven 3.8+ / 3.9+ (no requiere instalación global previa si se utiliza `./mvnw`).

---

## 🗄️ Importación de la Base de Datos para el Equipo

El repositorio incluye el archivo ejecutable `.sql` con la estructura completa de las **10 tablas relacionales** y los datos semilla en la ruta `/database/los_chaskis_db.sql`.

### **Instrucciones para Restaurar la BD en MySQL Workbench:**

1. **Clonar el proyecto** desde GitHub e ir a la carpeta `/database/`.
2. Abrir **MySQL Workbench** y conectarse a la instancia local de MySQL.
3. En el menú superior, seleccionar **`Server` > `Data Import`**.
4. En la opción **Import Options**, seleccionar **`Import from Self-Contained File`**.
5. Haz clic en el botón `...` y busca la ruta del archivo `database/los_chaskis_db.sql` dentro del proyecto.
6. En **Default Target Schema**, haz clic en `New...` y nombra la base de datos como: **`los_chaskis_db`**.
7. En la pestaña inferior derecha, haz clic en **`Start Import`**.
8. Una vez finalizado, refresca el panel de esquemas (*Schemas*) para verificar que se hayan creado las 10 tablas (`buses`, `viajes`, `ventas`, `pasajeros`, etc.).

> 💡 **Nota alternativa:** También puedes abrir el archivo `database/los_chaskis_db.sql` directamente en un Query Tab de MySQL Workbench y presionar el ícono del rayo (⚡) para ejecutar todo el script.

---

## 🚀 Guía de Clonación y Ejecución para el Equipo

Abre tu terminal o consola Git Bash y ejecuta:
```bash
git clone [https://github.com/TU-USUARIO/los-chaskis-web.git](https://github.com/TU-USUARIO/los-chaskis-web.git)
cd los-chaskis-web
