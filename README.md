To-DO
Realizado por: Andrés Salamanca e Iván Ortiz
El algoritmo VAR proporciona el Value at Risk VAR dado un nivel de confianza, un valor de capitalización y un ticker de una empresa cotizada en EEUU
El algoritmo oportunidaddesubida genera un jason con un histograma que recoge si una empresa cotizada en EEUU presenta una oportunidad de compra. Lo hace acumulando los cambios percentuales que se han producido en la acción entre un día de referencia y ndiasmaximo o lags sucesivos. Esto se repite tomando como referencia desde el día actual hasta 365 días hacia atrás. A la función le entra el número de lags o días máximo a considerar desde el día de referencia y el ticker de la empresa que queremos mirar. En nuestro caso comparamos el máximo del día de referencia con el mínimo del día lag considerado en el pasado. Si esa diferencia es negativa supone que la acción ha bajado de precio y se trata de producir un histograma con el acumulado de todas las subidas y bajadas de precio. Si ese histograma presenta gran cantidad de valores hacia la parte negativa, estaríamos en oportunidad de compra puesto que la acción ha acumulado gran cantidad de bajadas desde días anteriores.
El algoritmo prediction va a predecir el precio de la acción en días sucesivos que marquemos.

Considerar la sintaxis siguiente: 
a) En la consola: pip install ciff_2017_af3_asio
b) En python: 
import ciff_2017_af3_asio.<nombre_funcion> 
o también 
ciff_2017_af3_asio.ciff_2017_af3_asio.<nombre_funcion>
