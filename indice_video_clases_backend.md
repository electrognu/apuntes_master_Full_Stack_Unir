## 20240101_G63 Node.js
- 00:00:00 Intro
- 00:04:00 Node.js - Motor de ejecución javascript
- 00:08:00 Preparar entorno : `npm init`
- 00:15:00 librerias predefinidas lib extras `www.npmjs.com`
- 00:24:00 Deno, evolución de nodejs, tardarà unos años a implementarse …
- 00:27:00 Importar librerias `require` en nodejs, `Import from` es para Angular
- 00:37:00 Libreria Axios para peticones  http
- 00:40:00 fichero package-lock, dependencias de las librerias que se han instalado.
- 00:47:45 que me devuleve el metodo GET de axios , como saberlo.
- 00:51:43 como mirar los errores ...
- 00:55:00 Nodemailer, para enviar correos electrónicos.
- 01:00:00 bcriptjs :  encriptación …
- 01:01:00 diferntes formulas para importar librerias, nodejs por defecto usamos `require` em angula `import`
- 01:04:00 day.js :  manejo de fechas
- 01:11:00 Como **modularizamos nuestro codigo** , creamos librerias.
- 01:16:00 exportacion de funciones...
- 01:22:00 importación de lo que hemos exportado.
- 01:28:00 Destructuring, quedarme solo con las claves que me interesan. (ychannel 10 minutos programando)
- 01:44:00 Organización de proyectos express no tienen base estructural como Angular.
- 01:46:00 Variables `__dirname` y `__filename`
- 01:52:00 Muy importante dependencias en -> Packet Json 

## 20240102_G64_Tema_sistema_ficheros
- 00:00:00 Diferentes maneras de acceder al sistema ficheros, ejemplo `readdir`
- 00:26:00 Asíncrona
- 00:29:00 Función autoejecutada para async/await
- 01:03:00 Apend File
- 01:10:00 Documentación FileSystem : API Promesas, Callback API, metodos Syncronos...
- 01:13:00 Ejemplo : Mkdir callback, ejemplo existsSync
- 01:21:00 Introduccion Servidores
- 01:46:00 Otra extension **REST CLIENT**

## 20240103_G65_Tema_
- 00:00:00 Introduccion teorica Comunicación Front <-> Back
- 00:06:00 URL + Cabeceras ... autenticación API.
- 00:08:00 Resonse: Status (200,403,404), Headers, Body para el front.
- 00:21:00 Intro Express
- 00:33:00 Servidor express basico. app.get
- 00:53:00 Como rearrancar el servidor automaticamente con los cambios "nodemon" para 
            `npm install --save-dev nodemon` porque lo utilizaremos solo en desarrollo.
- 01:03:00 Scripts de inicio importantes !! en package.json
- 01:14:45 `nodemon index.js` reinicia el servidor ante cualquier cambio.
- 01:22:00 Variables de entorno en fichero `.env` Explicación desarrollo y Produccion, 
- 01:37:00 `npm install dotenv`
- 01:47:00 Operación || para valores por defecto `PORT = process.env.PORT || 3000`

## 20241008_G66_Tema_primer_proyecto.
- 00:05:00 Primer proyecto
- 00:08:58 Instalar librerias
- 00:11:00 packed.json
- 00:18:00 2o crear la aplicacions de express, que resondera las peticiones
- 00:19:30 Creando servidor. `create server` y le pasamos la app de expres, `require`
- 00:22:00 Configurando .env
- 00:23:00 servidor a escuchar.
- 00:25:00 Eventos : `listening`
- 00:28:47 Levantando servidor `npm run dev` arrancant mode dev amb nodemon
- 00:31:00 Rutas de aplicación - petición GET
- 00:35:00 Lista **peticiones.rest**, probando GET...
- 00:38:00 petición POST
- 00:40:00 Organización de bloques gestión urls
- 00:47:00 explicación ...
- 00:54:00 Rutas bàsicas `express.Router();`
- 00:58:00 Crear Snipets en VScode 
- 01:07:00 Explicación Router
- 01:17:00 Controllers - Las funciones manejadoras.
- 01:20:00 Exportación de las funciones manejadoras
- 01:25:00 Cuidado **son variables** que almacenan funciones ...
- 01:43:00 funcion updateuser 
- 01:53:00 **Resumen** de la clase.

## 20241009_G67_Tema
- 00:00:00 Recordatorio de ultima clase.
- 00:08:00 Incluyendo numero usuario en la petición `deleteUserById`
- 00:15:00 Explicación como recuperar el Id, `req.params`
- 00:27:00 Creación usuarios POST. Como cogemos los datos del body del mensaje. `req.body`
- 00:33:20 Creando peticion POT de prueba con datos en json
- 00:38:00 Linea de configuración para aceptar correctamente a json
- 00:53:00 Query params `re.query` - Destructuring
- 01:01:00 Valores por defecto por si acaso no se define ...
- 01:07:00 Explicación básica `Middleware`
- 01:20:00 Libreria `Days.js`
- 01:29:00 añadir 5 minutos, fechas, etc ...
- 01:33:04 mariogiron / NodeJSLibraries
- 01:42:00 Prueba aleatoria de entrada ...
- 01:48:00 Añadir datos a la petición desde middleware
- 01:55:01 `Express-init-template` desde Github

## 20241010_G68_Tema
- 00:02:00 Middlel ware y más sobre la funcion DAYJS
- 00:11:38 àcceder al sistema de ficheros con promesas
- 00:14:00 `appendFile` Middleware de Log Files...
- 00:23:10 Otros midelware ...
- 00:29:00 Funcion `isNaN`
- 00:37:00 Status: errores del cliente 418 - I'm a teapot
- 00:42:00 Comodidad en funciones middleware...
- 00:52:00 Base Datos para practica + Carga en workbench
- 01:05:00 Plantilla express-init-template desde Github clonar y borrar carpeta .git
- 01:10:00 Iniciación del proyecto, cambios package.json, y repaso basico config.
- 01:20:00 Explicación teorica interesante ...
- 01:32:00 Creamos Routes

## 20241014_G69_Tema_Grupos_ProyectoFinal
## 20241015_G70_Tema_Grupos_ProyectoFinal


## 20241016_G71_Tema_API_Gimnasio (repetir)
- 00:00:00 Retomando API gimansio
- 00:08:00 Libreria instalar `mysql2`
- 00:10:00 Carpeta config y conexion BD.
- 00:13:00 mysql metodo `createPool()` y exportarlo
- 00:21:00 Querys ....
- 00:47:00 Repaso `destructuring`
- 00:54:00 Capturar error fallo BD.
- 01:15:00 Exportar funcion
- 01:16:00 Importante Router
- 01:33:00 Inserción ...
- 01:39:00 Mención de swagger.io
- 01:43:50 Herramientas depuración **debug**
- 01:44:00 Configuracion debug ...


## 20241017_G72_Tema
- 00:00:00 Configuración debug con nodemon
- 00:05:00 POST y explicación de API
- 00:15:00 `insertClient` 3 formulas para pasar parametros
- 00:22:00 Cleancode github Javascript
- 00:39:00 - CreateCliente
- 00:46:00 - Recibir la respuesta que toca ... Id del nuevo objeto. Select by id
- 01:02:00 - Fat model skini Controllers
- 01:03:00 - Utilzando la funcion selectById para devolver datos CreateCliente
- 01:15:00 - Recuperar un cliente a partirt de su Id - definicon del problema
- 01:31:00 - Debugging para ver variables que tipo son etc ...
- 01:37:57 - Actualizar los datos de un cliente ...

## 20241022_G74_Tema_Finalizacion_CRUD_Rutas_complejas_Middleware
- 00:00:00 Intro
- 00:02:00 Explicación teorica repaso
- 00:03:00 apiClientesRoutas, clientes controlers y clientesModel
- 00:05:00 CRUD Delete, comomenzando al revés, orden inverso a lo qu hicimos hasta ahora ...
- 00:16:00 Define borrar cliente... 
- 00:30:00 Recuperar toda la lsita de monitores con sus clientes asociados.
- 00:59:00 APi monitores prueba .. GET
- 01:47:00 Explicación varias funciones en las rutas como middlewares muy especificos !! Importante!
- 01:53:00 Middleware checkClienteId (req,res,next) => ... ahorra mucho trabajo en funciones repetitivas ...

## 20241023_G75_Tema_finalizacion_CRUD_Encriptacion_passwords_bcrypt
- 00:00:00 Preguntas ...
- 00:06:00 Crear Middleware checkClientID comprobaciones...
- 00:45:00 APIs privadas ... teorica
- 00:49:00 Guia escrita importante !! Objetivo marcado.
- 00:50:00 API Staff registro -> Que url? Que metodo? Cabeceras, de momento no? Body: susraio mail, passwd 
- 00:53:00 Passwords inseridos encriptar Passwords ...
- 00:59:00 1er: apiStaffRoutes, 2o StaffModel, 3er StaffControles, apiRoutes S
- 01:01:00 Inciso : Version 23 de node, require es la formula por defecto !!
- 01:46:00 Libreria encriptación -> bcrypt.js - instalacion ...
- 01:50:00 bcrypt.hash()

## 20241025_G76_Tema_Registro_encriptación
- 00:02:00 Teoria: flujo de trabajo Login.
- 00:17:00 Seleccionar por email
- 00:32:00 Coinciden passwords? bcrypt
- 00:38:00 Prueba ...
- 00:42:00 Teoria Comunicacion front - back y logueado de usuarios y creación de TOKEN
- 00:49:00 Estructura del TOKEN, se codifica información: 
- 00:51:00 Carpeta Helpers, create token
- 00:54:00 instalar libreria jsonwebtoken y crear TOKEN
- 01:18:00 Midleware checkToken es una accion para todas la rutas, y cosas a preguntar
