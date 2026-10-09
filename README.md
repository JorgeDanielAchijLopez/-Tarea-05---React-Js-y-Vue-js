# FerreControl

Sistema de gestión para ferretería, construido con Vue 3 y Vite.

## Ejecutar

Abre esta carpeta en Visual Studio Code y escribe en su terminal:

```powershell
npm install
npm run dev
```

Abre la dirección local que te indique la terminal (normalmente http://localhost:5173/).

En Windows también puedes hacer doble clic en `INICIAR.bat`.

## Funciones

- Panel general con total de productos, existencias, ventas y alertas.
- Inventario: altas, consulta, edición, eliminación, búsqueda y filtro por categoría.
- Carrito de compras, cálculo de totales y validación de stock disponible.
- Registro de ventas, descuento automático de inventario y consulta de historial.
- Exportación del historial de ventas a CSV.
- Persistencia con localStorage (sin base de datos externa).
- Restauración de datos de demostración.

## Estructura

- `src/App.vue`: navegación, lógica del inventario y ventas.
- `src/components/ProductForm.vue`: formulario de alta y edición.
- `src/components/StatCard.vue`: tarjetas reutilizables del panel.
- `src/style.css`: estilos y diseño adaptable.
- `src/main.js`: punto de entrada que monta la aplicación.
- `index.html`: documento inicial.
- `package.json`: librerías y comandos del proyecto.

## Datos

Incluye 10 productos de demostración, y permite crear otros. Almacena datos **solo en el navegador actual**; si se borra el almacenamiento local, se restablecen los ejemplos. No necesita internet una vez instaladas las dependencias (excepto para descargar la tipografía opcional).

## Nota de tecnología

Este proyecto está hecho en **Vue 3** y sus componentes terminan en `.vue`. No es React. La consigna de clase indica que quien presentó Vue.js debe realizar la tarea en React.js: confirma con el docente si esta tecnología es aceptada antes de entregarlo.
