![maxresdefault (2)](https://user-images.githubusercontent.com/101933399/196845951-b5e1241f-30b6-47f2-b20c-35f503224819.jpg)

John the Ripper es una herramienta de crackeo de contraseñas escrita en C y muy utilizada por los analistas de seguridad para comprobar la robustez de una clave frente a ataques de fuerza bruta. Este programa es capaz de romper los hashes MD5, SHA-1 y otros muchos ampliamente utilizados en el mundo informático. Este programa es capaz de detectar de forma automática el tipo de hash que estamos crackeando, con el objetivo de facilitar al usuario su crackeo sin necesidad de preocuparse por el tipo de hash que está intentando «romper».

Algunas características muy importantes de este programa es que está optimizado para muchos modelos de procesadores, funciona en muchas arquitecturas de PC y también en diferentes sistemas operativos, no obstante, generalmente se utiliza en sistemas operativos basados en Linux, de hecho, las principales distribuciones Linux orientadas al pentesting y a la seguridad informática ya incorporan de forma predeterminada este programa.

    Versiones

Actualmente, nos podemos encontrar tres versiones de este software. En primer lugar tenemos la versión gratuita, que es la más utilizada, luego tenemos John the Ripper Pro, y la versión John The Ripper Jumbo. Cabe destacar, que se trata de software libre, distribuido bajo licencia GPL, que si bien permite que algunas partes se usen con otras licencias, otras están bajo el dominio público. En un principio fue creado para funcionar en sistemas Unix, pero actualmente podemos usarlo en unos 15 sistemas operativos diferentes. Entre ellos, once tipos de Unix, MS-DOS, Windows, BeOS y OpenVMS. Pero lo más habitual es encontrarlo en las distribuciones de Linux.

Si hablamos de la versión Pro, obviamente tendremos algunas ventajas frente a la gratuita. Por ejemplo, en esta versión de pago nos detectará de forma automática cualquier mejora en la tecnología que soporte el procesador de la máquina en la que se instaló. También tendremos un diccionario con más de 4 millones de entradas, donde detectará las mejoras de forma automática. De este modo nos ahorrará tiempo al evitarnos tener que realizar actualizaciones.

John the Ripper Jumbo, se trata de un parche que permite trabajar con una mayor cantidad de algoritmos. Como se trata de la versión que está en desarrollo, muchas de sus funciones no están a su máximo rendimiento, por lo cual puede llegar a presentar algún inconveniente.

    sudo apt install john
    
![image](https://user-images.githubusercontent.com/101933399/196846612-3b21122f-cafb-46f1-a955-2a08f6f616f3.png)

    ls /usr/share/john/

Nos muestra lo que tenemos en la carpeta John

    cat /usr/share/john/password.lst
Muestra el contenido del archivo password.lst

    sudo useradd -m test
Añade el usuario X con una clave

    sudo passwd test
Hacemos un test del nuevo password

    sudo tail /etc/shadow
almacena las contraseñas de las cuentas de usuario. Se utiliza este fichero por seguridad.

    sudo john --wordlist=/usr/share/john/password.lst /etc/shadow
Realiza la prueba de decifrar la contraseña y nos indica el tiempo que demora en desifrarla

    sudo passwd test
Hacemos un test del nuevo password

    sudo john /etc/shadow
Realiza la prueba de decifrar la contraseña
