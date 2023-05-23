<p align="middle">
  <a href="https://github.com/antz22/ultimate-guide-to-flutter"><img src="https://github.com/antz22/ultimate-guide-to-flutter/blob/master/assets/banner.svg"></a>
</p>
<p align="center">
  </p><h2 align="center">MacOS  - Flutter</h2>
<p></p>  <p align="center">
   Guia completa de instalacion en el sistema operativo MacOS 
  </p>
  <p align="center">
    <a href="https://github.com/antz22/ultimate-guide-to-flutter/stargazers" alt="Stars">
        <img src="https://img.shields.io/github/stars/antz22/ultimate-guide-to-flutter?style=for-the-badge"></a>
    <a href="https://github.com/antz22/ultimate-guide-to-flutter/network/members" alt="Forks">
        <img src="https://img.shields.io/github/forks/antz22/ultimate-guide-to-flutter?style=for-the-badge"></a>
    <a href="https://github.com/Solido/awesome-flutter">
        <img alt="Awesome Flutter" src="https://img.shields.io/badge/Awesome-Flutter-blue.svg?longCache=true&amp;style=for-the-badge">
    </a>
    <a href="https://img.shields.io/badge/flutter-2.2-green" alt="Flutter">
        <img src="https://img.shields.io/badge/flutter-2.2-green?style=for-the-badge"></a>
    <a href="https://img.shields.io/badge/dart-2.13-green" alt="Flutter">
        <img src="https://img.shields.io/badge/dart-2.13-green?style=for-the-badge"></a>
  </p>

<h2 id="requerimientos-del-sistema-operativo-macos">Requerimientos del sistema Operativo MacOS</h2>
<p>Requisitos del sistema<br>
Para instalar y ejecutar Flutter, tu entorno de desarrollo debe cumplir estos requisitos mínimos:</p>
<ul>
<li>
<p>Sistemas operativos: macOS, versión 10.14 (Mojave) o posterior.</p>
</li>
<li>
<p>Espacio en disco: 2,8 GB (no incluye espacio en disco para IDE/herramientas).</p>
</li>
<li>
<p>Herramientas: Flutter utiliza git para la instalación y actualización. Recomendamos instalar Xcode, que incluye git, pero también puedes instalar git por separado.</p>
</li>
</ul>

<h2  align="center"  id="rosseta-software">Rosseta Software <img src="https://cdn.iconscout.com/icon/free/png-256/free-rubygems-283026.png?f=webp" alt="align" width="40" height="40" href="https://cdn.iconscout.com/icon/free/png-256/free-rubygems-283026.png?f=webp"/></h2>

<p><strong>Rosetta</strong> es un traductor dinámico binario para Mac OS X que permite a muchas aplicaciones PowerPC correr en ciertas arquitecturas <a href="https://es.wikipedia.org/wiki/X86" title="X86">Intel</a> de las computadoras <a href="https://es.wikipedia.org/wiki/Macintosh" title="Macintosh">Macintosh</a></p>
<pre class=" language-bash"><code class="prism  language-bash">softwareupdate --install-rosetta
</code></pre>
<pre class=" language-bash"><code class="prism  language-bash"><span class="token function">sudo</span> softwareupdate --install-rosetta --agree-to-license
</code></pre>
<h2 id="xcode-command-line-tools">Xcode command line tools</h2>
<img src="https://github.com/antz22/ultimate-guide-to-flutter/blob/master/assets/container_style.png">
<p>Xcode es un entorno de desarrollo integrado para macOS que contiene un conjunto de herramientas creadas por Apple destinadas al desarrollo de software para macOS, iOS, watchOS y tvOS.</p>
<pre class=" language-bash"><code class="prism  language-bash"><span class="token function">sudo</span> Xcode-select --install
</code></pre>
<ul>
<li>Has clic en “Instalar” para comenzar el proceso de descarga e instalación.</li>
<li></li>
</ul>
<blockquote>
<p><a href="https://mac.install.guide/assets/images/ruby/install-Xcode-CLT-done.png">https://mac.install.guide/assets/images/ruby/install-Xcode-CLT-done.png</a></p>
</blockquote>
<ul>
<li></li>
</ul>
<pre class=" language-bash"><code class="prism  language-bash">xcode-select -p
</code></pre>
<p>Verás un mensaje de confirmación cuando se complete la instalación.</p>
<p>Comprueba que haya instalado correctamente las herramientas de línea de comandos de Xcode:</p>
<pre class=" language-bash"><code class="prism  language-bash">xcode-select -p
</code></pre>
<ul>
<li>Deberías ver lo siguiente:</li>
</ul>
<pre class=" language-bash"><code class="prism  language-bash">/Library/Developer/CommandLineTools
</code></pre>
<h2 id="homebrew">Homebrew</h2><a href="https://iconscout.com/icons/rubygems" target="_blank">Free Rubygems Icon</a> by <a href="https://iconscout.com/contributors/jagathish">Jagathish Saravanan</a> on <a href="https://iconscout.com">IconScout</a>

<img src="https://github.com/antz22/ultimate-guide-to-flutter/blob/master/assets/container_style.png">
<p>Homebrew es un sistema de gestión de paquetes que simplifica la instalación, actualización y eliminación de programas en los sistemas operativos Mac OS de Apple y GNU/Linux. Creado originalmente por Max Howell, el programa ha ganado popularidad en la comunidad de Ruby on Rails</p>
<pre class=" language-bash"><code class="prism  language-bash">/bin/bash -c <span class="token string">"<span class="token variable"><span class="token variable">$(</span>curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh<span class="token variable">)</span></span>"</span>
</code></pre>
<h3 id="wget">wget</h3>
<p>GNU Wget es una herramienta libre que permite la descarga de contenidos desde servidores web de una forma simple</p>
<pre class=" language-bash"><code class="prism  language-bash">brew <span class="token function">install</span> <span class="token function">wget</span>

</code></pre>
<h3 id="curl">curl</h3>
<p>cURL es un proyecto de software consistente en una biblioteca y un intérprete de comandos orientado a la transferencia de archivos. Soporta los protocolos FTP, FTPS, HTTP, HTTPS, TFTP, SCP, SFTP, Telnet, DICT, FILE y LDAP, entre otros</p>
<pre class=" language-bash"><code class="prism  language-bash">brew <span class="token function">install</span> <span class="token function">wget</span>
</code></pre>
<h3 id="git">git</h3>
<p>GitHub es una forja para alojar proyectos utilizando el sistema de control de versiones Git. Se utiliza principalmente para la creación de código fuente de programas de ordenador. El software que opera GitHub fue escrito en Ruby on Rails. Desde enero de 2010, GitHub opera bajo el nombre de GitHub, Inc.</p>
<pre class=" language-bash"><code class="prism  language-bash">brew <span class="token function">install</span> <span class="token function">git</span>
</code></pre>
<ul>
<li>entre las comillas introducce tu nomebrew de usuario</li>
</ul>
<pre class=" language-bash"><code class="prism  language-bash"><span class="token function">git</span> config --global user.name <span class="token string">"Tu nombre"</span>
</code></pre>
<ul>
<li>introduce tu correo electronico</li>
</ul>
<pre class=" language-bash"><code class="prism  language-bash"><span class="token function">git</span> config --global user.email <span class="token string">"Tu correo"</span>
</code></pre>
<h2 id="ruby">Ruby</h2>
<img src="https://github.com/antz22/ultimate-guide-to-flutter/blob/master/assets/container_style.png">
<p>RubyGems es un <strong>gestor de paquetes</strong> para el lenguaje de programación <strong>Ruby</strong> que proporciona un formato estándar y autocontenido (llamado gem) para poder distribuir programas o bibliotecas en <strong>Ruby</strong>, una herramienta destinada a gestionar la instalación de estos, y un servidor para su distribución.</p>
<hr>
<p>Instalacion <em>Ruby</em> by Homebrew  con el siguiente comando</p>
<pre class=" language-bash"><code class="prism  language-bash">brew <span class="token function">install</span> ruby
</code></pre>
<hr>

<table>
<thead>
<tr>
<th>RubyGems es un gestor de paquetes</th>
<th>Extension</th>
</tr>
</thead>
<tbody>
<tr>
<td>Git</td>
<td><a href="https://github.com/rubygems/rubygems">Git</a></td>
</tr>
<tr>
<td>Gem</td>
<td><a href="https://rubygems----------.org/gems/rubygems-update-3.4.13.gem">Gem</a></td>
</tr>
<tr>
<td>Zip</td>
<td><a href="https://rubygems.org/rubygems/rubygems-3.4.13.zip">Zip</a></td>
</tr>
<tr>
<td>Tgz</td>
<td><a href="https://rubygems.org/rubygems/rubygems-3.4.13.tgz">Tgz</a></td>
</tr>
</tbody>
</table><hr>
<ul>
<li>Despues de Descargar ell paquete el apquete y ejecutamos el siguiente comando en la terminal de macos</li>
</ul>
<pre class=" language-bash"><code class="prism  language-bash">gem update --system
</code></pre>
<hr>
<pre class=" language-bash"><code class="prism  language-bash">gem update --system
</code></pre>
<p>Descomprimir en un directorio y cd allí y Instalación con: ruby setup.rb</p>
<pre class=" language-bash"><code class="prism  language-bash">ruby setup.rb
</code></pre>
<p>Para más detalles y otras opciones, consulte:</p>
<pre class=" language-bash"><code class="prism  language-bash">ruby setup.rb --help
</code></pre>
<h3 id="git-1">Git</h3>
<p>GitHub es una forja para alojar proyectos utilizando el sistema de control de versiones Git. Se utiliza principalmente para la creación de código fuente de programas de ordenador. El software que opera GitHub fue escrito en Ruby on Rails. Desde enero de 2010, GitHub opera bajo el nombre de GitHub, Inc.</p>
<p>Once finished, run this command in the terminal to make sure your environment is all ready to go.</p>
<pre class=" language-bash"><code class="prism  language-bash">brew <span class="token function">install</span> <span class="token function">git</span>
<span class="token function">rm</span> <span class="token string">'/usr/local/bin/git-cvsserver'</span>
brew <span class="token function">link</span> --overwrite <span class="token function">git</span>
brew <span class="token function">install</span> git-lfs
<span class="token function">git</span> lfs <span class="token function">install</span>
</code></pre>
<h3 id="cocopoads">Cocopoads</h3>
<p>Traducción del inglés-CocoaPods es un administrador de dependencias de nivel de aplicación para Objective-C, Swift y cualquier otro lenguaje que se ejecute en el tiempo de ejecución de Objective-C, como RubyMotion, que proporciona un formato estándar para administrar bibliotecas externas.</p>
<pre class=" language-bash"><code class="prism  language-bash"><span class="token function">sudo</span> gem <span class="token function">install</span> cocoapods

</code></pre>
<h3 id="watchmen">watchmen</h3>
<p>Requerimiento y utiltidada para poder desarollar software en apple watch  asi como interfases y apps</p>
<pre class=" language-bash"><code class="prism  language-bash">brew <span class="token function">install</span> <span class="token function">git</span>
</code></pre>
<h3 id="pod">Pod</h3>
<p>Each widget built by Flutter can be passed a number of properties or parameters. As we saw earlier, the Container widget takes in a ‘child’ property, and it can also take in a ‘color’ property to define the background color of the Container.</p>
<p>Usually, you can also pass in all of your styles to the widget through the parameter.</p>
<h3 id="ffi">ffi</h3>
<p>Ruby-FFI es una gema para cargar mediante programación bibliotecas nativas enlazadas dinámicamente, enlazar funciones dentro de ellas y llamar a esas funciones desde código Ruby. Además, una extensión de Ruby-FFI funciona sin cambios en CRuby (MRI), JRuby, Rubinius y TruffleRub</p>
<pre class=" language-bash"><code class="prism  language-bash">gem <span class="token function">install</span> ffi
</code></pre>
<p>In Column widgets, you might need to vertically align your objects to the center of the page. Here’s how you could do that using the Column widget’s ‘mainAxisAlignment’ property (main axis of the column is vertical). You can also align text horizontally in a column widget using the ‘crossAxisAlignment’ property.</p>
<h3 id="postman">Postman</h3>
<p>Traducción del inglés-Postman es una plataforma API para que los desarrolladores diseñen, construyan, prueben e iteren sus API. En febrero de 2023, Postman informa que tiene más de 25 millones de usuarios registrados y 75 000 API abiertas, lo que, según afirma, constituye el centro de API público más grande del mundo.<br>
Usually, you can also pass in all of your styles to the widget through the parameter.</p>
<pre class=" language-bash"><code class="prism  language-bash">brew <span class="token function">install</span> --cask postman
</code></pre>
<h2 id="flutter">Flutter</h2>
<img src="https://github.com/antz22/ultimate-guide-to-flutter/blob/master/assets/container_style.png">
<p>Flutter es un SDK de código fuente abierto de desarrollo de aplicaciones móviles creado por Google. Suele usarse para desarrollar interfaces de usuario para aplicaciones en Android, iOS y Web así como método primario para crear aplicaciones para Google Fuchsia.​</p>
<h3 id="obtenga-el-sdk-de-flutter-1">Obtenga el SDK de Flutter (1)</h3>
<hr>

<table>
<thead>
<tr>
<th>Macos Flutter</th>
<th>SDK</th>
</tr>
</thead>
<tbody>
<tr>
<td>Macos con procesador Intel</td>
<td><a href="https://storage.googleapis.com/flutter_infra_release/releases/stable/macos/flutter_macos_3.10.1-stable.zip">Intel</a></td>
</tr>
<tr>
<td>Macos con procesador Apple Silicon</td>
<td><a href="https://storage.googleapis.com/flutter_infra_release/releases/stable/macos/flutter_macos_arm64_3.10.1-stable.zipp">Apple Silicon</a></td>
</tr>
</tbody>
</table><hr>
<ol start="2">
<li>Extrae el archivo descargado:
<ul>
<li>Navega a la ubicación donde se descargó el archivo y ábrelo.</li>
<li>Extrae el contenido del archivo comprimido en la ubicación que prefieras, por ejemplo, en tu directorio de inicio.</li>
</ul>
</li>
</ol>
<pre class=" language-bash"><code class="prism  language-bash"><span class="token function">cd</span> ~/development
unzip ~/Downloads/flutter_macos_3.10.1-stable.zip
</code></pre>
<ol start="3">
<li>Configura las variables de entorno:
<ul>
<li>Abre una terminal.</li>
<li>Ejecuta el siguiente comando para abrir el archivo de perfil de tu terminal en un editor de texto:</li>
</ul>
</li>
</ol>
<pre class=" language-bash"><code class="prism  language-bash">
<span class="token function">export</span> PATH<span class="token operator">=</span><span class="token string">"<span class="token variable">$PATH</span>:<span class="token variable"><span class="token variable">`</span><span class="token function">pwd</span><span class="token variable">`</span></span>/flutter/bin"</span>

</code></pre>
<ul>
<li>Agrega las siguientes líneas al archivo y guarda los cambios:</li>
</ul>
<pre class=" language-bash"><code class="prism  language-bash"> <span class="token function">export</span> PATH<span class="token operator">=</span><span class="token string">"<span class="token variable">$PATH</span>:[RUTA_DE_FLUTTER]/bin"</span>
     
</code></pre>
<pre class=" language-bash"><code class="prism  language-bash"><span class="token function">export</span> PATH<span class="token operator">=</span><span class="token string">"<span class="token variable">$PATH</span>:[RUTA_DE_FLUTTER]/bin/cache/dart-sdk/bin"</span>
</code></pre>
<ul>
<li>
<p>Reemplaza “[RUTA_DE_FLUTTER]” con la ruta donde extrajiste el archivo de Flutter.</p>
</li>
<li>
<p>Cierra y vuelve a abrir la terminal para que los cambios surtan efecto.</p>
</li>
</ul>
<ol start="4">
<li>Verifica la instalación de Flutter:
<ul>
<li>Ejecuta el siguiente comando para verificar si Flutter se instaló correctamente:</li>
</ul>
</li>
</ol>
<pre class=" language-bash"><code class="prism  language-bash">flutter doctor
</code></pre>
<h3 id="git-repo-install--2">Git repo install  (2)</h3>
<ul>
<li>Deberías ver una lista de verificaciones con el estado actual de tu configuración. Si hay algún problema, te mostrará los pasos necesarios para solucionarlo.<br>
Descargar directamente desde GitHub en lugar de utilizar un archivo comprimido<br>
Esto sólo se sugiere para casos de uso avanzado.</li>
</ul>
<p>También puedes usar git directamente en lugar de descargar el archivo preparado. Por ejemplo, para descargar la rama estable:</p>
<p>content_copy</p>
<pre class=" language-bash"><code class="prism  language-bash"> <span class="token function">git</span> clone https://github.com/flutter/flutter.git -b estable
</code></pre>
<pre class=" language-bash"><code class="prism  language-bash">flutter precache
</code></pre>
<p>Actualiza tu ruta, y ejecuta flutter doctor<br>
. Eso te permitirá saber si hay otras dependencias que necesites instalar para usar Flutter (por ejemplo, el SDK de Android).</p>
<p>Si no has utilizado el archivo, Flutter descargará los binarios de desarrollo necesarios a medida que se vayan necesitando (si has utilizado el archivo, están incluidos en la descarga). Es posible que desee descargar previamente estos binarios de desarrollo (por ejemplo, es posible que desee hacer esto al configurar entornos de compilación herméticos, o si sólo tiene disponibilidad de red intermitente). Para ello, ejecute el siguiente comando</p>
<pre class=" language-bash"><code class="prism  language-bash"> flutter precache
</code></pre>
<p>Para más opciones de descarga, consulte la ayuda de flutter precache.</p>
<h3 id="xcode-setup">Xcode setup</h3>
<ol start="5">
<li>En caso de no tener instalado el IDE editor de codigo   Xcode:
<ul>
<li>Abre la Mac App Store.</li>
<li>Busca “Xcode” y haz clic en el botón “Obtener” para instalarlo.</li>
<li>Sigue las instrucciones en pantalla para completar la instalación.</li>
</ul>
</li>
</ol>
<p>5.1 . Otra manera de hacer la instalacion de Xcode en caso de tenener  una version del sistema operativo macos antigua o verisones anteriores no soportadas por la Appstore puede descargar el IDE  desde la  terminal de  comandos  abriendolo y ejecutando como super usuario  el siguiente comando para poder realizar la descarga</p>
<pre class=" language-bash"><code class="prism  language-bash"> flutter precache
</code></pre>
<ol start="6">
<li>Para desarrollar aplicaciones Flutter para iOS, necesitas un Mac con Xcode instalado.Configura Xcode:</li>
</ol>
<ul>
<li>Abre Xcode.</li>
<li>Ve a “Preferencias” en el menú “Xcode”.</li>
<li>Haz clic en la pestaña “Ubicaciones” y selecciona la versión más reciente de Xcode en “Command Line Tools”.</li>
</ul>
<pre class=" language-bash"><code class="prism  language-bash"> <span class="token function">sudo</span> xcode-select --switch /Applications/Xcode.app/Contents/Developer
</code></pre>
<pre class=" language-bash"><code class="prism  language-bash"> <span class="token function">sudo</span> xcodebuild -runFirstLaunch
</code></pre>
<h3 id="configurar-el-simulador-ios">Configurar el simulador iOS</h3>
<p>Para prepararte para ejecutar y probar tu aplicación Flutter en el simulador de iOS, sigue estos pasos:</p>
<p>En tu Mac, busca el simulador a través de Spotlight o utilizando el siguiente comando:</p>
<pre class=" language-bash"><code class="prism  language-bash"> <span class="token function">open</span> -a Simulador
</code></pre>
<p>Asegúrese de que el simulador utiliza un dispositivo de 64 bits (iPhone 5s o posterior). Puede comprobar el dispositivo consultando la configuración en los menús Hardware &gt; Dispositivo o Archivo &gt; Abrir simulador del simulador.<br>
Dependiendo del tamaño de la pantalla de tu máquina de desarrollo, los dispositivos iOS simulados con alta densidad de pantalla podrían desbordar tu pantalla. Coge la esquina del simulador y arrástrala para cambiar la escala. También puedes utilizar las opciones Ventana &gt; Tamaño físico o Ventana &gt; Precisión de píxeles si la resolución de tu ordenador es lo suficientemente alta.</p>
<h3 id="implantar-en-dispositivos-ios">Implantar en dispositivos iOS</h3>
<p>Puede omitir este paso si sus aplicaciones no dependen de plugins de Flutter con código nativo de iOS. Instale y configure CocoaPods ejecutando los siguientes comandos:</p>
<pre class=" language-bash"><code class="prism  language-bash"> <span class="token function">sudo</span> gem <span class="token function">install</span> cocoapods

</code></pre>
<p>Nota: La versión por defecto de Ruby requiere sudo para instalar la gema CocoaPods. Si está utilizando un gestor de versiones de Ruby, es posible que tenga que ejecutar sin sudo.</p>
<p>Además, si está instalando en un Mac Apple Silicon, ejecute el comando</p>
<pre class=" language-bash"><code class="prism  language-bash"> <span class="token function">sudo</span> gem <span class="token function">install</span> cocoapods

</code></pre>
<p>Puede omitir este paso si sus aplicaciones no dependen de plugins de Flutter con código nativo de iOS. Instale y configure CocoaPods ejecutando los siguientes comandos:</p>
<p>Nota: La versión por defecto de Ruby requiere sudo para instalar la gema CocoaPods. Si está utilizando un gestor de versiones de Ruby, es posible que tenga que ejecutar sin sudo.</p>
<p>Además, si está instalando en un Mac Apple Silicon, ejecute el comando</p>
<p>content_copy<br>
sudo gem uninstall ffi &amp;&amp; sudo gem install ffi – --enable-libffi-alloc<br>
Siga el flujo de firma de Xcode para aprovisionar su proyecto:</p>
<pre class=" language-bash"><code class="prism  language-bash"> <span class="token function">sudo</span> gem uninstall ffi <span class="token operator">&amp;&amp;</span> <span class="token function">sudo</span> gem <span class="token function">install</span> ffi -- --enable-libffi-alloc
</code></pre>
<p>Siga el flujo de firma de Xcode para aprovisionar su proyecto:</p>
<p>¡Listo! Ahora tienes Flutter completamente instalado en tu macOS. Puedes comenzar a desarrollar aplicaciones Flutter en tu máquina. Recuerda mantener Flutter y sus dependencias actualizadas periódicamente ejecutando el comando “flutter upgrade” en la terminal. ¡Disfruta de tu experiencia de desarrollo con Flutter!</p>
<p>s</p>
<h2 id="dart">Dart</h2>
<p>Dart es un lenguaje de programación de código abierto, desarrollado por Google. Fue revelado en la conferencia goto; en Aarhus, Dinamarca el 10 de octubre de 2011</p>
<h2 id="vizual-code">Vizual Code</h2>
<h3 id="brew-install">Brew install</h3>
<pre class=" language-bash"><code class="prism  language-bash">brew <span class="token function">install</span> vscode 

</code></pre>
<p>Visual Studio Code es un editor de código fuente desarrollado por Microsoft para Windows, Linux, macOS y Web. Incluye soporte para la depuración, control integrado de Git, resaltado de sintaxis, finalización inteligente de código, fragmentos y refactorización de código.</p>
<h3 id="extensiones">Extensiones</h3>
<p>La extensión Visual Studio Code <strong>habilita una opción de versión preliminar en directo para ver la página de contenido de los portales dentro de la interfaz de Visual Studio Code durante la experiencia de desarrollo</strong>. en la parte superior derecha cuando se abre un archivo HTML en modo de edición…</p>
<h3 id="setup--config">Setup &amp; Config</h3>
<p>We can use a StreamBuilder for this purpose. A ‘Stream’ is essentially just a stream of data that we are constantly watching for changes in. One end of the stream is the Firestore database. The other end of the stream is our app.</p>
<h2 id="android-studio">Android Studio</h2>
<p>Descargar Android Studio</p>
<p>Abra cualquier navegador web y vaya a la página de descarga de Android Studio. Esta es la página web de Android Developers, donde puedes descargar Android Studio. Esta página detecta automáticamente su sistema operativo.<br>
Haga clic en Descargar Android Studio. Se abrirá la página de Términos y Condiciones con el Acuerdo de Licencia de Android Studio.<br>
Lea el Acuerdo de licencia.<br>
En la parte inferior de la página, si está de acuerdo con los términos y condiciones, seleccione la casilla de verificación He leído y acepto los términos y condiciones anteriores.<br>
Haz clic en Descargar Android Studio para iniciar la descarga.<br>
Cuando se le solicite, guarde el archivo en una ubicación donde pueda localizarlo fácilmente, como la carpeta Descargas.<br>
Espera a que se complete la descarga. Esto puede llevar un rato y puede ser un buen momento para disfrutar de un té.</p>
<p>Inicie el archivo DMG de Android Studio.<br>
Arrastre y suelte Android Studio en la carpeta Aplicaciones y, a continuación, inicie Android Studio.<br>
Elija si desea importar la configuración anterior de Android Studio y, a continuación, haga clic en Aceptar.<br>
Complete el asistente de configuración de Android Studio, que incluye la descarga de los componentes del SDK de Android necesarios para el desarrollo.<br>
El siguiente vídeo muestra cada paso del procedimiento de configuración recomendado:</p>
<p>A medida que estén disponibles nuevas herramientas y otras API, Android Studio le notificará mediante una ventana emergente. Para comprobar manualmente si hay actualizaciones, haga clic en Android Studio &gt; Buscar actualizaciones.</p>

