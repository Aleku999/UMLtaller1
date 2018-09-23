# UMLtaller1

## UML servidor de eclipse

### Main
- **main(String[]):void** En este metodo se ejecutara toda la aplicacion
- **Settings():void**
- **Setup():void:** Aqui se definen todas las variables y cosas que ejecutara la aplicacion
- **Draw():void:** Aqui se corre toda la parte grafica es mostrada en el lienzo
- **MousePressed():void:** Este metodo permetira comenzar con el juego

### Logica
- **Logica(PApplet):void:** Constructor de la clase
- **pintar():void:** Este  metodo se utiliza para pintar cada metodo pintar de las clases
- **lanzarObjeto:void:** Este metodo genera Recogibles que dan habilidades a los personajes
- **finDePartida:void:** Este metodo finaliza la partida mostrando los resultados

### Personaje
+ **Personaje(PApplet,int,int):void:** Constructor de la clase padre personaje
+ **pintar():void:** Este metodo pinta al personaje
+ **movimiento():void:** Este metodo muestra los movimientos de posición del personaje
+ **golpe():void:** Este metodo contiene la informacion para golpear la pelota
+ **getPosicion():void:** Se obtiene la posicion del personaje

### Servidor
+ **run():void:** Este es hilo por el cual se establece conexion con los clientes
+ **enviar():void:** Envia los datos obtenidos al servidor

### Receptor
+ **Receptor(Socket):void:**
+ **run():void:** Es el hilo por el cual se reciben los mensajes de los clientes

### Nicki
+ **Nicki(PApplet,int,int):void** Construtor de Nicki
+ **pintar():void:** En este metodo se pintan en el lienzo las imagenes u objetos
+ **movimiento():void:** Este es el metodo se cambia de posicion
+ **golpe():void:** Este metodo contiene la informacion para golpear la pelota

### Cardi
+ **Cardi(PApplet,int,int):void** Construtor de Cardi
+ **pintar():void:** En este metodo se pintan en el lienzo las imagenes u objetos
+ **movimiento():void:** Este es el metodo se cambia de posicion
+ **golpe():void:** Este metodo contiene la informacion para golpear la pelota

### Pelota 
+ **Pelota(PApplet,int,int):void** Constructor de la Pelota
+ **pintar():void:** En este metodo se pintan en el lienzo las imagenes u objetos
+ **movimiento():void:** Este es el metodo se cambia de posicion
+ **propiedad():void:** Este metodo contiene la informacion de quien fue el ultimo en tocarlo

### Tiempo
+ **Tiempo(PApplet,int,int):void** Constructor del Tiempo
+ **pintar():void:** En este metodo se pintan en el lienzo las imagenes u objetos
+ **movimiento():void:** Este es el metodo se cambia de posicion
+ **Obtener():void** Este metodo recoge el elemento
+ **Efecto():void:** Este metodo realiza el efecto asignado del recogible

### Acceleracion
+ **Acceleracion(PApplet,int,int):void** Constructor de la Acceleracion
+ **pintar():void:** En este metodo se pintan en el lienzo las imagenes u objetos
+ **movimiento():void:** Este es el metodo se cambia de posicion
+ **Obtener():void** Este metodo recoge el elemento
+ **Efecto():void:** Este metodo realiza el efecto asignado del recogible

### Tamano
+ **Tamano(PApplet,int,int):void** Constructor de la Tamano
+ **pintar():void:** En este metodo se pintan en el lienzo las imagenes u objetos
+ **movimiento():void:** Este es el metodo se cambia de posicion
+ **Obtener():void** Este metodo recoge el elemento
+ **Efecto():void:** Este metodo realiza el efecto asignado del recogible


## UML Cliente de Android Studio

### Main
+ **onCreate (Bundle):void:** Con este metodo se inicia la aplicacion
+ **Botones():void:** Con este metodo se obtiene las diferentes acciones de nicki y cardi

### Cliente
+ **Cliente(PApplet, int, int) : void:** Construcctor del cliente
+ **run( ):** Recibe los datos enviados por parte del servidor
+ **enviar():void** Envia los datos obtenidos de las acciones en los botones al servidor 

### Receptor

+ **Receptor(Socket):void:** Constructor del receptor
+ **run():** es el hilo que recibe datos enviados desde el servidor
+ **enviar():void:** Envia los datos obtenidos por las acciones de los botones al servidor.


