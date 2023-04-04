# Modelo de Regresion

El siguiente proyecto tiene como finalidad predecir el precio de unas propiedades. <br>

La base de datos cuenta con 1548 observaciones y 18 columnas que se detallan a continuación:<br>

 - 0   descripcion:              descripción de la propiedad (1548) <br>  
 - 1   ubicacion:                detalle de ubicación        (1543) <br>  
 - 2   precio_uf:                precio en UF				(1548) <br>  
 - 3   precio_pesos:             precio en pesos 			(1267) <br>  
 - 4   construido:               $m^2$ construidos 		    (1548) <br>  
 - 5   dormitorio:               número de dormitorios 	    (1548)<br>  
 - 6   banio:                    número de baños 		    (1540)<br>  
 - 7   coordenadas:              latitud y longitud		    (1548)<br>  
 - 8   superficie_total:         total de $m^2$			    (1544) <br>  
 - 9   superficie_util:          total de $m^2$ construidos  (1546)<br>  
 - 10  cantidad_pisos_edificio:  # de pisos del edificio     (1060)<br>  
 - 11  departamentos_por_piso:   # deptos. por pisos		    (833)<br>  
 - 12  piso_departamento:        # piso donde esta el depto. (1086)<br>  
 - 13  orientacion:              orientación 				(921)<br>   
 - 14  antiguedad:               años de antiguedad 		    (1041)<br>   
 - 15  gastos_comunes:           precio gastos comunes		(1379)<br>   
 - 16  estacionamiento:          tiene o no estacionamiento  (1039)<br>   
 - 17  bodega:                   tiene o no bodegas 		    (973)<br>   

 La cantidad presente en los paréntesis de cada una de las variables corresponde a las observaciones no nulas.

 ## Tratamiento de los datos

En primer lugar, se lleva a cabo un proceso de separación de la cantidad numérica de la unidad de medida correspondiente en cada variable. Por ejemplo, en el caso de la variable $precio_{uf}$, se pueden observar registros en formato "183000000 pesos", o bien la cantidad se presenta junto a su unidad de medida, como sucede con la variable $superficie_{total}$ expresada en $103 m^2$, entre otras situaciones similares.

Adicionalmente, se procede a crear nuevas variables que permitan identificar la presencia o ausencia de características específicas en las diferentes propiedades, como loggia, bodega, piscina o cercanía al metro, entre otras.

Finalmente, se desarrollan diversos modelos de regresión para predecir el precio de las propiedades, evaluando su desempeño respectivo.
