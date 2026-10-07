1.Instala o servidor BIND9 no equipo darthvader. Comproba que xa funciona coma servidor DNS caché pegando no documento de entrega a saída deste comando dig @localhost xunta.gal 

Esta es la salida que devolvió el comando:



![dig @localhost xunta.gal ](capturas/imagee.png)


Se puede ver que en el primer dig el Query Time fue de 419 ms y en cambio en el segundo fue de 1ms. Eso quiere decir que el servidor DNS está configurado en modo caché. Esto se debe a que en la primera isntrucción el servicio DNS fue a preguntar a Internet, y en la segunda respondió desde la memoria.



---





nslookup darthvader.starwars.lan

![alt text](capturas/image.png)

nslookup skywalker.starwars.lan

![alt text](capturas/image-1.png)

nslookup starwars.lan

![alt text](capturas/image-3.png)

nslookup -q=mx starwars.lan

![alt text](capturas/image-4.png)

nslookup -q=ns starwars.lan

![alt text](capturas/image-5.png)

nslookup -q=soa starwars.lan

![alt text](capturas/image-6.png)

nslookup -q=txt lenda.starwars.lan

![alt text](capturas/image-7.png)

nslookup 192.168.20.11

![alt text](capturas/image-8.png)
