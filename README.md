# 🔒 Administrador de Contraseñas - Proyecto Final

## 📖 Descripción del Proyecto

Sistema de gestión de contraseñas desarrollado en Python que permite almacenar, consultar y administrar contraseñas de forma segura mediante codificación Base64. Este proyecto demuestra el dominio de conceptos fundamentales de programación en Python.

## 🎯 Objetivos del Proyecto

- Implementar un sistema CRUD (Crear, Leer, Actualizar, Eliminar) completo
- Aplicar principios de seguridad básica mediante codificación
- Demostrar organización de código mediante funciones modulares
- Crear una interfaz de usuario intuitiva por consola
- Gestionar estructuras de datos (diccionarios) de manera eficiente

## ✨ Características Principales

### Funcionalidades Implementadas

1. **➕ Agregar Contraseñas**
   - Registro de nuevos sitios web/servicios
   - Validación de duplicados
   - Codificación automática en Base64

2. **📋 Listar Sitios**
   - Visualización ordenada alfabéticamente
   - Interfaz limpia y profesional

3. **🔍 Consultar Contraseñas**
   - Búsqueda por nombre de sitio
   - Decodificación automática
   - Manejo de errores para sitios no encontrados

4. **🗑️ Eliminar Contraseñas**
   - Eliminación segura de registros
   - Confirmación de operaciones

5. **🔐 Seguridad**
   - Codificación Base64 de contraseñas
   - Almacenamiento temporal en memoria

## 🛠️ Tecnologías Utilizadas

- **Lenguaje:** Python 3.x
- **Módulos Estándar:**
  - `base64` - Para codificación/decodificación
  - `os` - Para futuras mejoras de sistema de archivos

## 📂 Estructura del Código

```
proyecto_final.py
├── Funciones de Lógica (Codificación/Decodificación)
│   ├── codificar_contrasena()
│   └── decodificar_contrasena()
├── Funciones de Datos (CRUD)
│   ├── agregar_contrasena()
│   ├── obtener_contrasena()
│   └── eliminar_contrasena()
├── Funciones de Interfaz
│   ├── pedir_y_agregar()
│   ├── mostrar_una_contrasena()
│   ├── mostrar_todos_los_sitios()
│   └── pedir_y_eliminar()
└── Función Principal
    └── menu_principal()
```

## 🚀 Instalación y Uso

### Requisitos Previos

- Python 3.6 o superior instalado
- No requiere dependencias externas

### Pasos de Instalación

1. **Clonar o descargar el archivo:**
   ```bash
   # Si está en un repositorio
   git clone [URL_DEL_REPOSITORIO]
   
   # O simplemente descargar proyecto_final.py
   ```

2. **Navegar al directorio:**
   ```bash
   cd pylatino
   ```

3. **Ejecutar el programa:**
   ```bash
   python proyecto_final.py
   ```

## 📱 Guía de Uso

### Menú Principal

Al ejecutar el programa, verás el siguiente menú:

```
========================================
🔒 Administrador de Contraseñas (v1.0)
========================================
1. Agregar nueva contraseña
2. Ver **lista** de sitios guardados
3. Ver una contraseña **específica**
4. Eliminar contraseña
5. Salir
========================================
```

### Ejemplos de Uso

#### Agregar una contraseña:
```
Seleccione una opción (1-5): 1
➡️ Ingrese el nombre del sitio web/servicio: Gmail
➡️ Ingrese la contraseña: MiPassword123
✅ Contraseña para 'Gmail' agregada y codificada exitosamente.
```

#### Ver sitios guardados:
```
Seleccione una opción (1-5): 2
--- 🌐 SITIOS GUARDADOS ---
| * Facebook
| * Gmail
| * Netflix
--------------------------
```

#### Consultar una contraseña:
```
Seleccione una opción (1-5): 3
➡️ Ingrese el nombre del sitio para ver su contraseña: Gmail
🔐 Contraseña para 'Gmail': **MiPassword123**
```

## 🔒 Consideraciones de Seguridad

### Implementadas
- ✅ Codificación Base64 de contraseñas
- ✅ Validación de entradas vacías
- ✅ Prevención de duplicados

### Limitaciones Actuales
- ⚠️ Las contraseñas se almacenan solo en memoria (se pierden al cerrar)
- ⚠️ Base64 es codificación, NO encriptación
- ⚠️ No hay autenticación de usuario

### Mejoras Futuras Recomendadas
- 🔄 Persistencia en archivo encriptado
- 🔄 Implementar encriptación real (AES, Fernet)
- 🔄 Agregar contraseña maestra
- 🔄 Exportar/importar contraseñas
- 🔄 Generador de contraseñas seguras

## 📊 Conceptos de Python Demostrados

### Estructuras de Datos
- ✓ Diccionarios para almacenamiento clave-valor
- ✓ Manipulación de strings y bytes

### Control de Flujo
- ✓ Bucles `while` para menú interactivo
- ✓ Condicionales `if/elif/else`
- ✓ Manejo de casos especiales

### Funciones
- ✓ Funciones con parámetros y valores de retorno
- ✓ Docstrings para documentación
- ✓ Separación de responsabilidades

### Módulos
- ✓ Importación de módulos estándar
- ✓ Uso de `if __name__ == "__main__"`

### Buenas Prácticas
- ✓ Código comentado y documentado
- ✓ Nombres descriptivos de variables
- ✓ Organización modular
- ✓ Validación de entradas

## 🧪 Casos de Prueba

### Pruebas Funcionales

1. **Agregar contraseña válida:** ✅ Debe confirmar agregado
2. **Agregar duplicado:** ✅ Debe mostrar advertencia
3. **Consultar existente:** ✅ Debe mostrar contraseña
4. **Consultar inexistente:** ✅ Debe mostrar error
5. **Eliminar existente:** ✅ Debe confirmar eliminación
6. **Eliminar inexistente:** ✅ Debe mostrar error
7. **Listar sin datos:** ✅ Debe indicar vacío
8. **Entrada vacía:** ✅ Debe rechazar

## 👨‍💻 Autor

**Proyecto Final - Curso de Python**
- Fecha: Diciembre 2025
- Versión: 1.0

## 📄 Licencia

Este proyecto es de uso educativo y libre para modificación y distribución.

## 🙏 Agradecimientos

Proyecto desarrollado como parte del curso de Python, demostrando:
- Comprensión de estructuras de datos
- Manejo de funciones y modularización
- Implementación de interfaces de usuario
- Aplicación de conceptos de seguridad básica

---

**Nota:** Este es un proyecto educativo. Para uso en producción, se recomienda utilizar bibliotecas especializadas como `cryptography` o gestores de contraseñas profesionales.
