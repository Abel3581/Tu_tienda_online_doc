# 🛍️ Tu Tienda Online

**Plataforma desarrollada con Angular + Spring Boot**  
Documentación visual y funcional del sistema dividida por roles: **Cliente** y **Administrador**.

---

## 📑 Índice

- [🙍‍♂️ Rol Cliente](#-rol-cliente)
  - [🏠 Inicio](#-inicio)
  - [🧾 Detalle del Producto](#-detalle-del-producto)
  - [🔎 Búsqueda de Productos](#-búsqueda-de-productos)
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
  - [⚙️ Características de Productos](#-características)
- [🧩 Tecnologías Principales](#-tecnologías-principales)
- [👨‍💻 Autor](#-autor)

---

## 🙍‍♂️ Rol Cliente

### 🏠 Inicio
En esta sección se presentan los **productos destacados** junto con dos *sliders* configurables desde el panel de administración.  
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

### ⚙️ Características de Productos

Esta sección permite gestionar las **características** de los productos que se muestran en el **detalle** de cada artículo.
Cada característica se puede crear, editar o eliminar, y está asociada a una o varias categorías.

✨ Funcionalidades principales

- 🆕 Crear nuevas características por categoría (ejemplo: Marca, Peso, Talle, Gramos, Kilos, Tamaño, Color, etc.).

- ✏️ Editar el nombre o la categoría asignada a una característica existente.

- 🗑️ Eliminar características que ya no estén en uso.

- 🔍 Visualizar características existentes con su ID, nombre y categoría asociada.

- 📦 Las características se muestran dinámicamente al crear productos según la categoría seleccionada.

![Categorías](https://res.cloudinary.com/dlv9gwnw3/image/upload/v1761616858/caracteristicas_h0dr25.png)

---

## 🧩 Tecnologías Principales
**Frontend:** Angular, TypeScript, Bootstrap  
**Backend:** Spring Boot, Java 17, JPA, MySQL  
**Integraciones:** Mercado Pago, Cloudinary  
**Infraestructura:** REST API, Swagger  

---

## 👨‍💻 Autor
**Desarrollado por [Abel Acevedo](https://github.com/abelacevedo)**  
📍 Tortuguitas, Buenos Aires – Argentina  
🚀 Apasionado por el desarrollo web, el aprendizaje continuo y los proyectos de alto impacto.

---
