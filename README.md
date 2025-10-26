# 🛍️ Sistema de Gestión de Productos - Backend Laravel

Backend desarrollado en Laravel para un sistema de gestión de productos y categorías.

## 🚀 Características

- **API RESTful** para gestión de productos y categorías
- **Relación uno a muchos** entre categorías y productos
- **Validación de datos** en todas las operaciones
- **Migrations y Seeders** para estructura de base de datos
- **CORS configurado** para comunicación con frontend Angular

## 📋 Endpoints de la API

### Productos
- `GET /api/productos` - Listar todos los productos
- `POST /api/productos` - Crear nuevo producto
- `GET /api/productos/{id}` - Obtener producto específico
- `PUT /api/productos/{id}` - Actualizar producto
- `DELETE /api/productos/{id}` - Eliminar producto

### Categorías
- `GET /api/categorias` - Listar todas las categorías
- `POST /api/categorias` - Crear nueva categoría
- `GET /api/categorias/{id}` - Obtener categoría específica
- `PUT /api/categorias/{id}` - Actualizar categoría
- `DELETE /api/categorias/{id}` - Eliminar categoría

## 🗄️ Estructura de Base de Datos

### Tabla: categorias
- `id` (Primary Key)
- `nombre` (string)
- `timestamps`

### Tabla: productos
- `id` (Primary Key)
- `nombre` (string)
- `precio` (decimal)
- `categoria_id` (Foreign Key)
- `timestamps`

## 🛠️ Instalación

1. Clonar el repositorio
2. Instalar dependencias: `composer install`
3. Configurar `.env` con datos de base de datos
4. Ejecutar migraciones: `php artisan migrate`
5. Ejecutar seeders: `php artisan db:seed`
6. Iniciar servidor: `php artisan serve`

## 🔗 Frontend

Este backend está diseñado para trabajar con el frontend en Angular:
[Repositorio Frontend Angular](https://github.com/tuusuario/frontend-productos)

## 👨‍💻 Desarrollado por

Daniel Alejandro - Trabajo académico
