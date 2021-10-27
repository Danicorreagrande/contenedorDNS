“version ‘2.2’: Los archivos docker-compose.yml son versionados, lo que significa que es muy importante indicar la version de las instrucciones que queremos darle. A medida de que Docker evoluciona, habrá nuevas versiones, pero de todos modos, siempre hay compatabilidad hacia atras, al indicar la version de la receta.

“ports”: Aqui mapeamos los puertos locales 4000 (webserver jekyll) y 35729 (livereload) al servidor host. Esto permitirá que accediendo a Localhost:4000 podamos probar el sitio generador por Jekyll

“volumes”: Aqui hacemos que el directorio actual se mapee directamente con el /app, lugar donde hemos creado la aplicación. De este modo, cualquier cambio en el directorio local en el host, se hará de inmediato en el contenedor.