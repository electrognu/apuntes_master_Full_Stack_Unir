# Indice de videoclases MFSD

## 20240709_G37_Formularios 
Tema: formularios template y ...
00:00:00 Interesante discusión de ofertar paginas web y tecnologias.
00:16:00 Cambios que faltaron el dia 04 julio.
00:21:00 Evitar doCheck, consume muchos recursos, mejor opcion ...
00:29:00 Pintar lista de productos ...
00:50:00 Awesome favoritos ... 
01:08:00 Formularios tipo Model, modelo con validaciones.
01:10:00 Puntos del formulario Model Chuleta !!
01:13:00 Inicio HTML


## 20240710_G38 Tema: Formularios y validaciones
Tema: formularios ...
00:05:00 Expresiones regulares
00:38:00 form-model --- validar email: regex 
                        regexlib.com   regex101.com
                        ihateregex.io  cheatography.com
00:45:00 Crear Validadores propios 
01:50:00 Servicios introduccion 

## 20240711_G39 Tema: Servicios
El ejercicio servicios es una aplicación con un formulario, un selector de curso y presentación de los estudiantes del curso seleccionado. 
- 00:05:00 Explicacion teorica de servicio s
- 00:14:40 Noción de que és un  CRUD de datos
- 00:19:00 Creando componente servicio, se relaciona el nombre carpeta con la base de datos.

Como se inyecta el servicio? de dos formas:
- Antigua: como parametro en el constructor 
- Moderna: a través de la función Inject: 
Angular tirando a modelo funcional, aunque sigue con objetos. 
Framework React se ha convertido en funcional, React és una libreria.
- 00:22:00 Enseña la aplicación funcionando.
- 00:25:00 codigo
- 00:32:00 Crear interfaces, componentes i servicios, 
- 00:36:00 Carpeta simulacion bbdd
- 00:40:00 Llenar carpeta simulacion BBDD con datos ...
- 00:51:00 Metodos del servicio ... getAll() etc ...
- 01:00:00 Cargando todo en el componente principal
- 01:15:00 Student card INPUT! ???
- 01:24:00 Student Card
- 01:31:00 Filter
- 01:39::00 maquetar

## 20240716_G40 Tema: servicios 
Finalizando el ejercicio servicios.
00:04:00 Continuando
00:07:36 Realizando output filters.component
00:09:00 Conectar con studentsList.ts
00:11:30 llamo servicio
00:12:20 crear el servicio getById() creando filter  devuelve un array
00:16:20 Cambios en los errores de la BBDD
00:19:20 @ empty en el for - No dejar en blanco la pàgina ... ****
00:20:30 Y el caso de "todos los estudiantes"
00:27:00 Empieza la parte del formulario.
00:41:00 Cambiando errores BBDD
00:48:00 Arreglando student List 
00:55:00 cambios services ...
00:58:58 Volvemos al formulario.
01:06:50 Validadores en los campos del formulario.
01:18:00 Enviado campos al servicio
01:32:12 Libreria externa Sweetalert
01:48:00 Creacion interfaz dentro Students.services.ts - excepción: puedo usar mis propios tipos personalizados sin crear interfaces siempre y cuando estos no vayan a ser reutilizados.

### 20240717_G41 Tema: Rutas
00:02:27 Empieza explicación Rutas, rutas amigables, para que los buscadores puedan indexarlas
00:05:20 Deep web, contenido no indexable porque està en zonas privadas. Url internas, normalmente un identificador numero.
00:09:00 Creando nueva proyecto
00:12:00 Aplicar estilos y escripts para bootstrap ******** angular.jason
00:14:00 Componentes de pàginas. "Paginas: Todo componente que corresponde a una ruta y puede cargar componentes "
app.routes.ts se van a declarar todas las rutas ...
00:17:30 Definición de rutas : no borrar el router-outlet 
00:24:24 Generando página como componentes
```
ng g c pages/home --skip-test
``` 
00:27:30 Cargando componete home como ruta inicial.
00:34:00 Gestionar Pagina 404 - Error cuando la pagina no existe.
00:38:00 Creando pagina error 404 ng ...
00:39:00 creando cabezera con links
00:46:00 Como definimos las rutas? herf="..url.." no funciona bien, recarga toda la pagina
00:49:00 Se sustituyen href por \[routerLink\]  ->  Importar RouterLink
00:53:00 Router Link activate
01:03:00 Call to action !! desde un y otros enlaces ...
01:12:00 Boton submit 
01:18:00 Atención ... inyeccion de dependencias router ... redirigimos desde el ts donde no podemos poner rutas...
01:26:00 Creamos los productos -> ruta del producto, estamos en la parte pública de la web -> URL publica ...
01:29:00 Creamos BBDD en array de los servicios + interface servicios + creamos pagina con  servicios
01:51:00 Rutas dinámicas ...

### 20240718_G42 Tema: Rutas
Finalizando el ejercicio rutas ...
00:04:00 Recapitulación del último dia
00:06:00 Cuidado Distinción de rutas incorrectas
00:14:00 Aquí empieza lo interesante ...que es un observable ?
00:21:00 Ojo los parametros ruta son siempre alfanumericos aunque sean un numero.
00:43:00 Componetizar "ServicioCard"
00:51:00 Añadiendo buscador ...
01:18:00 Inicio del ejercicio MARKETPLACE
01:29:00 Base de datos en fichero ...
01:44:00 Montando las rutas ... rutas hijas ...

### 20240723_G43 Tema: Rutas - MARKETPLACE
00:13:00 Seguimos con Marketplace
00:15:00 Creamos servicio...
00:20:00 Header + login
00:30:00 Navegación Panel Control
00:37:00 Product-list component ... comentario de inyectables de dos maneras ... inyectando de dos formas ...
00:46:00 Creando componente producto card 
00:48:00 Pintando los productos ...
01:09:00 Parametro optativo en getProducByStock ...
01:12:00 Creando un tipo para params route subscribe
01:23:00 Product view component
01:34:00 Creando el selector de categorias ...
01:49:00 Enlazar todo en Product-list
01:55:00 Añadiendo formulario, que sera tipo pàgina.

### 20240724_G44 Tema: MarketPlace - Peticiones HTTP
00:03:00 Recapitulando
00:04:25 Parametros de ruta product-view
00:18:00 Product Formulario ...
00:24:00 Ctrl + espacio...
00:46:40 pathValue vs setValue
01:01:00 Verificando inserción correcta ...
01:21:00 Proyecto HTTP
01:24:00 Peticiones HTTP ... fetch en JS, HTTPClient con observables y con promesas.
01:28:00 Peticiones Online , cada API tiene resupestas distintas ... Quicktype.io
01:36:00 Crear interfaces y servicios
01:44:00 CRUD - create-read-update-delete   -> post-get-put-delete; con observables y con promesas.
01:57:00 Con Promesa ...
01:59:00 Con Promesa async await

### 20240730_G45 Peticiones HTTP - CRM Empleados
00:01:00 Repaso explica peticion de la pràctica.
00:06:00 Resumen pasos
00:14:00 Creando proyecto CRM Empleados, con metodos parecido a la practica que tenemos que hacer nosotros.
00:21:00 Definición de la App CRM Empleados
00:25:00 Genrando interface
00:30:00 definiendo rutas
00:37:00 Creando Rutas
00:39:00 Html home
00:52:00 Creando servicio empleados.
01:00:00 Employee-list component, navbar, 
01:24:00 En caso de nuestra aplicacion ...
01:29:00 Employee card INPUT (truco)

### 20240730_G46 Peticiones HTTP - CRM Empleados
00:03:00 Retomamos donde de fundiewros los plomos + SVG Awesome fonts
00:13:59 Esconder ciertos campor para responsive salga mejor.
00:21:00 Creanr Employes View ...

### 20240731_G47 
00:04:00 Botones Goto Page
00:12:35 Arreglando problema de header y router-ou+tlet
00:23:00 Generando Formulario
00:30:00 Employ view ... Capturar la ruta !! Activa
00:44:00 Borrar empleado
00:54:00 Crear metodo delete en el servicio. Después de borrar ahy que recargar la vista de empleados.
00:59:00 Nuevo empleado ... no se aplicar validaciones
01:18:00 GetDataForm ---
01:38:00 Actualización de un usuario ...

### 20240903_G48_Tema_Guards_y_interceptors
Logueo con token etc ...
00:07:00 CRM empleados, Cabeceras de autentificación 
00:09:00 Proceso Login y maquetado de formulario entrada
00:20:00 Explicación y creación de servicio e interfaz.
00:38:20 Concepto cabeceras, hasta que creemos el interceptor y manejo de error.
00:53:21 Devolucion token
00:54:00 Generic type tipo respuesta ...
00:56:30 Guardar el token en local store y redirigir al dash board.
00:58:00 Concepto: Local storage, cookies técnicas y de publicidad. Conceptos de almacenamientos.