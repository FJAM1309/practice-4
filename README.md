practice-4
Frecuencíometro Digital 

Describa, utilizando Verilog un circuito que funcione como un Frecuencímetro digital sobre su tarjeta. El rango a medir ira de 0 a 9999Hz, utilizando como base de tiempo de medición 1 segundo. 
Uno de los LEDs de la tarjeta mostrara cuando el sistema está midiendo. Esto quiere decir que durante el proceso de medición debe de existir un LED que brille y saber que el sistema no está trabado en algún número. 
Una vez tomada la medición de frecuencia, el sistema actualizara los datos en los displays de 7 segmentos. Si la frecuencia de entrada es mayor a 9999Hz, deberá mostrar en los displays ‘1---‘, para indicar el overflow que tiene la cuenta. 
Si se mete una frecuencia más alta, en ningún momento se debe de ver algo distinto a ‘1---‘ 
¡¡Es muy importante generar un circuito de protección para la tarjeta!!
La entrada, se conectara a uno de los pines de conexión auxiliar de la tarjeta.
