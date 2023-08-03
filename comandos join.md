# estucturas jouin

## unir tablas con  inner join

select * from clientes inner join productos on clientes.producto = productos.producto // devuelve los registros de la tabla clientes y productos que tengan el mismo valor en la columna producto

## unir tablas con left join

select * from clientes left join productos on clientes.producto = productos.producto // devuelve los registros de la tabla clientes y productos que tengan el mismo valor en la columna producto y los registros de la tabla clientes que no tengan registros en la tabla productos

## unir tablas con right join

select * from clientes right join productos on clientes.producto = productos.producto // devuelve los registros de la tabla clientes y productos que tengan el mismo valor en la columna producto y los registros de la tabla productos que no tengan registros en la tabla clientes

## unir tablas con full join

select * from clientes full join productos on clientes.producto = productos.producto // devuelve los registros de la tabla clientes y productos que tengan el mismo valor en la columna producto y los registros de la tabla clientes y productos que no tengan registros en la otra tabla

## unir tablas con cross join

select * from clientes cross join productos // devuelve los registros de la tabla clientes y productos combinando todos los registros de la tabla clientes con todos los registros de la tabla productos

