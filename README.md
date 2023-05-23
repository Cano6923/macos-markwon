

<p align="middle">
  <a href="https://github.com/antz22/ultimate-guide-to-flutter"><img src="https://github.com/antz22/ultimate-guide-to-flutter/blob/master/assets/banner.svg"></a>
</p>

<p align="center">
  <h2 align="center">MacOS  - Flutter</h2>

  <p align="center">
   Guia completa de instalacion en el sistema operativo MacOS 
  </p>

  <p align="center">
    <a href="https://github.com/antz22/ultimate-guide-to-flutter/stargazers" alt="Stars">
        <img src="https://img.shields.io/github/stars/antz22/ultimate-guide-to-flutter?style=for-the-badge" /></a>
    <a href="https://github.com/antz22/ultimate-guide-to-flutter/network/members" alt="Forks">
        <img src="https://img.shields.io/github/forks/antz22/ultimate-guide-to-flutter?style=for-the-badge" /></a>
    <a href="https://github.com/Solido/awesome-flutter">
        <img alt="Awesome Flutter" src="https://img.shields.io/badge/Awesome-Flutter-blue.svg?longCache=true&style=for-the-badge" />
    </a>
    <a href="https://img.shields.io/badge/flutter-2.2-green" alt="Flutter">
        <img src="https://img.shields.io/badge/flutter-2.2-green?style=for-the-badge" /></a>
    <a href="https://img.shields.io/badge/dart-2.13-green" alt="Flutter">
        <img src="https://img.shields.io/badge/dart-2.13-green?style=for-the-badge" /></a>
  </p>
</p>

## Requerimientos del sistema Operativo MacOS 

Requisitos del sistema
Para instalar y ejecutar Flutter, tu entorno de desarrollo debe cumplir estos requisitos mínimos:

* Sistemas operativos: macOS, versión 10.14 (Mojave) o posterior.

* Espacio en disco: 2,8 GB (no incluye espacio en disco para IDE/herramientas).

* Herramientas: Flutter utiliza git para la instalación y actualización. Recomendamos instalar Xcode, que incluye git, pero también puedes instalar git por separado.



## Rosseta Software




<img src="https://github.com/antz22/ultimate-guide-to-flutter/blob/master/assets/container_style.png">

**Rosetta** es un traductor dinámico binario para Mac OS X que permite a muchas aplicaciones PowerPC correr en ciertas arquitecturas [Intel](https://es.wikipedia.org/wiki/X86 "X86") de las computadoras [Macintosh](https://es.wikipedia.org/wiki/Macintosh "Macintosh")
```bash
softwareupdate --install-rosetta
```
```bash
sudo softwareupdate --install-rosetta --agree-to-license
```

## Xcode command line tools



<img src="https://github.com/antz22/ultimate-guide-to-flutter/blob/master/assets/container_style.png">

Xcode es un entorno de desarrollo integrado para macOS que contiene un conjunto de herramientas creadas por Apple destinadas al desarrollo de software para macOS, iOS, watchOS y tvOS.


```bash
sudo Xcode-select --install
```
* Has clic en "Instalar" para comenzar el proceso de descarga e instalación.
* 

> https://mac.install.guide/assets/images/ruby/install-Xcode-CLT-done.png
* 


```bash
xcode-select -p
```

Verás un mensaje de confirmación cuando se complete la instalación.

Comprueba que haya instalado correctamente las herramientas de línea de comandos de Xcode:

```bash
xcode-select -p
```
* Deberías ver lo siguiente:


```bash
/Library/Developer/CommandLineTools
```



## Homebrew




<img src="https://github.com/antz22/ultimate-guide-to-flutter/blob/master/assets/container_style.png">

Homebrew es un sistema de gestión de paquetes que simplifica la instalación, actualización y eliminación de programas en los sistemas operativos Mac OS de Apple y GNU/Linux. Creado originalmente por Max Howell, el programa ha ganado popularidad en la comunidad de Ruby on Rails
```bash
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```
###  wget 
GNU Wget es una herramienta libre que permite la descarga de contenidos desde servidores web de una forma simple

```bash
brew install wget

```


###  curl

cURL es un proyecto de software consistente en una biblioteca y un intérprete de comandos orientado a la transferencia de archivos. Soporta los protocolos FTP, FTPS, HTTP, HTTPS, TFTP, SCP, SFTP, Telnet, DICT, FILE y LDAP, entre otros
```bash
brew install wget
```


###  git




GitHub es una forja para alojar proyectos utilizando el sistema de control de versiones Git. Se utiliza principalmente para la creación de código fuente de programas de ordenador. El software que opera GitHub fue escrito en Ruby on Rails. Desde enero de 2010, GitHub opera bajo el nombre de GitHub, Inc.

```bash
brew install git
```


* entre las comillas introducce tu nomebrew de usuario 
```bash
git config --global user.name "Tu nombre"
```

* introduce tu correo electronico
```bash 
git config --global user.email "Tu correo"
```


## Ruby



<img src="https://github.com/antz22/ultimate-guide-to-flutter/blob/master/assets/container_style.png">


RubyGems es un **gestor de paquetes** para el lenguaje de programación **Ruby** que proporciona un formato estándar y autocontenido (llamado gem) para poder distribuir programas o bibliotecas en **Ruby**, una herramienta destinada a gestionar la instalación de estos, y un servidor para su distribución.

--------
Instalacion *Ruby* by Homebrew  con el siguiente comando 

```bash 
brew install ruby
```


-------------
|RubyGems es un gestor de paquetes  | Extension  |
|--|--|
| Git  | [Git](https://github.com/rubygems/rubygems) |
| Gem  |[Gem](https://rubygems----------.org/gems/rubygems-update-3.4.13.gem)  |
|  Zip| [Zip](https://rubygems.org/rubygems/rubygems-3.4.13.zip) |
| Tgz | [Tgz](https://rubygems.org/rubygems/rubygems-3.4.13.tgz)
------------

* Despues de Descargar ell paquete el apquete y ejecutamos el siguiente comando en la terminal de macos  

```bash 
gem update --system
```



---- 


```bash 
gem update --system
```


Descomprimir en un directorio y cd allí y Instalación con: ruby setup.rb

```bash 
ruby setup.rb
```
Para más detalles y otras opciones, consulte:

```bash 
ruby setup.rb --help
```




### Git

GitHub es una forja para alojar proyectos utilizando el sistema de control de versiones Git. Se utiliza principalmente para la creación de código fuente de programas de ordenador. El software que opera GitHub fue escrito en Ruby on Rails. Desde enero de 2010, GitHub opera bajo el nombre de GitHub, Inc.

Once finished, run this command in the terminal to make sure your environment is all ready to go.


```bash
brew install git
rm '/usr/local/bin/git-cvsserver'
brew link --overwrite git
brew install git-lfs
git lfs install
```






### Cocopoads


Traducción del inglés-CocoaPods es un administrador de dependencias de nivel de aplicación para Objective-C, Swift y cualquier otro lenguaje que se ejecute en el tiempo de ejecución de Objective-C, como RubyMotion, que proporciona un formato estándar para administrar bibliotecas externas.

```bash
sudo gem install cocoapods

```



### watchmen


Requerimiento y utiltidada para poder desarollar software en apple watch  asi como interfases y apps 

```bash
brew install git
```






### Pod
Each widget built by Flutter can be passed a number of properties or parameters. As we saw earlier, the Container widget takes in a 'child' property, and it can also take in a 'color' property to define the background color of the Container.

Usually, you can also pass in all of your styles to the widget through the parameter.



### ffi 

Ruby-FFI es una gema para cargar mediante programación bibliotecas nativas enlazadas dinámicamente, enlazar funciones dentro de ellas y llamar a esas funciones desde código Ruby. Además, una extensión de Ruby-FFI funciona sin cambios en CRuby (MRI), JRuby, Rubinius y TruffleRub

```bash
gem install ffi
```

In Column widgets, you might need to vertically align your objects to the center of the page. Here's how you could do that using the Column widget's 'mainAxisAlignment' property (main axis of the column is vertical). You can also align text horizontally in a column widget using the 'crossAxisAlignment' property.



### Postman 

Traducción del inglés-Postman es una plataforma API para que los desarrolladores diseñen, construyan, prueben e iteren sus API. En febrero de 2023, Postman informa que tiene más de 25 millones de usuarios registrados y 75 000 API abiertas, lo que, según afirma, constituye el centro de API público más grande del mundo.
Usually, you can also pass in all of your styles to the widget through the parameter.


```bash
brew install --cask postman
```



## Flutter 

<img src="https://github.com/antz22/ultimate-guide-to-flutter/blob/master/assets/container_style.png">

Flutter es un SDK de código fuente abierto de desarrollo de aplicaciones móviles creado por Google. Suele usarse para desarrollar interfaces de usuario para aplicaciones en Android, iOS y Web así como método primario para crear aplicaciones para Google Fuchsia.​

### Obtenga el SDK de Flutter (1)
-------------
| Macos Flutter| SDK |
|--|--|
| Macos con procesador Intel   | [Intel](https://storage.googleapis.com/flutter_infra_release/releases/stable/macos/flutter_macos_3.10.1-stable.zip) |
|Macos con procesador Apple Silicon  |[Apple Silicon](https://storage.googleapis.com/flutter_infra_release/releases/stable/macos/flutter_macos_arm64_3.10.1-stable.zipp)  |

------------

2. Extrae el archivo descargado:
   - Navega a la ubicación donde se descargó el archivo y ábrelo.
   - Extrae el contenido del archivo comprimido en la ubicación que prefieras, por ejemplo, en tu directorio de inicio.

```bash
cd ~/development
unzip ~/Downloads/flutter_macos_3.10.1-stable.zip
```
3. Configura las variables de entorno:
   - Abre una terminal.
   - Ejecuta el siguiente comando para abrir el archivo de perfil de tu terminal en un editor de texto:


```bash

export PATH="$PATH:`pwd`/flutter/bin"

```

   - Agrega las siguientes líneas al archivo y guarda los cambios:

```bash
 export PATH="$PATH:[RUTA_DE_FLUTTER]/bin"
     
```

```bash
export PATH="$PATH:[RUTA_DE_FLUTTER]/bin/cache/dart-sdk/bin"
```
 - Reemplaza "[RUTA_DE_FLUTTER]" con la ruta donde extrajiste el archivo de Flutter.
 
  - Cierra y vuelve a abrir la terminal para que los cambios surtan efecto.


4. Verifica la instalación de Flutter:
   - Ejecuta el siguiente comando para verificar si Flutter se instaló correctamente:


```bash
flutter doctor
```

### Git repo install  (2)


 - Deberías ver una lista de verificaciones con el estado actual de tu configuración. Si hay algún problema, te mostrará los pasos necesarios para solucionarlo.
Descargar directamente desde GitHub en lugar de utilizar un archivo comprimido
Esto sólo se sugiere para casos de uso avanzado.

También puedes usar git directamente en lugar de descargar el archivo preparado. Por ejemplo, para descargar la rama estable:

content_copy

```bash
 git clone https://github.com/flutter/flutter.git -b estable
```

```bash
flutter precache
```

Actualiza tu ruta, y ejecuta flutter doctor
. Eso te permitirá saber si hay otras dependencias que necesites instalar para usar Flutter (por ejemplo, el SDK de Android).

Si no has utilizado el archivo, Flutter descargará los binarios de desarrollo necesarios a medida que se vayan necesitando (si has utilizado el archivo, están incluidos en la descarga). Es posible que desee descargar previamente estos binarios de desarrollo (por ejemplo, es posible que desee hacer esto al configurar entornos de compilación herméticos, o si sólo tiene disponibilidad de red intermitente). Para ello, ejecute el siguiente comando


```bash
 flutter precache
```

Para más opciones de descarga, consulte la ayuda de flutter precache.

### Xcode setup 

5. En caso de no tener instalado el IDE editor de codigo   Xcode:
   - Abre la Mac App Store.
   - Busca "Xcode" y haz clic en el botón "Obtener" para instalarlo.
   - Sigue las instrucciones en pantalla para completar la instalación.
  

5.1 . Otra manera de hacer la instalacion de Xcode en caso de tenener  una version del sistema operativo macos antigua o verisones anteriores no soportadas por la Appstore puede descargar el IDE  desde la  terminal de  comandos  abriendolo y ejecutando como super usuario  el siguiente comando para poder realizar la descarga 


```bash
 flutter precache
```


6.  Para desarrollar aplicaciones Flutter para iOS, necesitas un Mac con Xcode instalado.Configura Xcode:
   - Abre Xcode.
   - Ve a "Preferencias" en el menú "Xcode".
   - Haz clic en la pestaña "Ubicaciones" y selecciona la versión más reciente de Xcode en "Command Line Tools".

```bash
 sudo xcode-select --switch /Applications/Xcode.app/Contents/Developer
```
```bash
 sudo xcodebuild -runFirstLaunch
```

### Configurar el simulador iOS 

Para prepararte para ejecutar y probar tu aplicación Flutter en el simulador de iOS, sigue estos pasos:

En tu Mac, busca el simulador a través de Spotlight o utilizando el siguiente comando:

```bash
 open -a Simulador
```
Asegúrese de que el simulador utiliza un dispositivo de 64 bits (iPhone 5s o posterior). Puede comprobar el dispositivo consultando la configuración en los menús Hardware > Dispositivo o Archivo > Abrir simulador del simulador.
Dependiendo del tamaño de la pantalla de tu máquina de desarrollo, los dispositivos iOS simulados con alta densidad de pantalla podrían desbordar tu pantalla. Coge la esquina del simulador y arrástrala para cambiar la escala. También puedes utilizar las opciones Ventana > Tamaño físico o Ventana > Precisión de píxeles si la resolución de tu ordenador es lo suficientemente alta.

### Implantar en dispositivos iOS


Puede omitir este paso si sus aplicaciones no dependen de plugins de Flutter con código nativo de iOS. Instale y configure CocoaPods ejecutando los siguientes comandos:



```bash
 sudo gem install cocoapods

```
 Nota: La versión por defecto de Ruby requiere sudo para instalar la gema CocoaPods. Si está utilizando un gestor de versiones de Ruby, es posible que tenga que ejecutar sin sudo.

Además, si está instalando en un Mac Apple Silicon, ejecute el comando

```bash
 sudo gem install cocoapods

```

Puede omitir este paso si sus aplicaciones no dependen de plugins de Flutter con código nativo de iOS. Instale y configure CocoaPods ejecutando los siguientes comandos:



 Nota: La versión por defecto de Ruby requiere sudo para instalar la gema CocoaPods. Si está utilizando un gestor de versiones de Ruby, es posible que tenga que ejecutar sin sudo.

Además, si está instalando en un Mac Apple Silicon, ejecute el comando

content_copy
 sudo gem uninstall ffi && sudo gem install ffi -- --enable-libffi-alloc
Siga el flujo de firma de Xcode para aprovisionar su proyecto:

```bash
 sudo gem uninstall ffi && sudo gem install ffi -- --enable-libffi-alloc
```
 
Siga el flujo de firma de Xcode para aprovisionar su proyecto:


¡Listo! Ahora tienes Flutter completamente instalado en tu macOS. Puedes comenzar a desarrollar aplicaciones Flutter en tu máquina. Recuerda mantener Flutter y sus dependencias actualizadas periódicamente ejecutando el comando "flutter upgrade" en la terminal. ¡Disfruta de tu experiencia de desarrollo con Flutter!




s







## Dart 

Dart es un lenguaje de programación de código abierto, desarrollado por Google. Fue revelado en la conferencia goto; en Aarhus, Dinamarca el 10 de octubre de 2011




## Vizual Code

### Brew install 

```bash
brew install vscode 

```



Visual Studio Code es un editor de código fuente desarrollado por Microsoft para Windows, Linux, macOS y Web. Incluye soporte para la depuración, control integrado de Git, resaltado de sintaxis, finalización inteligente de código, fragmentos y refactorización de código.

### Extensiones 

La extensión Visual Studio Code **habilita una opción de versión preliminar en directo para ver la página de contenido de los portales dentro de la interfaz de Visual Studio Code durante la experiencia de desarrollo**. en la parte superior derecha cuando se abre un archivo HTML en modo de edición.. 


### Setup & Config

We can use a StreamBuilder for this purpose. A 'Stream' is essentially just a stream of data that we are constantly watching for changes in. One end of the stream is the Firestore database. The other end of the stream is our app. 



## Android Studio 

Descargar Android Studio

Abra cualquier navegador web y vaya a la página de descarga de Android Studio. Esta es la página web de Android Developers, donde puedes descargar Android Studio. Esta página detecta automáticamente su sistema operativo.
Haga clic en Descargar Android Studio. Se abrirá la página de Términos y Condiciones con el Acuerdo de Licencia de Android Studio.
Lea el Acuerdo de licencia.
En la parte inferior de la página, si está de acuerdo con los términos y condiciones, seleccione la casilla de verificación He leído y acepto los términos y condiciones anteriores.
Haz clic en Descargar Android Studio para iniciar la descarga.
Cuando se le solicite, guarde el archivo en una ubicación donde pueda localizarlo fácilmente, como la carpeta Descargas.
Espera a que se complete la descarga. Esto puede llevar un rato y puede ser un buen momento para disfrutar de un té.


Inicie el archivo DMG de Android Studio.
Arrastre y suelte Android Studio en la carpeta Aplicaciones y, a continuación, inicie Android Studio.
Elija si desea importar la configuración anterior de Android Studio y, a continuación, haga clic en Aceptar.
Complete el asistente de configuración de Android Studio, que incluye la descarga de los componentes del SDK de Android necesarios para el desarrollo.
El siguiente vídeo muestra cada paso del procedimiento de configuración recomendado:

A medida que estén disponibles nuevas herramientas y otras API, Android Studio le notificará mediante una ventana emergente. Para comprobar manualmente si hay actualizaciones, haga clic en Android Studio > Buscar actualizaciones.
