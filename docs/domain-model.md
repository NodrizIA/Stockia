## Usuario

Representa a una persona con acceso al sistema.

- id
- nombre
- email
- rol
- creado_en

## Producto

Representa un artículo que se compra, almacena y vende.

- id
- sku
- nombre
- categoria
- precio_venta
- stock_minimo
- creado_en

## Proveedor

Representa una empresa que suministra productos.

- id
- nombre
- email
- telefono
- ciudad
- creado_en

## PedidoCompra

Representa una compra realizada a un único proveedor.

- id
- proveedor_id
- creado_por_usuario_id
- estado
- creado_en
- enviado_en
- cancelado_en

## LineaPedidoCompra

Representa cada producto solicitado dentro de un pedido.

- id
- pedido_compra_id
- producto_id
- cantidad_solicitada
- precio_unitario

## MovimientoStock

Representa un cambio físico del inventario.

- id
- producto_id
- tipo
- cantidad
- motivo
- registrado_por_usuario_id
- linea_pedido_compra_id (opcional)
- creado_en

## ReservaStock

Representa unidades apartadas temporalmente, sin alterar el stock físico.

- id
- producto_id
- cantidad
- estado
- creada_por_usuario_id
- creada_en
- expira_en
- liberada_en (opcional)
