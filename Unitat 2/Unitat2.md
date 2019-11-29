# **1ER DAM. Desarrotllament D'Aplicacions Multiplataforma. EDD. Entorns de Desenvolupament.**

# **Docker, Contenidors, Servidor CollabNet Subversion Edge, Git i RCS**

***2019-Editat amb [VisualStudioCode](https://code.visualstudio.com/) per a Windows, Linux i Mac.***

![Docker](/imatges/imatge0.png)

##### DOCKER. Una plataforma oberta per a construir, envíar i executar aplicacions distribuïdes. 

# Index:



>### UNITAT 2. Eines per al desenvolupament de programari.
>
>***[1.-Com instalar VSCODE en Ubuntu 18.](https://github.com/Maxim1erDAM/EDD/blob/master/Unitat%202/Unitat2.md#1-com-instalar-vscode-en-ubuntu-18)***
>
>***[2.-Com instalar extensions en VSCODE .](https://github.com/Maxim1erDAM/EDD/blob/master/Unitat%202/Unitat2.md#2-com-instalar-extensions-en-vscode)***
>
>***[3.-Programar en JAVA.](https://github.com/Maxim1erDAM/EDD/blob/master/Unitat%202/Unitat2.md#3-programar-en-java)***
>
>***[4.-Instalació Java JRE o JDK.](https://github.com/Maxim1erDAM/EDD/blob/master/treballdocker_maximsanchezporta.md#4-java-jre-o-jdk)***
>
>***[5.-Opcional. Instalació de Netbeans 11.1](https://github.com/Maxim1erDAM/EDD/blob/master/treballdocker_maximsanchezporta.md#5-opcional-instalaci%C3%B3-de-netbeans-111)***
>
>***[6.-Compilar Java desde VSCODE](https://github.com/Maxim1erDAM/EDD/blob/master/treballdocker_maximsanchezporta.md#6-compilar-java-desde-vscode)***

#    **-Activitat pràctica-**



# UNITAT 2. Práctica de Visual Studio Code.


## 1.-Com instalar VSCODE en Ubuntu 18.

>***`Actualizar llistat de repositoris de Ubuntu:`***  

sudo apt update

>***`Instalar dependencies:`***  

sudo apt install software-properties-common apt-transport-https wget

>***`Importar la clau GPG a Ubuntu:`***  

wget -q https://packages.microsoft.com/keys/microsoft.asc -O- | sudo apt-key add -

>***`Afegir el repositori a el llistat d'Ubuntu:`***  

sudo add-apt-repository "deb [arch=amd64] https://packages.microsoft.com/repos/vscode stable main"

>***`Actualitzar llistat de repositoris de Ubuntu:`***  

sudo apt update

>***`Instalar Visual Studio Code:`***  

sudo apt install code

## 2.-Com instalar extensions en VSCODE.

Podem buscar e instalar extensions desde aquest apartat de VSCODE, podem instalar, desinstalar, activar i desactivar extensions automáticament. Depenent del codi que vullgam activar funcionalitats especials, com etiquetes, o vulgam fer una previsualizació del codi, tindrem que instalar diferents extensions. Solen tardar a instalarse i funcionar per el seu pes, perque contenen les ferramentes i depèndencies per a que funcionen les extensions.

![Imatge](/imatges/imatgevscodeexts.png)

## 3.-Programar en JAVA.
    ¿Quina es la diferència entre JDK y JRE?

JDK es el Java Development Kit o, en español, Herramientas de Desarrollo de Java. Amb ell podem construir programes utilitzant el llenguatje de programació Java. Incorpora ferramentes útils como el compilador (javac), el desensamblador de binaris (javap), debugger, entre altres ferramentes. El JDK proveu ferramentes d'evaluació de rendiment d'aplicacions, como son VisualVM y Mission Control. Una instalació de JDK ya conté un JRE dins del seus directoris.

JRE es el Java Runtime Environment o, en español, el Entorno de Ejecución de Java. Conté a la Maquina Virtual de Java i altres ferramentes que permiteixen l'execució de les aplicacions Java. JRE no incorpora compiladors ni ferramentes per a desarrotllar les aplicacions Java, nomes incorpora les ferramentes per a executarles.

    ¿Quan deuria utilitzar-los?

Instales el JDK quan vols desarrotllar. Instalat nomes el JRE en els equips on nomes vas a executar aplicacions Java. Per eixemple, si vas a desarrotllar una aplicació GUI en Java, instala el JDK. Si vols que algún amic puga vore eixa aplicació en el seu equip, ell tindrá que instalarse el JRE per a poder executar l'aplicació Java.

*Normalment en un entorn productiu, depen, a mode de evitarte problemes, instalar el JDK.

*Si consideres que el teu entorn productiu será només per a execució de les teues aplicacions Java, entonces convé instalar nomes JRE.

*Si creus que necesites alguna de las ferramentes de desarrotllament en el teu servidor per a fer probes molt básiques desde eixos equips, per eixemple construir una aplicació xicoteta per a probar la conectivitat a una base de dades, entonces instala el JDK.

## 4.-Java JRE o JDK

Instalem desde la font oficial d'Oracle el JRE o el JDK de Java:

> https://www.oracle.com/technetwork/java/javase/downloads/ **Fa falta crear un usuari pero podem trobarlo d'altres fonts

Nosaltres descarregarem el JRE. Pero podem utilitzar un dels dos.
Elegim el paquet JRE o el JDK.

![Imatge](/imatges/JREoJDK.png)

Descarreguem la versió del nostre sistema operatiu. (.exe per a Windows, .rpm per a Linux, tinguent en compte si l'equip es i586-x86 o bé x64)

![Imatge](/imatges/JREoJDK2.png)

En Ubuntu per comandes podriem instalar el JRE o JDK amb la versió per defecte als repositoris d'Ubuntu, directament amb :

>sudo apt install default-jre

>sudo apt install default-jdk

Per a descomprimir el .tar.gz  del paquet de Java, per si el descarreguem en Ubuntu:

>sudo tar xzvf fichero.tar.gz

## 5. Opcional. Instalació de NetBeans 11.1 


>[>Redirigir a Guia d’instal.lació de NetBeans 11.1. ](https://github.com/Maxim1erDAM/EDD/blob/master/NetbeansInstalar.pdf)

## 6.-Instalar extensions de Java en VSCODE i utilitzar ferramentes de JRE o JDK

Anem a l'apartat d'extensions de Visual Studio Code i instalem "@id:vscjava.vscode-java-pack".
A partir de la font de vscode de :https://aka.ms/vscode-java-installer-win


![Imatge](/imatges/javaextvscodepack.png)

Podem descarregar també el Visual Studio Code Java Pack Installer :https://vscjavaci.blob.core.windows.net/vscodejavainstaller/release/0.2.1/VSCodeJavaInstaller-online-win-0.2.1.exe

*Si tenim algun problema en VSCODE o en les extensions, ho he solventat amb fer click en l'opcio "Buscar actualizaciones"

![Imatge](/imatges/solucioproblemesvscode.png)

*El directori de Windows al instalar JRE sol ser:

"C:\Program Files\java\jre_versiodejava\", amb els directoris "C:\Program Files\java\jre_versiodejava\bin" i "C:\Program Files\java\jre_versiodejava\lib".


## 6. Compilar Java desde VSCODE

Després de actualitzar VSCODE, e instalar les extensions, compilarem Java desde el terminal de MS-DOS de Windows, pero en un xicotet apartat de VSCODE.

Ejemplo de fichero HelloWorld.java en VSCODE
```java
    class HelloWorld
    {
        public static void main(String args[])
        {
            System.out.println("Hola Mundo");
        }
    }
```


Compilando Java en Terminal

    javac HelloWorld.java (deja un archivo .class compilado en el directorio actual)

Ejecutando Java en Terminal

    java HelloWorld (execució del compilat)

![Imatge](/imatges/compilariejecutarjavaSOLUCION.png)
