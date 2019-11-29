# **1ER. Desarrotllament D'Aplicacions Multiplataforma.**
# **TEMA 1.ENTORNS DE DESENVOLUPAMENT**
### **-Activitat pràctica d’avaluació continuada 1.(APAC1)-**

###### Modified With                   ***[Dillinger.io](https://dillinger.io/ )***

![La Gioconda (Wikipedia)](https://ladob.net/wp-content/uploads/2018/03/web-1935737_640.png) 


Els informátics utilitzem cualsevol eina que mos ajude a treballar millor a l'hora de programar

 
  
   
    
     
      
#### Ejercici 1. Llenguatges de programació.


    Investigueu sobre els deu llenguatges més utilitzats segons Octoverse, i feu una xicoteta descripció d’ells ,indicant en quines de les categories esmentades a la unitat es classificarien cadascun. Podeu seguir la següent plantilla:

    >-> Llenguatge
    >-> Nivell d’abstracció 
    >-> Alt/Baix/Intermedi 
    >-> Propòsit General/Específic Generació 1GL/2GL
    >-> Format d'execució Executat/Compilat/Altres 
    >-> Com planteja els problemes Imperatiu/Declaratiu
    >-> Paradigma Procedural o Orientat a objectes 
    >-> Lloc habitual d’execució Client/Servidor/Indistint.



*********`Ejercicio 1. `*********



| `ÍNDICE DE OCTOVERSE`| `Generación`   | `Función` | `Información adicional` | `Paradigma Procedural` |
| -------------- |--------------------------------------|---------------------|---------------------|--------------------|
|  `1.` Kotlin | 3era/4rta GEN|  Programación imperativa |Se puede compilar de código fuente Kotlin a Java.| Alto nivel. 	Propósito general. 	 Multiplataforma
| `2.` HCL |  1/2 GEN |  Programación imperativa | La infraestructura se define utilizando la sintaxis de configuración de HashiCorp denominada HashiCorp Configuration Language (HCL) o, en su defecto, el formato JSON.| Permite a los usuarios definir y configurar la infraestructura de un centro de datos en un lenguaje de alto nivel, generando un plan de ejecución para desplegar la infraestructura en OpenStack1, por ejemplo, u otros proveedores de servicio tales como AWS, IBM Cloud (antiguamente Bluemix), Google Cloud Platform, Linode, Microsoft Azure, Oracle Cloud Infrastructure o VMware vSphere. 
|  `3.` TypeScript  | 3era/4rta GEN |  Programación imperativa |  TypeScript se incluye como lenguaje de programación de primer nivel en Microsoft Visual Studio 2013 Update 2 y posteriores, junto a C# y otros lenguajes de Microsoft. Una extensión oficial permite a Visual Studio 2012 soportar también TypeScript | El compilador de TypeScript está escrito asimismo en TypeScript, compilado a JavaScript y con Licencia Apache 2. Alto nivel,Propósito general,programacion funcional,programación imperativa,programación orientada a objetos..| 
|  `4.` PowerShell | 1era/2nda GEN |  Programación imperativa |  PowerShell (originalmente llamada Windows PowerShell) es una interfaz de consola (CLI) con posibilidad de escritura y unión de comandos por medio de instrucciones (scripts en inglés). Esta interfaz de consola está diseñada para su uso por parte de administradores de sistemas, con el propósito de automatizar tareas o realizarlas de forma más controlada. Originalmente denominada como MONAD en 2003, su nombre oficial cambió al actual cuando fue lanzada al público el 25 de abril de 2006. El 15 de agosto de 2016, Microsoft publicó el código fuente de PowerShell en GitHub, y cambió su nombre a PowerShell Core. La versión 6 se ofrece con licencia MIT. | El compilador de TypeScript está escrito asimismo en TypeScript, compilado a JavaScript y con Licencia Apache 2. Alto nivel,Propósito general,programacion funcional,programación imperativa,programación orientada a objetos..| 
| `5.` Rust | 2 GEN |  Programación imperativa |  Rust es un lenguaje de programación compilado, de propósito general y multiparadigma que está siendo desarrollado por Mozilla. Ha sido diseñado para ser “un lenguaje seguro, concurrente y práctico”. Es un lenguaje de programación multiparadigma, soporta programación funcional pura, por procedimientos, imperativa y orientada a objetos. | Alto nivel 	Propósito general 	Extensión .rs. 	La programación imperativa. 	Compilado . 	Multiplataforma..| 
| `6.` CMake | 2/3 GEN |  Programación imperativa |  CMake es una herramienta multiplataforma de generación o automatización de código. Soporte para builds paralelos.Compilador cruzado Vista global de todas las dependencias, usando CMake para generar un diagrama graphviz. Soporte para builds multiplataforma. Linux y otros sistemas POSIX | Cmake genera makefiles nativos y espacios de trabajo que pueden usarse en el entorno de desarrollo deseado. Comparable al GNU build system de Unix en que el proceso es controlado por ficheros de configuración, en el caso de CMake llamados CMakeLists.txt. 	Análisis automático de dependencias para C, C++, Fortran, y Java. Soporte para varias versiones de Microsoft Visual Studio Compilado . Alto nivel 	Propósito general 	 	Multiplataforma.| 
| `7.` Go  | 2 GEN |  Programación imperativa |  Go es un lenguaje de programación concurrente y compilado inspirado en la sintaxis de C .Actualmente está disponible en formato binario para los sistemas operativos Windows, GNU/Linux, FreeBSD y Mac OS X, pudiendo también ser instalado en estos y en otros sistemas con el código fuente. | Go es un lenguaje de programación compilado, concurrente, Alto nivel, imperativo, estructurado, orientado a objetos y con recolector de basura que de momento está soportado en diferentes tipos de sistemas UNIX, incluidos Linux, FreeBSD, Mac OS X y Plan 9.| 
| `8.` Python  | 3ra/4ta GEN |  Programación imperativa |  Python es un lenguaje de programación interpretado cuya filosofía hace hincapié en una sintaxis que favorezca un código legible. Se trata de un lenguaje de programación multiparadigma. | Soporta orientación a objetos, programación imperativa y, en menor medida, programación funcional. Es un lenguaje interpretado,Alto nivel, dinámico y multiplataforma. És administrado por la Python Software Foundation. Posee una licencia de código abierto, denominada Python Software Foundation License.| 
| `9.` Groovy | 3era/rta GEN | Groovy es un lenguaje de programación orientado a objetos implementado sobre la plataforma Java. Tiene características similares a Python, Ruby, Perl y Smalltalk. La especificación JSR 241 se encarga de su estandarización para una futura inclusión como componente oficial de la plataforma Java. Groovy usa una sintaxis muy parecida a Java, comparte el mismo modelo de objetos, de hilos y de seguridad. Desde Groovy se puede acceder directamente a todas las API existentes en Java. El bytecode generado en el proceso de compilación es totalmente compatible con el generado por el lenguaje Java para la Java Virtual Machine (JVM), por tanto puede usarse directamente en cualquier aplicación Java. Todo lo anterior unido a que la mayor parte de código escrito en Java es totalmente válido en Groovy hacen que este lenguaje sea de muy fácil adopción para programadores Java. | És un lenguaje que nació en 2003, basado en algunas funcionalidades similares a Python, Ruby, Perl y Smalltalk, todo ello ejecutándose sobre la máquina virtual de Java, lo que conlleva la posibilidad de utilizar la riquísima biblioteca de librerías de Java, entre otros beneficios.Groovy es un lenguaje muy versátil, permitiendo usarse para desarrollar aplicaciones web, aplicaciones de escritorio, aplicaciones móviles para Android o incluso usándolo como lenguaje de scripting.|Programación orientada a objetos, programacion funcional.Alto Nivel 	Multiplataforma| 
| `10.` SQL-PL | 4rta/5nta GEN | /SQL (Procedural Language/Structured Query Language) es un lenguaje de programación incrustado en Oracle. PL/SQL soportará todas las consultas, ya que la manipulación de datos que se usa es la misma que en SQL, incluyendo nuevas características:El manejo de variables, Estructuras modulares, Estructuras de control de flujo y toma de decisiones y el Control de excepciones. El lenguaje PL/SQL está incorporado en:en el servidor de la base de datos. En un entorno de base de datos los programadores pueden construir bloques PL/SQL para utilizarlos como procedimientos o funciones, o bien pueden escribir estos bloques como parte de scripts SQL*Plus. Los programas o paquetes de PL/SQL se pueden almacenar en la base de datos como otro objeto, y todos los usuarios que estén autorizados tienen acceso a estos paquetes. Los programas se ejecutan en el servidor para ahorrar recursos a los clientes.. | Utilizado en programación, diseñado para administrar, y recuperar información de sistemas de gestión de bases de datos relacionales. Una de sus principales características es el manejo del álgebra y el cálculo relacional para efectuar consultas con el fin de recuperar, de forma sencilla, información de bases de datos, así como realizar cambios en ellas.|Lenguaje Estructurado de consultas a bases de datos, Programación orientada a objetos, programacion funcional….Alto Nivel 	Multiplataforma| 

  |`Lenguaje`| ---------------------------------`Descripción`---------------------------------   |`Nivel de abstracción` | `Próposito` |------ `Formato de ejecución`--------------- | --------------`---Como---- ------plantea--------los---- ----problemas----`---------------------| `Paradigma Procedural` | -----`Lugar de ejecución`---------- |
| ---------------------------------------------- |:--------------------------------------:|:---------------------:|:---------------------:|:-------:|:-----:|:-------:|:----------------:|
| `1.` Kotlin         |  Kotlin es un lenguaje de programación fuertemente tipado desarrollado por JetBrains (los creadores de IntelliJ IDEA). Ha sido fuertemente influenciado por lenguajes como Groovy, Scala o C#. Permite generar código para la JVM (máquina virtual de Java 6) Javascript y en las últimas versiones también ejecutables nativos. | Alto nivel | Propósito general| Se puede compilar de código fuente Kotlin a Java. | La programación imperativa. | Programación orientada a objetos, programacion funcional. | Android, Linux, Windows, Mac servidores,  y sus archivos binarios tambien estan accesibles incluso para WebAssembly y sistemas integrados como STM32.
| `2.` HCL         | Terraform es un software de infraestructura como código (infrastructure as code) desarrollado por HashiCorp. Permite a los usuarios definir y configurar la infraestructura de un centro de datos en un lenguaje de alto nivel, generando un plan de ejecución para desplegar la infraestructura en OpenStack, por ejemplo, u otros proveedores de servicio tales como AWS, IBM Cloud (antiguamente Bluemix), Google Cloud Platform, Linode, Microsoft Azure, Oracle Cloud Infrastructure o VMware vSphere. La infraestructura se define utilizando la sintaxis de configuración de HashiCorp denominada HashiCorp Configuration Language (HCL) o, en su defecto, el formato JSON.9 HashiCorp también mantiene el repositorio de configuraciones Terraform Module Registry, lanzado en 2017 durante la conferencia HashiConf.10  .| Alto nivel | Propósito general| Los ficheros Terraform con este formato se crearan con la extensión “.tf.json”. | Permite a los usuarios definir y configurar la infraestructura de un centro de datos en un lenguaje de alto nivel, generando un plan de ejecución para desplegar la infraestructura en OpenStack1, por ejemplo, u otros proveedores de servicio tales como AWS, IBM Cloud (antiguamente Bluemix), Google Cloud Platform, Linode, Microsoft Azure, Oracle Cloud Infrastructure o VMware vSphere. La infraestructura se define utilizando la sintaxis de configuración de HashiCorp denominada HashiCorp Configuration Language (HCL) o, en su defecto, el formato JSON. | Programación orientada a objetos, programacion funcional. | Android, Linux, Windows, Mac servidores,  y sus archivos binarios tambien estan accesibles incluso para WebAssembly y sistemas integrados como STM32.
| `3.` TypeScript     |                      TypeScript es un lenguaje de programación libre y de código abierto desarrollado y mantenido por Microsoft. Es un superconjunto de JavaScript, que esencialmente añade tipos estáticos y objetos basados en clases. TypeScript puede ser usado para desarrollar aplicaciones JavaScript que se ejecutarán en el lado del cliente o del servidor (Node.js). TypeScript extiende la sintaxis de JavaScript, por tanto cualquier código JavaScript existente debería funcionar sin problemas. Está pensado para grandes proyectos, los cuales a través de un compilador de TypeScript se traducen a código JavaScript original. TypeScript soporta ficheros de definición que contengan información sobre los tipos de librerías JavaScript existentes, similares a los ficheros de cabeceras de C/C++ que describen la estructura de ficheros de objetos existentes. Esto permite a otros programas usar los valores definidos en los ficheros como si fueran entidades TypeScript de tipado estático. Existen cabeceras para librerías populares como jQuery, MongoDB y D3.js, y los módulos básicos de Node.js. El compilador de TypeScript está escrito asimismo en TypeScript, compilado a JavaScript y con Licencia Apache 2. | Alto nivel | Propósito general| El compilador de TypeScript está escrito asimismo en TypeScript, compilado a JavaScript y con Licencia Apache 2. | La programación imperativa. | Programación orientada a objetos, programacion funcional. | TypeScript se incluye como lenguaje de programación de primer nivel en Microsoft Visual Studio 2013 Update 2 y posteriores, junto a C# y otros lenguajes de Microsoft. Una extensión oficial permite a Visual Studio 2012 soportar también TypeScript
| `4.` PowerShell     |                      PowerShell (originalmente llamada Windows PowerShell) es una interfaz de consola (CLI) con posibilidad de escritura y unión de comandos por medio de instrucciones (scripts en inglés). Esta interfaz de consola está diseñada para su uso por parte de administradores de sistemas, con el propósito de automatizar tareas o realizarlas de forma más controlada. Originalmente denominada como MONAD en 2003, su nombre oficial cambió al actual cuando fue lanzada al público el 25 de abril de 2006. El 15 de agosto de 2016, Microsoft publicó el código fuente de PowerShell en GitHub, y cambió su nombre a PowerShell Core. La versión 6 se ofrece con licencia MIT. | Alto nivel | Se basa en el framework .NET y es perfecto para automatizar procesos por lotes y tareas del sistema | PowerShell files for all versions are .ps1 (or .psm1, .psd1, etc.).. | La programación imperativa. | En Windows y Linux ,s e ha integrado en Microsoft desde Windows Server 2003 R2.. | Windows, Linux, etc...
| `5.` Rust           |                   Rust es un lenguaje de programación compilado, de propósito general y multiparadigma que está siendo desarrollado por Mozilla. Ha sido diseñado para ser "un lenguaje seguro, concurrente y práctico". Es un lenguaje de programación multiparadigma, soporta programación funcional pura, por procedimientos, imperativa y orientada a objetos.El lenguaje surgió de un proyecto personal desarrollado por Graydon Hoare (trabajador de Mozilla), quien empezó a trabajar en él en 2006; Mozilla se involucró en este proyecto en 2009, y lo dio a conocer oficialmente en 2010. Ese mismo año, el trabajo pasó del compilador inicial (escrito en OCaml) al compilador autocontenido, escrito en sí mismo. Conocido como rustc, en 2011 se compiló a sí mismo. El compilador autocontenido usa LLVM como su back-end.La primera versión alfa numerada del compilador de Rust apareció en enero de 2012. La versión 1.0 fue lanzada el 15 de mayo de 2015. Según la política de Mozilla,Rust es desarrollado de forma totalmente abierta y busca la opinión y contribución de la comunidad. El diseño del lenguaje se ha ido perfeccionando a través de las experiencias en el desarrollo del motor de navegador Servo, y el propio compilador de Rust. Aunque es desarrollado y patrocinado por Mozilla y Samsung, es un proyecto comunitario. Una gran parte de las contribuciones proceden de los miembros de la comunidad.| Alto nivel | Propósito general| Extensión .rs. | La programación imperativa. | Compilado . | Multiplataforma.
| `6.` CMake          |                      CMake es una herramienta multiplataforma de generación o automatización de código. El nombre es una abreviatura para "cross platform make" (make multiplataforma); más allá del uso de "make" en el nombre, CMake es una suite separada y de más alto nivel que el sistema make común de Unix, siendo similar a las autotools.CMake es una familia de herramientas diseñada para construir, probar y empaquetar software. CMake se utiliza para controlar el proceso de compilación del software usando ficheros de configuración sencillos e independientes de la plataforma. | Alto nivel | Soporte para builds paralelos.Compilador cruzado Vista global de todas las dependencias, usando CMake para generar un diagrama graphviz. Soporte para builds multiplataforma. Linux y otros sistemas POSIX (incluyendo AIX, *BSD, HP-UX, IRIX/SGI, y Solaris). Mac OS X Windows 95/98/NT/2000/XP, Windows Vista, Windows 7 y MinGW/MSYS Integrado con DART (software), CDash, CTest y CPack, una colección de herramientas para prueba y liberación de software…| Cmake genera makefiles nativos y espacios de trabajo que pueden usarse en el entorno de desarrollo deseado. Comparable al GNU build system de Unix en que el proceso es controlado por ficheros de configuración, en el caso de CMake llamados CMakeLists.txt. Al contrario que el GNU build system, que está restringido a plataformas Unix, CMake soporta la generación de ficheros para varios sistemas operativos, lo que facilita el mantenimiento y elimina la necesidad de tener varios conjuntos de ficheros para cada plataforma. Generar ficheros de proyecto para Code::Blocks, Eclipse CDT, Microsoft Visual Studio de la 6 a la 10 incluyendo versiones de 64 bits y KDevelop. | La programación imperativa. | Análisis automático de dependencias para C, C++, Fortran, y Java. Soporte para varias versiones de Microsoft Visual Studio, incluyendo la 6, 7, 7.1, 8.0, 9.0 y 10.0    Genera ficheros para Eclipse CDT (C/C++ Development Tools). Detección de cambios en ficheros usando timestamps tradicionales.  | Multiplataforma .
| `7.` Go             |                      Go es un lenguaje de programación concurrente y compilado inspirado en la sintaxis de C. Ha sido desarrollado por Google, y sus diseñadores iniciales son Robert Griesemer, Rob Pike y Ken Thompson. Actualmente está disponible en formato binario para los sistemas operativos Windows, GNU/Linux, FreeBSD y Mac OS X, pudiendo también ser instalado en estos y en otros sistemas con el código fuente.2?3? Go es un lenguaje de programación compilado, concurrente, imperativo, estructurado, orientado a objetos y con recolector de basura que de momento está soportado en diferentes tipos de sistemas UNIX, incluidos Linux, FreeBSD, Mac OS X y Plan 9 (puesto que parte del compilador está basado en un trabajo previo sobre el sistema operativo Inferno). Las arquitecturas soportadas son i386, amd64 y ARM. | Alto nivel | Propósito general| Compilado, similar a código C y C++. . | La programación imperativa. | Paradigma	compilado concurrente, imperativo, estructurado. | Multiplataforma.
| `8.` Python         |                      Python es un lenguaje de programación interpretado cuya filosofía hace hincapié en una sintaxis que favorezca un código legible. Se trata de un lenguaje de programación multiparadigma, ya que soporta orientación a objetos, programación imperativa y, en menor medida, programación funcional. Es un lenguaje interpretado, dinámico y multiplataforma. És administrado por la Python Software Foundation. Posee una licencia de código abierto, denominada Python Software Foundation License,2? que es compatible con la Licencia pública general de GNU a partir de la versión 2.1.1, e incompatible en ciertas versiones anteriores.| Alto nivel | Propósito general| Los archivos PY , se crean para guardar scripts u otros archivos asociados a programas que han sido codificados en el lenguaje de programación Python. Estos archivos PY pueden abrirse y editarse fácilmente con cualquier editor de texto, pero se recomienda utilizar un editor de texto que ofrezca resaltado de sintaxis.. | Programación funcional en Python. Una de las principales características de Python es que este es un lenguaje multiparadigma.  | Podemos desarrollar proyectos utilizando un enfoque orientado a objetos, imperativo e inclusive (en menor medida) funcional. Scripting. | Multiplataforma.
| `9.` Groovy         |                      Groovy es un lenguaje de programación orientado a objetos implementado sobre la plataforma Java. Tiene características similares a Python, Ruby, Perl y Smalltalk. La especificación JSR 241 se encarga de su estandarización para una futura inclusión como componente oficial de la plataforma Java. Groovy usa una sintaxis muy parecida a Java, comparte el mismo modelo de objetos, de hilos y de seguridad. Desde Groovy se puede acceder directamente a todas las API existentes en Java. El bytecode generado en el proceso de compilación es totalmente compatible con el generado por el lenguaje Java para la Java Virtual Machine (JVM), por tanto puede usarse directamente en cualquier aplicación Java. Todo lo anterior unido a que la mayor parte de código escrito en Java es totalmente válido en Groovy hacen que este lenguaje sea de muy fácil adopción para programadores Java; la curva de aprendizaje se reduce mucho en comparación con otros lenguajes que generan bytecode para la JVM, tales como Jython o JRuby. Groovy puede usarse también de manera dinámica como un lenguaje de scripting. Groovy 1.0 apareció el 2 de enero de 2007. Después de varias versiones beta y otras tantas candidatas a release, el 7 de diciembre de 2007 apareció la versión Groovy 1.1 que finalmente fue renombrada a Groovy 1.5 con el fin de notar la gran cantidad de cambios que ha sufrido con respecto a la versión 1.0. En diciembre de 2009 se publicó la versión 1.7. | És un lenguaje que nació en 2003, basado en algunas funcionalidades similares a Python, Ruby, Perl y Smalltalk, todo ello ejecutándose sobre la máquina virtual de Java, lo que conlleva la posibilidad de utilizar la riquísima biblioteca de librerías de Java, entre otros beneficios.Groovy es un lenguaje muy versátil, permitiendo usarse para desarrollar aplicaciones web, aplicaciones de escritorio, aplicaciones móviles para Android o incluso usándolo como lenguaje de scripting. Además, no es necesario utilizar en exclusiva, ya que se puede usar a la vez dentro de un proyecto Java ya existente y comenzar a realizar los test utilizando la potencia de este lenguaje. | Programación orientada a objetos, programacion funcional.  Multiplataforma
| `10.` SQL-PL          |                      PL/SQL (Procedural Language/Structured Query Language) es un lenguaje de programación incrustado en Oracle. PL/SQL soportará todas las consultas, ya que la manipulación de datos que se usa es la misma que en SQL, incluyendo nuevas características:El manejo de variables, Estructuras modulares, Estructuras de control de flujo y toma de decisiones y el Control de excepciones. El lenguaje PL/SQL está incorporado en:en el servidor de la base de datos. En un entorno de base de datos los programadores pueden construir bloques PL/SQL para utilizarlos como procedimientos o funciones, o bien pueden escribir estos bloques como parte de scripts SQL*Plus. Los programas o paquetes de PL/SQL se pueden almacenar en la base de datos como otro objeto, y todos los usuarios que estén autorizados tienen acceso a estos paquetes. Los programas se ejecutan en el servidor para ahorrar recursos a los clientes.| Alto nivel,permite una alta productividad en codificación y la orientación a objetos | Utilizado en programación, diseñado para administrar, y recuperar información de sistemas de gestión de bases de datos relacionales.  Una de sus principales características es el manejo del álgebra y el cálculo relacional para efectuar consultas con el fin de recuperar, de forma sencilla, información de bases de datos, así como realizar cambios en ellas. | Los cambios en las bases de datos se y sus consultas se interpretan en una estructura de codigo de administracion de PL/SQL o SQL para modificar las tablas. Estas una vez el servidor de SQL se encuentre en ejecución se pueden realizar consultas PL/SQL a través de clientes requiriendolés o no autenticación. Estás bases de datos y tablas pueden realizar cálculos de todo tipo. El paradigma de programación de PL/SQL es imperativo combinado con instrucciones declarativas con el lenguaje de consulta SQL. Las instrucciones imperativas se usan para ejecutar asignación, operaciones aritmética, comparativas y ejecutar ciclos, entre otros.. | Lenguaje Estructurado de consultas a bases de datos, Programación orientada a objetos, programacion funcional.. | Android, Linux, Windows, Mac servidores,  y sus archivos binarios tambien estan accesibles incluso para WebAssembly y sistemas integrados como STM32.

#### Ejercici 2. Aplicacions multiplataforma. 

    Investigueu sobre les algunes de les següents aplicacions multiplataforma, feu-ne una xicoteta descripció i esbrineu en quin llenguatge de programació estan desenvolupades:
 
    •LibreOffice
    •Mozilla Firefox
    •GIMP
    •Plucker
    •Skype
    •Opera.


*********`Ejercicio 2. `*********



Información:

>`>LibreOffice`
>Su entorno está programado en: C++, Java y Python.

>`>Mozilla Firefox`
>Su entorno está programado  en: C++, XUL, XBL, JavaScript, CSS, C y Rust (lenguaje de programación).

>`>Gimp`
>Programado en: C y GTK.

>`>Plucker`
>Programado en: C y C++ (palm OS & PDA's).

>`>Skype`
>Programado en: Delphi, Objective-C, C++, Object Pascal y JavaScript.

>`>Opera`
>Programado en: C++.



#### Ejercici 3. Compilació i execució de codi.

    Sobre la pràctica 3 del butlletí de pràctiques, modifiqueu els diferents programes d’Hola Món enels diferents llenguatges de programació per a que mostre el missatge Holaatots! Emdiuen... iestudie1rdeDAM! , reemplaçant els ... amb el vostre nom. Incloeu a la memòria el codimodificat i els passos seguits per executar-los, i si és el cas, per compilar-los.
    
*********`Ejercicio 3. `*********


>`Código C - Archivo`


    #include <stdio.h>
    int main()
    {
       // printf() displays the string inside quotation
       printf("Hola a tots! Em diuen, Máxim i estudie 1er de DAM!!!");
       return 0;
    }

>`Compilando C en Terminal`

    gcc hello.c  -o hello    
    
>`Ejecutando C en Terminal`
    
    ./hello

>`Python - Archivo`

    print("Hola a tots! Em diuen, Máxim i estudie 1er de DAM!!") 
	
>`Ejecución Python`

    "py Hello.py" o bien "python Hello.py"
    
>`Node JS - Archivo`

    console.log("Hola a tots! Em diuen, Máxim i estudie 1er de DAM!!");

>`Ejecutar desde terminal, código Node JS`

    nodejs hello.js
	
>`Java`

     class HelloWorld
    {
        public static void main(String args[])
        {
            System.out.println("Hola Mundo");
        }
    }
    
>`Compilando Java en Terminal`
    
    javac HelloWorld.java (deja un archivo .class compilado en el directorio actual)
    
>`Ejecutando Java en Terminal`
    
    java HelloWorld (resultado del compilado)
