![nmap](https://user-images.githubusercontent.com/101933399/196842445-d87fa00b-1f36-4e96-9d9d-92341338efdf.jpg)

Nmap es un programa de código abierto que sirve para efectuar rastreo de puertos escrito originalmente por Gordon Lyon (más conocido por su alias Fyodor Vaskovich[1]​) y cuyo desarrollo se encuentra hoy a cargo de una comunidad. Fue creado originalmente para Linux aunque actualmente es multiplataforma. Se usa para evaluar la seguridad de sistemas informáticos, así como para descubrir servicios o servidores en una red informática, para ello Nmap envía unos paquetes definidos a otros equipos y analiza sus respuestas.

Nmap es un software de código abierto que se utiliza para escanear una red y sus puertos con el objetivo de obtener información importante sobre la misma para controlar y gestionar su seguridad. Es una aplicación que se utiliza normalmente para realizar auditorías de seguridad y monitoreo de redes.

![Nmap](https://user-images.githubusercontent.com/101933399/196843440-ee012854-6464-4f1c-b3bb-930c67055d04.gif)

    nmap localhost
    
Estos son los puertos abiertos para la dirección “localhost”, que no es otra dirección más que la propia de la máquina servidor. Estos puertos evidentemente son locales, lo que quiere decir que no todos ellos necesiten ser abiertos en un router para poder dar los servicios hacia Internet, aunque muchos de ellos si.

    nmap 172.25.160.1

Este es el formato básico para Nmap y devolverá información sobre los puertos en ese sistema.

    nmap -sP -n xxx.xxx.xxx.0/24
    
Escaneo de nodos receptivos

    nmap -sP -n xxx.xxx.xxx.100-110
    
La forma más eficiente es con nmap. Use awk para imprimir solo las IP, ahora es una lista útil.

    nmap -iL lista_ip.txt
    
Se pasan los objetivos en un fichero, cada uno en una línea

    nmap scanme.nmap.org
    
Esta opción escanea todos los puertos TCP reservados en la máquina scanme.nmap.org.

    nmap 1.1.1.1 8.8.8.8
    
Esta opción escanea dos direcciones IP a la misma vez.

    nmap udenar.edu.co
    
Auditar la seguridad de la red, el mapeo de la red, identificar puertos abiertos y buscar dispositivos en línea, en el caso de la pagina de la universidad no nos dio acceso por permisos o tiene un buen servicio de proteccion y nos bloqueo para hacer un chequeo externo, tocaria estar dentro de la red principal.
