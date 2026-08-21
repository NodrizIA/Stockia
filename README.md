# Stockia
es una api para el control y seguimiento del stock de productos en un almacen.
¿Qué problema resuelve StockPilot?
almacena,visualiza y gestiona los productos que entran y salen del almacen y el estado de los pedidos realizados

¿Quién lo utilizará? Por ejemplo: administrador, responsable de almacén, empleado de compras.
El ceo de la empresa puede ver metricas, stock actual y el responsable de almacen puede ver todo , cambiar stock y demas modificaciones.

¿Qué es un producto y qué datos mínimos necesita?
cualquien producto que se quiera poner a la venta, y necesitara sku, nombre,categoria,cantidad minima,precio.

¿Qué tipos de movimiento de stock existirán?
entrada,salidas,reservas,rotos y ajuste.(cada modificacion del stock registrara el porque,quien y cuando)

¿Qué condiciones deben cumplirse para recibir un pedido?
cantidad de producto recibido/solicitado,categoria, proveedor,fecha,importe.

¿Qué debe ocurrir al cancelar un pedido ya recibido?
se crea una linea de devoluciono ajuste incluyendo proveedor, fecha, importe,motivo.

¿Puede el stock ser negativo? ¿Por qué?
el stock no puede ser negativo porque no se puede vender lo que no se tiene (en el frontend del comercio aparecera un mensaje de no disponible añadir a lista de deseos)

¿Qué información debe registrarse en cada movimiento para poder auditarlo?
cada modificacion del stock registrara el porque (venta,entrada,rotura),quien y cuando.
cada incorporacion de un pedido (entrada de mercancia) generara un ID unico con el lote de productos que integra
