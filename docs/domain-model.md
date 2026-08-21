## Producto (es el articulo que se compra y se va a inventariar)

- id
- sku
- nombre
- categoria
- precio_venta
- stock_minimo
- fecha

## MovimientoStock (accion sobre la cantidad disponible de los articulos)

- id
- producto_id
- tipo
- cantidad
- motivo
- usuario_id
- fecha

## Usuario (es el cliente o el admin del almacen que puede modificar el stock)

- usuario_id
- fecha
- motivo
- cantidad
- producto_id
- tipo

## Proveedor (son los que tienen las mercancias que registraremos y luego venderemos)

- usuario_id
- id
- fecha
- precio
- estado
- producto_id
- ciudad
- telefono
- email

## Pedido_compra (datos sobre un pedido que hacemos a los proveedores)

- usuario_id
- proveedor
- fecha
- producto_id
- cantidad_solicitada
- cantidad_entregada
- precio
- estado

## Lineapedidocompra (el pedido que nos entrega los proveedores)

- usuario_id
- proveedor
- producto_id
- cantidad_solicitada
- cantidad_entregada
- precio
- fecha
- estado

## ReservaStock (sistema para reservar productos con fecha de caducidad)

- usuario_id
- producto_id
- fecha_inicial
- fecha_limite
- estado
- cantidad
