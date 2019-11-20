# **1ER. Desarrotllament D'Aplicacions Multiplataforma. Entorns de desenvolupament**
# **TEMA 1.-DOCKER, CONTENIDORS Y SERVIDOR COLLABNET SUBVERSION EDGE-**
### **-Activitat pràctica-**

 ***2019-Editat amb [VisualStudioCode](https://code.visualstudio.com/) per a Windows, Linux i Mac.***

![Programació(Wikipedia)](/imatges/imatge0.png) 
#### DOCKER. Una plataforma oberta per a construir, envíar i executar aplicacions distribuides. 

 
  
   
    
     
      
## Ejercici sobre Docker y servidor de CollabNet Subversion Edge.


###***`1.¿Que és Docker? Docker es una aplicació de códi obert que permiteix que una aplicació Linux i les seues dependencies s'empaqueten como un contenidor. La virtualització basada en contenidors aísla les aplicacions entre sí amb un sistema operatiu (OS) compartit. Actualment és compatible amb Windows, Linux y Mac, per tant es multiplataforma.`***


### ***`2.¿Que és Subversion Edge? CollabNet Subversion Edge es la distribució principal del servidor de Apache Subversion. Subversion Edge inclou una pila completa de software Apache HTTP Server, Subversion y ViewVC, així como una potent interfície d'usuari basada en la web per administrar el servidor. Subversion Edge implementa i administra servidors Apache Subversion de manera eficient amb un entorn d'usuari centralitzat e intuitiu.`***


#### -Configurar VirtualBox.

>***`*En VirtualBox, ((ctrl+alt DERECHO)+c) configura la finestra o maquina virtual.  `***  
####`En configuració podem configurar el portafolis bidireccional. Per a activarlo`:
> ***`((ctrl+alt DERECHO)+c)`***+***`Dispositivos>Portapapeles Compartido> Bidireccional`***+***` Dispositivos>Arrastrar y Soltar> Bidireccional`***

#### -Com activar el portafolis i "Arrastrar y soltar".

![Imatge](/imatges/imatge6.png)

``Asignem "Bidireccional" en els dos casos.``


 #### -Instalar "Guest Additions".

``Fem clic en "Insertar imagen de CD de las <<Guest Additions>>". Es montará la unitat de cdrom amb la ISO corresponent.``

>***`alumne@alumne-VirtualBox:/media/alumne$ `*** cd /
>***`alumne@alumne-VirtualBox:/media/alumne$ `***  cd /media/alumne/VBox_GAs_6.0.12/

>***`Instalar guest additions en una maquina virtual basada en Ubuntu `***    
>***`alumne@alumne-VirtualBox:/media/alumne$ `*** sudo sh VBoxGuestAdditions.run 


 #### -Ferramentes per a la máquina virtual.


>***`*Opcional. Instalar editor de text Vim`***
$sudo apt-get install vim

>***`*Opcional. Instalar terminal Tilix`***
$sudo apt-get install tilix





## -Com instalar docker en Ubuntu 18 o altres distribucions de linux.


>***`Asignar contraseña a root e iniciar contraseña, en el meu cas "alumne" es el usuari de la maquina virtual`***
`USUARIO@USUARIO-VirtualBox:$sudo passwd root`
`>root >root` ***`<Así afegim la contraseña de root y la confirmem`***

>***`En el meu cas`***
alumne@alumne-VirtualBox:~$sudo passwd root
`>root >root` ***`<Así afegim la contraseña de root y la confirmem`***



>***`Iniciar sessió amb root`***
 >alumne@alumne-VirtualBox:~$ su root
Contraseña: ***`<Así afegim la contraseña de root`***
root@alumne-VirtualBox:/home/alumne# ***`<Así ja hem iniciat sesió amb root`***



>***`Afegir repositori deb de docker (disponible en so basat en ubuntu 18 bionic)`***
$sudo add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/ubuntu bionic stable"


   
      
## Instalar docker:
>***`Instalar dependencies de els paquets de docker`***
$sudo apt install apt-transport-https ca-certificates curl software-properties-common


>***`Instalar docker des dels repositoris de docker, en Ubuntu 18`*** 
sudo apt install docker-ce
## Configurar docker:

>***`Asignem contraseña a root`*** 
sudo passwd root

>***`Iniciem sessió com a root`*** 
su root

>***`Ara inicia sessió en root per a no tindre problemes en docker, pero podriem utilitzar altre usuari amb privilegis com a root`***  
su root

>***`Descarrega la imatge busybox (mini imatge de system o de root per a poder executar aplicacions independentment de root y system de ubuntu)`***  
docker pull busybox


>***`Descarrega la imatge subversion edge`***  
apt install subversion

>***`Afegir clau gpg de docker per a afegirla en ubuntu`***
$curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -

>***`Comprobar si s'ha descarregat la firma o empremta digital`***
$sudo apt-key fingerprint 0EBFCD88

>***`Tornar a actualizar paquets`***
$sudo apt update

>***`Instalar paquets del repositori de docker`***
$sudo apt install docker-ce

>***`Actualitzar cache de la politica o privacitat de docker`***
$sudo apt-cache policy docker-ce

##Comandos y configuración de docker
####
>***`>Iniciem sessió como root`***
 >alumne@alumne-VirtualBox:~$ su root
Contraseña: ***`<Así afegim la contraseña de root`***
root@alumne-VirtualBox:/home/alumne# 

>***`Mostrar hello world de docker `***
 docker run hello-world

>***`Activar el servei de docker`***
 systemctl enable docker

>***`Desactivar el servei de docker`***
 systemctl disable docker

>***`Descarregar el busybox per a Docker (estructura de system o root per a contenidors o imatges de docker)`***
 docker pull busybox

>***`Vore imatges que estan instalades en docker`***
 docker images

>***`Mostra hola per pantalla amb la imatge de busybox per a docker`***
 docker run busybox echo "hola"

>***`Mostra el ls per pantalla amb la imatge de busybox per a docker`***
docker run busybox ls

>***`Mostra el archiu de text del usuari /etc/passwd de la imatge busybox`***
docker run busybox cat /etc/passwd

>***`Mostra els contenidors de la imatge`***
docker run busybox ps aux

>***`Activar mode shell dins de la imatge de docker busybox (utilitzar comandes dins de la imatge busybox)`***
docker run -it busybox sh

>***`Vore els procesos que shan creat en la sessió actual del usuari i docker*`***
docker ps -a

>***`Per a eliminar un contenidor, afegir el codi del contenidor eixemple:5dde99182cec`***
 docker rm 5dde99182cec

>***`Ids dels contenidors que ja han acabat la tasca perque tenen status com a exited`***
docker ps -a -q -f status=exited

>***`Combinar comando de contenidors que han acabat la taska amb "comando de matar els procesos amb status exited"`***
 docker rm$(docker ps -a -q -fstatus=exited)

>***`Executar imatge o contenidor de subversion-edge amb docker `***
docker run -d mamohr/subversion-edge

>***`Veiem si el contenidor de subversion-edge es troba en execució`***
 docker ps

>***`Per a eliminar el contingut de subversion-edge`***
docker rm "codi del contenidor"

>***`Tornar a executar subversion-edge correctament (si no te les images les descarrega)`***
docker run -d -p 3343:3343 -p 4434:4434 -p 18080:18080  --name svn-server mamohr/subversion-edge

>***`Tinguent en compte que la carpeta "/opt/csvn/data" del contenidor, que és on el CSVN guarda tota la informació que genera, la sincronitzarem al volum(directori) "/srv/svn-data" . Amb açò ja podem accedir al servidor via web, generar usuaris, i generar repositoris guardant els canvis. Per tant , executarem el contenidor indicant els ports que es redirigixen en de el contenidor a la maquina local`***
>$docker run -d -p 3343:3343 -p 4434:4434 -p 18080:18080 -v /srv/svn-data:/opt/csvn/data --name svn-server mamohr/subversion-edge



>>>$ 
Unable to find image 'mamohr/subversion-edge:latest' locally
latest: Pulling from mamohr/subversion-edge
469cfcc7a4b3: Pull complete 
7e814dc876c6: Pull complete 
144c1c97a750: Pull complete 
17eb6ecf9d0a: Pull complete 
12492ca50197: Pull complete 
32dc87336990: Pull complete 
Digest: sha256:547356c2d4c2b2a7eb6e8f7b84de52118ca7089b98d2400f7c723e2280022ab6
Status: Downloaded newer image for mamohr/subversion-edge:latest
77c16450dbb29a614a205e95f9c3ca2072f156dc46a67e5a6b2e1b296e660d03


>***`**Instalar el contenidor i les dependencies  del servidor de Subversion Edge de manera manual, si la comanda anterior no lo descarrega`***
apt install subversion

>***`*Accedir a la pagina http de subversion edge amb usuari:admin contraseña:admin, crear un usuari en el meu cas "alumne123." i el repositori "Projecte1"`***

>http://127.0.0.1:3343/csvn/

>***`Pulsar start per a encendre el servidor subversion desde el navegador.`***

>***`Crear usuari "alumne123." i el repositori "Projecte1" desde el servidor subversionedge`***

>***`Detindre el servei de subversion (es troba renombrat així en la ordre de ejecució del contenidor)`***
docker stop svn-server

>***`Activar el servei de subversion (es troba renombrat així en la ordre de ejecució del contenidor) `***
docker start svn-server

####Accedim al servidor en amb el usuari administrador "admin" i contraseña 'admin' per defecte per a subversion.

![Imatge](/imatges/imatge1.png)

####Accedim a la pantalla de creació de usuaris.

![Imatge](/imatges/imatge2.png)



![Imatge](/imatges/imatge3.png)

####Crearem un usuari , este cas e creat "alumne123." i afegim tots els permisos en el cas de que siga administrador.

![Imatge](/imatges/imatge4.png)


>***`Donar permisos y accesibilitat al usuari, a este enllaç de host en la red local i crear els seus directoris de tags,trunk y branches.*Desde usuari root amb password asignada amb passwd.   `***



####Donem permisos i es crearan els directoris 
>***`svn co http://127.0.0.1:18080/svn/Projecte1 alumne123.`***
>A    alumne123./tags
>A    alumne123./trunk
>A    alumne123./branches
>Revisión obtenida: 1


>***`Donar permisos y accesibilitat al usuari, a este enllaç de host en la red local i crear els seus directoris de tags,trunk y branches.* Desde usuario administrador de Ubuntu con otro nombre como usuario "alumne". `***

>***`alumne@alumne-VirtualBox:~$ sudo svn co http://127.0.0.1:18080/svn/Projecte1 alumne123.`***
>Reino de autentificación: <http://127.0.0.1:18080> CollabNet Subversion Repository
>Clave de 'alumne123.': **********
>`-----------------------------------------------------------------------`
>ATENCIÓN!  Su contraseña para el reino de autenticación:
>   <http://127.0.0.1:18080> CollabNet Subversion Repository
>solo se puede almacenar en discos sin cifrar.  Está avisado de configurar
>su sistema de manera que Subversion pueda almacenar contraseñas cifradas, si
>es posible.  Vea la documentación para tener más detalles.
>Puede evitar futuras apariciones de este aviso configurando el valor
>de la opción «store-plaintext-passwords» a «yes» o «no» en
>«/home/alumne/.subversion/servers».
>`-----------------------------------------------------------------------`
>Almacenar la clave sin cifrar (sí/no)? S
>Por favor ingrese 'sí' o 'no': Si
>Por favor ingrese 'sí' o 'no': Sí
A alumne123./tags
A alumne123./trunk
A alumne123./branches
Revisión obtenida: 1

![Imatge](/imatges/imatge5.png)
***`La contraseña de subversion edge la demana gráficament, és la que esta asignada per defecte per a l'administració del servidor de apache de subversion edge.`***

####***`Finalment, subversion edge esta configurat i funcionant, podem fer el mateix amb cualsevol contenidor  per a Docker, y amb un procediment paregut el servei funcionaría de la mateixa manera utilitzant els directoris de Docker. Tinguem en compte que els directoris de configuracio de  "/opt/csvn/data" y "/srv/svn-data" son relatives als contenidors que instalem, i poden cambiar o no els directoris segons la seua configuracio per defecte y el metode de instalació al instalar els contenidors de altres serveis disponibles .  `***

## Com treballar en GIT.

***`Instalem GIT des dels repositoris d'Ubuntu. Li asignem una configuració básica d'usuari de git.`***

![Imatge](/imatges/imatge7.png)

***`Podem asignar l'editor per defecte amb la línea`*** 
git config --global core.editor "nomdeeditor"

***`Podem mostrar les variables de configuració amb:`*** 
git config --list

![Imatge](/imatges/imatge8.png)

***`Com crear un commit, al modificar o crear o eliminar archius:`*** 
Eixemple: git commit -a -m "Primer Commit"

![Imatge](/imatges/imatge9.png)

***`Mostrar commits creats:`*** 
Eixemple: git log


***`Creem un parell de fixers de text:`*** 
Eixemple:
 `touch fitxer 1.md`
 `touch fitxer 2.md`


 
***`Creem un altre commit afegit de prova :`*** 
Eixemple: git commit -a -m "nous canvis"

***`Y tornem a mostrar la informació dels commits amb:`*** 
 git log

![Imatge](/imatges/imatge11.png)




