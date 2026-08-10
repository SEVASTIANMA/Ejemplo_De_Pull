# Tema: Sistema de gestión de inventario 
##  Desarrollar módulo de gestión de inventario 
Descripción: Desarrollar un módulo que permita registrar, consultar, modificar y eliminar productos de un inventario, facilitando el control de las existencias de la empresa.
 Criterios de aceptación:
* El usuario puede registrar un producto con nombre, código, precio y cantidad.
* El sistema permite consultar los productos registrados. 
* El usuario puede modificar la información de un producto.
* El usuario puede eliminar un producto. 
* El sistema permite buscar productos. 
* El sistema muestra una advertencia cuando la cantidad disponible sea 
* ## 1. ¿Cómo Funciona un Sistema de Inventarios?
El funcionamiento se basa en un ciclo continuo apoyado por tecnología (como códigos de barras o chips RFID):

[ Recepción ] ➔ [ Almacenamiento ] ➔ [ Monitoreo ] ➔ [ Venta / Despacho ] ➔ [ Reaprovisionamiento ]

* Entrada de mercancía: Al recibir stock del proveedor, se escanea el código de barras/QR de cada unidad o lote. El sistema actualiza automáticamente las cantidades disponibles.

* Ubicación en almacén: El sistema asigna un pasillo, estante o posición exacta a cada producto para facilitar su localización rápida.

* Control de salidas (Venta): Cuando entra un pedido o se vende un ítem, el sistema descuenta la unidad inmediatamente de la base de datos central (inventario en tiempo real).

* Puntos de reorden y alertas: Cuando las existencias de un producto bajan de cierto nivel de seguridad, el sistema genera automáticamente una alerta o una orden de compra sugerida.

## 2. Métodos Clave de Gestión
Para que el sistema sepa cómo mover el stock, se aplican métodos específicos según el tipo de negocio:

* FIFO / PEPS (First In, First Out / Primero en Entrar, Primero en Salir): Las unidades más antiguas son las primeras en venderse. Es vital para productos perecederos (alimentos, medicamentos) o de rápida obsolescencia (moda, tecnología).

* LIFO / UEPS (Last In, First Out / Último en Entrar, Primero en Salir): Lo último que entró es lo primero en salir. Se aplica a productos no perecederos ni sujetos a moda (como materiales de construcción en bultos o arena).

* Just in Time (JIT): Se produce o compra solo lo necesario en el momento justo. Minimiza los costos de almacenamiento al extremo, pero exige una cadena de suministro extremadamente confiable.
*  **Análisis ABC:** Clasifica los productos según su valor e impacto en las ventas:

* Clase A: 20% de los productos que generan el 80% de los ingresos (alto control).

* Clase B: 30% del inventario con impacto moderado.

* Clase C: 50% de los productos que representan solo el 5% de los ingresos (bajo control).
* ## 3. Ejemplos Prácticos en Distintas Industrias
**Ejemplo :** Supermercado o Comercio Minorista (E-commerce)
Reto: Miles de productos diferentes con alta rotación y fechas de caducidad variables.

**Cómo funciona:**

* Al llegar una caja de yogures, se registra la fecha de vencimiento y el lote.

* Cuando el cajero escanea el producto (o se descuenta por la tienda online), el inventario se actualiza en el acto.

* El sistema aplica FIFO: alerta al personal si hay lotes próximos a vencer para colocar esas bandejas al frente de la repisa o aplicar promociones.
