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
