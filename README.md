# Tu Tienda Online - Documentación

Documentación visual de la tienda online (Angular + Spring Boot).

# 🙍‍♂️ Rol Cliente

## 🏠 Inicio

En esta sección se presentan los productos destacados junto con dos sliders totalmente configurables desde el panel de administración.  
El buscador principal permite filtrar los productos por **nombre, categoría, subcategoría, características, marcas** y otros criterios, ofreciendo una experiencia de búsqueda **dinámica y personalizada**.

![Página de inicio](https://res.cloudinary.com/dlv9gwnw3/image/upload/v1761580413/home_ojsacs.png)

## 🧾 Detalle del Producto

En esta sección se muestra la información completa del producto seleccionado, incluyendo su **imagen, nombre, categoría, código, peso y precio actual**, así como sus características.  
Si el artículo cuenta con un descuento, se visualiza el **precio original tachado** junto con el **porcentaje de ahorro** correspondiente.

El usuario puede **agregar el producto al carrito**, seleccionar la cantidad deseada y calcular el **costo del envío** directamente desde esta vista.  
Debajo, se presentan los **productos relacionados**, que se actualizan dinámicamente según la subcategoría o similitud del producto, permitiendo una **navegación fluida** entre artículos similares o complementarios.

Además, la interfaz mantiene elementos clave de navegación como la **barra superior con el buscador**, las **opciones de cuenta** y el **acceso rápido al carrito**, brindando una experiencia de usuario coherente e intuitiva en todo el sitio.

![Detalle del producto](https://res.cloudinary.com/dlv9gwnw3/image/upload/v1761580886/detalle_dn6fcb.png)

## 🛍️ Sección de Búsqueda de Productos

En esta vista se muestran los **productos filtrados** según la búsqueda realizada.  
En la columna izquierda se listan las **coincidencias por marcas, categorías** y **productos con promociones**, destacando los descuentos según el porcentaje aplicado.

Además, se incluye un **menú desplegable** que permite ordenar los productos por **precio** (mayor a menor o menor a mayor) y alfabéticamente (**de la A a la Z**).

![Filtro](https://res.cloudinary.com/dlv9gwnw3/image/upload/v1761582932/busqueda-productos_vvvcpp.png)


## 🛒 Carrito de Compras

En esta sección se listan todos los productos seleccionados por el usuario, mostrando su **imagen, nombre, precio actual, precio anterior en caso de descuento** y controles para **modificar la cantidad o eliminar artículos**.  
E carrito realiza una **validación dinámica del stock disponible** para evitar agregar productos que superen la cantidad permitida.

También se muestra el **total de la compra** actualizado en tiempo real y un botón para continuar con el proceso de pago.  
La **dirección de envío** se obtiene automáticamente según la ubicación configurada por el usuario, permitiendo calcular costos de entrega antes de confirmar la compra.

El sistema valida además un **importe mínimo de compra** que debe alcanzarse para habilitar la opción de finalizar el pedido.  
Se maneja la **concurrencia** para garantizar la consistencia de los datos en caso de múltiples usuarios realizando operaciones simultáneas, asegurando que los precios y cantidades se mantengan actualizados correctamente.

![Carrito de compras](https://res.cloudinary.com/dlv9gwnw3/image/upload/v1761582812/carrito_ea5t0d.png)

## 🛒 Vista de Checkout / Carrito de Compras

En esta vista el usuario puede revisar los productos agregados al carrito, modificar cantidades, eliminar ítems y visualizar el resumen completo de su compra.

🔹 Funcionalidades principales

Listado de productos agrupados por categoría, mostrando imagen, nombre, precio actual y precio anterior cuando aplica un descuento.

Controles de cantidad (+ / -) y botón de eliminación individual.

Cálculo automático de subtotales y totales según las cantidades seleccionadas.

Sección de políticas de reemplazo ante falta de stock, con tres opciones:

Contactarme para reemplazo.

No reemplazar producto.

Utilizar criterio del vendedor.

Resumen lateral de compra con subtotal, costo de envío, descuentos aplicados y total final.

Botón de confirmación de compra habilitado solo cuando se cumplen las condiciones del pedido.

![Carrito de compras](https://res.cloudinary.com/dlv9gwnw3/image/upload/v1761584331/checkout_bf25ju.png)

## ✅ Confirmación de Pago y Creación del Pedido

Una vez que el pago es aprobado a través de Mercado Pago, el sistema ejecuta automáticamente un flujo completo de confirmación y actualización, garantizando la coherencia de datos entre el frontend, backend y servicios externos.

🔹 Flujo automatizado con Webhook

Recepción del webhook de Mercado Pago: el backend escucha la confirmación del pago mediante un endpoint seguro configurado en Spring Boot.

Validación del estado del pago: se comprueba que la transacción haya sido efectivamente aprobada antes de continuar el proceso.

Actualización de stock: se descuentan las unidades correspondientes de cada producto adquirido para mantener la integridad del inventario.

Creación del pedido: se registra un nuevo pedido en la base de datos con detalle de productos, totales, usuario, dirección y método de pago.

Envío automático de email al cliente confirmando la compra, incluyendo resumen de los productos, monto total y datos de entrega.

Notificación interna a la aplicación (por ejemplo, para panel del vendedor o dashboard administrativo) informando que se generó un nuevo pedido.

![Finalizacion de compra](https://res.cloudinary.com/dlv9gwnw3/image/upload/v1761585397/finalizar-compra_ethaym.png)

## ✅ Modal Crear compra

![Modal de compra](https://res.cloudinary.com/dlv9gwnw3/image/upload/v1761587490/modal-mercado-pago_boxtdz.png)

---

## ✅ Respuesta compra

![Modal de compra](https://res.cloudinary.com/dlv9gwnw3/image/upload/v1761587490/compra-exito_q3i0br.png)


---

![Modal de compra](https://res.cloudinary.com/dlv9gwnw3/image/upload/v1761587492/respuesta-compra_gjowxh.png)



# 🙍‍♂️ Rol Administrador

## 📊 Vista Dashboard

Funcionalidades principales:

📦 Visualización del total de productos registrados en la tienda.

💰 Consulta de las ventas del día y el total acumulado de ventas globales.

🖼️ Posibilidad de agregar o modificar la imagen de la marca que se muestra en la aplicación.

🗓️ Registro y visualización de la fecha de inicio de actividades del comercio o empresa.

![Modal de compra](https://res.cloudinary.com/dlv9gwnw3/image/upload/v1761595326/dashboard_d2oves.png)

## 👥 Vista de Clientes

En esta sección se listan todos los clientes registrados en el eCommerce.

📄 Los resultados se muestran mediante paginación, permitiendo una navegación ordenada entre los registros.

🔍 Incluye un filtro de búsqueda que facilita encontrar clientes por nombre, correo u otros criterios relevantes

![Modal de compra](https://res.cloudinary.com/dlv9gwnw3/image/upload/v1761596604/usuarios_r6eufh.png)

## 🛍️ Vista de Listar Productos Comunes

En esta sección se gestionan los productos disponibles en el eCommerce.

📦 Permite listar todos los productos registrados en el sistema.

✏️ Opción para actualizar información de cada producto.

🚫 Posibilidad de desactivar productos temporalmente sin eliminarlos.

📄 Incluye paginación para una navegación ordenada.

🔍 Dispone de un filtro de búsqueda para encontrar productos fácilmente.

![Modal de compra](https://res.cloudinary.com/dlv9gwnw3/image/upload/v1761597648/listar-productos-comunes_t8tyaz.png)


## 🛍️ Vista de Creación de Productos Comunes

En esta sección se pueden crear nuevos productos ingresando toda la información necesaria desde un formulario intuitivo.

Características principales:

📝 Permite registrar productos normales seleccionando sus datos correspondientes (nombre, categoría, precio, descripción, etc.).

🏷️ Si se marca la opción “En promoción”, el producto mostrará un badge promocional y el sistema calculará automáticamente el porcentaje de descuento.

💥 En caso de seleccionar “En oferta” o “Ofertas semanales”, se asigna el badge de oferta y también se calcula automáticamente el porcentaje de descuento.

🖼️ Es posible agregar hasta tres imágenes por producto, eligiendo cuál será la imagen principal que se mostrará en la tienda.

⚙️ Todo el proceso sigue instrucciones claras para garantizar la correcta carga del producto.

![Modal de compra](https://res.cloudinary.com/dlv9gwnw3/image/upload/v1761597960/crear-producto-normal_jgsvwl.png)










<!-- 
🧱 Arquitectura del Proyecto

El backend está implementado siguiendo una arquitectura en capas (Layered Architecture), una práctica estándar en el desarrollo empresarial con Spring Boot.
Esta estructura organiza el código de manera clara, promoviendo la separación de responsabilidades, la mantenibilidad y la escalabilidad.

🔹 Capas principales:

Controller (Web Layer): expone los endpoints REST y gestiona las solicitudes HTTP.

Service (Business Layer): contiene la lógica de negocio y las reglas de aplicación.

Repository (Data Access Layer): se encarga de la comunicación con la base de datos utilizando Spring Data JPA.

Model / Entity Layer: define las entidades, DTOs y modelos de datos.

📌 Esta organización se basa en el patrón MVC extendido (Model–View–Controller), garantizando un flujo claro desde la capa de presentación hasta la persistencia de datos.

🟦 Frontend – Angular

El frontend se desarrolla bajo una arquitectura modular basada en features (Feature-Based Modular Architecture), complementada con principios de Clean Architecture y el patrón Core–Shared–Feature.
Esta estructura está pensada para proyectos escalables y de fácil mantenimiento.


```text
src/
 ├── app/
 │    ├── core/                  # Servicios singleton, interceptores, guards, modelos globales
 │    │    ├── services/
 │    │    ├── guards/
 │    │    ├── interceptors/
 │    │    ├── models/
 │    │    └── core.module.ts
 │    │
 │    ├── shared/                # Componentes, pipes, directivas reutilizables
 │    │    ├── components/
 │    │    ├── pipes/
 │    │    ├── directives/
 │    │    └── shared.module.ts
 │    │
 │    ├── features/              # Módulos principales divididos por función/feature
 │    │    ├── auth/             # Login, registro, recuperación de contraseña
 │    │    │     ├── components/
 │    │    │     ├── services/
 │    │    │     └── auth.module.ts
 │    │    │
 │    │    ├── admin/            # Dashboard, gestión de productos, usuarios, pedidos (solo admin)
 │    │    │     ├── components/
 │    │    │     ├── services/
 │    │    │     └── admin.module.ts
 │    │    │
 │    │    ├── cliente/          # Catálogo, carrito, perfil, historial de pedidos
 │    │    │     ├── components/
 │    │    │     ├── services/
 │    │    │     └── cliente.module.ts
 │    │    │
 │    │    ├── shared-features/  # Funcionalidades compartidas como catálogo de productos
 │    │
 │    ├── app-routing.module.ts # Rutas principales con lazy loading por módulo
 │    └── app.component.ts
 │
 └── assets/                     # Imágenes, estilos globales, fuentes -->
