# comando like

select * from clientes where nombre like "a%" // para seleccionar los nombres que empiecen por a

# comando  distinct

select distinct cuidad from clientes // devuelve los valores de la columna cuidad sin repetir

# comando limit

select * from clientes limit 5 // devuelve los primeros 5 registros de la tabla clientes

# comando order by

select * from clientes order by nombre // devuelve los registros de la tabla clientes ordenados por nombre

# comando group by

select cuidad, count(*) from clientes group by cuidad // devuelve los registros de la tabla clientes agrupados por cuidad y la cantidad de registros por cuidad

# comando having

select cuidad, count(*) from clientes group by cuidad having count(*) > 1 // devuelve los registros de la tabla clientes agrupados por cuidad y la cantidad de registros por cuidad que sean mayores a 1

# comando case

select nombre, case when edad < 18 then "menor de edad" else "mayor de edad" end as estado from clientes // devuelve los registros de la tabla clientes con la columna estado que indica si es mayor o menor de edad