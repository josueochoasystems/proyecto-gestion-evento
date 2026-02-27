# 🎓 Sistema de Gestión de Eventos

Plataforma web y móvil para la gestión integral de eventos académicos (como jornadas científicas), con control de asistencia mediante códigos QR, categorización de ponencias y autenticación segura.

## 📌 Descripción del Proyecto

El Sistema de Gestión de Eventos permite organizar, administrar y controlar jornadas académicas, congresos y seminarios, incluyendo:

Registro de participantes

Gestión de ponencias por categorías

Generación y escaneo de códigos QR

Control de asistencia en tiempo real

Reportes y estadísticas del evento

La plataforma está compuesta por:

### 🌐 Aplicación Web (React)

### 📱 Aplicación Móvil (Flutter)

### ⚙ Backend API REST (Laravel)

### 🔐 Autenticación OAuth2 con Laravel Passport

### 🗄 Base de Datos MySQL

## 🏗️ Arquitectura del Sistema

El sistema sigue una arquitectura basada en API REST desacoplada:

Backend: API REST desarrollada con Laravel

Autenticación: OAuth2 con Laravel Passport

Base de Datos: MySQL

Frontend Web: React

Aplicación Móvil: Flutter

Comunicación: JSON sobre HTTP/HTTPS

## 🧠 Fundamento Tecnológico
### 🔹 Laravel

Laravel es un framework PHP moderno que facilita el desarrollo de aplicaciones web con arquitectura MVC.

Ventajas:

Eloquent ORM

Migraciones de base de datos

Sistema de colas

Middleware

Seguridad integrada

### 🔹 Laravel Passport

Laravel Passport es un paquete oficial que implementa un servidor OAuth2 para autenticación segura mediante tokens.

Permite:

Emisión de tokens JWT

Autenticación basada en API

Protección de endpoints

Gestión de clientes OAuth

### 🔹 MySQL

MySQL es un sistema de gestión de bases de datos relacional ampliamente utilizado en aplicaciones empresariales.

Características:

Soporte de transacciones

Integridad referencial

Alta disponibilidad

Escalabilidad

### 🔹 React

React es una biblioteca JavaScript para construir interfaces web modernas basadas en componentes reutilizables.

Ventajas:

Virtual DOM

SPA (Single Page Application)

Alto rendimiento

Gran ecosistema

### 🔹 Flutter

Flutter es un framework desarrollado por Google para crear aplicaciones móviles multiplataforma (Android e iOS) desde una sola base de código.

Ventajas:

Alto rendimiento

Diseño moderno

Desarrollo multiplataforma

Integración con APIs REST

## 🎯 Funcionalidades Principales
### 👤 Gestión de Usuarios

Registro de participantes

Roles (Administrador, Organizador, Ponente, Asistente)

Autenticación segura con OAuth2

### 📚 Gestión de Ponencias

Creación de ponencias

Asignación a categorías

Programación por fecha y horario

Asignación de sala

### 🏷 Gestión de Categorías

Categorías temáticas (Ej: Ingeniería, Salud, Educación)

Asociación de ponencias a categorías

### 📱 Control de Asistencia con QR

Generación de código QR único por participante

Escaneo desde aplicación móvil

Validación en tiempo real

Prevención de duplicidad de registro

### 📊 Reportes y Estadísticas

Total de asistentes por ponencia

Asistencia por categoría

Participación por usuario

Exportación de datos

### 🔄 Flujo del Sistema

El usuario se registra en la plataforma.

Se genera un código QR único asociado a su identidad.

El asistente presenta su QR en la entrada de cada ponencia.

El organizador escanea el QR mediante la app móvil.

El backend valida el token y registra la asistencia.

Los datos se actualizan en tiempo real.

## 🔐 Seguridad

Autenticación OAuth2 con Laravel Passport

Tokens Bearer

Middleware de protección de rutas

Validación de duplicidad de asistencia

Protección contra acceso no autorizado

## 🚀 Instalación y Configuración
### 1️⃣ Clonar el repositorio

git clone https://github.com/josueochoasystems/proyecto-gestion-evento.git

cd proyecto-gestion-evento


### 2️⃣ Configurar Backend (Laravel)

cd backend

composer install

cp .env.example .env

php artisan key:generate

Configurar base de datos en .env:

DB_DATABASE=gestion_eventos

DB_USERNAME=root

DB_PASSWORD=tu_password

Migrar base de datos:

php artisan migrate

php artisan passport:install

php artisan serve

### 3️⃣ Ejecutar Frontend (React)

cd gestion-evento-react

npm install

npm start


### 4️⃣ Ejecutar Aplicación Móvil (Flutter)
cd gestion_evento_flutter

flutter pub get

flutter run

## 📊 Casos de Uso

Registro de participante

Registro de ponencia

Generación de QR

Escaneo y validación de asistencia

Generación de reportes

## 📈 Mejoras Futuras

Integración con notificaciones push

Certificados automáticos en PDF

Dashboard analítico avanzado

Implementación de Docker

CI/CD

Despliegue en nube (AWS, Azure, GCP)

## 🧪 Pruebas

Pruebas unitarias con PHPUnit

Pruebas de API

Testing de componentes React

Testing de widgets en Flutter

---

## 👨‍💻 Autor

**Josue Ochoa**  
Estudiante de Ingeniería de Sistemas

Proyecto académico desarrollado para la gestión digital de jornadas científicas y eventos universitarios con control de asistencia inteligente mediante QR.
---

✨ *Gracias por visitar el proyecto* ✨