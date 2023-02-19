# AndroidStudio With Java

Aprende a desarrollar en AndroidStudio con Java

## Este documento

Los conceptos en este archivo explicados fueron generados mediante inteligencia artificial, cada vez la inteligencia artificial agiliza procesos, no solo mecanicos y automatizables en la industria de la produccion si no tambien en los procesos de creacion, diseño y aprendizaje

## Estructura del proyecto

- Carpeta "app": La carpeta "app" es la principal en el proyecto de Android, y contiene todo lo que necesitas para construir la aplicación en sí. Aquí es donde encontrarás los archivos de código fuente, los recursos, las configuraciones de compilación, los manifestos y otros componentes de la aplicación.

- Carpeta "src": La carpeta "src" es donde se encuentra todo el código fuente de la aplicación. Dentro de esta carpeta, encontrarás las carpetas "main" y "test". La carpeta "main" contiene el código fuente y los recursos que se utilizan en la versión principal de la aplicación, mientras que la carpeta "test" contiene los archivos de prueba para la aplicación.

- Carpeta "res": La carpeta "res" contiene todos los recursos necesarios para la aplicación, como diseños de interfaz de usuario, imágenes, iconos, archivos de audio y otros recursos.

- Carpeta "build": La carpeta "build" es donde se generan los archivos de compilación y donde se almacenan los archivos temporales. No se recomienda modificar nada en esta carpeta manualmente, ya que podría provocar problemas en la aplicación.

- Carpeta "gradle": La carpeta "gradle" contiene los archivos de configuración de Gradle, que es una herramienta de construcción de proyectos que se utiliza en Android Studio.

- Archivo "AndroidManifest.xml": Este archivo describe la información básica de la aplicación, como el nombre de la aplicación, el nombre del paquete, los permisos necesarios para la aplicación, etc.

- Archivo "build.gradle": Este archivo contiene las configuraciones de construcción de la aplicación, como las dependencias, la versión del SDK de Android y la versión de la aplicación.

- Carpeta "app/libs": Esta carpeta contiene las bibliotecas de terceros que se utilizan en la aplicación.

## Ciclo de vida de una activity

1. onCreate(): Esta es la primera etapa del ciclo de vida de un Activity. Se llama cuando se crea una instancia del Activity y se utiliza para realizar cualquier configuración inicial, como la creación de una interfaz de usuario y la inicialización de variables.

2. onStart(): Esta etapa se llama después de onCreate() y se utiliza para preparar el Activity para que sea visible al usuario.

3. onResume(): Esta etapa se llama después de onStart() y se utiliza para iniciar la interacción del usuario con el Activity. Es en esta etapa en la que el Activity se vuelve visible y activo.

4. onPause(): Esta etapa se llama cuando el Activity pierde el foco, por ejemplo, cuando el usuario cambia a otra aplicación o a otra pantalla. En esta etapa, se detiene la interacción del usuario con el Activity.

5. onStop(): Esta etapa se llama cuando el Activity se vuelve invisible para el usuario. En esta etapa, el Activity aún existe, pero ya no es visible.

6. onRestart(): Esta etapa se llama cuando el Activity se reinicia después de haber sido detenido. En esta etapa, el Activity se prepara para volver a ser visible.

7. onDestroy(): Esta es la última etapa del ciclo de vida de un Activity. Se llama cuando el Activity se destruye y se utiliza para liberar recursos, cerrar conexiones y limpiar el estado del Activity.

## Elementos de la UI

- Layouts: Los layouts son contenedores que se utilizan para organizar los elementos de la UI en una pantalla. En Android, existen varios tipos de layouts, como LinearLayout, RelativeLayout, GridLayout, entre otros. Cada tipo de layout tiene su propio comportamiento y se utiliza para diferentes propósitos.

- Views: Las views son elementos de la UI que se utilizan para mostrar información o interactuar con el usuario. Algunos ejemplos de views son TextView, ImageView, Button, EditText, CheckBox, RadioButton, entre otros. Cada view tiene sus propios atributos y métodos que se pueden utilizar para personalizar su apariencia y comportamiento.

- Fragments: Los fragments son componentes de la UI que se pueden utilizar para crear interfaces de usuario más complejas. Los fragments son similares a los Activity, pero se utilizan para crear interfaces de usuario más modulares y reutilizables. Un fragment puede ser utilizado en varios Activity y se puede actualizar de forma independiente.

- Menús: Los menús se utilizan para mostrar opciones y acciones en la UI de una aplicación. En Android, hay dos tipos de menús: el menú de opciones (Options Menu) y el menú contextual (Context Menu). El menú de opciones se muestra cuando el usuario presiona el botón de menú en el dispositivo, mientras que el menú contextual se muestra cuando el usuario mantiene presionado un elemento en la UI.

- RecyclerViews: Los RecyclerViews son componentes de la UI que se utilizan para mostrar listas de elementos que pueden desplazarse. Los RecyclerViews son similares a ListView, pero son más flexibles y ofrecen más opciones de personalización.

## Intent

En Android, un Intent es un objeto que se utiliza para comunicar información entre componentes de una aplicación, así como entre aplicaciones diferentes. Un Intent es un mecanismo importante para iniciar actividades (Activities), servicios (Services) y emisión de transmisiones (Broadcasts) en Android. Un Intent se compone de dos partes principales: el Action (acción) y el Data (datos).
Un Intent explícito se utiliza para iniciar una actividad, servicio o receptor de emisión específico dentro de la misma aplicación. En este tipo de Intent, se especifica el nombre completo de la clase de componente que se desea iniciar. Este tipo de Intent es útil cuando se sabe exactamente qué componente de la aplicación se desea iniciar y se tiene acceso directo a su nombre de clase.
Un Intent implícito, por otro lado, se utiliza para iniciar una actividad, servicio o receptor de emisión en cualquier aplicación del sistema que pueda manejar la acción específica especificada en el Intent. En este tipo de Intent, se especifica una acción que se desea realizar, junto con cualquier dato adicional que se desee enviar. Este tipo de Intent es útil cuando se desea realizar una tarea específica y se desea permitir que cualquier aplicación del sistema que pueda manejar la acción, la maneje, por ejemplo un intent para abrir la camara o ejecutar una funcion o solicitar un permiso de android

## Persistencia de datos

- Almacenamiento en memoria interna: Android permite a las aplicaciones almacenar datos en el almacenamiento interno del dispositivo. Esto se puede hacer utilizando los archivos de almacenamiento interno, que son privados a la aplicación y no se pueden acceder directamente desde otras aplicaciones o el usuario.

- Almacenamiento en memoria externa: Android también permite a las aplicaciones almacenar datos en el almacenamiento externo del dispositivo, como una tarjeta SD. Esto se puede hacer utilizando archivos de almacenamiento externo, que son públicos y pueden ser accedidos por otras aplicaciones o el usuario.

- Bases de datos: Android proporciona soporte para la creación y uso de bases de datos SQLite. Las bases de datos SQLite son una forma eficiente de almacenar grandes cantidades de datos estructurados. Las aplicaciones pueden utilizar bases de datos SQLite para almacenar información, como configuraciones de usuario, preferencias, datos de usuario y más.

- Almacenamiento en la nube: Las aplicaciones también pueden almacenar y recuperar datos en la nube utilizando servicios como Firebase Realtime Database o Google Cloud Storage. El almacenamiento en la nube permite que las aplicaciones sincronicen datos en tiempo real y los mantengan actualizados en todos los dispositivos.

- Shared Preferences: Este es un mecanismo de almacenamiento de datos simples para pequeñas cantidades de datos, como configuraciones de usuario y preferencias. Shared Preferences es una solución rápida y fácil para almacenar y recuperar datos simples.

## Navigation Drawer

Un Navigation Drawer, también conocido como "cajón de navegación", es un patrón de diseño de interfaz de usuario utilizado en aplicaciones móviles y web para proporcionar una navegación fácil y accesible. En Android, un Navigation Drawer es un panel lateral que se desliza desde el borde izquierdo o derecho de la pantalla y que contiene un menú de opciones de navegación.

## Http request

En Android Studio, se puede realizar una solicitud HTTP utilizando la clase HttpUrlConnection. HttpUrlConnection es una clase de Android que permite realizar solicitudes HTTP y HTTPS de forma sencilla y flexible.

## Arquitecturas y patrones de diseño para Android Studio

- MVP (Modelo-Vista-Presentador): Este patrón separa la lógica de presentación de la lógica de negocio y datos. El modelo representa los datos y la lógica de negocio, la vista representa la interfaz de usuario y el presentador actúa como intermediario entre el modelo y la vista, controlando la interacción entre ellos.

- MVVM (Modelo-Vista-ViewModel): Este patrón es similar al MVP, pero utiliza un ViewModel para manejar la lógica de presentación en lugar de un presentador. El ViewModel se encarga de mantener el estado de la vista y proporcionar datos a la vista según sea necesario.

- Clean Architecture: Esta arquitectura enfatiza la separación de preocupaciones y la independencia de la plataforma. Consiste en tres capas principales: la capa de presentación, la capa de dominio y la capa de infraestructura. La capa de presentación se encarga de la interfaz de usuario, la capa de dominio contiene la lógica de negocio y la capa de infraestructura proporciona la implementación de detalles técnicos, como la persistencia de datos y la comunicación en red.

- Arquitectura de componentes de Android: Esta es una arquitectura de Android recomendada por Google que utiliza los componentes de arquitectura de Android, como LiveData, ViewModel y Room, para simplificar el desarrollo de aplicaciones Android. LiveData se utiliza para observar los cambios en los datos, ViewModel se utiliza para mantener el estado de la vista y Room se utiliza para manejar la persistencia de datos.
