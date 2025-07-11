# 🛒 Orders — Sistema de Gestión de Pedidos

Proyecto desarrollado en **C# con .NET** y **Blazor**, que permite la gestión completa de usuarios, productos, pedidos y catálogo. Incluye control de roles y autenticación, así como administración avanzada de pedidos en diferentes estados.

---

## 🚀 Tecnologías utilizadas

- **Lenguaje:** C#
- **Framework:** .NET 7+  
- **Frontend:** Blazor
- **Base de datos:** SQL Server
- **ORM:** Entity Framework Core
- **Autenticación:** Identity con tokens (JWT)

---

## 👥 Roles y funcionalidades

El sistema tiene 3 tipos de usuarios: **Administrador**, **Usuario** y **Anónimo**. Cada uno tiene acceso a diferentes funcionalidades:

| Funcionalidad | Administrador | Usuario | Anónimo |
|---------------|:-------------:|:-------:|:-------:|
| Ingresar al sistema con email y contraseña | ✅ | ✅ | ❌ |
| Editar datos de usuario (incluyendo foto de perfil) | ✅ | ✅ | ❌ |
| Cambiar contraseña | ✅ | ✅ | ❌ |
| Recuperar contraseña (con token enviado por correo) | ✅ | ✅ | ❌ |
| Administrar usuarios (crear, ver, editar, eliminar) | ✅ | ❌ | ❌ |
| Administrar países, estados y departamentos | ✅ | ❌ | ❌ |
| Confirmar cuenta vía correo electrónico | ✅ | ✅ | ❌ |
| Administrar categorías de productos | ✅ | ❌ | ❌ |
| Administrar productos (crear, editar, borrar, imágenes) | ✅ | ❌ | ❌ |
| Ver catálogo de productos y filtrarlos | ✅ | ✅ | ✅ |
| Agregar productos al carrito de compras | ✅ | ✅ | ✅ |
| Confirmar el pedido | ✅ | ✅ | ❌ |
| Ver estado de mis pedidos (nuevo, en proceso, enviado, confirmado, etc.) | ✅ | ✅ | ❌ |
| Administrar pedidos de todos los usuarios y cambiar su estado | ✅ | ❌ | ❌ |

---

## 📦 Estructura del Proyecto

El proyecto se divide en varias capas independientes:

- **Orders.Backend:** Lógica de negocio y API RESTful en .NET
- **Orders.Frontend:** Interfaz de usuario en Blazor
- **Orders.Shared:** Clases y modelos compartidos entre backend y frontend
- **Orders.Tests:** Pruebas unitarias
- **Orders:** (Eliminada como subrepositorio, ahora integrada)

---

## 🔧 Instalación

1. Clona este repositorio:
   ```bash
   git clone https://github.com/Juandicode2017/Orders1.git