      Comandos
  
![188697933-cc320a74-cf45-4d54-b899-081fd1e23d6d](https://user-images.githubusercontent.com/101933399/196839508-7a9dafdf-7120-4a5d-b8ec-7e19000f8015.png)

![188697774-43bff4ae-b721-4d48-bca3-350f9d00a2f2](https://user-images.githubusercontent.com/101933399/196839528-073b6d1c-7be9-4297-bd01-77e50c36ffde.png)

Explicación comandos.

    ip route | grep default 
    
En su uso podemos establecer una ruta predeterminada en redes que usan protocolos de enrutamiento dinámico, incluidas las redes remotas descubiertas de manera dinámica, las rutas conectadas directamente y las rutas estáticas.
    
    tracert.exe 8.8.8.8
    
Determina la ruta a un destino mediante el envío de paquetes de eco de Protocolo de mensajes de control de Internet (ICMP) al destino.
    
    netstat.exe -nat | grep -c 'ESTABLISHED'

Genera visualizaciones que muestran el estado de la red y estadísticas de protocolo. El estado de los protocolos TCP, SCTP y los puntos finales de UDP puede visualizarse en formato de tabla. También puede visualizarse información sobre la tabla de enrutamiento e información de interfaces..
ESTABLISHED: La conexión ha sido establecida.
LISTEN: para revisar los puertos que están escuchando en la red, adicional en el proceso de identificacion con actividades especificas.

    cat ports_up.txt

Un texto introducido se encuentra en un archivo especifico 'new. txt'. Esto se puede comprobar a través del comando 'cat new. txt' por ejemplo.
