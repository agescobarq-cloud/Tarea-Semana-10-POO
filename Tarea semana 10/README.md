# Sistema de Gestión de Inventarios

Proyecto académico desarrollado en Python utilizando **Programación Orientada a Objetos (POO)** para gestionar el inventario de una tienda pequeña.  
Incluye persistencia en archivo de texto y manejo de excepciones.

## Descripción del Proyecto

Este sistema permite:

- Añadir productos nuevos (con validación de ID único)
- Eliminar productos por ID
- Actualizar cantidad o precio de un producto existente
- Buscar productos por nombre (coincidencia parcial)
- Listar todos los productos del inventario
- **Persistencia**: todos los cambios se guardan automáticamente en un archivo `inventario.txt`
- **Recuperación**: al iniciar el programa se cargan automáticamente los productos del archivo
- Manejo de errores en operaciones de archivo (archivo no existe, permisos denegados, líneas mal formadas, etc.)

## Estructura del Proyecto
sistema-inventarios/
├── modelos/
│   └── producto.py          # Clase Producto con atributos y getters/setters
├── servicios/
│   └── inventario.py        # Clase Inventario (lógica principal + persistencia)
├── main.py                  # Punto de entrada + menú interactivo en consola
├── inventario.txt           # Archivo de datos (se genera automáticamente)
└── README.md                # Este archivo
text
