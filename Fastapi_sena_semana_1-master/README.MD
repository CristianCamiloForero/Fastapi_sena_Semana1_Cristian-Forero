readme = r"""# 📋 Sistema de Gestión de Tareas 1.0.0

Este documento describe la API del *Sistema de Gestión de Tareas*.

## 📄 Especificación OpenAPI 3.1
La especificación completa está disponible en **/openapi.json**.

---

## 🚀 Módulos y Endpoints

### 👥 Módulo de Usuarios (*Users*)

- **POST /users/**  
  - **Descripción:** *Crea un nuevo usuario*.  
  - **Permisos:** *N/A* (generalmente público para registro).

- **GET /users/{user_id}**  
  - **Descripción:** *Obtiene los detalles de un usuario específico*.  
  - **Parámetros de ruta:**  
    - `user_id` (*integer*): ID del usuario.  
  - **Permisos:** *Requiere autenticación*.

- **PUT /users/{user_id}**  
  - **Descripción:** *Actualiza la información de un usuario existente*.  
  - **Parámetros de ruta:**  
    - `user_id` (*integer*): ID del usuario a actualizar.  
  - **Permisos:** *Requiere autenticación* (generalmente el propietario del perfil).

- **DELETE /users/{user_id}**  
  - **Descripción:** *Elimina un usuario del sistema*.  
  - **Parámetros de ruta:**  
    - `user_id` (*integer*): ID del usuario a eliminar.  
  - **Permisos:** *Requiere autenticación* (propietario o administrador).

---

### 📂 Módulo de Categorías (*Categories*)

- **GET /categories/**  
  - **Descripción:** *Lista todas las categorías disponibles*.  
  - **Permisos:** *Requiere autenticación*.

- **POST /categories/**  
  - **Descripción:** *Crea una nueva categoría*.  
  - **Permisos:** *Requiere autenticación*.

- **PUT /categories/{category_id}**  
  - **Descripción:** *Actualiza una categoría existente*.  
  - **Parámetros de ruta:**  
    - `category_id` (*integer*): ID de la categoría a actualizar.  
  - **Permisos:** *Requiere autenticación*.

- **DELETE /categories/{category_id}**  
  - **Descripción:** *Elimina una categoría*.  
  - **Parámetros de ruta:**  
    - `category_id` (*integer*): ID de la categoría a eliminar.  
  - **Permisos:** *Requiere autenticación*.

---

### ✅ Módulo de Tareas (*Tasks*)

- **POST /tasks/**  
  - **Descripción:** *Crea una nueva tarea*.  
  - **Permisos:** *Requiere autenticación*.

- **GET /tasks/**  
  - **Descripción:** *Lista todas las tareas del usuario autenticado*.  
  - **Permisos:** *Requiere autenticación*.

- **GET /tasks/{task_id}**  
  - **Descripción:** *Obtiene los detalles de una tarea específica*.  
  - **Parámetros de ruta:**  
    - `task_id` (*integer*): ID de la tarea.  
  - **Permisos:** *Requiere autenticación*.

- **PUT /tasks/{task_id}**  
  - **Descripción:** *Actualiza una tarea existente*.  
  - **Parámetros de ruta:**  
    - `task_id` (*integer*): ID de la tarea a actualizar.  
  - **Permisos:** *Requiere autenticación*.

- **DELETE /tasks/{task_id}**  
  - **Descripción:** *Elimina una tarea*.  
  - **Parámetros de ruta:**  
    - `task_id` (*integer*): ID de la tarea a eliminar.  
  - **Permisos:** *Requiere autenticación*.

---

### 📊 Módulo de Estadísticas (*Statistics*)

- **GET /stats/overview**  
  - **Descripción:** *Resumen general de las tareas del usuario*.  
  - **Permisos:** *Requiere autenticación*.

- **GET /stats/productivity**  
  - **Descripción:** *Informe detallado de productividad*.  
  - **Permisos:** *Requiere autenticación*.

---

### 🌐 Endpoints por Defecto (*Default*)

- **GET /**  
  - **Descripción:** Punto de verificación del servicio.  
  - **Respuesta:** `Hello World` 👋

- **GET /info**  
  - **Descripción:** Información básica de la API (versión y metadatos). ℹ️
"""
