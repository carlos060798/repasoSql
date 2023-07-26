# CREAR BASE DE DATOS
CREATE database JUGOS;

# ELIMINAR BASE DE DATOS

DROP database JUGOS;

# EJEMPLO DE CREACION DE UNA TABLA DE DATOS SQL
CREATE TABLE TBCLIENTES(
 DNI VARCHAR (20),
 NOMBRE VARCHAR (150),
 DIRECCION VARCHAR (20),
    DIRECCION2 VARCHAR (20),
    BARRIO VARCHAR (20),
    CUIDAD VARCHAR (50),
    DEPARTAMENTO VARCHAR(50),
    CP VARCHAR (10),
    EDAD SMALLINT,
    SEXO VARCHAR(1),
    LIMITE_CREDITO  FLOAT,
VOLUMENDECOMPRA FLOAT,
PRIMERA_COMPRA BIT(1))  


# para eliminar table por comando 
DROP TABLE `tbclientes2`"

# Comando para  insertar valores en tabla
INSERT INTO `tbproductos`(`producto`, `nombre`, `envase`, `Volumen`, `sabor`, `precio`) VALUES ('777324','clean','botella pet','1 litro','naranja',8.01);
# para mostrar los valores de la tabla productos 
SELECT * FROM tbproductos;
# comado para modificar los valores de la tabla
UPDATE `tbproductos` SET `producto`='57394',`nombre`='gaseosa' WHERE 1

# comando para eliminar valores de la tabla /  where es para seleccionar el valor que se quiere eliminar
DELETE FROM `tbproductos` WHERE precio = 46;
# crear las llaves primarias de la base de datos 
ALTER  TABLE tbproductos  ADD PRIMARY KEY(producto) 

# para agregar una nueva columna a la tabla tb clientes
ALTER TABLE tbclientes ADD COLUMN (Fechanacimineto DATE)
# para seleccionar un campo en especifico
SELECT * FROM `tbproductos` WHERE sabor= "mora"; 

# filtros de busqueda avanzados ejemplos
SELECT * FROM `tbclientes` WHERE  EDAD >27  // CON ESTE FILTRO SELECCIONAMOS LOS CLIENTES MAYORES DE 27 AÑOS

SELECT * FROM `tbclientes` WHERE  EDAD <> 14 // PARA  HACER COMPARACIONES DE DIFERENTE QUE
SELECT * FROM `tbclientes` WHERE YEAR(Fechanacimineto)= 2023; // PARA SELECCIONAR POR AÑO con fechas 
SELECT * FROM `tbclientes` WHERE DAY(Fechanacimineto)= 18; // PARA SELECCIONAR POR DIA con fechas

