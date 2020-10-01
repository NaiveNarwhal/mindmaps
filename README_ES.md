# mapas mentales
mindmaps es una aplicación de mapas mentales basada en HTML5. Te permite crear mapas mentales de aspecto ordenado en el navegador.

Este proyecto comenzó en 2011 como una exploración de lo que se puede hacer en los navegadores que utilizan API modernas. Hoy en día, la mayoría de estas cosas son bastante comunes y el código base está un poco desactualizado. Esto fue mucho antes de React, ES6, webpack. Diablos, ni siquiera usa Backbone.

Sin embargo, no hay razón para cambiar nada de eso y hace que el código base sea bastante fácil de asimilar. No hay ningún paso de compilación, ni complementos de babel, ni marcos. Solo una aplicación de JavaScript y un patrón modelo-vista-presentador muy simple.

## Material HTML5 que fue adecuado en 2011
- Capacidad 100% sin conexión a través de ApplicationCache
- Almacena mapas mentales en LocalStorage
- La API FileReader lee los mapas mentales almacenados en el disco duro
- Canvas API dibuja el mapa mental

## Pruébalo
La última versión estable está alojada [aquí] (https://www.mindmaps.app).

## Construir
* Primero ejecute `npm install` para instalar las dependencias requeridas
* Ejecute `npm run start` para iniciar un servidor de desarrollo local. La aplicación se alojará en [http: // localhost: 3000] (http: // localhost: 3000).
* Ejecute `npm run build` para compilar el paquete de producción. Los artefactos se ubicarán en `/ dist`.


## Hostea tu mismo
Todo lo que necesita es un servidor web para archivos estáticos. Después de compilar, copie todos los archivos de / dist en su directorio web y ejecute la aplicación con index.html.
Asegúrese de que su servidor web sirva archivos .appcache con el tipo mime `text / cache-manifest` para que la aplicación
ser accesible sin conexión.

En Apache, agregue la siguiente línea a su .htaccess:

''
AddType text / cache-manifest .appcache
''

En nginx agregue esto a conf / mime.types:

''
texto / caché-manifiesto appcache;
''

Alternativamente, puede iniciar un servidor de depuración local con `npm start` que inicia un servidor en localhost: 8080.

## Licencia
mindmaps tiene licencia de AGPL V3, consulte LICENCIA para obtener más información.
