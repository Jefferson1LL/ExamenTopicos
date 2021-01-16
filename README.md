# ExamenTopicos
Examen de primer Bimestre 

Chat Desarrollado con autentitacion y registro usando ionic, laravel, firebase y ocupando las bibliotecas necesarias 
Despues de haber creado el proyecto genere dos paginas que son el login y el registro a la parte del chat fue generada como componente 
ya que dentro de la programacion esto se lo despliega como un modal.

A continucación se generan los servicios de autenticación y el que es para el chat.
Dentro del servicio de autenticación importamos las librerias necesarias como lo son:
 * *AngularFirestore
 * *AngularFireAuth
 * *Router
 se puede decir que estas tres son las principales para el funcionamiento de login.
 En el mismo archivo ocupamos 3 funciones como son las de login la cual adquiere dos parámetros que son email y password
 tenemos un logOut para el cierre de sesión y tenemos el de registrar donde los parametros que se piden son
 email, password y name, el parametro name no es necesario pero dentro de la base de datos nos sirve para identificar
 al usuario cuando se crea la base de datos como una colección.
 Podemos también explicar lo de router el cual nos ayuda a la navegación entre páginas.
 
 Dentro de chatservice declaramos al inicio 4 atributos como lo son description, name, id e img las cuales nos ayudarán 
 a visualizar los usuarios del chat.
 
 Dentro de la página home que se crea en conjunto con el proyecto visualizamos los usuarios en el html, dentro de home.page.ts
 importamos libreras necesarias y creamos un modal el cual cuando demos un click en cualquier usuario nos mostrara el panel donde podemos enviar 
 el mensaje, al mismo tiempo tenemos otra funcion la cual la creamos para cerrar sesión esta la sacamos directamente
 de la documentación de ionic.
 
 dentro de registro.page.ts creamos la funcion para el registro la cual nos validara los datos como el email, password y contraseña
 y al mismo tiempo mediante el router cuando demos click en el boton nos redigirá directamente al home, asi mismo nuestro
 login cuenta con un igual archivo typescript en el cual colocamos la funcion de inicio de sesión que al igual el boton valida
 los campos y nos redirige al home.
 Cada página o componente cuenta con un archivo scss para dar un diseño agradable a la vista del usuario.
 Debemos recalcar también que tenemos unos archivos que son de importancia en el sistema y estos son:
 * * app-routing.module: Este es donde se guardan las direcciones de cada página creada y las que nos ayudan a la navegación
 * *app.module.ts: Este es donde importamos las librerias del sistema necesarias para el funcionamiento aqui se debe colocar todo lo
 que vamos a ocupar ya que sin eso el sistema nos da errores en cualquier momento.
 * *envireonment: Dentro de este archivo lo que colocamos son las credenciales de firebase
