# 🛍️ Tu Tienda Online

**Plataforma desarrollada con Angular + Spring Boot**.

Documentación visual y funcional del sistema dividida por roles: **Cliente** y **Administrador**.

🧩 Credenciales para Probar la Aplicación:

Puedes acceder a la aplicación utilizando los siguientes usuarios de prueba según el rol:

👤 Rol Cliente

- Email: cliente_test@gmail.com

- Contraseña: 12345678

🛠️ Rol Administrador

- Email: admin@gmail.com

- Contraseña: admin123

💳 Datos de Prueba para Mercado Pago

Para realizar una compra de prueba, debes iniciar sesión en modo privado/incógnito y utilizar el siguiente comprador de prueba:

- Usuario comprador: TETE9700722

- Contraseña: Y8in2kBZCV

💡 Nota:
La aplicación está desplegada en Render (backend) y Vercel (frontend), en servicios gratis por lo que anda media lenta.

💰 Precio del código: $5000

---

## 📑 Índice

- [🙍‍♂️ Rol Cliente](#-rol-cliente)
  - [🏠 Inicio](#-inicio)
  - [🧾 Detalle del Producto](#-detalle-del-producto)
  - [🔎 Búsqueda de Productos](#-búsqueda-de-productos)
  - [👤 Mi Cuenta](#-mi-cuenta)
  - [👤 Perfil](#-perfil)
  - [🚚 Opciones de Entrega](#-opciones-de-entrega)
  - [🧾 mis Pedidos](#-mis-pedidos)
  - [📦 Detalles del Pedido](#-detalles-del-pedido)
  - [🛒 Carrito de Compras](#-carrito-de-compras)
  - [💳 Checkout](#-checkout)
  - [✅ Confirmación de Pago y Creación del Pedido](#-confirmación-de-pago-y-creación-del-pedido)
  - [💰 Modal y Respuesta de Compra](#-modal-y-respuesta-de-compra)
- [⚙️ Rol Administrador](#️-rol-administrador)
  - [📊 Dashboard](#-dashboard)
  - [👥 Gestión de Clientes](#-gestión-de-clientes)
  - [🛍️ Productos Comunes](#️-productos-comunes)
  - [🌟 Productos Destacados](#-productos-destacados)
  - [📦 Carga Masiva de Productos](#-carga-masiva-de-productos)
  - [🚚 Logística – Métodos de Envío](#-logística--métodos-de-envío)
  - [💰 Compra Mínima del Carrito](#-compra-mínima-del-carrito)
  - [🚛 Zonas de Envío](#-zonas-de-envío)
  - [🧾 Gestión de Pedidos](#-gestión-de-pedidos)
  - [📦 Detalle de Pedido](#-detalle-de-pedido)
  - [🗂️ Categorías](#️-categorías)
  - [Características de Productos](#características-de-productos)
  - [Subcategorías de Productos](#subcategorías-de-productos)
  - [Slider Principal de la Página de Inicio](#slider-principal-de-la-página-de-inicio)

- [🧩 Tecnologías Principales](#-tecnologías-principales)


---

## 🙍‍♂️ Rol Cliente

### 🏠 Inicio

En esta sección se presentan los **productos destacados** junto con dos _sliders_ configurables desde el panel de administración.  
El **buscador principal** permite filtrar productos por **nombre, categoría, subcategoría, características o marca**, ofreciendo una experiencia de búsqueda **dinámica y personalizada**.

![Inicio](https://res.cloudinary.com/dlv9gwnw3/image/upload/v1761580413/home_ojsacs.png)

---

### 🧾 Detalle del Producto

Muestra toda la información del producto: **imagen, nombre, categoría, peso, precio y características**.  
Si tiene descuento, se muestra el **precio original tachado** y el **porcentaje de ahorro**.  
Incluye botón para **agregar al carrito**, calcular el **costo de envío** y ver **productos relacionados**.

![Detalle del producto](https://res.cloudinary.com/dlv9gwnw3/image/upload/v1761580886/detalle_dn6fcb.png)

---

### 🔎 Búsqueda de Productos

Listado filtrado según la búsqueda del usuario.  
Incluye **filtros por marca, categoría y promociones**, además de ordenamiento por precio o nombre.

![Búsqueda](https://res.cloudinary.com/dlv9gwnw3/image/upload/v1761582932/busqueda-productos_vvvcpp.png)

---

### 👤 Mi Cuenta

Desde este panel podés consultar y modificar toda la información de tu cuenta personal, administrar tus opciones de entrega y revisar el historial de tus pedidos realizados dentro del eCommerce.

![Búsqueda](https://res.cloudinary.com/dlv9gwnw3/image/upload/v1761666610/micuenta_pmkxtv.png)

---

### 👤 Perfil

- Aqui puedes actualizar los datos del cliente.

![Búsqueda](https://res.cloudinary.com/dlv9gwnw3/image/upload/v1761667362/miperfil_wftayc.png)

---

### 🚚 Opciones de Entrega

Desde esta sección puedes crear y seleccionar tu dirección de envío de manera sencilla.
Tienes dos opciones disponibles:

- 📍 Usar la API de Google Maps para establecer tu ubicación directamente en el mapa.

- ✏️ Ingresarla manualmente si prefieres hacerlo de forma tradicional.

Esta será la dirección donde se entregarán tus pedidos.

![Google](https://res.cloudinary.com/dlv9gwnw3/image/upload/v1761667735/zona-envio-1_m3eqpj.png)

---

![Manual](https://res.cloudinary.com/dlv9gwnw3/image/upload/v1761667736/zona-envio-2_mpyhmv.png)

---

### 🧾 Mis Pedidos

En esta vista, el usuario puede consultar el historial completo de pedidos realizados desde su cuenta.
Cada pedido muestra información detallada como la fecha de compra, el total, los productos adquiridos y el estado actual del pedido.
Además, se adapta perfectamente a dispositivos móviles, garantizando una experiencia fluida y responsive.

- 📸 Vista general de pedidos:
Permite acceder fácilmente al detalle de cada compra mediante el botón "Ver detalles del pedido".
También incluye una estructura ordenada para visualizar los artículos, precios y estado de entrega.

![Carrito](https://res.cloudinary.com/dlv9gwnw3/image/upload/v1761668702/Pedidos_ei3xzz.png)

---

### 📦 Detalles del Pedido
Esta sección muestra la información completa del pedido seleccionado, incluyendo:

- 📍 Dirección de envío

- 💳 Método de pago utilizado

- 💰 Resumen del pedido (subtotal, descuentos, costos de envío y total)

- 🚚 Estado del pedido con línea de progreso visual

- 🧾 Listado detallado de los productos comprados, cantidades y precios unitarios

La interfaz permite al usuario seguir el estado de su compra en tiempo real y descargar el comprobante una vez que el pedido está en proceso o completado.

![Carrito](https://res.cloudinary.com/dlv9gwnw3/image/upload/v1761668702/Pedidos-2_u4eax0.png)

---

### 🛒 Carrito de Compras

Muestra los productos seleccionados con control de cantidad, **validación de stock** y **actualización en tiempo real** del total.  
Incluye un **importe mínimo requerido** antes de finalizar la compra y manejo de **concurrencia** entre usuarios.

![Carrito](https://res.cloudinary.com/dlv9gwnw3/image/upload/v1761606062/carrito-compras_tutk7f.png)

---

### 💳 Checkout

Permite revisar, modificar y confirmar los productos antes de pagar.  
Cuenta con:

- Subtotales, descuentos y totales automáticos.
- Botones de modificación (+ / -).
- Validación del stock.
- Políticas de reemplazo por falta de productos.

![Checkout](https://res.cloudinary.com/dlv9gwnw3/image/upload/v1761584331/checkout_bf25ju.png)

---

### ✅ Confirmación de Pago y Creación del Pedido

Flujo automatizado con **Mercado Pago** y actualización por **Webhook**:

1. Se recibe el webhook de Mercado Pago.
2. Se valida el estado del pago.
3. Se actualiza el stock.
4. Se genera el pedido y se envía correo de confirmación.

![Confirmación](https://res.cloudinary.com/dlv9gwnw3/image/upload/v1761585397/finalizar-compra_ethaym.png)

---

### 💰 Modal y Respuesta de Compra

Visualización del proceso de pago y respuesta de compra exitosa.

![Modal](https://res.cloudinary.com/dlv9gwnw3/image/upload/v1761587490/modal-mercado-pago_boxtdz.png)
![Compra exitosa](https://res.cloudinary.com/dlv9gwnw3/image/upload/v1761587490/compra-exito_q3i0br.png)
![Respuesta](https://res.cloudinary.com/dlv9gwnw3/image/upload/v1761587492/respuesta-compra_gjowxh.png)

---

## ⚙️ Rol Administrador

### 📊 Dashboard

Visualiza métricas del ecommerce: productos registrados, ventas del día y globales.  
Permite configurar imagen de marca y fecha de inicio del comercio.

![Dashboard](https://res.cloudinary.com/dlv9gwnw3/image/upload/v1761595326/dashboard_d2oves.png)

---

### 👥 Gestión de Clientes

Listado de clientes con **buscador avanzado** y **paginación**.

![Clientes](https://res.cloudinary.com/dlv9gwnw3/image/upload/v1761596604/usuarios_r6eufh.png)

---

### 🛍️ Productos Comunes

Permite **listar, editar, crear y desactivar productos**.  
Incluye carga de hasta 3 imágenes, cálculo automático de descuentos y etiquetado de ofertas.

![Productos comunes](https://res.cloudinary.com/dlv9gwnw3/image/upload/v1761597648/listar-productos-comunes_t8tyaz.png)

---

### 🌟 Productos Destacados

Gestiona los productos visibles en la **página principal**.  
Permite activar, editar o eliminar artículos destacados.

![Destacados](https://res.cloudinary.com/dlv9gwnw3/image/upload/v1761598805/listar-productos-destacados_hph5dz.png)

---

### 📦 Carga Masiva de Productos

Permite importar productos mediante **archivos .csv** e imágenes **.zip**, optimizando la gestión masiva del catálogo.

![Carga masiva](https://res.cloudinary.com/dlv9gwnw3/image/upload/v1761605460/carga-masiva_bcd23e.png)

---

### 🚚 Logística – Métodos de Envío

Panel para administrar los métodos de envío: propio o tercerizado.  
Permite modificar **plazos, disponibilidad y costos**.

![Logística](https://res.cloudinary.com/dlv9gwnw3/image/upload/v1761606756/logistica-listar_jmnyrz.png)

---

### 💰 Compra Mínima del Carrito

Define el **monto mínimo requerido** para finalizar una compra, garantizando un valor base en el carrito.

![Compra mínima](https://res.cloudinary.com/dlv9gwnw3/image/upload/v1761607877/compra-minima_d87rcu.png)

---

### 🚛 Zonas de Envío

Consulta y gestión de **zonas de envío** con cobertura en **toda Argentina**.  
Permite actualizar los **costos por región** en tiempo real.

![Zonas de envío](https://res.cloudinary.com/dlv9gwnw3/image/upload/v1761608464/zonas-envio_fgul2f.png)

---

### 🧾 Gestión de Pedidos

Listado de pedidos ordenados del **más reciente al más antiguo**, con buscador y paginación.  
Incluye botón para acceder al **detalle del pedido**.

![Pedidos](https://res.cloudinary.com/dlv9gwnw3/image/upload/v1761609876/listar-pedidos_kx8kst.png)

---

### 📦 Detalle de Pedido

Visualiza toda la información del pedido: dirección, método de pago, resumen, cliente y estado.  
Permite:

- ❌ Cancelar pedido y devolver dinero.
- 🚚 Despachar pedido con seguimiento.
- 🔄 Actualizar estado de entrega.

![Detalle de pedido](https://res.cloudinary.com/dlv9gwnw3/image/upload/v1761610281/detalle-pedido_msehhu.png)

---

### 🗂️ Categorías

Listado y gestión de categorías con subcategorías y productos asociados.  
Si se desactiva una categoría, también se **desactivan todos sus productos**.  
Incluye buscador y opción para crear nuevas categorías.

![Categorías](https://res.cloudinary.com/dlv9gwnw3/image/upload/v1761610627/categorias_w7hjy0.png)

---

### Características de Productos

Esta sección permite gestionar las **características** de los productos que se muestran en el **detalle** de cada artículo.
Cada característica se puede crear, editar o eliminar, y está asociada a una o varias categorías.

✨ Funcionalidades principales

- 🆕 Crear nuevas características por categoría (ejemplo: Marca, Peso, Talle, Gramos, Kilos, Tamaño, Color, etc.).

- ✏️ Editar el nombre o la categoría asignada a una característica existente.

- 🗑️ Eliminar características que ya no estén en uso.

- 🔍 Visualizar características existentes con su ID, nombre y categoría asociada.

- 📦 Las características se muestran dinámicamente al crear productos según la categoría seleccionada.

![Características](https://res.cloudinary.com/dlv9gwnw3/image/upload/v1761616858/caracteristicas_h0dr25.png)

---

### Subcategorías de Productos

Esta sección permite crear y listar subcategorías asociadas a las categorías existentes en el ecommerce.
Las subcategorías se pueden crear, editar o eliminar, y están vinculadas a una categoría principal.

✨ Funcionalidades principales

- 🆕 Crear nuevas subcategorías: asigna un nombre y selecciona la categoría principal a la que pertenecerá.

- ✏️ Editar subcategorías existentes: modificar el nombre.

- 🗑️ Eliminar subcategorías que ya no sean necesarias.

- 🔍 Listado completo: ver todas las subcategorías registradas, con su ID, nombre y categoría asociada.

- 📄 Paginación: navegar fácilmente por grandes cantidades de subcategorías.

- 📦 Las subcategorías disponibles se muestran dinámicamente al crear productos para mantener la consistencia del catálogo.

![Subcategorías](https://res.cloudinary.com/dlv9gwnw3/image/upload/v1761618127/subcategorias_d5hdfb.png)

---

### Slider Principal de la Página de Inicio

Esta sección permite administrar las imágenes de los sliders principales que se muestra en la página de inicio del ecommerce.
Cada slider puede contener hasta 8 imágenes, que se pueden subir, listar o eliminar según se requiera.

✨ Funcionalidades principales

- 🆕 Subir imágenes: agrega nuevas imágenes al slider, respetando la resolución recomendada (1283x352 px, aceptando entre 1080x290 px y 1283x400 px).

- 🗂️ Seleccionar slider: permite elegir entre distintos sliders configurables en el sistema.

- 🗑️ Eliminar imágenes: elimina una imagen específica del slider.

- 🔄 Vaciar slider: borra todas las imágenes de un slider para comenzar de nuevo.

- 📄 Listado de imágenes: visualiza todas las imágenes subidas, con detalles de nombre, tipo y resolución.

- ⚠️ Validación de límite: el sistema no permite subir más de 8 imágenes por slider.

![Slider](https://res.cloudinary.com/dlv9gwnw3/image/upload/v1761618863/sliders_xigequ.png)

---

### 🧩 Tecnologías Principales

Este proyecto está desarrollado utilizando un stack moderno y completo para ofrecer una experiencia de usuario robusta y eficiente, tanto en frontend como en backend.

⚡ Frontend

- Angular 17: Framework principal para el desarrollo de la interfaz de usuario.

- Angular Material: Librería de componentes UI para Angular.

- HTML5 & CSS3 / Sass: Estructura y estilos modernos, incluyendo preprocesador Sass.

- Bootstrap 5: Framework CSS para diseño responsivo y componentes predefinidos.

⚡ Backend

- Java 17: Lenguaje principal del backend.

- Spring Boot: Framework para aplicaciones Java, incluyendo REST APIs.

- Hibernate / JPA: Para manejo de persistencia y relaciones en la base de datos.

- Maven: Gestión de dependencias y compilación del proyecto.

⚡ Base de Datos y Cache

- PostgreSQL: Base de datos relacional.

- Redis Cache: Almacenamiento en caché para mejorar la performance.

⚡ Integraciones y APIs

- MercadoPago: Sistema de pagos integrado.

- Google Maps Geocoding API: Para geolocalización y rutas.

- Spring Security JWT: Autenticación y autorización mediante tokens JWT.

---

## 🏗️ Arquitectura y Buenas Prácticas

Este proyecto aplica una arquitectura modular y buenas prácticas de ingeniería de software para garantizar mantenibilidad, escalabilidad y rendimiento. Se priorizó el **diseño orientado a objetos (POO)**, **principios SOLID**, **Clean Code** y patrones arquitectónicos probados para evitar cuellos de botella y facilitar el escalado.

### Principios y buenas prácticas aplicadas
- **SOLID**: separación de responsabilidades, inversión de dependencias y diseño orientado a interfaces para facilitar testing y evolución.
- **Clean Code**: nombres claros, funciones pequeñas, responsabilidades únicas y código fácilmente legible.
- **DRY / KISS / YAGNI**: evitar duplicación, mantener soluciones simples y no sobrecomplicar con features innecesarias.
- **Inyección de dependencias**: facilita el mocking en pruebas y desacopla componentes.
- **Manejo de errores centralizado**: excepciones controladas y respuestas consistentes para el frontend.
- **Seguridad**: uso de Spring Security + JWT para autenticación/autorization, validación y saneamiento de inputs.
- **Pruebas**: diseño pensando en testabilidad (unitarias y de integración).
- **Observabilidad**: logs estructurados y métricas para detectar cuellos de botella en producción.

### Estrategias para evitar cuellos de botella y optimizar rendimiento
- **Paginación y carga lazy** en APIs y frontend para evitar transferencias y renders pesados.
- **Caching**: uso de Redis para cachear consultas frecuentes y reducir carga en la DB.
- **Batching y procesamiento asíncrono** para tareas pesadas (envío de emails, procesamiento de imágenes, etc.).
- **Pool de conexiones** (DB) y configuración óptima de HikariCP.
- **Índices y optimización de consultas** en la base de datos (proyecciones DTO, consultas específicas y `SELECT` controlados).
- **Limitación de concurrencia / optimistic locking** cuando corresponde para evitar inconsistencias en stock.

### Arquitectura Backend (Java / Spring Boot)
📚 Patrón general:

- Layered Architecture con inspiración en Domain-Driven Design

Estructura de paquetes principal utilizada:

```text
src/
└── main/
└── java/
└── com.api.ecommerce
├── config
├── controller
├── despertarrender
├── dtos
├── entity
├── enums
├── exception
├── jwt
├── mapper
├── repository
├── seeder
├── serviceImpl
├── specification
└── util
```

Patrones y responsabilidades:
- **Controller**: manejo de endpoints REST y validación inicial.
- **DTOs / Mapper**: separación entre entidades y modelos expuestos (reduce overfetching).
- **Repository (JPA/Hibernate)**: capa de persistencia con consultas optimizadas.
- **Service / ServiceImpl**: lógica de negocio, transacciones y coordinación entre repositorios.
- **Specification**: consultas dinámicas y filtros reutilizables.
- **Exception**: manejo centralizado de errores.
- **JWT / Security**: autenticación y autorización.
- **Seeder**: datos iniciales para ambientes de desarrollo/testing.
- **Util / Config**: configuración central, beans y utilidades.

### Arquitectura Frontend (Angular)
📚 Patrón general:

- Feature-Based Modular Architecture con Core y Shared Modules.

Estructura de módulos y carpetas:

```text
src/
└── app/
├── core/ # Servicios singleton, interceptores, guards, modelos globales
│ ├── services/
│ ├── guards/
│ ├── interceptors/
│ ├── models/
│ └── core.module.ts
├── shared/ # Componentes, pipes, directivas reutilizables
│ ├── components/
│ ├── pipes/
│ ├── directives/
│ ├── services/
│ └── shared.module.ts
├── features/ # Módulos principales por dominio (lazy loaded)
│ ├── auth/
│ ├── admin/
│ ├── cliente/
│ ├── home/
├── app-routing.module.ts # Routes con lazy loading por módulo
└── app.component.ts
```


Buenas prácticas en frontend:
- **Lazy loading** por módulos para mejorar tiempo de carga.
- **Servicios singleton** en `core` para estado compartido (API clients, auth).
- **Shared module** para componentes/pipes/directivas reutilizables.
- **Interceptors** para manejo central de tokens, errores y tiempo de requests.
- **OnPush change detection** y `trackBy` en listas para optimizar rendering.
- **RxJS**: manejo correcto de suscripciones (unsubscribe, takeUntil) y uso de streams para UI reactiva.
- **AOT, tree-shaking y optimización de bundles** para producción.
- **Accesibilidad y responsive** con Angular Material y Bootstrap.
- **Validaciones front y back**: validación en formularios y revalidación en backend.

### Resultado esperado
La combinación de esta arquitectura modular, los principios SOLID y las prácticas de rendimiento te permiten tener:
- Código **más mantenible y testeable**.
- **Escalado horizontal y vertical** más sencillo.
- Menor probabilidad de **cuellos de botella** y mejor experiencia de usuario.