
# 🧴 Sistema de Registro de Pacientes Dermatológicos

## 📝 Descripción
Sistema web para la gestión de pacientes en un consultorio dermatológico. Permite registrar, consultar y gestionar historiales clínicos, citas, usuarios y reportes.

## ❗ Problema identificado
El consultorio actualmente utiliza registros físicos y hojas de cálculo, lo que genera pérdida de información, lentitud en búsquedas y falta de trazabilidad clínica.

## ✅ Solución
Implementación de un sistema digital modular, con arquitectura en capas, interfaz web intuitiva, autenticación de roles y soporte para exportación de reportes.

## 🏗️ Arquitectura
- Frontend: HTML/CSS/JS con framework responsive
- Backend: Java con Spring Boot (MVC)
- Base de datos: MySQL/PostgreSQL
- CI/CD: GitHub + Travis-CI
- Infraestructura: Nginx (web) + Tomcat (aplicación)

---

## 📑 Tabla de contenidos (ToC)
- [Descripción](#-descripción)
- [Problema identificado](#-problema-identificado)
- [Solución](#-solución)
- [Arquitectura](#-arquitectura)
- [Requerimientos](#-requerimientos)
- [Instalación](#-instalación)
- [Configuración](#-configuración)
- [Uso](#-uso)
  - [Usuario final](#usuario-final)
  - [Administrador](#administrador)
- [Contribución](#-contribución)
- [Roadmap](#-roadmap)

---

## 📦 Requerimientos

### Aplicación
- Java 17+
- Spring Boot 3.x
- Maven o Gradle
- Git

### Infraestructura
- Servidor web: Nginx o Apache
- Servidor de aplicaciones: Tomcat o Spring Boot embebido
- Base de datos: MySQL o PostgreSQL

### Paquetes adicionales
- Lombok
- JUnit 5
- ModelMapper
- Travis-CI

---

## ⚙️ Instalación

### Ambiente de desarrollo
```bash
git clone https://github.com/usuario/proyecto-dermatologia.git
cd proyecto-dermatologia
./mvnw clean install
```

### Ejecutar pruebas manualmente
```bash
./mvnw test
```

### Despliegue local o en Heroku
1. Crear archivo `.env` con variables de entorno.
2. Ejecutar con `java -jar target/app.jar`
3. Para Heroku:
```bash
heroku create
git push heroku main
```

---

## 🔧 Configuración

### Archivos
- `application.properties` o `application.yml` para entorno.
- Variables de entorno `.env` para base de datos y tokens.

### Base de datos
```properties
spring.datasource.url=jdbc:mysql://localhost:3306/dermatologia
spring.datasource.username=usuario
spring.datasource.password=secreto
```

---

## 📚 Uso

### Usuario final
- Iniciar sesión y consultar historial clínico.
- Registrar pacientes y agendar citas.
- Exportar reportes en PDF.

### Administrador
- Gestionar usuarios y roles.
- Respaldo y restauración de la base de datos.
- Control de accesos.

---

## 🤝 Contribución

1. Clonar el repositorio:
```bash
git clone https://github.com/usuario/proyecto-dermatologia.git
```
2. Crear una nueva rama:
```bash
git checkout -b feature/nueva-funcionalidad
```
3. Hacer cambios y enviar PR:
```bash
git push origin feature/nueva-funcionalidad
```
4. Esperar revisión y merge.

---

## 🛣️ Roadmap

- [ ] Módulo de alergias y medicamentos
- [ ] Buscador rápido de pacientes por nombre o cita
- [ ] Exportación avanzada de reportes
- [ ] Integración con sistema de facturación
- [ ] Soporte multilingüe
