1.Instala o servidor BIND9 no equipo darthvader. Comproba que xa funciona coma servidor DNS caché pegando no documento de entrega a saída deste comando dig @localhost xunta.gal 

Esta es la salida que devolvió el comando:



![dig @localhost xunta.gal ](capturas/image.png)


Se puede ver que en el primer dig el Query Time fue de 419 ms y en cambio en el segundo fue de 1ms. Eso quiere decir que el servidor DNS está configurado en modo caché. Esto se debe a que en la primera isntrucción el servicio DNS fue a preguntar a Internet, y en la segunda respondió desde la memoria.



2.Configura o servidor BIND9 no equipo mandalorian para que empregue como reenviador a darthvader pegando no documento de entrega contido do ficheiro /etc/bind/named.conf.options e a saída deste comando: dig @localhost santiagodecompostela.gal. Para un correcto funcionamento deberás borrar as root-hints do servidor mandalorian.
