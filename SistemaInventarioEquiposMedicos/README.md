# MedInventory | Sistema de Inventario de Equipos Médicos

Página web de presentación y prototipo interactivo de un sistema para administrar el inventario de productos y equipos médicos de una empresa con una matriz y varias sucursales.

## Descripción

MedInventory propone una forma sencilla de consultar existencias, detectar productos por agotarse y registrar traspasos de mercancía entre la matriz y las sucursales. Este repositorio contiene la página del proyecto: una landing page con contenido promocional y una demostración interactiva del inventario que funciona con datos de ejemplo.

## Problema

El control manual de productos (libretas u hojas de cálculo separadas) dificulta conocer las existencias reales, registrar movimientos y saber qué mercancía se envió a cada sucursal. Los faltantes suelen descubrirse cuando el cliente ya solicitó el producto.

## Objetivo

Facilitar la administración del inventario mediante un sistema que permita registrar productos, consultar existencias por ubicación y controlar los movimientos entre la matriz y las sucursales.

## Contenido de la página

| Sección | Qué muestra |
|---|---|
| Barra de oferta | Aviso de lanzamiento con el código `LANZA20` (se puede cerrar) |
| Inicio | Propuesta del sistema e inventario interactivo de demostración |
| Cinta de características | Franja animada con las funciones principales |
| El problema | Comparación entre trabajar sin sistema y con MedInventory |
| Funciones | Catálogo de productos, existencias por ubicación, traspasos, alertas y reportes (en pestañas) |
| Proceso | Flujo de reabastecimiento en 4 pasos |
| Roles | Administrador, encargado de sucursal y almacén de matriz |
| Planes | Básico, Profesional y Empresarial, con interruptor mensual/anual |
| Oferta de lanzamiento | Código copiable y cuenta regresiva hasta el 31 de diciembre de 2026 |
| Opiniones | Testimonios de ejemplo |
| Preguntas frecuentes | Dudas comunes en acordeones desplegables |
| Llamado final y contacto | Franja de invitación y formulario de demostración con validación |

## Demostración interactiva

El panel de inventario del inicio permite:

- Cambiar entre **Matriz**, **Sucursal Saucos** y **Sucursal Centro**.
- Buscar productos por nombre.
- Ver el estado de cada producto: *Disponible*, *Stock bajo* o *Agotado*, según su nivel mínimo.
- Usar **Pedir a matriz** en una sucursal para simular un traspaso: se descuenta la cantidad de la matriz, se suma a la sucursal y se muestra un aviso del movimiento.

Los productos y cantidades son datos de ejemplo definidos en el arreglo `productos` dentro del script. No hay base de datos ni servidor: los cambios se pierden al recargar la página.

## Contenido promocional

- **Planes:** el interruptor mensual/anual cambia los precios mostrados, y cada botón de plan rellena el mensaje del formulario de contacto.
- **Oferta:** el código `LANZA20` se copia con un clic y la cuenta regresiva se actualiza cada segundo; al terminar la fecha, el aviso cambia solo.
- **Aviso:** los precios, la oferta y los testimonios son ficticios y están marcados como ejemplo en la página.

## Funcionalidades del sistema propuesto

- Registro y administración de productos con nivel mínimo por producto.
- Control de existencias por ubicación.
- Organización por categorías.
- Registro de movimientos de inventario (entradas, salidas y traspasos).
- Administración de sucursales.
- Alertas de stock bajo y consulta de reportes.
- Permisos según el rol del usuario.

> La página implementa la demostración de existencias, estados y traspasos. El resto de las funcionalidades corresponde al alcance del sistema completo.

## Tecnologías

- **HTML5** para la estructura semántica.
- **CSS3** para el diseño: variables, Grid, Flexbox, degradados, animaciones y diseño adaptable a celular.
- **JavaScript** (sin librerías) para el inventario interactivo, pestañas, menú móvil, cuenta regresiva, animaciones al hacer scroll y validación del formulario.
- **Git y GitHub** para el control de versiones.

## Diseño, accesibilidad y adaptabilidad

- Animaciones de entrada al hacer scroll, barra de progreso de lectura, menú que resalta la sección actual y botón para volver arriba.
- Navegación por teclado con foco visible y roles ARIA en pestañas y avisos dinámicos.
- Respeta la preferencia de movimiento reducido del sistema.
- Se adapta a computadora, tableta y teléfono.

## Estructura del proyecto

```
medinventory/
├── medinventory.html   # Página completa (HTML, CSS y JavaScript)
└── README.md
```

## Cómo ejecutarlo

1. Clona o descarga el repositorio.
2. Abre `medinventory.html` en cualquier navegador. No requiere instalación ni servidor.

```bash
git clone <url-del-repositorio>
cd medinventory
```

## Proyecto académico

Desarrollo de un sistema de inventario para una empresa de equipos médicos, realizado como proyecto de la carrera de Tecnologías de la Información.