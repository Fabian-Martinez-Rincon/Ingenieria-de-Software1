<div align="center">

[![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/Nomadiix/IS1)
[![GitHub stars](https://img.shields.io/github/stars/Nomadiix/IS1)](https://github.com/FabianMartinez1234567/IS1/stargazers/)
[![GitHub repo size in bytes](https://img.shields.io/github/repo-size/Nomadiix/IS1)](https://github.com/Nomadiix/IS1)
 </div>
<h1 align="center"> 👤 Practica 2</h1>


<div align='center'>

[Practica 1 | Teoria](/Documentos/Practica1.md)<br>
[Practica 2 | Historias de Usuario](/Documentos/Practica2.md)<br>
[Practica 3 | Casos de Uso](/Documentos/Practica3.md)<br>
[Practica 4 | DTE](/Documentos/Practica4.md)<br>
[Practica 5 | Redes de Petri](/Documentos/Practica5.md)<br>
[Practica 6 | Tablas de Desición](/Documentos/Practica6.md)
</div>

<img src= 'https://i.gifer.com/origin/8c/8cd3f1898255c045143e1da97fbabf10_w200.gif' height="20" width="100%">

- [1) Alquiler de mobiliario](#problema-1-alquiler-de-mobiliario)
- [2) Posgrado](#problema-2-posgrado)
- [3) Contratos](#problema-3-contratos)
- [4) Venta de bebidas](#problema-4-venta-de-bebidas)
- [5) Casa de fotografía](#problema-5-casa-de-fotografía)
- [6) Biblioteca](#problema-6-biblioteca)
- [7) Mutual](#problema-7-mutual)
- [8) Teatro](#problema-8-teatro)
- [9) Pago Electrónico](#problema-9-pago-electrónico)
- [10) Un Aventón](#problema-10-un-aventón)
- [11) Concursos](#problema-11-concursos)
- [12) Créditos bancarios](#problema-12-créditos-bancarios)
- [12) Venta de libros](#problema-12-venta-de-libros)
- [13) Manejo de tarjetas de crédito](#problema-13-manejo-de-tarjetas-de-crédito)
- [13) Manejo de canchas de tenis](#problema-13-manejo-de-canchas-de-tenis)
- [14) Procesamiento de imágenes](#problema-14-procesamiento-de-imágenes)


<img src= 'https://i.gifer.com/origin/8c/8cd3f1898255c045143e1da97fbabf10_w200.gif' height="20" width="100%">

Quiero aclarar que estos colores los elegi yo porque a mi me gustaron, no es nada especifico de la catedra

| Colores Para identificar      | ![Color Picker Boxes](https://draculatheme.com/static/img/color-boxes/eyedropper.png)   |
| ------------ | --------------------------------------------------------------------------------------- |
| Reglas de negocios         | ![Cyan Color](https://draculatheme.com/static/img/color-boxes/cyan.png)                 |
| Historias de Usuario       | ![Orange Color](https://draculatheme.com/static/img/color-boxes/orange.png)             |
| Datos solicitados o que debe realizar       | ![Purple Color](https://draculatheme.com/static/img/color-boxes/purple.png)             |
| Roles       | ![Yellow Color](https://draculatheme.com/static/img/color-boxes/yellow.png)             |

Para cada Historia de Usuario se deben indicar los siguientes ítems:

<table><tr><td> 

**ID:** 
 
**TÍTULO:** 

**REGLAS DE NEGOCIO:** 

</td></tr><tr><td>

**CRITERIOS DE ACEPTACIÓN:** 

**Escenario 1:** título del criterio.

Dado 

Cuando 

Entonces 

---

</td></tr></table>

## Estas son las historias que son iguales en todos los ejercicios

### Pagar con Tarjeta

<table><tr><td> 

**ID:** Pagar con tarjeta
 
**TÍTULO:** Como usuario quiero pagar con tarjeta para pode reservar un alquiler

**REGLAS DE NEGOCIO:** 

- Numero de tarjeta valido
- Tiene fondos suficientes


</td></tr><tr><td>

**CRITERIOS DE ACEPTACIÓN:** Pagar con tarjeta

**Escenario 1:** Pago exitoso

Dado que se pudo establecer conexión con el servidor del banco, el nro 123 de la tarjeta es valido y posee fondos suficientes

Cuando el cliente ingresa 123.

Entonces el sistema registra el pago

---

**Escenario 2:** Pago Fallido por falla con la conexión del banco

Dado que no se pudo establecer conexión con el banco

Cuando el cliente quiere pagar

Entonces el sistema informa que no se pudo establecer conexion con el banco

---

**Escenario 3:** Pago fallido por numero de tarjeta invalido

Dado que se pudo establecer conexión con el servidor del banco, el nro 777 de la tarjeta es invalido

Cuando el cliente ingresa 777.

Entonces el sistema informa que el nro de la tarjeta es invalido y no registra el pago

---

**Escenario 4:** Pago fallido por saldo insuficiente

Dado que se pudo establecer conexión con el servidor del banco, el nro 1010 de la terjeta es valido y no tiene fondos

Cuando el cliente ingresa 1010

Entonces el sistema informa que la tarjeta no tiene fondos suficientes y no registra el cobro

</td></tr></table>

---

### Registrar Usuario

<table><tr><td> 

**ID:** Registrar Alumno
 
**TÍTULO:** Como alumno quiero registrarme para tener una cuenta

**REGLAS DE NEGOCIO:** 
- Nombre de usuario unico
- Contaseña con mas de 6 digitos (Esta puede variar)

 </td> </tr>
<tr><td>

**CRITERIOS DE ACEPTACIÓN:** 

**Escenario 1:** Registrar Alumno

Dado que el usuario fabo es unico y la contraseña kapo013 tiene mas de 6 digitos

Cuando el alumno ingresa fabo, kapo013

Entonces el sistema registra al usuario

---

**Escenario 2:** Registro fallido por usuario ya existente

Dado que el usuario tomo no es unico y la contraseña pepe555 tiene mas de 6 digitos

Cuando el alumno ingresa tomo, pepe555

Entonces el sistema Informa que el usuario ingresado ya existe, y no realiza el registro

---

**Escenario 3:** Registro fallido por contraseña con menos de 6 digitos

Dado que el usuario messi es unico y la contraseña 2023 tiene menos de 6 digitos

Cuando el alumno ingresa messi, 2023

Entonces el sistema informa que la contraseña ingresada tiene menos de 6 digitos y no realiza el registro

</td></tr></table>

---

### Iniciar Sesión

<table><tr><td> 

**ID:** Iniciar Sesión
 
**TÍTULO:** Como usuario quiero iniciar sesión para poder entrar en mi cuenta

**REGLAS DE NEGOCIO:** 

 </td> </tr>
<tr><td>

**CRITERIOS DE ACEPTACIÓN:** Iniciar Sesión

**Escenario 1:** Inicio exitoso

Dado que el usuario fabo se encuentra registrado y la contraseña kapo013 es correcta

Cuando el usuario ingresa fabo, kapo013

Entonces el sistema realiza el inicio de sesión y habilita sus respectivas opciones

---

**Escenario 2:** Inicio fallido por usuario no registrado

Dado que el usuario maradona no se encuentra registrado

Cuando el usuario ingresa maradona, cocacola21

Entonces el sistema informa que el usuario no se encuentra registrado y no realiza el inicio de sesión

---

**Escenario 3:** Inicio fallido por contraseña incorrecta

Dado que el usuario stalin se encuentra registrado y la contraseña presi19 es incorrecta

Cuando el usuario ingresa stalin, presi19

Entonces el sistema informa que la contraseña es incorrecta y no realiza el inicio de sesión

</td></tr></table>

---

### Cerrar Sesión

<table><tr><td> 

**ID:** Cerrar Sesión
 
**TÍTULO:** 

**REGLAS DE NEGOCIO:** Cerrar Sesión

 </td> </tr>
<tr><td>

**CRITERIOS DE ACEPTACIÓN:** 

**Escenario 1:** Cierre exitoso

Dado que el usuario tiene una sesión abierta

Cuando el usuario aprieta el boton de cerrar su sesión

Entonces el sistema cierra la sesión y deshabilita sus respectivas opciones 


</td></tr></table>



<img src= 'https://i.gifer.com/origin/8c/8cd3f1898255c045143e1da97fbabf10_w200.gif' height="20" width="100%">


**Para cada problema planteado realice las tarjetas completas de todas las historias de usuario identificadas**

<img src= 'https://i.gifer.com/origin/8c/8cd3f1898255c045143e1da97fbabf10_w200.gif' height="20" width="100%">

<div align = center>

## `Problema 1` Alquiler de mobiliario

</div>

Suponga que trabaja en una consultora la cual ha sido recientemente contactada por una empresa de alquiler de mobiliario para eventos para la realización de una app.

De las diferentes entrevistas se ha obtenido la siguiente información:

El gerente nos dijo que resulta fundamental tener una aplicación móvil que nos permita manejar la agenda de la empresa, sabiendo qué disponibilidad tenemos y permitiendo que nuestros clientes alquilen a través de la app. Para esta primera versión de la app, el gerente nos pidió que sea posible dar de alta los diferentes mobiliarios, así como la posibilidad de que los usuarios puedan realizar una reserva de alquiler desde sus dispositivos. Para el detalle de cómo se realiza la carga de los muebles, el gerente nos sugirió hablar con el encargado del departamento de mobiliario. El encargado de mobiliario nos comentó que de cada mueble se debe cargar código de inventario, tipo de mueble, fecha de creación, fecha de último mantenimiento, estado (libre, de baja, alquilado) y el precio de alquiler. Además, no pueden existir códigos repetidos y por el contrato de la franquicia, el precio debe cargarse en dólares. Para que el encargado pueda dar de alta el mobiliario debe autenticarse en el sistema. El registro de los usuarios de carga no debe modelarse.

El encargado del departamento de alquileres no comentó acerca de las reservas de los alquileres. Por una política comercial de la marca una reserva tiene que incluir como mínimo 3 muebles. La reserva debe tener una fecha, lugar del evento, cantidad de días y mobiliario junto a su cantidad. Para realizar una reserva se debe abonar el 20% del total del alquiler. El pago de la reserva se realiza únicamente con tarjeta de crédito validando número de tarjeta y fondos a través de un servicio del banco. Luego de efectuado el pago, se emite un número de reserva único que será luego utilizado por el
cliente para hacer efectivo el alquiler.

---

![image](https://user-images.githubusercontent.com/55964635/232102581-8c67db96-908f-4d34-aebe-3f0d2b1f725e.png)

---

### Roles

- Usuario
- Encargado del departamento

### Historias de Usuario
- Reservar Alquiler
- Dar alta inmueble
- Pagar con tarjeta

---

### Reservar Alquiler

<table><tr><td> 

**ID:** Reservar Alquiler
 
**TÍTULO:** Como usuario quiero hacer una reserva de alquiler para poder vivir un tiempo

**REGLAS DE NEGOCIO:** Reservar Alquiler
- Incluye minimo 3 muebles
- Se abona el 20% del total con tarjeta de credito

</td></tr><tr><td>

**CRITERIOS DE ACEPTACIÓN:** 

**Escenario 1:** Reservar Exitosa

Dado que el alquiler tiene 3 muebles y se pago el 20% con una tarjeta de credito valida

Cuando el usuario ingresa 10-10-2010, La Plata, 3 dias, 3 muebles y los datos de una tarjeta de credito valida

Entonces el sistema emite un numero de reserva unico.

---

**Escenario 2:** Reservar Fallida por muebles insuficientes

Dado que el alquiler tiene 1 mueble y se pago el 20% con una tarjeta de credito valida

Cuando el usuario ingresa 05-05-2020, La Plata, 11 dias, 1 muebles y los datos de una tarjeta de credito valida

Entonces el sistema informa que el inmueble no cumple con los requisitos minimos

---

**Escenario 3:** Reserva Fallida por problemas con la tarjeta de credito

Dado que el alquiler tiene 5 muebles y se pago el 20% con una tarjeta invalida

Cuando el usuario ingresa 20-03-2015, Buenos Aires, 30 dias, 5 muebles y los datos de una tarjeta de credito invalida

Entonces el sistema informa que la tarjeta es invalida y no registra el pago


</td></tr></table>

--------------------------------------------------------------

### Dar Alta Inmueble

<table><tr><td> 

**ID:** Dar alta inmueble
 
**TÍTULO:** Como encargado de departamento quiero dar alta un inmueble para que pueda ser alquilado

**REGLAS DE NEGOCIO:** 
- Codigo Unico
- Se cargo en dolares

</td></tr><tr><td>

**CRITERIOS DE ACEPTACIÓN:** Dar alta inmueble

**Escenario 1:** Alta Exitosa

Dado que el codigo 0202 es unico y el precio 10$ se cargo en dolares

Cuando el empleado de mesa ingresa 0202, Mesa, 1-1-2000, 20-20-2020, libre, 10$

Entonces el sistema registra el mueble en el sistema

---

**Escenario 2:** Alta Fallida por codigo ya existente

Dado que el codigo 1010 no es unico y el precio 20$ se cargo en dolares

Cuando el empleado de mesa ingresa 1010, Ropero, 3-3-2003, 04-04-2004, de baja, 20$

Entonces el sistema informa que el codigo ya se encuentra registrado y no realiza el alta

---

**Escenario 3:** Alta Fallida por precio cargado en euros

Dado que el codigo 4040 es unico y el precio 10$ se cargo en euros

Cuando el empleado de mesa ingresa 4040, Cama, 2-2-2002, 21-21-2021, alquilado, 30$

Entonces el sistema informa que el precio debe cargarse en dolares y no realiza el alta


</td></tr></table>

--------------------------------------------------------------

### Pagar con tarjeta

<table><tr><td> 

**ID:** Pagar con tarjeta
 
**TÍTULO:** Como usuario quiero pagar con tarjeta para pode reservar un alquiler

**REGLAS DE NEGOCIO:** 

- Numero de tarjeta valido
- Tiene fondos suficientes


</td></tr><tr><td>

**CRITERIOS DE ACEPTACIÓN:** Pagar con tarjeta

**Escenario 1:** Pago exitoso

Dado que se pudo establecer conexión con el servidor del banco, el nro 123 de la tarjeta es valido y posee fondos suficientes

Cuando el cliente ingresa 123.

Entonces el sistema registra el pago

---

**Escenario 2:** Pago Fallido por falla con la conexión del banco

Dado que no se pudo establecer conexión con el banco

Cuando el cliente quiere pagar

Entonces el sistema informa que no se pudo establecer conexion con el banco

---

**Escenario 3:** Pago fallido por numero de tarjeta invalido

Dado que se pudo establecer conexión con el servidor del banco, el nro 777 de la tarjeta es invalido

Cuando el cliente ingresa 777.

Entonces el sistema informa que el nro de la tarjeta es invalido y no registra el pago

---

**Escenario 4:** Pago fallido por saldo insuficiente

Dado que se pudo establecer conexión con el servidor del banco, el nro 1010 de la terjeta es valido y no tiene fondos

Cuando el cliente ingresa 1010

Entonces el sistema informa que la tarjeta no tiene fondos suficientes y no registra el cobro

</td></tr></table>

<img src= 'https://i.gifer.com/origin/8c/8cd3f1898255c045143e1da97fbabf10_w200.gif' height="20" width="100%">

<div align = center>

## `Problema 2` Posgrado

</div>

Suponga que trabaja en el área de sistemas de la Facultad de Informática y se le solicitó la automatización del pago de carreras de posgrado. Inicialmente se coordinó una reunión con el director del posgrado y se obtuvo la siguiente información:

Ya que no se desea seguir cobrando el dinero en la secretaría, es necesario que los alumnos puedan pagar las carreras vía web. Como el director de posgrado no realiza tareas administrativas nos recomendó hablar con el secretario académico. De la entrevista con el secretario académico se obtuvo la siguiente información:

Es necesario cargar las carreras a un sistema. En esta primera versión del sistema sólo se nos pidió esta funcionalidad, sin la modificación ni eliminación. De cada carrera se conoce: nombre de la carrera (no puede repetirse), duración en años (a partir de la consulta del estatuto de posgrado se obtuvo que como máximo son 5 años), costo y cantidad máxima de cuotas para el pago. La carga de las carreras no la realiza el secretario académico sino un empleado administrativo.

Al preguntarle por la dinámica del sistema, el secretario académico nos derivó con el jefe del área administrativa, con el cual hicimos otra entrevista y pudimos obtener la siguiente información:

El requerimiento fue que el alumno ingrese a la web de posgrado y pueda registrarse ingresando: nombre, apellido, nombre de usuario (único) y contraseña (más de 6 dígitos). Cualquier alumno previamente registrado, puede iniciar sesión con su nombre de usuario y contraseña, habilitándose la inscripción a alguna de las carreras. Para ejemplificar esta
funcionalidad nos otorgaron acceso al sistema SIGEF, el cual realiza funcionalidades similares para las carreras de grado. 

Para inscribirse, el alumno deberá seleccionar la carrera, ingresar la cantidad de cuotas a pagar, ingresar el número de tarjeta y, en caso de que la tarjeta sea válida y tenga fondos, se hará efectivo el cobro y la inscripción. La tarjeta de crédito se valida a través de un servicio del banco con el cual la universidad tiene convenio. Luego de efectuado el cobro, el sistema debe imprimir dos comprobantes, uno de inscripción y otro de pago. La única forma que tiene el alumno de pagar es con tarjeta de crédito

![image](https://user-images.githubusercontent.com/55964635/232157667-7fe023af-566c-4d5d-8d5a-03114a6aae62.png)
![image](https://user-images.githubusercontent.com/55964635/232158030-b58db95a-76bf-400a-a703-7ff4b999d6b3.png)

---

### Roles

- Alumno (Usuario no registrado)
- Usuario
- Empleado Administrativo

### Historias de Usuario

- Inscribir a carrera
- Dar alta carrera
- Registrar alumno
- Iniciar Sesión 
- Cerrar Sesión 
- Pagar con tarjeta 



---
### Inscribir a carrera

<table><tr><td>

**ID:** Inscribir a carrera
 
**TÍTULO:** Como usuario quiero inscribirme a una carrera para poder estudiar

**REGLAS DE NEGOCIO:** Inscribir a carrera

- Las cuotas no superan el maximo permitido

Aca quiero aclarar que el usuario no ingresa las cuotas a mano, sino que le aparece un menu con las cuotas disponibles, por eso no es una regla de negocio

</td> </tr><tr><td>

**CRITERIOS DE ACEPTACIÓN:** 

**Escenario 1:** Inscripción exitosa

Dado que el usuario posee una tarjeta de credito valida

Cuando el usuario selecciona la carrera Filosofia y los datos de una tarjeta de credito valida

Entonces El sistema registra la inscripción del usuario e imprime dos comprobantes, uno de inscripcion y otro de pago

---

**Escenario 2:** Inscripción fallida por tarjeta invalida

Dado que el usuario posee una tarjeta de credito invalida

Cuando el usuario selecciona la carrera Biologia y los datos de una tarjeta de credito invalida

Entonces El sistema registra la inscripción del usuario e imprime dos comprobantes, uno de inscripcion y otro de pago


</td></tr></table>

---
### Alta carrera

<table><tr><td> 

**ID:** Alta carrera
 
**TÍTULO:** Como empleado administrativo quiero dar de alta la carrera para que los usuarios puedas inscribirse en ella

**REGLAS DE NEGOCIO:** 
- Nombre Unico
- Duración maxima de 5 años


 </td> </tr>
<tr><td>

**CRITERIOS DE ACEPTACIÓN:** Alta carrera

**Escenario 1:** Alta de carrera exitosa.

Dado que el nombre Informatica es unico, y la carrera dura 4 años

Cuando el empleado administrativo ingresa Informatica, 4 años, 100$, 20 cuotas

Entonces El sistema da de alta la carrera

---

**Escenario 2:** Alta de carrera fallida por codigo ya existente

Dado que el nombre Arte no es unico y la carrera dura 5 años

Cuando el empleado administrativo ingresa Arte, 5 años, 300$, 10 cuotas

Entonces el sistema informa que el nombre de la carrera ya existe y no realiza el alta

---

**Escenario 3:** Alta de carrera fallida por duracion supera los 5 años

Dado que el nombre Astrologia es unico y la carrera dura 100 años

Cuando el empleado administrativo ingresa Astrologia, 100 años, 2$ y 1000 cuotas

Entonces el sistema informa que la duración ingresada supera los 5 años que son permitidos y no realiza el alta a la carrera

</td></tr></table>

### Registrar Usuario

<table><tr><td> 

**ID:** Registrar Alumno
 
**TÍTULO:** Como alumno quiero registrarme para anotarme a una carrera

**REGLAS DE NEGOCIO:** 
- Nombre de usuario unico
- Contaseña con mas de 6 digitos 

 </td> </tr>
<tr><td>

**CRITERIOS DE ACEPTACIÓN:** 

**Escenario 1:** Registrar Alumno

Dado que el usuario fabo es unico y la contraseña kapo013 tiene mas de 6 digitos

Cuando el alumno ingresa Fabian, Martinez ,fabo, kapo013

Entonces el sistema registra al usuario

---

**Escenario 2:** Registro fallido por usuario ya existente

Dado que el usuario tomo no es unico y la contraseña pepe555 tiene mas de 6 digitos

Cuando el alumno ingresa Tomas, Gomez, tomo, pepe555

Entonces el sistema Informa que el usuario ingresado ya existe, y no realiza el registro

---

**Escenario 3:** Registro fallido por contraseña con menos de 6 digitos

Dado que el usuario messi es unico y la contraseña 2023 tiene menos de 6 digitos

Cuando el alumno ingresa Lionel, Messi, messi, 2023

Entonces el sistema informa que la contraseña ingresada tiene menos de 6 digitos y no realiza el registro

</td></tr></table>

---

### Iniciar Sesión

<table><tr><td> 

**ID:** Iniciar Sesión
 
**TÍTULO:** Como usuario quiero iniciar sesión para poder anotarme en alguna carrera

**REGLAS DE NEGOCIO:** 

 </td> </tr>
<tr><td>

**CRITERIOS DE ACEPTACIÓN:** Iniciar Sesión

**Escenario 1:** Inicio exitoso

Dado que el usuario fabo se encuentra registrado y la contraseña kapo013 es correcta

Cuando el usuario ingresa fabo, kapo013

Entonces el sistema realiza el inicio de sesión y habilita la inscripción a algunas carreras

---

**Escenario 2:** Inicio fallido por usuario no registrado

Dado que el usuario maradona no se encuentra registrado

Cuando el usuario ingresa maradona, cocacola21

Entonces el sistema informa que el usuario no se encuentra registrado y no realiza el inicio de sesión

---

**Escenario 3:** Inicio fallido por contraseña incorrecta

Dado que el usuario stalin se encuentra registrado y la contraseña presi19 es incorrecta

Cuando el usuario ingresa stalin, presi19

Entonces el sistema informa que la contraseña es incorrecta y no realiza el inicio de sesión

</td></tr></table>

---

### Cerrar Sesión

<table><tr><td> 

**ID:** Cerrar Sesión
 
**TÍTULO:** 

**REGLAS DE NEGOCIO:** Cerrar Sesión

 </td> </tr>
<tr><td>

**CRITERIOS DE ACEPTACIÓN:** 

**Escenario 3:** Cierre exitoso

Dado que el usuario tiene una sesión abierta

Cuando el usuario aprieta el boton de cerrar su sesión

Entonces el sistema cierra la sesión y deshabilita sus respectivas opciones 


</td></tr></table>



<img src= 'https://i.gifer.com/origin/8c/8cd3f1898255c045143e1da97fbabf10_w200.gif' height="20" width="100%">

<div align = center>

## `Problema 3` Contratos

</div>

Suponga que trabaja en un grupo en el área de sistemas de una organización y está por comenzar un nuevo proyecto para desarrollar un sistema que depende del departamento contable.

El sistema deberá administrar los contratos realizado con terceros. En una de las reuniones con el jefe de departamento nos dijo que él no usará el sistema pero que recibirá listados del personal contratado ya que deberá firmarlos para elevarlos a las autoridades.

Para obtener más información generamos una reunión con el empleado de mesa de entradas. Nos contó que el problema que tienen actualmente es que realizan todas las minutas a mano por lo cual desean automatizar esta tarea. Las minutas son el paso previo a un contrato. Para confeccionar una minuta, el empleado de mesa de entradas debe ingresar nombre y número de CUIT de una persona a contratar, tipo de contrato, fecha de comienzo, duración y monto, a lo que el sistema le asociará un número de minuta automáticamente. Nos recomendó leer la reglamentación vigente acerca de contratos de la que obtuvimos que los montos de los mismos no pueden superar los $25.000 y que la duración debe ser como máximo de 6 meses.

Una vez confeccionada la minuta por parte del empleado de mesa de entradas, la misma queda pendiente de aprobación. El que puede aprobar una minuta es el empleado de rendiciones. Realizamos una reunión con él y nos contó que su tarea consiste en evaluar las minutas para determinar su aprobación. También nos dijo que en otro trabajo que tiene usan un sistema llamado MiMiNuTa al que nos puede dar acceso para ver como hacen esa tarea. Después del análisis de este sistema, se concluyó que para aprobar una minuta necesitaría ingresar un número de minuta y que el sistema muestre los datos de la misma para poder aprobarla. Nos dijo que no puede aprobar la minuta si la persona a contratar tiene 3 contratos vigentes (minutas aprobadas) ni tampoco si el CUIT de la persona a contratar está inhabilitado por la AFIP. Actualmente se comunica telefónicamente con la AFIP para realizar esta verificación, pero sabe que ésta provee un servicio para aplicaciones que permite hacer la verificación en línea. Esto último nos obligó a generar una reunión con el administrador de servidores de la AFIP. Nos dijo que para poder conectarnos con un servidor de la AFIP, el sistema debe mandar un token (código que identificará de manera única a nuestra aplicación) y CUIT, si el token es correcto, el servidor responde si el CUIT está habilitado o no.

Por último el empleado de rendiciones será el responsable de imprimir los listados con las minutas aprobadas, es decir, un listado con el personal contratado para poder dárselo al jefe de departamento para que lo firme.

![image](https://user-images.githubusercontent.com/55964635/232234621-77ecdb9f-55f2-4dab-8055-571bbdf9f69f.png)

### Roles
- Empleado de mesa de entrada
- Empleado de rendiciones

### Historias de Usuario
- Confeccionar minuta
- Aprobar minuta
- Imprimir Listado

### Confeccionar minuta

<table><tr><td> 

**ID:** Confeccionar minuta
 
**TÍTULO:** Como empleado de mesa quiero confeccionar una minuta para que pueda ser aprobada

**REGLAS DE NEGOCIO:**
- El monto no puede superar los $25000
- Duración maxima de 6 meses

</td></tr><tr><td>

**CRITERIOS DE ACEPTACIÓN:** 

**Escenario 1:** Confección exitosa

Dado que el monto $1000 no supera los $25000 y la duración de 3 meses es valida

Cuando el empleado de mesa ingresa Fabian, 777, temporal, 01-01-2001, 3 meses, $1000

Entonces el sistema confecciona la minuta

---

**Escenario 2:** Confección fallida por monto superior a $25000

Dado que el monto $50000 supera los $25000 y duración 1 mes es valida

Cuando el empleado de mesa ingresa Tomas, 666, fijo, 10-10-2010, 1 mes, $50000

Entonces el sistema informa que el monto ingresado supera los $25000 y no confecciona la minuta

---

**Escenario 3:** Confección fallida porque la duración excede los 6 meses 

Dado que el monto $500 no supera los $25000 y duración 10 meses es valida

Cuando el empleado de mesa ingresa Franco, 1010, temporal, 11-11-2011, 10 meses, $500

Entonces el sistema informa que el la duración ingresada supera los 6 meses

</td></tr></table>

### Aprobar minuta

<table><tr><td> 

**ID:** Aprobar minuta
 
**TÍTULO:** Como empleado de rendiciones quiero aprobar la minuta par poder hacer un contrato en un futuro

**REGLAS DE NEGOCIO:** 
- Nro de minuta existente
- No se apruba si tiene 3 contratos vigentes
- Cuit habilitado por el AFIP (esta habilitado si el servidor responde ante el token)

Para la regla de minuta existente, podria darse el caso de que la minuta ya se haya usado o tambien podria ser el caso de que se ingreso algun nro incorreco o que directamente no exista, bueno, todos estos casos lo pongo como regla de negocio, no lo especifica en ningun lado asique queda a criterio de cada uno.

En este ejercicio tambien esta la posibilidad de `conectarnos con el servidor` para que mandemos el token y nos apruebe, pero como eso lo hace el servidor, nosotros lo vemos en segundo plano o no lo vemos directamente, por lo que no lo considero una HU (para mi)

</td></tr><tr><td>

**CRITERIOS DE ACEPTACIÓN:** 

**Escenario 1:** Aprobación de minuta exitosa

Dado que el nro de minuta 123 es valida, tiene dos contratos vigentes y el cuit esta habilitado por el AFIP

Cuando el empleado de rendiciones ingresa 123

Entonces el sistema aprueba la minuta y la agrega a un listado

---

**Escenario 2:** Aprobación fallida por minuta invalida

Dado que el nro de minuta 777 es invalido, tiene dos contratos vigentes y el cuit esta habilitado por el AFIP

Cuando el empleado de rendiciones ingresa 777

Entonces el sistema informa que la minuta ingresada es invalida y no agrega la minuta al listado

---

**Escenario 3:** Aprobación fallida por tener tres contratos vigentes

Dado que el nro de minuta 666 es valido, tiene tres contratos vigentes y el cuit esta habilitado por el AFIP

Cuando el empleado de rendiciones ingresa 666

Entonces el sistema informa que el usuario ya tiene tres contratos vigentes y no agrega la minuta al listado

---

**Escenario 4:** Aprobación fallida por cuit inhabilidato por el AFIP

Dado que el nro de minuta 404 es valido, tiene un contrato vigente y el cuit esta inhabilitado por el AFIP

Cuando el empleado de rendiciones ingresa 404

Entonces el sistema informa que el usuario tiene el CUIT inhabilitado por el AFIP

</td></tr></table>

### Imprimir Listado

<table><tr><td> 

**ID:** Imprimir listado
 
**TÍTULO:** Como empleado de rendiciones quiero imprimir el listado para poder darselo al jefe de departamento 

**REGLAS DE NEGOCIO:** 
- Existe al menos una minuta

Esta regla de negocio podria estar en duda pero bueno

</td></tr><tr><td>

**CRITERIOS DE ACEPTACIÓN:** 

**Escenario 1:** Impresión exitosa

Dado que el litado tiene 15 minutas

Cuando el empleado de rendiciones le da al boton `imprimir minutas`

Entonces el sistema imprime (o el empleado no se bien) imprime el listado 

---

**Escenario 2:** Impresión fallida por lista vacia

Dado que el listado tiene 0 minutas

Cuaando el empleado de rendiciones le da al boton `imprimir minutas`

Entonces el sistema informa que el listado se encuentra vacio

</td></tr></table>



<img src= 'https://i.gifer.com/origin/8c/8cd3f1898255c045143e1da97fbabf10_w200.gif' height="20" width="100%">

<div align = center>

## `Problema 4` Venta de bebidas

</div>

Se desea modelar un sistema para el manejo de venta de bebidas alcohólicas en linea. Para poder empezar a comprar en el sitio, es necesario que las personas se registren ingresando nombre, apellido, mail (será utilizado como nombre de usuario por lo tanto debe ser único) y edad. Solo se permite que se registren al sitio personas mayores a 18 años, de lo contrario el sistema debe mostrar en pantalla el texto de la ley que impide la venta de bebidas alcohólicas a menores. Si el registro es exitoso el sistema genera una contraseña que es enviada al mail ingresado en el registro.

Para comprar el usuario debe iniciar sesión y una vez logueado el sistema muestra una lista de bebidas, una vez que el usuario selecciona todos los productos que desea comprar, si el usuario es premium se le hace un descuento del 20% y se informa en pantalla el total menos el 20%. Ademas si el usuario seleccionó productos por un monto superior a los $4500 se le hace un 10% de descuento y se informa en pantalla el total menos el 10%. Tenga en cuenta que si el usuario es premium y compra por un monto superior a $4500 se deben aplicar ambos descuentos

![image](https://user-images.githubusercontent.com/55964635/232245201-80c3a9e9-1f85-4f5c-b3fb-02f6b06a0f46.png)
![image](https://user-images.githubusercontent.com/55964635/232245230-8f12ad19-a8dd-4c31-a99f-2de5db4ce65d.png)

### Roles
- Persona (no registrada)
- Usuario

### Historias de Usuario
- Registrar Persona
- Iniciar sesión
- Cerrar sesión
- Comprar Bebidas

<table><tr><td> 

**ID:** Registra Persona
 
**TÍTULO:** Como persona quiero registrarme para comprar bebidas

**REGLAS DE NEGOCIO:** 
- Mail unico
- Persona mayor de 18 años

</td></tr><tr><td>

**CRITERIOS DE ACEPTACIÓN:** 

**Escenario 1:** Registro exitoso

Dado que el mail menem@gmail.com es unico y la persona tiene 90 años

Cuando la persona ingresa Calos, Menem, menem@gmail.com, 90 años

Entonces el sistema registra a la persona, genera una contraseña y la manda al mail menem@gmail.com

---

**Escenario 2:** Registro fallido por mail ya registrado

Dado que el mail pepe@gmail.com no es unico y la persona tiene 30 años

Cuando la persona ingresa Pepe, ElSapo, pepe@gmail.com, 30 años

Entonces el sistema informa que el mail ya se encuentra registrado y no realiza el registro

---
**Escenario 1:** Registro fallido por persona menor de 18 años

Dado que el mail juansito@gmail.com es unico y la persona tiene 10 años

Cuando la persona ingresa Juan, Carosella, juansito@gmail.com, 10 años

Entonces el sistema muestra en pantalla la ley que impidee la venta de bebidas alcoholicas a menores


</td></tr></table>

### Iniciar sesión

<table><tr><td> 

**ID:** Iniciar Sesión
 
**TÍTULO:** Como usuario quiero iniciar sesión para poder comprar bebidas

**REGLAS DE NEGOCIO:** 

</td></tr><tr><td>

**CRITERIOS DE ACEPTACIÓN:** Iniciar Sesión

**Escenario 1:** Inicio exitoso

Dado que el usuario menem@gmail.com esta registrado y la contraseña xxxx es correcta

Cuando el usuario ingresa menem@gmail.com, xxxx

Entonces el sistema muestra un listado de bebidas para que el usuario seleccione

---

**Escenario 2:** Inicio fallido por mail no registrado

Dado que el usuario manolo@gmail.com no esta registrado

Cuando el usuario ingresa manolo@gmail.com

Entonces el sistema informa que el mail no se encuentra registrado

---

**Escenario 3:** Inicio fallido por contraseña incorrecta

Dado que el usuario diego@gmail.com esta registrado y la contraseña 20203 es correcta

Cuando el usuario ingresa diego@gmail.com, 20203

Entonces el sistema informa que la contraseña ingresada es incorrecta

</td></tr></table>

---

### Cerrar sesión

<table><tr><td> 

**ID:** Cerrar Sesión
 
**TÍTULO:** Como usuario logueado quiero cerrar mi sesión para proteger mis datos

**REGLAS DE NEGOCIO:** 

</td></tr><tr><td>

**CRITERIOS DE ACEPTACIÓN:** 

**Escenario 1:** Cierre exitoso

Dado que el usuario tiene una sesión abierta

Cuando el usuario presiona el boton `cerrar sesión`

Entonces el sistema cierra la sesión y deshabilita las opciones de selección y compra de bebidas

---

</td></tr></table>

---

### Comprar Bebidas

<table><tr><td> 

**ID:** Comprar Bebidas
 
**TÍTULO:** Como usuario logueado quiero comprar bebidas para ir a una fiesta

**REGLAS DE NEGOCIO:** 
- Es premium
- Monto superior a $4500

Aca puede darse el caso de que el usuario le diera al boton comprar sin haber seleccionado ninguna bebida, creo que lo podria agregar como otro escenario.

</td></tr><tr><td>

**CRITERIOS DE ACEPTACIÓN:** 

**Escenario 1:** Compra exitosa con 30% de decuento

Dado que el usuario messi@gmail.com es premium y su compra es de $50000

Cuando el usuario selecciona las bebidas y le da al boton `comprar`

Entonces el sistema aplica un descuento del 30% sobre el total y registra la compra

---

**Escenario 2:** Compra exitosa con 20% de decuento

Dado que el usuario benzema@gmail.com es premium y su compra es de $50

Cuando el usuario selecciona las bebidas y le da al boton `comprar`

Entonces el sistema aplica un descuento del 20% sobre el total y registra la compra

---

**Escenario 3:** Compra exitosa con 10% de decuento

Dado que el usuario guardiola@gmail.com no es premium y su compra es de $20000

Cuando el usuario selecciona las bebidas y le da al boton `comprar`

Entonces el sistema aplica un descuento del 10% sobre el total y registra la compra

---

**Escenario 4:** Compra exitosa sin descuentos

Dado que el usuario messi@gmail.com no es premium y su compra es de $2

Cuando el usuario selecciona las bebidas y le da al boton `comprar`

Entonces el sistema no aplica un descuento sobre el total y registra la compra

</td></tr></table>

<img src= 'https://i.gifer.com/origin/8c/8cd3f1898255c045143e1da97fbabf10_w200.gif' height="20" width="100%">

<div align = center>

## `Problema 5` Casa de fotografía
</div>


Se desea desarrollar un sistema para la impresión de fotos para una casa fotográfica. Los clientes pueden subir sus fotos, pagar por internet y luego ser retiradas personalmente por el local.

Para subir las fotos la persona debe registrarse en el sitio, ingresando sus datos personales, nombre, apellido, email, domicilio, nombre de usuario y contraseña.

Una vez autenticado, el usuario puede subir un máximo de 50 fotos para ser impresas. Las fotos se ingresan de a una. Una vez subidas, el usuario debe abonar el monto total (el valor de cada foto es de $15). El pago se realiza con tarjeta de crédito, ingresando los datos de la misma (número de tarjeta, código de seguridad y nombre del titular), la cual debe ser validada a través del sistema del banco. Una vez que se realiza el pago se le otorga al cliente un código único que le servirá posteriormente para retirar las fotos.

Un cliente debe acercarse a la sucursal para retirar las fotos enviadas previamente. Para esto debe presentar el código único a un empleado. Este registra el código, la fecha de retiro y entrega las fotos al cliente.

![image](https://user-images.githubusercontent.com/55964635/232247520-3ee3818c-84f9-42c4-b49c-f344f7844377.png)

---

### Roles
- Persona (No registrada)
- Usuario
- Empleado

### Historias de Usuario
- Registrar Persona
- Iniciar Sesión
- Cerrar Sesión
- Pagar con tarjeta
- Subir Foto
- Retirar Foto

---

### Registrar Persona

<table><tr><td> 

**ID:** Registrar Persona
 
**TÍTULO:** Como persona quiero registrame para poder subir fotos

**REGLAS DE NEGOCIO:** 
- nombre de usuario no registrado 

Aunque el enuncado no lo especifica, despues le pregunto al ayudante si va

</td></tr><tr><td>

**CRITERIOS DE ACEPTACIÓN:** 

**Escenario 1:** Registro exitoso

Dado que el nombre de usuario manolo20 no esta registrado

Cuando la persona ingresa Manolo, Cuevas, manolo@gmail.com, 24 entre 51 y 50, manolo20, contraseña123

Entonces sistema realiza el registro del usuario y lo informa en pantalla

---

**Escenario 2:** Registro Fallido por usuario ya existente

Dado que el nombre de usuario vegeta666 esta registrado

Cuando la persona ingresa Vegeta, Sayan, vegeta@gmail.com, 1 entre 22 y 23, vegeta666, nameku1000

Entonces sistema informa que el usuario ya se encuentra registrado en el sistema

</td></tr></table>

---

### Iniciar Sesión

<table><tr><td> 

**ID:** Iniciar Sesión
 
**TÍTULO:** Como usuario quiero iniciar sesión para poder comprar las fotos

**REGLAS DE NEGOCIO:** 

</td></tr><tr><td>

**CRITERIOS DE ACEPTACIÓN:** Iniciar Sesión

**Escenario 1:** Inicio Exitoso

Dado que el manolo20 se encuentra registrado y la contraseña contraseña123 es correcta

Cuando el usuario ingresa manolo20, contraseña123

Entonces el sistema realiza el inicio de sesión y habilita la opcion para subir imagenes y pagar

---

**Escenario 2:** Inicio Fallido por usuario no registrado

Dado que el goku50 no se encuentra registrado

Cuando el usuario ingresa goku50

Entonces el sistema informa que el usuario no se encuentra registrado

---

**Escenario 3:** Inicio Fallido por contraseña incorrecta

Dado que el manolo20 se encuentra registrado y la contraseña contraseña123 es correcta

Cuando el usuario ingresa manolo20, contraseña123

Entonces el sistema informa que la contraseña es incorrecta

</td></tr></table>

---

### Cerrar Sesión

<table><tr><td> 

**ID:** Cerrar Sesión
 
**TÍTULO:** Como usuario logueado quiero cerrar mi sesión para proteger mis datos

**REGLAS DE NEGOCIO:** 

</td></tr><tr><td>

**CRITERIOS DE ACEPTACIÓN:** 

**Escenario 1:** Cierre exitoso

Dado que el usuario manolo20 tiene la sesión abierta

Cuando el usuario presiona el boton `cerrar sesión`

Entonces el sistema cierra la sesión y deshabilita las opciones para subir imagenes y pagar


</td></tr></table>

---

### Pagar con tarjeta

<table><tr><td> 

**ID:** Pagar con tarjeta
 
**TÍTULO:** Como usuario quiero pagar con tarjeta para poder retirar las fotos

**REGLAS DE NEGOCIO:** 
- Fondos para pagar $15 por foto

</td></tr><tr><td>

**CRITERIOS DE ACEPTACIÓN:** 

**Escenario 1:** Pago exitoso

Dado que se pudo establecer conexión con el servidor, el nro de tarjeta 4342 es correcto y posee fondos suficientes para pagar $15 por foto

Cuando el usuario ingresa 4342, 012, Fabian

Entonces el sistema registra el pago y retorna un nro para que pueda retirar las fotos

---

**Escenario 2:** Pago fallido por falta de conexión con el servidor

Dado que no se pudo establecer conexión con el servidor

Cuando el usuario intenta pagar

Entonces el sistema informa que no hay conexión con el banco y no realiza el pago

---

**Escenario 3:** Pago fallido por nro de tarjeta invalido

Dado que se pudo establecer conexión con el servidor, el nro de tarjeta 9578 no es correcto

Cuando el usuario ingresa 9578, 23, Jordan

Entonces el sistema informa que el nro de tarjeta es invalido y no registra el pago

---

**Escenario 4:** Pago fallido por fondos insuficientes

Dado que se pudo establecer conexión con el servidor, el nro de tarjeta 8414 es correcto y no posee fondos suficientes para pagar $15 por foto

Cuando el usuario ingresa 8414, 010, Messi

Entonces el sistema informa que la tarjeta no posee fondos suficientes y no registra el pago

</td></tr></table>

---

### Subir Foto

<table><tr><td> 

**ID:** Subir Foto
 
**TÍTULO:** Como usuario quiero subir foto para luego retirarla

**REGLAS DE NEGOCIO:** 
- Un maximo de 50 fotos
- Se suben de a una
- El pago debe realizarse con tarjeta de credito


</td></tr><tr><td>

**CRITERIOS DE ACEPTACIÓN:** 

**Escenario 1:** Subida exitosa

Dado que el usuario subio 20 fotos y fueron una a la vez 

Cuando el usuario sube perros.png

Entonces el sistema carga la foto 

---

**Escenario 2:** Subida fallida por cantidad excesiva de fotos

Dado que el usuario subio 51 fotos y fueron una a la vez 

Cuando el usuario sube gatos.png

Entonces el sistema informa que el usuario no puede subir mas de 50 imagenes 

---

**Escenario 1:** Subida fallida por subir mas de una foto a la vez

Dado que el usuario subio 3 fotos, fueron a la vez 

Cuando el usuario sube perros.png, gatos.png, ratas.png

Entonces el sistema informa que el usuario esta subiendo mas de una foto a la vez

---

</td></tr></table>

---

### Retirar Foto

<table><tr><td> 

**ID:** Retirar Foto
 
**TÍTULO:** Como empleado quiero retirar las fotos para darselas al cliente

**REGLAS DE NEGOCIO:** 
- El codigo debe estar cargado en el sistema

</td></tr><tr><td>

**CRITERIOS DE ACEPTACIÓN:** 

**Escenario 1:** Retiro exitoso

Dado que el codigo 4321 esta cargado en el sistema

Cuando el empleado ingresa 4321

Entonces el sistema imprime las fotos 

---

**Escenario 1:** Retiro fallido por codigo inexistente

Dado que el codigo 6353 no esta cargado en el sistema

Cuando el empleado ingresa 6353

Entonces el sistema informa que el codigo ingresado no existe en el sistema

</td></tr></table>

<img src= 'https://i.gifer.com/origin/8c/8cd3f1898255c045143e1da97fbabf10_w200.gif' height="20" width="100%">

<div align = center>

## `Problema 6` Biblioteca

</div>

La biblioteca de una escuela primaria realiza su trabajo de forma manual y requiere un sistema informático que automatice su funcionamiento.

La bibliotecaria recibe libros por donaciones de los padres de los chicos que asisten a la escuela. De un mismo libro se pueden tener varios ejemplares.

Para que un alumno pueda asociarse debe presentar el DNI y certificado de alumno regular. Una vez asociado, se le otorga un carnet con su correspondiente número de socio.

Los préstamos se realizan exclusivamente a socios habilitados, que no posean más de tres préstamos vigentes y no tengan préstamos vencidos. La bibliotecaria presta libros que se encuentren en buen estado. Cuando un libro se encuentra deteriorado ya no se presta.

Cuando el socio retorna un libro se verifica si el préstamo se encuentra vencido. En este caso, la bibliotecaria suspende al socio, que por 15 días no podrá solicitar nuevos préstamos.

![image](https://user-images.githubusercontent.com/55964635/232251137-9bbf9a21-f02d-4908-a670-8512253fcd11.png)

---

### Roles

- Alumno (No asociado)
- Socio
- Bibliotecario

### Historias de Usuario

- Asociar alumno
- Prestar libro
- Devolver libro

---

### Asociar alumno
<table><tr><td> 

**ID:** Asociar alumno
 
**TÍTULO:** Como alumno me quiero asociar para poder retirar libros

**REGLAS DE NEGOCIO:** 
- Ser alumno regular

</td></tr><tr><td>

**CRITERIOS DE ACEPTACIÓN:** 

**Escenario 1:** Asociación exitosa

Dado que es un alumno regular

Cuando el alumno ingresa 203200 y entrega el certificado de alumno regular

Entonces el sistema asocia al alumno y le otorga un carnet con un nro de socio

---

**Escenario 1:** Asociación fallida por ser alumno irregular

Dado que es un alumno irregular

Cuando el alumno ingresa 12340 y no entrega el certificado de alumno regular

Entonces el sistema informa que no es alumno regular y no entrega el carnet


</td></tr></table>

### Prestar Libro

<table><tr><td> 

**ID:** Prestar Libro
 
**TÍTULO:** Como bibliotecaria quiero prestar un libro para que el socio lo pueda leer

**REGLAS DE NEGOCIO:** 
- No posee mas de tres prestamos vigentes
- No tener prestamos vencidos
- Libro en buen estado



</td></tr><tr><td>

**CRITERIOS DE ACEPTACIÓN:** 

**Escenario 1:** Prestamo exitoso

Dado que le socio 1 posee dos prestamos vigentes, no tiene prestamos vencidos y el libro "Harry Potter" esta en buen estado

Cuando el socio presenta carnet y solicita el libro "Harry Potter"

Entonces el sistema registra el prestamo en el sistema

---

**Escenario 1:** Prestamo Fallido por poseer tres prestamos vigentes

Dado que le socio 1 posee dos prestamos vigentes, no tiene prestamos vencidos y el libro "Harry Potter" esta en buen estado

Cuando el socio presenta carnet y solicita el libro "Harry Potter"

Entonces el sistema registra el prestamo en el sistema

---

**Escenario 1:** Prestamos fallido por tener prestamos vendidos

Dado que le socio 1 posee dos prestamos vigentes, no tiene prestamos vencidos y el libro "Harry Potter" esta en buen estado

Cuando el socio presenta carnet y solicita el libro "Harry Potter"

Entonces el sistema registra el prestamo en el sistema

---

**Escenario 1:** Prestamo fallido por libro en mal estado

Dado que le socio 1 posee dos prestamos vigentes, no tiene prestamos vencidos y el libro "Harry Potter" esta en buen estado

Cuando el socio presenta carnet y solicita el libro "Harry Potter"

Entonces el sistema registra el prestamo en el sistema

</td></tr></table>

### Devolver Libro

<table><tr><td> 

**ID:** 
 
**TÍTULO:** 

**REGLAS DE NEGOCIO:** 

</td></tr><tr><td>

**CRITERIOS DE ACEPTACIÓN:** 

**Escenario 1:** título del criterio.

Dado 

Cuando 

Entonces 

---

</td></tr></table>

<img src= 'https://i.gifer.com/origin/8c/8cd3f1898255c045143e1da97fbabf10_w200.gif' height="20" width="100%">

<div align = center>

## `Problema 7` Mutual

</div>

Una mutual necesita automatizar el manejo de las prestaciones que ofrece a sus afiliados.

Una persona puede afiliarse sólo si posee una tarjeta de crédito para que se pueda hacer el pago de la cuota mensual
automáticamente. Una vez que la persona se ha afiliado, puede pasar a tener a cargo a su pareja e hijos (hasta 18 años,
luego es dado de baja). A cada uno se le otorga un número de afiliado.

Las prestaciones que brinda, siempre y cuando esté asentado el pago del mes anterior al que es solicitado, son:

- `Ortodoncia`: Se reconoce sólo una y a los afiliados menores de 15 años que estén afiliados desde al menos nueve meses. Debe presentarse historia clínica elaborado por el profesional.
- `Plantillas`: A cualquier afiliado, hasta dos por año calendario. Debe presentarse la indicación del profesional y factura del comercio que la confeccionó.
- `Anteojos`: A cualquier afiliado con fecha de afiliación superior a tres meses, un par cada 18 meses.
- `Internación`: A cualquier afiliado, sin límite.
- `Consultas médicas`: A cualquier afiliado, hasta 2 por mes.

<img src= 'https://i.gifer.com/origin/8c/8cd3f1898255c045143e1da97fbabf10_w200.gif' height="20" width="100%">

<div align = center>

## `Problema 8` Teatro

</div>

Se desea modelar un sistema de gestión de ventas de entradas para un teatro. Las personas compran sus entradas a través de una página web, o personalmente.

El sistema permite, sólo de modo personal en el teatro, la reserva de entradas de forma gratuita. El empleado debe ingresar los datos de la obra (fecha, hora, y nombre) junto el nombre y DNI del espectador. En este caso, sólo se podrá reservar hasta 2 entradas. Las entradas reservadas no compradas caducarán tres horas antes del evento. Para seleccionar el nombre de la obra, el sistema muestra una grilla de funciones disponibles para que el usuario seleccione una.

Para comprar una entrada vía web, el sistema muestra la grilla de funciones disponibles. El usuario selecciona una opción, ingresa su DNI, la cantidad de lugares solicitados y selecciona la opción “pagar”. El pago se realiza con tarjeta de crédito. Para esto debe ser autorizada a través del sistema del banco. Este pide el número de tarjeta, vencimiento, y código de seguridad. Verifica todos los campos y autoriza la compra. Autorizada la tarjeta, se emite un código de compra con el que el cliente podrá retirar sus entradas en la boletería del cine.

Para comprar una entrada personalmente, el vendedor de la boletería solicita los datos de la función al cliente, procediendo de un modo similar a la compra web, con la diferencia que en este caso no se muestra el código de compra sino que se imprimen directamente la/s entrada/s. El pago es unicamente con tarjeta de crédito, igual que en el caso anterior.

Para retirar las entradas reservadas previamente, el empleado solicita nombre y DNI del espectador, el sistema valida que la persona posea entradas reservadas, y que no estén caducas. El resto del procedimiento se realiza igual que la compra de entradas descriptas anteriormente.

Cuando una persona llega con el código de compra, el vendedor debe ingresar el código para que el sistema, luego de verificarlo, imprima las entradas correspondientes.

Además se desea administrar la programación de las salas. El administrador ingresa la distribución semanal de las obras en las salas de manera que se encuentre disponible para la realización de la venta de entradas

<img src= 'https://i.gifer.com/origin/8c/8cd3f1898255c045143e1da97fbabf10_w200.gif' height="20" width="100%">

<div align = center>

## `Problema 9` Pago Electrónico

</div>

Se desea modelar un sistema de pago electrónico de impuestos y servicios en efectivo.

Cuando un cliente llega para realizar un pago, el empleado o el gerente de la sucursal ingresa el código de pago
electrónico y el sistema se conecta con la central de cobro para recuperar los datos de la factura (empresa, nro de
cliente, 1era fecha de vencimiento, 2da fecha de vencimiento, recargo, y monto original). Una vez recuperados los datos,
el sistema debe verificar los vencimientos para determinar el monto a cobrar. Teniendo esto en cuenta, cuando el 2do
vencimiento está vencido se debe informar que la factura no se puede cobrar por dicho motivo. Cuando el 1er
vencimiento está vencido hay que aplicar el recargo al monto original. Si la factura no está vencida, se cobra el monto
original.

Una vez al día, el gerente de la sucursal debe registrar en la central de cobros los pagos que hicieron los clientes.
Para esto el sistema requiere la clave maestra y de ser correcta, recupera las transacciones de los impuestos y servicios
cobrados en el día, se conecta a la central de cobro y se las envía. Cuando la central confirma la recepción exitosa, el
sistema las registra como enviadas. Este último paso es importante porque no deben enviarse dos veces las
transacciones. Si el gerente intenta enviar una segunda vez, el sistema no debe permitirlo.

Finalmente el Gerente puede ver las estadísticas de los impuestos y servicios cobrados. Para esto, se ingresa la clave
maestra, un rango de fechas sobre las cuales debe calcularse las estadísticas y el sistema debe mostrar los montos y la
cantidad de cobros realizados, agrupando por empresa.

Tenga en cuenta que cada vez que el sistema debe conectarse a la central, debe enviarle un token (código que
identifica al sistema). Una vez que la central valida el token, el sistema envía el requerimiento para recuperar los datos de
la factura o el requerimiento para registrar los pagos del día según corresponda

<img src= 'https://i.gifer.com/origin/8c/8cd3f1898255c045143e1da97fbabf10_w200.gif' height="20" width="100%">

<div align = center>

## `Problema 10` Un Aventón

</div>

Se desea desarrollar un sistema que permita compartir un vehículo para un viaje. La idea es que cuando una persona tiene que realizar un viaje lo publique en la aplicación. Luego, el resto de los usuarios se postulan para acompañarla y el chofer podrá seleccionar quienes viajan. El objetivo es abaratar costos y evitar congestiones en el tránsito. El sistema es gratuito.

Para utilizar el sistema, una persona debe registrarse y estar correctamente identificado antes de poder utilizarlo. Al registrarse, se pide un nombre de usuario, un correo electrónico y una contraseña. No puede haber dos correos electrónicos iguales en el sistema. Una vez autenticado, podrá dar de alta diferentes viajes, identificando la fecha, hora y el automóvil que utilizará. Los diferentes viajes que una persona publique no pueden superponerse. Un usuario que adeuda calificaciones tampoco podrá publicar un viaje.

Cualquier usuario identificado podrá postularse a un viaje. Luego, el usuario dueño del viaje podrá aceptar o rechazar los candidatos para que realicen el viaje con él.

En el sistema existe una política de reputaciones que permiten a los usuarios conocer la opinión del resto sobre los viajes realizados. Luego de terminado un viaje, tanto el piloto como los copilotos que viajaron deberán calificarse entre sí. El piloto califica a todos sus copilotos. Cada copiloto califica al piloto del viaje. Las calificaciones podrán ser positivas (suma un punto de reputación) o negativas (restan un punto de reputación)

<img src= 'https://i.gifer.com/origin/8c/8cd3f1898255c045143e1da97fbabf10_w200.gif' height="20" width="100%">

<div align = center>

## `Problema 11` Concursos

</div>

Suponga que el área para la cual trabaja fue contactada para implementar un sistema para el manejo de concursos de los docentes de la Facultad de Informática.

El docente que quiera inscribirse a un concurso deberá registrarse previamente en el sistema. Para esto deberá ingresar los siguientes datos: Dni, nombre, apellido y dirección de mail. Una vez completado los datos el sistema mandará a la casilla de correo ingresada la contraseña asignada automáticamente. El mail debe ser único y será utilizado como nombre de usuario. Según el estatuto de la UNLP los dni permitidos para concursar son aquellos menores a 55 millones y mayores a 12 millones.

Una vez registrado el docente puede inscribirse al concurso, para lo cual, una vez que haya ingresado al sistema, deberá seleccionar la materia a la cual desea inscribirse. Según el reglamento interno de la Facultad de informática que nos facilitó el jefe del área de personal, el docente no podrá inscribirse a más de 3 concursos. Cuando el docente acepta la inscripción el sistema deberá imprimir un comprobante.

Por último, para cumplir con la ordenanza número 123/19 de la UNLP, el jefe del área de concursos, el cual ya cuenta con un nombre de usuario y contraseña, deberá poder imprimir un listado con los inscriptos a una materia determinada para poder enviar dicho listado al secretario administrativo quien lo firma y eleva al decano de la Facultad. Suponga que el sistema Siu-Guarani realiza una tarea similar a la solicitada y que puede consultar su implementación y registros.

<img src= 'https://i.gifer.com/origin/8c/8cd3f1898255c045143e1da97fbabf10_w200.gif' height="20" width="100%">

<div align = center>

## `Problema 12` Créditos bancarios

</div>

Se desea modelar mediante historias de usuario el manejo de créditos otorgados por un banco a sus clientes.

Los clientes que desean pedir un crédito, deben iniciar un trámite a través de un sitio web del banco ingresando dni, nombre, apellido, mail, tipo de crédito (personal, vivienda, etc.) y monto solicitado. El sistema acepta el inicio de trámite si el dni ingresado corresponde a un cliente del banco y si el crédito solicitado no supera los $400.000. En caso de que no sea cliente del banco el sistema deberá enviar un correo electrónico al email ingresado con un instructivo para hacerse cliente del banco. Si el monto supera los $400.000 el sistema rechaza el inicio de trámite y muestra el mensaje “El monto solicitado excede el límite permitido”. Si los datos son correctos, el sistema almacena el trámite para que sea analizado por el área económica e imprime un número de comprobante para el cliente.

Por otro lado, los clientes pueden consultar el estado de un trámite, para esto es necesario que se ingrese un número de comprobante. Si el número de comprobante es válido, el sistema retorna un informe con el estado del mismo, de lo contrario mostrará un mensaje “trámite inexistente”. Si el cliente ingresa tres veces un código inexistente el sistema bloquea la ip (dirección de red de la máquina que efectúa la consulta) del cliente por 24 horas mostrando un mensaje “Usted ha excedido el número de consultas inválidas”.

Por último, el gerente del banco puede pedir un listado de créditos aprobados entre fechas. Si las fechas ingresadas son válidas, el sistema mostrará un listado con los créditos aprobados, de lo contrario mostrará un mensaje “las fechas ingresadas no son válidas”. El sistema utiliza un sistema de autenticación general del banco, por lo que no es necesario modelar el iniciar y cerrar sesión. Si no hay créditos aprobados para las fechas ingresadas el sistema mostrará el siguiente mensaje: ”No hay créditos aprobados en las fechas ingresadas”.

<img src= 'https://i.gifer.com/origin/8c/8cd3f1898255c045143e1da97fbabf10_w200.gif' height="20" width="100%">

<div align = center>

## `Problema 12` Venta de libros

</div>

Una nueva empresa de venta de libros en línea está diseñando su sitio web. Cualquier visitante puede acceder a su catálogo de libros y navegar los distintos libros que se encuentren en él y solo los usuarios registrados pueden realizar compras.

Para poder comprar los libros se necesita un usuario registrado. El proceso de registro se realiza en dos pasos. En el primer paso el sistema requiere Nombre, Apellido, DNI y cuenta de correo electrónico (que no exista en el sistema) y una clave de 6 caracteres para darlo de alta de forma parcial. En este proceso el sistema debe generar un código de 16 dígitos y enviarlo por correo para que luego el visitante confirme la cuenta. Como segundo paso el visitante debe entrar a la página de confirmación e ingresar su dirección de correo y el código de 16 dígitos. Si estos datos son correctos el sistema lo registra definitivamente como usuario.

Una vez registrado, para autenticarse, el sistema requiere el correo del usuario y la clave de 6 caracteres.

Para realizar la compra de un libro el sistema pide ingresar el ISBN del mismo y muestra al usuario la portada con una descripción del libro y la opción “Comprar”. Cuando el usuario selecciona “Comprar” se le pide los datos de la tarjeta:

Apellido, Nombre, Nro de tarjeta. Es importante tener en cuenta que por disposición del Banco Central solo el titular de la tarjeta puede realizar la compra, por lo que el nombre y apellido registrado debe coincidir con el de la tarjeta. Realizada esta verificación se procede a enviar los datos al servidor de la tarjeta para realizar el cobro. Si todo es correcto
se genera un enlace de descarga al correo del usuario

<img src= 'https://i.gifer.com/origin/8c/8cd3f1898255c045143e1da97fbabf10_w200.gif' height="20" width="100%">

<div align = center>

## `Problema 13` Manejo de tarjetas de crédito

</div>

La gerencia del banco donde trabajamos nos pide realizar un subsistema para el manejo de las tarjetas de crédito SIVA. El sistema podrá ser operado únicamente por el personal de área comercial y por el gerente de la sucursal. En ambos casos las funcionalidades solo serán habilitadas con autenticación previa.

El registro del personal en el sistema no es necesario implementarlo, ya que las credenciales son obtenidas del sistema central del banco. Entonces, para autenticarse, el usuario debe ingresar sus credenciales (las mismas que usa para otros servicios del banco) y estas son corroboradas por el sistema del banco central (al cual nos comunicamos por intranet), enviándonos un token de autenticación válido en caso de ser correctas. 

Una vez autenticado, todo el personal debe poder dar de alta una nueva tarjeta y dar de baja una existente. Para dar de alta se requiere nombre completo, DNI y CUIT del titular. Luego, se debe seleccionar un tipo de tarjeta (Básica o Gold). Para dar de alta la tarjeta la persona debe ser cliente del banco y no podrá darse de alta una tarjeta si la persona es morosa en el sistema SIVA (externo al banco). Para esto, nuestro sistema debe comunicarse con el SIVA y verificar la morosidad de la persona con el DNI. En el mismo momento, el sistema SIVA nos dará un número de tarjeta nuevo.

Para dar de baja una tarjeta, simplemente se debe ingresar el número de tarjeta y el sistema la debe eliminar de la base de datos del banco. El gerente, además, podrá pedir un listado de las operaciones realizadas entre dos fechas. Para esto el sistema le pedirá que ingrese ambas fechas y le mostrará un listado. No debe ser posible ingresar fechas futuras al presente, ni tampoco que la fecha de inicio sea mayor a la fecha de fin

<img src= 'https://i.gifer.com/origin/8c/8cd3f1898255c045143e1da97fbabf10_w200.gif' height="20" width="100%">

<div align = center>

## `Problema 13` Manejo de canchas de tenis

</div>

Suponga que la consultora para la cual trabaja ha sido contactada para realizar un sistema para el manejo de turnos en
canchas de tenis.

Luego de varias reuniones con el cliente se ha concluido que es necesario la realización de un sistema web donde las
personas interesadas puedan obtener turnos en diferentes canchas de tenis de un complejo. Para esto las personas
deben registrarse en la plataforma indicando nombre, apellido, mail (será utilizado como nombre de usuario), edad y
domicilio. El cliente nos ha indicado que solo quiere que se registren personas mayores de edad (18 años o más). Una vez
que la persona se registra con éxito el sistema genera una contraseña que será enviada al correo que ha sido ingresado.
Una vez registrada la persona puede solicitar turnos en una cancha del complejo, para esto debe iniciar sesión
previamente. El cliente desea que si un usuario falla tres veces al iniciar sesión su cuenta sea bloqueada.

Para solicitar un turno, el usuario ingresa cancha, fecha y hora. Si la cancha está libre el turno se le asigna al usuario
informando “Su turno ha sido registrado con éxito”, si la cancha está ocupada se le informará “Cancha ocupada, por favor
seleccione otro día y horario”, dándole la posibilidad de volver a seleccionar un turno nuevo. El sistema no debe permitir
dar turno con menos de 2 días a la fecha en que se solicita.

<img src= 'https://i.gifer.com/origin/8c/8cd3f1898255c045143e1da97fbabf10_w200.gif' height="20" width="100%">

<div align = center>

## `Problema 14` Procesamiento de imágenes

</div>

Se desea modelar un sub-sistema de procesamiento de imágenes astronómicas para un observatorio. El objetivo del sub-sistema será cargar una imagen, que un usuario experto la analice y recorte ciertas áreas de interés.

Para poder usar el sistema, el operario debe autenticarse. Para esto, el sub-sistema se conecta al sistema general del observatorio (no administrado por nosotros) para validar las credenciales (nombre de usuario y contraseña). De ser correctas, el sistema de autenticación retorna un token indicando la autenticación correcta. Al terminar de usar el sistema, el usuario debe cerrar la sesión.

Una vez autenticado, el operario debe poder hacer dos operaciones principales: cargar una imagen nueva y recortar áreas de interés. Para cargar una nueva imagen, el sistema debe mostrar una serie de archivos posibles donde el usuario debe seleccionar el deseado. El sistema no debe mostrar como opciones imágenes que tengan menos de 2Megapixeles de resolución. Una vez seleccionada la imagen, el sistema debe mostrar la opción de visualizarla en escala de grises o a color. El usuario puede seleccionar la opción que quiera.

Para recortar áreas de interés, debe haber previamente cargada una imagen. No se podrán recortar más de 4 áreas. El sistema dejará al usuario que marque consecutivamente cada área de interés. Si algún área se superpone con otra el sistema debe notificarlo como un error. Una vez seleccionadas las áreas, el sistema almacena en disco los resultados.

Por último, debe existir un usuario supervisor, que además de las funcionalidades del operario, también podrá pedir un listado de las últimas imágenes procesadas. El supervisor debe poder seleccionar entre qué fechas mostrar el listado. Luego el sistema mostrará una debajo de la otra todas las imágenes procesadas. Por cuestiones de visualización, el sistema no debe permitir mostrar más de 20 imágenes a la vez.

<img src= 'https://i.gifer.com/origin/8c/8cd3f1898255c045143e1da97fbabf10_w200.gif' height="20" width="100%">