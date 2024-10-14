# Evidencia06: Caso - Tienda Online (e-shop)

## Objetivo
Desarrollar un diagrama de clases UML a partir de la descripción de un contexto problema, específicamente para un sistema de compras en línea.

## Participantes:
- Integrante: Daniela Díaz
- Integrante: Gustavo Pérez

## Contexto
Contexto:

El objetivo es representar los elementos del dominio problema (ej: cliente, usuario web, cuenta, carrito de compras, producto, pedido, pago, etc.) y las relaciones entre ellos. Podría utilizarse como un elemento común entre analistas del negocio, ejecutivos comerciales y desarrolladores de software.

Cada cliente está vinculado exactamente a una cuenta, una cuenta no puede existir sin un cliente asociado.

Un carrito de compras está asociado a una única cuenta, dicho carrito no puede existir sin estar vinculado a una cuenta.

El cliente puede registrarse como usuario de la web para poder comprar artículos en línea. No se requiere que el cliente sea obligatoriamente un usuario de la web para hacer las compras (las compras también se pueden realizar por otros medios, ej: teléfono o mediante pedidos desde catálogos). El usuario web puede estar en uno de los siguientes estados: nuevo, activo, bloqueado temporalmente o prohibido, y estar vinculado a un carrito de compras.

La cuenta también esta compuesta de los pedidos de los clientes. Es posible que el cliente no tenga pedidos. Cada pedido puede referirse a varios medios de pago o posiblemente ninguno. Cada medio pago está relacionado exactamente con una cuenta.


Cada pedido tiene el estado actual del pedido. Dichos estados pueden ser: nuevo, creado, despachado, recibido, cerrado. Tanto el pedido como el carrito de la compra están asociados con familias de productos que estás asociados a un producto específico. Cada familia de productos está relacionado exactamente con un producto. Un producto puede estar asociado a muchas familias de productos o a ninguno.

## Clases
Se consideraron las siguientes clases para el contexto dado:
- Cliente
- Cuenta
- Pedido
- Familia de Productos
- Producto
- Carrito de Compras
Y los siguientes enums para estados o variantes de ciertas clases:
- Medios de pago
- Usuario Web (Dado que este podia estar bloqueado, prohibido, activo o ser nuevo)
- Estado Pedido

