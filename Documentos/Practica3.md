<div align="center">

[![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/Nomadiix/IS1)
[![GitHub stars](https://img.shields.io/github/stars/Nomadiix/IS1)](https://github.com/FabianMartinez1234567/IS1/stargazers/)
[![GitHub repo size in bytes](https://img.shields.io/github/repo-size/Nomadiix/IS1)](https://github.com/Nomadiix/IS1)
 </div>
 
<h1 align="center"> 👥 Practica 3</h1>

</div>



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
- [4) Máquina de reciclado](#problema-4-máquina-de-reciclado)
- [5) Impresión de Fotos](#problema-5-impresión-de-fotos)
- [6) Ventas de Entradas para Teatro](#problema-6-ventas-de-entradas-para-teatro)
- [7) Préstamos Personales](#problema-7-préstamos-personales)
- [8) Pago de Impuestos y Servicios](#problema-8-pago-de-impuestos-y-servicios)
- [9) Un Aventón](#problema-9-un-aventón)
- [10) Gimnasio](#problema-10-gimnasio)
- [11) Carga de empleados](#problema-11-carga-de-empleados)

<img src= 'https://i.gifer.com/origin/8c/8cd3f1898255c045143e1da97fbabf10_w200.gif' height="20" width="100%">

Quiero aclarar que estos colores los elegi yo porque a mi me gustaron, no es nada especifico de la catedra

| Colores Para identificar      | ![Color Picker Boxes](https://draculatheme.com/static/img/color-boxes/eyedropper.png)   |
| ------------ | --------------------------------------------------------------------------------------- |
| Verifica el sistema         | ![Cyan Color](https://draculatheme.com/static/img/color-boxes/cyan.png)                 |
| Casos de uso       | ![Orange Color](https://draculatheme.com/static/img/color-boxes/orange.png)             |
| Datos solicitados o que debe realizar       | ![Purple Color](https://draculatheme.com/static/img/color-boxes/purple.png)             |
| Actores       | ![Yellow Color](https://draculatheme.com/static/img/color-boxes/yellow.png)             |

Para cada Historia de Usuario se deben indicar los siguientes ítems:

---

<table ><tr><td width="660"> 

**Nombre:** 
 
**Descripción:** 

**Actores:** 

**Precondiciones:** 

---

CURSO NORMAL<table> <tr><td>Acciones del actor</td> <td>Acciones del Sistema</td></tr>
<td width="320">  

Paso x:

</td><td width="320">

Paso x: 

</td></table>

---

**Curso alterno:**

**Postcondición:**

</table>


---

<div align = 'center'>

## `Problema 1` Alquiler de mobiliario

</div>

Suponga que trabaja en una consultora la cual ha sido recientemente contactada por una empresa de alquiler de mobiliario para eventos para la realización de una app.

De las diferentes entrevistas se ha obtenido la siguiente información:

El gerente nos dijo que resulta fundamental tener una aplicación móvil que nos permita manejar la agenda de la empresa, sabiendo qué disponibilidad tenemos y permitiendo que nuestros clientes alquilen a través de la app. Para esta primera versión de la app, el gerente nos pidió que sea posible dar de alta los diferentes mobiliarios, así como la posibilidad de que los usuarios puedan realizar una reserva de alquiler desde sus dispositivos. Para el detalle de cómo se realiza la carga de los muebles, el gerente nos sugirió hablar con el encargado del departamento de mobiliario. El encargado de mobiliario nos comentó que de cada mueble se debe cargar código de inventario, tipo de mueble, fecha de creación, fecha de último mantenimiento, estado (libre, de baja, alquilado) y el precio de alquiler. Además, no pueden existir códigos repetidos y por el contrato de la franquicia, el precio debe cargarse en dólares. Para que el encargado pueda dar de alta el mobiliario debe autenticarse en el sistema. El registro de los usuarios de carga no debe modelarse.

El encargado del departamento de alquileres no comentó acerca de las reservas de los alquileres. Por una política comercial de la marca una reserva tiene que incluir como mínimo 3 muebles. La reserva debe tener una fecha, lugar del evento, cantidad de días y mobiliario junto a su cantidad. Para realizar una reserva se debe abonar el 20% del total del alquiler. El pago de la reserva se realiza únicamente con tarjeta de crédito validando número de tarjeta y fondos a través de un servicio del banco. Luego de efectuado el pago, se emite un número de reserva único que será luego utilizado por el cliente para hacer efectivo el alquiler.

---

### Actores
- Usuario
- Servidor del banco
- Encargado mobiliario

### Casos de Uso
- Reservar alquiler
- Autenticarse en el sistema (No hay que modelar)
- Carga mueble
- Pagar con tarjeta

---

- [Imagen Completa](/Practicas/Practica%203/Imagenes/1.jpg)

### Diagrama

![](2023-05-04-13-36-00.png)

---

<div align="center">

### Reservar Alquiler

<table ><tr><td width="660"> 

**Nombre:** Reservar Alquiler
 
**Descripción:** Este cu describe la forma en la que un usuario realiza la reserva de un alquiler

**Actores:** Usuario

**Precondiciones:** ---

---

CURSO NORMAL<table> <tr><td>Acciones del actor</td> <td>Acciones del Sistema</td></tr>
<td width="320">  

Paso 1: El usuario selecciona la opcion `Reservar alquiler`

Paso 3: El usuario ingresa los datos solicitados

</td><td width="320">

Paso 2: El Sistema solicita al fecha, lugar del evento, cantidad de dias y mobiliario junto a su cantidad

Paso 4: El sistema verifica que la cantidad ingresada no sea menor a 3

Paso 5: El sistema ejecuta el caso de uso `pagar con tarjeta `

Paso 6: El sistema registra la reserva del alquiler y emite un codigo de reserva unico

</td></table>

---

**Curso alterno:** 
- Paso alternativo 4:La cantidad ingresada es menor a 3. Se informa que minimo se incluyen 3. Retoma al paso 2
- Paso alternativo 5: El pago no se realiza. Se notifica al usuario. Fin de CU

**Postcondición:** Se registro una reserva y se emitió un nro de reserva único

</table>


---

### Pagar con tarjeta

<table ><tr><td width="660"> 

**Nombre:** Pagar con tarjeta
 
**Descripción:** Este cu describe el cobro de una reserva de alquiler mediante una tarjeta

**Actores:** Usuario, Servidor del banco

**Precondiciones:** Se debe haber ejecutado el CU `Reservar Alquiler`

---

CURSO NORMAL<table> <tr><td>Acciones del actor</td> <td>Acciones del Sistema</td></tr>
<td width="320">  

Paso 2: El usuario ingresa datos solicitados 

Paso 4: El servidor del banco acepta la conexión y solicita nro de tarjeta y codigo de seguridad

Paso 6: El servidor del banco valida los datos de la tarjeta y fondos suficientes para abonar el 20% total del alquiler

Paso 7: El servidor del banco retorna el resultado

</td><td width="320">

Paso 1: El sistema solicita nro de tarjeta y codigo de seguridad 

Paso 3: El sistema solicita conexión con el servidor del banco

Paso 5: El sistema envia los datos de la tarjeta al servidor del banco

Paso 8: El sistema recibe que los datos de la tarjeta son correctos

Paso 9: El sistema recibe que los fondos son suficientes para abonar el 20% del total

Paso 10: El sistema registra el pago y cierra la conexión con el servidor del banco

</td></table>

---

**Curso alterno:**
- Paso alternativo 3: Falla la conexión con el servidor del banco. Se informa el error. Fin del CU
- Paso alternativo 8: La validación de los datos es incorrecta. Se informa error en los datos de la tarjeta. Fin de CU
- Paso alternativo 9: Los fondos son insuficientes para abonar el 20% total del alquiler. Se informa fondos insuficientes. Fin de CU

**Postcondición:** Se realizo y se registro el pago a traves de la tarjeta

</table>


---

### Cargar mueble

<table ><tr><td width="660"> 

**Nombre:** Cargar Mueble
 
**Descripción:** Este cu describe la forma en la que un encargado del departamento carga muebles

**Actores:** Encargado del departamento

**Precondiciones:** El encargado del departamento debe tener una sesión iniciada

---

CURSO NORMAL<table> <tr><td>Acciones del actor</td> <td>Acciones del Sistema</td></tr>
<td width="320">  

Paso 1 : el encargado del departamento selecciona la opción 'Cargar mueble'

Paso 3: el encargado del departamento ingresa los datos solicitados 

</td><td width="320">

Paso 2: El sistema solicita codigo de inventario, tipo de mueble, fecha de creación, fecha de ultimo mantenimiento, estado y el precio de alquiler

Paso 4: El sistema valida que el codigo sea unico

Paso 5: El sistema valida que el precio se cargo en dolares

Paso 6: El sistemas registra la carga del mueble 

</td></table>

---

**Curso alterno:**
- Paso alterno 4: El codigo ingresado no es unico. Se informa el error. Fin del CU
- Paso alterno 5: El precio no se cargo en dolares. Se informa el error. Regresa al paso 2

**Postcondición:** Se registro un mueble

</table>

</div>

<img src= 'https://i.gifer.com/origin/8c/8cd3f1898255c045143e1da97fbabf10_w200.gif' height="20" width="100%">

<div align = 'center'>

## `Problema 2` Posgrado

</div>

Suponga que trabaja en el área de sistemas de la Facultad de Informática y se le solicitó la automatización del pago de carreras de posgrado. Inicialmente se coordinó una reunión con el director del posgrado y se obtuvo la siguiente información:

Ya que no se desea seguir cobrando el dinero en la secretaría, es necesario que los alumnos puedan pagar las carreras vía web. Como el director de posgrado no realiza tareas administrativas nos recomendó hablar con el secretario académico.

De la entrevista con el secretario académico se obtuvo la siguiente información:

Es necesario cargar las carreras a un sistema. En esta primera versión del sistema sólo se nos pidió esta funcionalidad, sin la modificación ni eliminación. De cada carrera se conoce: nombre de la carrera (no puede repetirse), duración en años (a partir de la consulta del estatuto de posgrado se obtuvo que como máximo son 5 años), costo y cantidad máxima de cuotas para el pago. La carga de las carreras no la realiza el secretario académico sino un empleado administrativo.

Al preguntarle por la dinámica del sistema, el secretario académico nos derivó con el jefe del área administrativa, con el cual hicimos otra entrevista y pudimos obtener la siguiente información:

El requerimiento fue que el alumno ingrese a la web de posgrado y pueda registrarse ingresando: nombre, apellido, nombre de usuario (único) y contraseña (más de 6 dígitos). Cualquier alumno previamente registrado, puede iniciar sesión con su nombre de usuario y contraseña, habilitándose la inscripción a alguna de las carreras. Para ejemplificar esta funcionalidad nos otorgaron acceso al sistema SIGEF, el cual realiza funcionalidades similares para las carreras de grado.

Para inscribirse, el alumno deberá seleccionar la carrera, ingresar la cantidad de cuotas a pagar, ingresar el número de tarjeta y, en caso de que la tarjeta sea válida y tenga fondos, se hará efectivo el cobro y la inscripción. La tarjeta de crédito se valida a través de un servicio del banco con el cual la universidad tiene convenio. Luego de efectuado el cobro, el sistema debe imprimir dos comprobantes, uno de inscripción y otro de pago. La única forma que tiene el alumno de pagar es con tarjeta de crédito.

---

### Actores

- Alumno registrado
- Alumno no registrado
- Empleado administrativo
- Servidor del banco

### Casos de Uso

- Cargar carrera
- Cerrar sesión
- Iniciar sesión
- Registrar alumno
- Pagar con tarjeta
- Inscribirse a Carrera

---

- [Imagen Completa](/Practicas/Practica%203/Imagenes/2.jpg)

### Diagrama

![](2023-05-04-13-37-17.png)

---

<div align="center">

## Cargar Carrera

<table ><tr><td width="660"> 

**Nombre:** Cargar Carrera
 
**Descripción:** Este cu describe como un empleado administrativo realiza la carga de una carrera

**Actores:** Empleado administrativo

**Precondiciones:** ---

---

CURSO NORMAL<table> <tr><td>Acciones del actor</td> <td>Acciones del Sistema</td></tr>
<td width="320">  

Paso 1: El empleado administrativo selecciona la opción "Cargar carrera"

Paso 3: El empleado administrativo ingresa datos solicitados

</td><td width="320">

Paso 2: El sistema solicita nombre de la carrera, duración en años, costo y cantidad maxima de cuotas para el pago

Paso 4: El sistema valida que el nombre no se repita

Paso 5: El sistema valida que la duración sea menor o igual a 5 años

Paso 6: El sistema registra la carrera

</td></table>

---

**Curso alterno:**
- Curso alterno 4: El nombre se repite. Se informa el error. Retoma desde el paso 2
- Curso alterno 5: La duración supera los 5 años. Se informa el error. Retoma desde el paso 2

**Postcondición:** Se cargo una nueva carrera en el sistema

</table>

---

## Inscribirse a carrera

<table ><tr><td width="660"> 

**Nombre:** Inscribirse a carrera
 
**Descripción:** Este cu describe como un alumno registrado se inscribe a una carrera

**Actores:** Alumno Registrado

**Precondiciones:** El Alumno debe tener una sesión iniciada

---

CURSO NORMAL<table> <tr><td>Acciones del actor</td> <td>Acciones del Sistema</td></tr>
<td width="320">  

Paso 1: El Alumno registrado selecciona la opción "Inscribirse a carrera"

Paso 3: El Alumno registrado selecciona una de las carreras e ingresa datos solicitados

</td><td width="320">

Paso 2: El sistema muestra un listado de carreras y solicita cantidad de cuotas a pagar

Paso 4: El sistema valida que las cuotas no superen el maximo disponible

Paso 5: El sistema ejecuta el CU "Pagar con tarjeta"

Paso 6: El sistema imprime dos comprobantes, uno de inscripción y otro de pago

</td></table>

---

**Curso alterno:**
- Paso alterno 4: Las cuotas superan el maximo. Se notifica. Volver al paso 2
- Paso alterno 5: El pago no se realiza. Se notifica al Alumno registrado. Fin del CU.

**Postcondición:** Se realizo la inscripcion a una carrera
</table>

---

## Iniciar Sesión

<table ><tr><td width="660"> 

**Nombre:** Iniciar Sesión
 
**Descripción:** Este cu describe como un Alumno registrado inicia sesión

**Actores:** Alumno Registrado

**Precondiciones:** ---

---

CURSO NORMAL<table> <tr><td>Acciones del actor</td> <td>Acciones del Sistema</td></tr>
<td width="320">  

Paso 1: El Alumno registrado selecciona la opcion "Iniciar Sesión"

Paso 3: El Alumno registrado ingresa datos solicitados


</td><td width="320">

Paso 2: El sistema solicita nombre de usuario y contraseña

Paso 4: El sistema verifica datos ingresados

Paso 5: El sistema registra la sesión iniciada y habilida las acciones del usuario registrado

</td></table>

---

**Curso alterno:**
- Paso alternativo 4: El nombre de usuario o la contraseña no son validos. Se notifica el error. Volver al paso 2

**Postcondición:** La sesión ha sido habilitada y las opciones para usuarios registrados aparecen habilitadas

</table>

---

## Cerrar Sesión

<table ><tr><td width="660"> 

**Nombre:** Cerrar Sesión
 
**Descripción:** Este cu describe como un alumno registrado realiza el cierre de sesión

**Actores:** Alumno Registrado

**Precondiciones:** El alumno registrado debe tener una sesión abierta

---

CURSO NORMAL<table> <tr><td>Acciones del actor</td> <td>Acciones del Sistema</td></tr>
<td width="320">  

Paso 1: El Alumno registrado selecciona la opción "Cerrar Sesión"

Paso 3: El Alumno registrado acepta confirmación

</td><td width="320">

Paso 2: El sistema solicita confirmación del Alumno

Paso 4: El sistema cierra la sesión y deshabilita las acciones del Alumno

</td></table>

---

**Curso alterno:**
- El usuario registrado cancela la operación. Fin del CU

**Postcondición:** La sesión ha sido cerrada, las operaciones para usuarios registrados son deshabilitadas y se eliminan los datos de la sesión.

</table>

---

## Registrar alumno

<table ><tr><td width="660"> 

**Nombre:** Registrar alumno
 
**Descripción:** Este cu describe como un alumno no registrado realiza el registro

**Actores:** Alumno no registrado

**Precondiciones:** ---

---

CURSO NORMAL<table> <tr><td>Acciones del actor</td> <td>Acciones del Sistema</td></tr>
<td width="320">  

Paso 1: El Alumno no registrado selecciona la opción "Registrar Alumno"

Paso 3: El alumno no registrado ingresa datos solicitados

</td><td width="320">

Paso 2: El sistema solicita nombre, apellido, nombre de usuario y contraseña

Paso 4: El sistema valida que el nombre sea unico

Paso 5: El sistema valida que la contraseña tenga mas de 6 digitos

Paso 6: El sistema registra al usuario y habilita la inscripción a alguna de las carreras

</td></table>

---

**Curso alterno:**
- Paso alternativo 4: El nombre no se unico. Se informa el error. Volver al paso 2.
- Paso alternativo 5: La contraseña tiene menos de 6 digitos. Se informa el error. Volver al paso 2.

**Postcondición:** Se registro al usuario de manera existosa habilitanse las incripciones a las carreras

</table>

---

## Pagar con tarjeta

<table ><tr><td width="660"> 

**Nombre:** Pagar con tarjeta
 
**Descripción:** 

**Actores:** Servidor del banco, Alumno Registrado

**Precondiciones:** Se debe haber ejecutado el cu "Inscribirse a carrera"

---

CURSO NORMAL<table> <tr><td>Acciones del actor</td> <td>Acciones del Sistema</td></tr>
<td width="320">  

Paso 2: El Alumno registrado ingresa datos solicitados

Paso 4: El servidor del banco acepta la conexión y solicita numero de la tarjeta

Paso 6: El servidor del banco valida numero de tarjeta y fondos suficientes

Paso 7: El servidor del banco retorna resultado

</td><td width="320">

Paso 1: El sistema solicita numero de tarjeta 

Paso 3: El sistema solicita conexión con el servidor del banco

Paso 5: El sistema envia el numero de la tarjeta al servidor del banco

Paso 8: El sistema recibe que el numero de la tarjeta es valido

Paso 9: El sistema recibe el posee fondos suficientes

Paso 10: El sistema registra el pago

</td></table>

---

**Curso alterno:**
- Curso alternativo 2: No se establecio conexión con el servidor del banco. Se informa. Fin del CU
- Curso alternativo 8: El nro de la tarjeta es invalido. Se notifica. Volver al paso 1.
- Curso alternativo 9: No posee fondos suficientes. Se notifica. Fin del CU.

**Postcondición:** Se efectuo y registro el pago a traves de la tarjeta

</table>

</div>

<img src= 'https://i.gifer.com/origin/8c/8cd3f1898255c045143e1da97fbabf10_w200.gif' height="20" width="100%">

<div align = 'center'>

## `Problema 3` Contratos

</div>

Suponga que trabaja en un grupo en el área de sistemas de una organización y está por comenzar un nuevo proyecto para desarrollar un sistema que depende del departamento contable.

El sistema deberá administrar los contratos realizado con terceros. En una de las reuniones con el jefe de departamento nos dijo que él no usará el sistema pero que recibirá listados del personal contratado ya que deberá firmarlos para elevarlos a las autoridades.

Para obtener más información generamos una reunión con el empleado de mesa de entradas. Nos contó que el problema que tienen actualmente es que realizan todas las minutas a mano por lo cual desean automatizar esta tarea. Las minutas son el paso previo a un contrato. Para confeccionar una minuta, el
empleado de mesa de entradas debe ingresar nombre y número de CUIT de una persona a contratar, tipo de contrato, fecha de comienzo, duración y monto, a lo que el sistema le asociará un número de minuta automáticamente. Nos recomendó leer la reglamentación vigente acerca de contratos de la que obtuvimos que los montos de los mismos no pueden superar los $25.000 y que la duración debe ser como máximo de 6 meses.

Una vez confeccionada la minuta por parte del empleado de mesa de entradas, la misma queda pendiente de aprobación. El que puede aprobar una minuta es el empleado de rendiciones. Realizamos una reunión con él y nos contó que su tarea consiste en evaluar las minutas para determinar su aprobación. También nos dijo que en otro trabajo que tiene usan un sistema llamado MiMiNuTa al que nos puede dar acceso para ver como hacen esa tarea. Después del análisis de este sistema, se concluyó que para aprobar una minuta necesitaría ingresar un número de minuta y que el sistema muestre los datos de la misma para poder aprobarla. Nos dijo que no puede aprobar la minuta si la persona a contratar tiene 3 contratos vigentes (minutas aprobadas) ni tampoco si el CUIT de la persona a contratar está inhabilitado por la AFIP. Actualmente se comunica telefónicamente con la AFIP para realizar esta verificación, pero sabe que ésta provee un servicio para aplicaciones que permite hacer la verificación en línea. Esto último nos obligó a generar una reunión con el administrador de servidores de la AFIP. Nos dijo que para poder conectarnos con un servidor de la AFIP, el sistema debe mandar un token (código que identificará de manera única a nuestra aplicación) y CUIT, si el token es correcto, el servidor responde si el CUIT está habilitado o no.

Por último el empleado de rendiciones será el responsable de imprimir los listados con las minutas aprobadas, es decir, un listado con el personal contratado para poder dárselo al jefe de departamento para que lo firme.

---

### Actores
- Empleado de Mesa
- Empleado de Rendiciones
- Servidor AFIP

### Casos de Uso
- Confeccionar minuta
- Aprobar minuta
- Imprimir Listado
- Validar Cuit

---

### Diagrama

- [Imagen Completa](/Practicas/Practica%203/Imagenes/3.jpg)

![](2023-05-04-13-37-58.png)

---

<div align="center">

### Confeccionar Minuta

<table ><tr><td width="660"> 

**Nombre:** Confeccionar Minuta
 
**Descripción:** Este cu describe como como un empleado de mesa realiza la confecció de una minuta

**Actores:** Empleado de mesa

**Precondiciones:** 

---

CURSO NORMAL<table> <tr><td>Acciones del actor</td> <td>Acciones del Sistema</td></tr>
<td width="320">  

Paso 1: El empleado de mesa selecciona la opción "Confeccionar minuta"

Paso 3: El empleado de mesa ingresa datos solicitados

</td><td width="320">

Paso 2: El sistema solicita nombre, CUIT, tipo de contrato, fecha de comienzo, duración y monto

Paso 4: El sistema valida que el monto no supera los $25.000

Paso 5: El sistema valida que la duración no supera los 6 meses

Paso 6: El sistema confecciona y asocia un numero de minuta automaticamente

</td></table>

---

**Curso alterno:**
- Paso alternativo 4: 
- Paso alternativo 5: 

**Postcondición:** Se confecciona la minuta y se le asocia un numero automaticamente

</table>

---

### Aprobar Minuta

<table ><tr><td width="660"> 

**Nombre:** Aprobar Minuta
 
**Descripción:** Este cu describe como un empleado de rendiciones realiza la aprobación de una minuta

**Actores:** Empleado de rendiciones

**Precondiciones:** ---

---

CURSO NORMAL<table> <tr><td>Acciones del actor</td> <td>Acciones del Sistema</td></tr>
<td width="320">  

Paso 1: El Empleado de rendiciones seleciona la opción "Aprobar Minuta"

Paso 3: El Empleado de rendiciones ingresa datos solicitados

</td><td width="320">

Paso 2: El sistema solicita numero de minuta

Paso 4: El sistema muestra los datos de la misma

Paso 5: El sistema valida que la persona no tenga 3 contratos vigentes

Paso 6: El sistema ejecuta el cu Validar Cuit

Paso 7: El sistema aprueba la minuta y se agrega al listado

</td></table>

---

**Curso alterno:**
- Paso alternativo 4: No se muestran los datos. Se informa que ya fue usada. Fin del CU
- Paso alternativo 5: La persona tiene 3 contratos vigentes. Se notifica. Fin de CU
- Paso alternativo 6: Cuit Invalido. Se notifica. Fin del CU

**Postcondición:** La minuta fue aprobada

</table>

---

### Imprimir Listado

<table ><tr><td width="660"> 

**Nombre:** Imprimir Listado
 
**Descripción:** Este cu describe como un Empleado de rendiciones imprime un listado de las minutas

**Actores:** Empleado de rendiciones

**Precondiciones:** ---

---

CURSO NORMAL<table> <tr><td>Acciones del actor</td> <td>Acciones del Sistema</td></tr>
<td width="320">  

Paso 1: el Empleado de rendiciones selecciona la opcion "Imprimir listado"

</td><td width="320">

Paso 2: El sistema imprime un listado de minutas

</td></table>

---

**Curso alterno:** ---

**Postcondición:** Se imprimio un listado de minutas aprobadas

</table>

---

### Validar Cuit

<table ><tr><td width="660"> 

**Nombre:** Validar Cuit
 
**Descripción:** Este cu describe la validación de un CUIT

**Actores:** Servidor AFIP

**Precondiciones:** Se debe haber ejecutado el cu "Aprobar minuta"

---

CURSO NORMAL<table> <tr><td>Acciones del actor</td> <td>Acciones del Sistema</td></tr>
<td width="320">  

Paso 2: El servidor AFIP acepta la conexión y solicita Token y CUIT

Paso 4: El servidor AFIP valida el token y CUIT

Paso 5: El servidor AFIP retorna el resultado

</td><td width="320">

Paso 1: El sistema solicita conexión con el servidor AFIP

Paso 3: El sistema envia token y CUIT

Paso 6: El sistema recibe que el Token es correcto

Paso 7: El sistema recibe que el CUIT esta habilitado

Paso 8: El sistema valida el Cuit y cierra la conexión con el servidor externo



</td></table>

---

**Curso alterno:**
- Paso Alternativo 1: No se establecio conexión con el servidor. Se notifica. Fin del CU
- Paso Alternativo 4: El Token es incorrecto. Se notifica. Fin del CU
- Paso Alternativo 5: El CUIT esta inhabilitado por el AFIP. Se notifica. Fin del CU

**Postcondición:** El cuit fue validado

</table>

</div>

<img src= 'https://i.gifer.com/origin/8c/8cd3f1898255c045143e1da97fbabf10_w200.gif' height="20" width="100%">

<div align = 'center'>

## `Problema 4` Máquina de reciclado

</div>

Se desea modelar un sistema que controle una máquina de reciclado. La máquina cuenta con un recipiente externo donde se depositan los materiales a reciclar (vidrio, papel, plástico o aluminio). La persona coloca lo que desea reciclar en el recipiente y luego presiona la opción “reciclar”. El sistema detecta el tipo de material y registra el peso; por último imprime un recibo con el monto total que se le debe pagar a la persona por lo reciclado. Si el sistema no detecta correctamente el tipo de material aborta el proceso
retornando el producto.

El sistema también es utilizado por un operador a través de una consola que se encuentra bajo llave. El operador puede solicitar un listado con los tipos de materiales reciclados en un periodo de fechas determinado, detallando además el total abonado por dicho material. También, el operador puede actualizar los montos a pagar por kilo de cada tipo de material que la máquina puede reciclar. Para esto, el sistema primero solicita el tipo de material a actualizar. Luego se pide el nuevo monto. Si el operador acepta, se actualiza el material seleccionado.

---

### Actores
- Persona
- Operador

### Casos de Uso
- Reciclar
- Solicitar Listado
- Actualizar Monto

---

### Diagrama

- [Imagen Completa](/Practicas/Practica%203/Imagenes/4.jpg)

![](2023-05-04-13-38-46.png)

---

<div align='center'>

### Reciclar

<table ><tr><td width="660"> 

**Nombre:** Reciclar 
 
**Descripción:** Este cu describe como una persona recicla 

**Actores:** Persona

**Precondiciones:** 

---

CURSO NORMAL<table> <tr><td>Acciones del actor</td> <td>Acciones del Sistema</td></tr>
<td width="320">  

Paso x:

</td><td width="320">

Paso x: 

</td></table>

---

**Curso alterno:**

**Postcondición:**

</table>

---

### Solicitar Listado

<table ><tr><td width="660"> 

**Nombre:** 
 
**Descripción:** 

**Actores:** 

**Precondiciones:** 

---

CURSO NORMAL<table> <tr><td>Acciones del actor</td> <td>Acciones del Sistema</td></tr>
<td width="320">  

Paso x:

</td><td width="320">

Paso x: 

</td></table>

---

**Curso alterno:**

**Postcondición:**

</table>

---

### Actualizar Monto

<table ><tr><td width="660"> 

**Nombre:** 
 
**Descripción:** 

**Actores:** 

**Precondiciones:** 

---

CURSO NORMAL<table> <tr><td>Acciones del actor</td> <td>Acciones del Sistema</td></tr>
<td width="320">  

Paso x:

</td><td width="320">

Paso x: 

</td></table>

---

**Curso alterno:**

**Postcondición:**

</table>

</div>

<img src= 'https://i.gifer.com/origin/8c/8cd3f1898255c045143e1da97fbabf10_w200.gif' height="20" width="100%">

<div align = 'center'>

## `Problema 5` Impresión de Fotos

</div>

Se desea desarrollar un sistema para la impresión de fotos para una casa fotográfica. Los clientes pueden subir sus fotos, pagar por internet y luego ser retiradas personalmente por el local.

Para subir las fotos la persona debe registrarse en el sitio, ingresando sus datos personales, nombre, apellido, email, domicilio, nombre de usuario y contraseña.

Una vez autenticado, el usuario puede subir un máximo de 50 fotos para ser impresas. Las fotos se ingresan de a una. Una vez subidas, el usuario debe abonar el monto total (el valor de cada foto es de $15). El pago se realiza con tarjeta de crédito, ingresando los datos de la misma (número de tarjeta, código de seguridad y nombre del titular), la cual debe ser validada a través del sistema del banco. Una vez que se realiza el pago se le otorga al cliente un código único que le servirá posteriormente para retirar las fotos.

Un cliente debe acercarse a la sucursal para retirar las fotos enviadas previamente. Para esto debe presentar el código único a un empleado. Este registra el código, la fecha de retiro y entrega las fotos al
cliente.

---

### Actores
- Persona (Usuario no registrado)
- Usuario
- Empleado
- Servidor del banco

### Casos de uso
- Subir Fotos
- Registrar Persona
- Iniciar Sesión
- Cerrar Sesión
- Pagar con tarjeta
- Registrar Codigo

---

### Diagrama

- [Imagen Completa](/Practicas/Practica%203/Imagenes/5.jpg)

![](2023-05-04-13-39-14.png)

---

### Subir Fotos

<table ><tr><td width="660"> 

**Nombre:** Subir Fotos
 
**Descripción:** Este cu describe como un usuario sube fotos para abonarlas

**Actores:** Usuario

**Precondiciones:** El usuario debe tener una sesión iniciada

---

CURSO NORMAL<table> <tr><td>Acciones del actor</td> <td>Acciones del Sistema</td></tr>
<td width="320">  

Paso 1: El usuario selecciona la opción "Subir Foto"

Paso 3: El usuario ingresa una foto

Paso 6: El usuario acepta la confirmación para pagar

</td><td width="320">

Paso 2: El sistema solicita que ingrese una foto

Paso 4: El sistema valida si se ingresaron menos de 50 fotos

Paso 5: El sistema solicita la confirmación del usuario para pagar

Paso 7: El sistema multiplica cada foto por $15 y guarda el total

Paso 8: El sistema ejecuta el cu "Pagar con Tarjeta"

Paso 9: El sistema imprime un codigo unico para retirar las fotos


</td></table>

---

**Curso alterno:**
- Paso alternativo 4: Se ingresaron 50 fotos. Se Informa que se alcanzo el limite. Se adelanta al Paso 8 (Si no paga muere :D)
- Paso alternativo 5: El usuario cancelo la confirmación. Informo. Vuelvo al paso 2.
- Paso alternativo 8: El pago no se realiza. Se notifica. Fin del CU.


**Postcondición:**

</table>

---

### Registrar Persona

<table ><tr><td width="660"> 

**Nombre:** Registrar Persona
 
**Descripción:** Este cu describe como una persona se registra

**Actores:** Persona

**Precondiciones:** 

---

CURSO NORMAL<table> <tr><td>Acciones del actor</td> <td>Acciones del Sistema</td></tr>
<td width="320">  

Paso 1: La Persona selecciona la opción "Registrar Persona"

Paso 3: La Persona ingresa datos solicitados

</td><td width="320">

Paso 2: El sistema solicita datos personales, nombre, apellido, mail, domicilio nombre de usuario y contraseña

Paso 4: El sistema valida nombre de usuario unico

Paso 5: El sistema da de alta al nuevo usuario

</td></table>

---

**Curso alterno:**
- Paso alternativo 4: El nombre del usuario ya existe. Se informa. Vuele al Paso 2.

**Postcondición:** Se da de alta un nuevo usuario

</table>

---

### Iniciar Sesión

<table ><tr><td width="660"> 

**Nombre:** Iniciar Sesión
 
**Descripción:** Este cu describe como un usuario inicia su sesión

**Actores:** Usuario

**Precondiciones:** 

---

CURSO NORMAL<table> <tr><td>Acciones del actor</td> <td>Acciones del Sistema</td></tr>
<td width="320">  

Paso 1: El usuario selecciona la opción "Iniciar Sesión"

Paso 3: El usuario ingresa datos solicitados

</td><td width="320">

Paso 2: El sistema solicita nombre de usuario y contraseña

Paso 4: El sistema valida los datos ingresados

Paso 5: El sistema registra la sesión iniciada y lo habilita para subir fotos 

</td></table>

---

**Curso alterno:** El usuario o la contraseña no son validos. Se notifica la discrepancia. Vuelve al paso 2

**Postcondición:** La sesión ha sido iniciada y se habilita la opción para subir fotos

</table>

---

### Cerrar Sesión

<table ><tr><td width="660"> 

**Nombre:** Cerrar Sesión
 
**Descripción:** 

**Actores:** 

**Precondiciones:** 

---

CURSO NORMAL<table> <tr><td>Acciones del actor</td> <td>Acciones del Sistema</td></tr>
<td width="320">  

Paso x:

</td><td width="320">

Paso x: 

</td></table>

---

**Curso alterno:**

**Postcondición:**

</table>

---

### Pagar con tarjeta

<table ><tr><td width="660"> 

**Nombre:** Pagar con tarjeta
 
**Descripción:** 

**Actores:** 

**Precondiciones:** 

---

CURSO NORMAL<table> <tr><td>Acciones del actor</td> <td>Acciones del Sistema</td></tr>
<td width="320">  

Paso x:

</td><td width="320">

Paso x: 

</td></table>

---

**Curso alterno:**

**Postcondición:**

</table>

---

### Registrar Codigo

<table ><tr><td width="660"> 

**Nombre:** Registrar Codigo
 
**Descripción:** 

**Actores:** 

**Precondiciones:** 

---

CURSO NORMAL<table> <tr><td>Acciones del actor</td> <td>Acciones del Sistema</td></tr>
<td width="320">  

Paso x:

</td><td width="320">

Paso x: 

</td></table>

---

**Curso alterno:**

**Postcondición:**

</table>


<img src= 'https://i.gifer.com/origin/8c/8cd3f1898255c045143e1da97fbabf10_w200.gif' height="20" width="100%">

<div align = 'center'>

## `Problema 6` Ventas de Entradas para Teatro

</div>

Se desea modelar un sistema de gestión de ventas de entradas para un teatro. Las personas compran sus entradas a través de una página web, o personalmente.

El sistema permite, sólo de modo personal en el teatro, la reserva de entradas de forma gratuita. El empleado debe ingresar los datos de la obra (fecha, hora, y nombre) junto el nombre y DNI del espectador. En este caso, sólo se podrá reservar hasta 2 entradas. Las entradas reservadas no compradas caducarán tres horas antes del evento. Para seleccionar el nombre de la obra, el sistema muestra una grilla de funciones disponibles para que el usuario seleccione una.

Para comprar una entrada vía web, el sistema muestra la grilla de funciones disponibles. El usuario selecciona una opción, ingresa su DNI, la cantidad de lugares solicitados y selecciona la opción “pagar”. El pago se realiza con tarjeta de crédito. Para esto debe ser autorizada a través del sistema del banco. Este pide el número de tarjeta, vencimiento, y código de seguridad. Verifica todos los campos y autoriza la compra. Autorizada la tarjeta, se emite un código de compra con el que el cliente podrá retirar sus entradas en la boletería del cine.

Para comprar una entrada personalmente, el vendedor de la boletería solicita los datos de la función al cliente, procediendo de un modo similar a la compra web, con la diferencia que en este caso no se muestra el código de compra sino que se imprimen directamente la/s entrada/s. El pago es únicamente con tarjeta de crédito, igual que en el caso anterior.

Para retirar las entradas reservadas previamente, el empleado solicita nombre y DNI del espectador, el sistema valida que la persona posea entradas reservadas, y que no estén caducas. El resto del procedimiento se realiza igual que la compra de entradas descriptas anteriormente.

Cuando una persona llega con el código de compra, el vendedor debe ingresar el código para que el sistema, luego de verificarlo, imprima las entradas correspondientes. 

Además se desea administrar la programación de las salas. El administrador ingresa la distribución semanal de las obras en las salas de manera que se encuentre disponible para la realización de la venta de entradas.

---

### Actores
- Empleado
- Persona
- Usuario
- Servidor del Banco

### Casos de Uso
- Registrar Codigo
- Reservar Entrada Gratuita
- Registrar Reserva
- Pagar Con Tarjeta
- Comprar Entrada Presencial
- Comprar Entrada Online

---

### Diagrama

- [Imagen Completa](/Practicas/Practica%203/Imagenes/6.jpg)

![](2023-05-04-13-40-29.png)

---

<div align="center">

### Registrar Codigo

<table ><tr><td width="660"> 

**Nombre:** 
 
**Descripción:** 

**Actores:** 

**Precondiciones:** 

---

CURSO NORMAL<table> <tr><td>Acciones del actor</td> <td>Acciones del Sistema</td></tr>
<td width="320">  

Paso x:

</td><td width="320">

Paso x: 

</td></table>

---

**Curso alterno:**

**Postcondición:**

</table>

---

### Reservar Entrada Gratuita

<table ><tr><td width="660"> 

**Nombre:** 
 
**Descripción:** 

**Actores:** 

**Precondiciones:** 

---

CURSO NORMAL<table> <tr><td>Acciones del actor</td> <td>Acciones del Sistema</td></tr>
<td width="320">  

Paso x:

</td><td width="320">

Paso x: 

</td></table>

---

**Curso alterno:**

**Postcondición:**

</table>

---

### Registrar Reserva

<table ><tr><td width="660"> 

**Nombre:** 
 
**Descripción:** 

**Actores:** 

**Precondiciones:** 

---

CURSO NORMAL<table> <tr><td>Acciones del actor</td> <td>Acciones del Sistema</td></tr>
<td width="320">  

Paso x:

</td><td width="320">

Paso x: 

</td></table>

---

**Curso alterno:**

**Postcondición:**

</table>

---

### Pagar Con Tarjeta

<table ><tr><td width="660"> 

**Nombre:** 
 
**Descripción:** 

**Actores:** 

**Precondiciones:** 

---

CURSO NORMAL<table> <tr><td>Acciones del actor</td> <td>Acciones del Sistema</td></tr>
<td width="320">  

Paso x:

</td><td width="320">

Paso x: 

</td></table>

---

**Curso alterno:**

**Postcondición:**

</table>

---

### Comprar Entrada Presencial

<table ><tr><td width="660"> 

**Nombre:** 
 
**Descripción:** 

**Actores:** 

**Precondiciones:** 

---

CURSO NORMAL<table> <tr><td>Acciones del actor</td> <td>Acciones del Sistema</td></tr>
<td width="320">  

Paso x:

</td><td width="320">

Paso x: 

</td></table>

---

**Curso alterno:**

**Postcondición:**

</table>

---

### Comprar Entrada Online

<table ><tr><td width="660"> 

**Nombre:** 
 
**Descripción:** 

**Actores:** 

**Precondiciones:** 

---

CURSO NORMAL<table> <tr><td>Acciones del actor</td> <td>Acciones del Sistema</td></tr>
<td width="320">  

Paso x:

</td><td width="320">

Paso x: 

</td></table>

---

**Curso alterno:**

**Postcondición:**

</table>

</div>

<img src= 'https://i.gifer.com/origin/8c/8cd3f1898255c045143e1da97fbabf10_w200.gif' height="20" width="100%">

<div align = 'center'>

## `Problema 7` Préstamos Personales

</div>

Se necesita modelar un subsistema web de administración de préstamos personales.

El sistema forma parte de un sistema mayor que implementa un servicio de homebanking para clientes del banco. Para todas las operaciones que realiza el cliente, se asume que está debidamente autenticado.

Un cliente del banco puede solicitar un préstamo personal vía web. Cada cliente puede solicitar un máximo de 3 préstamos y hasta un monto total de $30.000. Para realizar la solicitud, el cliente ingresa el motivo, selecciona la cuenta de donde se descontará automáticamente la cuota mensualmente e ingresa el monto del préstamo. El sistema debe verificar que el cliente no figure en el Veraz (banco de datos con información de deudores). Para realizar la comprobación, el sistema envía un código de seguridad para validar la identidad de la aplicación del banco. Una vez validada la identidad, la aplicación le envía el nombre y apellido de la persona y su número de CUIL/CUIT para determinar si existe o no como deudor. En caso de que todo sea válido, el sistema registra el préstamo correspondiente, genera un identificador del préstamo, un código de  verificación y un comprobante con los datos del préstamo.

El cliente podrá adelantar cuotas a partir del sexto mes de otorgado el préstamo. Para esto, el sistema muestra un listado de préstamos vigentes donde se debe seleccionar el que se desea pagar. A continuación el sistema solicita ingresar la cantidad de cuotas a abonar. Luego, el sistema muestra un listado de cuentas del cliente, donde se deberá seleccionar una de ellas para realizar el pago. Si hay saldo suficiente, el monto se deberá descontar de la cuenta del cliente. En caso de no poseer saldo se le informa al cliente.

El cliente podrá realizar la cancelación total del préstamo a partir del noveno mes. Para ello, se debe presentar personalmente en el banco con su DNI para acreditar su identidad. Cuando se introduce el DNI, el sistema lista los préstamos para que se seleccione cual desea pagar. Luego se verifica que la cuenta asociada originalmente posea saldo suficiente para alcanzar el monto total adeudado. De ser así se registrará dicha cancelación y emitirá un comprobante con los datos de la operación.

---

### Actores
- Cliente
- Veraz

### Casos de Uso
- Solicitar Prestamo
- Adelantar Cuotas
- Cancelar Prestamo
- Iniciar Sesión
- Cerrar Sesión

---

### Diagrama

- [Imagen Completa](/Practicas/Practica%203/Imagenes/7.jpg)

![](2023-05-04-13-40-58.png)

---

<div align="center">

### Solicitar Prestamo

<table ><tr><td width="660"> 

**Nombre:** 
 
**Descripción:** 

**Actores:** 

**Precondiciones:** 

---

CURSO NORMAL<table> <tr><td>Acciones del actor</td> <td>Acciones del Sistema</td></tr>
<td width="320">  

Paso x:

</td><td width="320">

Paso x: 

</td></table>

---

**Curso alterno:**

**Postcondición:**

</table>

---

### Adelantar Cuotas

<table ><tr><td width="660"> 

**Nombre:** 
 
**Descripción:** 

**Actores:** 

**Precondiciones:** 

---

CURSO NORMAL<table> <tr><td>Acciones del actor</td> <td>Acciones del Sistema</td></tr>
<td width="320">  

Paso x:

</td><td width="320">

Paso x: 

</td></table>

---

**Curso alterno:**

**Postcondición:**

</table>

---

### Cancelar Prestamo

<table ><tr><td width="660"> 

**Nombre:** 
 
**Descripción:** 

**Actores:** 

**Precondiciones:** 

---

CURSO NORMAL<table> <tr><td>Acciones del actor</td> <td>Acciones del Sistema</td></tr>
<td width="320">  

Paso x:

</td><td width="320">

Paso x: 

</td></table>

---

**Curso alterno:**

**Postcondición:**

</table>

---

### Iniciar Sesión

<table ><tr><td width="660"> 

**Nombre:** 
 
**Descripción:** 

**Actores:** 

**Precondiciones:** 

---

CURSO NORMAL<table> <tr><td>Acciones del actor</td> <td>Acciones del Sistema</td></tr>
<td width="320">  

Paso x:

</td><td width="320">

Paso x: 

</td></table>

---

**Curso alterno:**

**Postcondición:**

</table>

---

### Cerrar Sesión

<table ><tr><td width="660"> 

**Nombre:** 
 
**Descripción:** 

**Actores:** 

**Precondiciones:** 

---

CURSO NORMAL<table> <tr><td>Acciones del actor</td> <td>Acciones del Sistema</td></tr>
<td width="320">  

Paso x:

</td><td width="320">

Paso x: 

</td></table>

---

**Curso alterno:**

**Postcondición:**

</table>

</div>

<img src= 'https://i.gifer.com/origin/8c/8cd3f1898255c045143e1da97fbabf10_w200.gif' height="20" width="100%">

<div align = 'center'>

## `Problema 8` Pago de Impuestos y Servicios

</div>

Se desea modelar un sistema de pago electrónico de impuestos y servicios en efectivo.

Cuando un cliente llega para realizar un pago, el empleado o el gerente de la sucursal ingresa el código de pago electrónico y el sistema se conecta con la central de cobro para recuperar los datos de la factura (empresa, nro de cliente, 1era fecha de vencimiento, 2da fecha de vencimiento, recargo, y monto original). Una vez recuperados los datos, el sistema debe verificar los vencimientos para determinar el monto a cobrar. Teniendo esto en cuenta, cuando el 2do vencimiento está vencido se debe informar que la factura no se puede cobrar por dicho motivo. Cuando el 1er vencimiento está vencido hay que aplicar el recargo al monto original. Si la factura no está vencida, se cobra el monto original.

Una vez al día, el gerente de la sucursal debe registrar en la central de cobros los pagos que hicieron los clientes. Para esto el sistema requiere la clave maestra y de ser correcta, recupera las transacciones de los impuestos y servicios cobrados en el día, se conecta a la central de cobro y se las envía. Cuando la central confirma la recepción exitosa, el sistema las registra como enviadas. Este último paso es importante porque no deben enviarse dos veces las transacciones. Si el gerente intenta enviar una segunda vez, el sistema no debe permitirlo.

Finalmente el Gerente puede ver las estadísticas de los impuestos y servicios cobrados. Para esto, se ingresa la clave maestra, un rango de fechas sobre las cuales debe calcularse las estadísticas y el sistema debe mostrar los montos y la cantidad de cobros realizados, agrupando por empresa.

Tenga en cuenta que cada vez que el sistema debe conectarse a la central, debe enviarle un token (código que identifica al sistema). Una vez que la central valida el token, el sistema envía el requerimiento para recuperar los datos de la factura o el requerimiento para registrar los pagos del día según corresponda.

---

### Actores
- Empleado
- Persona
- Jerente
- Central de Combros

### Casos de Uso
- Realizar Pago
- Recuperar Pago
- Ver Estadisticas
- Enviar Pago
- Registrar Pago

---

### Diagrama

- [Imagen Completa](/Practicas/Practica%203/Imagenes/8.jpg)

![](2023-05-04-13-41-43.png)

---

<div align="center">

### Realizar Pago

<table ><tr><td width="660"> 

**Nombre:** 
 
**Descripción:** 

**Actores:** 

**Precondiciones:** 

---

CURSO NORMAL<table> <tr><td>Acciones del actor</td> <td>Acciones del Sistema</td></tr>
<td width="320">  

Paso x:

</td><td width="320">

Paso x: 

</td></table>

---

**Curso alterno:**

**Postcondición:**

</table>

---
### Recuperar Pago

<table ><tr><td width="660"> 

**Nombre:** 
 
**Descripción:** 

**Actores:** 

**Precondiciones:** 

---

CURSO NORMAL<table> <tr><td>Acciones del actor</td> <td>Acciones del Sistema</td></tr>
<td width="320">  

Paso x:

</td><td width="320">

Paso x: 

</td></table>

---

**Curso alterno:**

**Postcondición:**

</table>

---
### Ver Estadisticas

<table ><tr><td width="660"> 

**Nombre:** 
 
**Descripción:** 

**Actores:** 

**Precondiciones:** 

---

CURSO NORMAL<table> <tr><td>Acciones del actor</td> <td>Acciones del Sistema</td></tr>
<td width="320">  

Paso x:

</td><td width="320">

Paso x: 

</td></table>

---

**Curso alterno:**

**Postcondición:**

</table>

---
### Enviar Pago

<table ><tr><td width="660"> 

**Nombre:** 
 
**Descripción:** 

**Actores:** 

**Precondiciones:** 

---

CURSO NORMAL<table> <tr><td>Acciones del actor</td> <td>Acciones del Sistema</td></tr>
<td width="320">  

Paso x:

</td><td width="320">

Paso x: 

</td></table>

---

**Curso alterno:**

**Postcondición:**

</table>

---
### Registrar Pago

<table ><tr><td width="660"> 

**Nombre:** 
 
**Descripción:** 

**Actores:** 

**Precondiciones:** 

---

CURSO NORMAL<table> <tr><td>Acciones del actor</td> <td>Acciones del Sistema</td></tr>
<td width="320">  

Paso x:

</td><td width="320">

Paso x: 

</td></table>

---

**Curso alterno:**

**Postcondición:**

</table>

</div>
<img src= 'https://i.gifer.com/origin/8c/8cd3f1898255c045143e1da97fbabf10_w200.gif' height="20" width="100%">

<div align = 'center'>

## `Problema 9` Un Aventón

</div>

Se desea desarrollar un sistema que permita compartir un vehículo para un viaje. La idea es que cuando una persona tiene que realizar un viaje lo publique en la aplicación. Luego, el resto de los usuarios se postulan para acompañarla y el chofer podrá seleccionar quienes viajan. El objetivo es abaratar costos y evitar congestiones en el tránsito. El sistema es gratuito.

Para utilizar el sistema, una persona debe registrarse y estar correctamente identificado antes de poder utilizarlo. Al registrarse, se pide un nombre de usuario, un correo electrónico y una contraseña. No puede haber dos correos electrónicos iguales en el sistema. Una vez autenticado, podrá dar de alta diferentes viajes, identificando la fecha, hora y el automóvil que utilizará. Los diferentes viajes que una persona publique no pueden superponerse. Un usuario que adeuda calificaciones tampoco podrá publicar un viaje. Cualquier usuario identificado podrá postularse a un viaje. Luego, el usuario dueño del viaje podrá aceptar o rechazar los candidatos para que realicen el viaje con él.

En el sistema existe una política de reputaciones que permiten a los usuarios conocer la opinión del resto sobre los viajes realizados. Luego de terminado un viaje, tanto el piloto como los copilotos que viajaron deberán calificarse entre sí. El piloto califica a todos sus copilotos. Cada copiloto califica al piloto del viaje. Las calificaciones podrán ser positivas (suma un punto de reputación) o negativas (restan un punto de reputación).

---

### Actores
- Persona
- Usuario
- Piloto
- Copiloto

### Casos de Uso
- Registrar Persona
- Iniciar Sesión
- Cerrar Sesión
- Alta Viaje
- Postularse a un Viaje
- Evaluar Candidato
- Clasificar Copilotos
- Clasificar Piloto

---

### Diagrama

- [Imagen Completa](/Practicas/Practica%203/Imagenes/9.jpg)

![](2023-05-04-13-43-25.png)

---
<div align="center">

### Registrar Persona

<table ><tr><td width="660"> 

**Nombre:** 
 
**Descripción:** 

**Actores:** 

**Precondiciones:** 

---

CURSO NORMAL<table> <tr><td>Acciones del actor</td> <td>Acciones del Sistema</td></tr>
<td width="320">  

Paso x:

</td><td width="320">

Paso x: 

</td></table>

---

**Curso alterno:**

**Postcondición:**

</table>

---
### Iniciar Sesión

<table ><tr><td width="660"> 

**Nombre:** 
 
**Descripción:** 

**Actores:** 

**Precondiciones:** 

---

CURSO NORMAL<table> <tr><td>Acciones del actor</td> <td>Acciones del Sistema</td></tr>
<td width="320">  

Paso x:

</td><td width="320">

Paso x: 

</td></table>

---

**Curso alterno:**

**Postcondición:**

</table>

---
### Cerrar Sesión



---
### Alta Viaje

<table ><tr><td width="660"> 

**Nombre:** 
 
**Descripción:** 

**Actores:** 

**Precondiciones:** 

---

CURSO NORMAL<table> <tr><td>Acciones del actor</td> <td>Acciones del Sistema</td></tr>
<td width="320">  

Paso x:

</td><td width="320">

Paso x: 

</td></table>

---

**Curso alterno:**

**Postcondición:**

</table>

---
### Postularse a un Viaje

<table ><tr><td width="660"> 

**Nombre:** 
 
**Descripción:** 

**Actores:** 

**Precondiciones:** 

---

CURSO NORMAL<table> <tr><td>Acciones del actor</td> <td>Acciones del Sistema</td></tr>
<td width="320">  

Paso x:

</td><td width="320">

Paso x: 

</td></table>

---

**Curso alterno:**

**Postcondición:**

</table>

---
### Evaluar Candidato

<table ><tr><td width="660"> 

**Nombre:** 
 
**Descripción:** 

**Actores:** 

**Precondiciones:** 

---

CURSO NORMAL<table> <tr><td>Acciones del actor</td> <td>Acciones del Sistema</td></tr>
<td width="320">  

Paso x:

</td><td width="320">

Paso x: 

</td></table>

---

**Curso alterno:**

**Postcondición:**

</table>

---
### Clasificar Copilotos

<table ><tr><td width="660"> 

**Nombre:** 
 
**Descripción:** 

**Actores:** 

**Precondiciones:** 

---

CURSO NORMAL<table> <tr><td>Acciones del actor</td> <td>Acciones del Sistema</td></tr>
<td width="320">  

Paso x:

</td><td width="320">

Paso x: 

</td></table>

---

**Curso alterno:**

**Postcondición:**

</table>

---
### Clasificar Piloto

<table ><tr><td width="660"> 

**Nombre:** 
 
**Descripción:** 

**Actores:** 

**Precondiciones:** 

---

CURSO NORMAL<table> <tr><td>Acciones del actor</td> <td>Acciones del Sistema</td></tr>
<td width="320">  

Paso x:

</td><td width="320">

Paso x: 

</td></table>

---

**Curso alterno:**

**Postcondición:**

</table>

</div>
<img src= 'https://i.gifer.com/origin/8c/8cd3f1898255c045143e1da97fbabf10_w200.gif' height="20" width="100%">

<div align = 'center'>

## `Problema 10` Gimnasio

</div>

Se desea modelar con casos de uso un sistema web para el manejo de turnos de un gimnasio. Las personas que desean solicitar un turno para concurrir al gimnasio primero deben registrarse. Para ello deben ingresar el dni, el nombre, el apellido y el mail que será utilizado como nombre de usuario (por lo tanto, no puede repetirse). Una vez que el usuario se registra, el sistema genera una contraseña que es enviada al correo de la persona.

Para solicitar un turno, el cliente del gimnasio, previa autenticación, debe ingresar: fecha, hora y actividad. Si hay cupo para esa actividad en ese día y a esa hora, el sistema registra el turno, de lo contrario, muestra un mensaje de cupo no disponible.

Por último cuando un cliente llega al gimnasio debe registrar su llegada, para esto la secretaria del gimnasio solicita el número de dni del cliente para hacer el registro. El gimnasio se maneja con un sistema externo que suma puntos a aquellos clientes que cumplen con las reservas realizadas. Es necesario que cuando se registre la asistencia del cliente al gimnasio se haga la suma correspondiente para lo cual el sistema se conecta con el servidor externo, envía el dni del cliente y la actividad que va a realizar y el servidor se encarga de sumar los puntos.

---

### Actores
- Persona
- Cliente
- Secretaria
- Servidor Externo

### Casos de Uso
- Registrar Persona
- Iniciar Sesión
- Cerrar Sesión
- Solicitar Turno
- Registrar Llegada
- Sumar Puntos

---

### Diagrama

- [Imagen Completa](/Practicas/Practica%203/Imagenes/10.jpg)

![](2023-05-04-13-44-09.png)

---

<div align="center">

### Registrar Persona

<table ><tr><td width="660"> 

**Nombre:** 
 
**Descripción:** 

**Actores:** 

**Precondiciones:** 

---

CURSO NORMAL<table> <tr><td>Acciones del actor</td> <td>Acciones del Sistema</td></tr>
<td width="320">  

Paso x:

</td><td width="320">

Paso x: 

</td></table>

---

**Curso alterno:**

**Postcondición:**

</table>

---

### Iniciar Sesión

<table ><tr><td width="660"> 

**Nombre:** 
 
**Descripción:** 

**Actores:** 

**Precondiciones:** 

---

CURSO NORMAL<table> <tr><td>Acciones del actor</td> <td>Acciones del Sistema</td></tr>
<td width="320">  

Paso x:

</td><td width="320">

Paso x: 

</td></table>

---

**Curso alterno:**

**Postcondición:**

</table>

---

### Cerrar Sesión

<table ><tr><td width="660"> 

**Nombre:** 
 
**Descripción:** 

**Actores:** 

**Precondiciones:** 

---

CURSO NORMAL<table> <tr><td>Acciones del actor</td> <td>Acciones del Sistema</td></tr>
<td width="320">  

Paso x:

</td><td width="320">

Paso x: 

</td></table>

---

**Curso alterno:**

**Postcondición:**

</table>

---

### Solicitar Turno

<table ><tr><td width="660"> 

**Nombre:** 
 
**Descripción:** 

**Actores:** 

**Precondiciones:** 

---

CURSO NORMAL<table> <tr><td>Acciones del actor</td> <td>Acciones del Sistema</td></tr>
<td width="320">  

Paso x:

</td><td width="320">

Paso x: 

</td></table>

---

**Curso alterno:**

**Postcondición:**

</table>

---

### Registrar Llegada

<table ><tr><td width="660"> 

**Nombre:** 
 
**Descripción:** 

**Actores:** 

**Precondiciones:** 

---

CURSO NORMAL<table> <tr><td>Acciones del actor</td> <td>Acciones del Sistema</td></tr>
<td width="320">  

Paso x:

</td><td width="320">

Paso x: 

</td></table>

---

**Curso alterno:**

**Postcondición:**

</table>

---

### Sumar Puntos

<table ><tr><td width="660"> 

**Nombre:** 
 
**Descripción:** 

**Actores:** 

**Precondiciones:** 

---

CURSO NORMAL<table> <tr><td>Acciones del actor</td> <td>Acciones del Sistema</td></tr>
<td width="320">  

Paso x:

</td><td width="320">

Paso x: 

</td></table>

---

**Curso alterno:**

**Postcondición:**

</table>

</div>

<img src= 'https://i.gifer.com/origin/8c/8cd3f1898255c045143e1da97fbabf10_w200.gif' height="20" width="100%">

<div align = 'center'>

## `Problema 11` Carga de empleados

</div>

Se desea modelar un sistema de carga de empleados de la facultad de Informática. Se ha realizado una reunión con el jefe de recursos humanos el cual nos detalló lo siguiente: cuando un nuevo empleado es contratado, debe ir a la oficina de recursos humanos y presentar a la secretaria, quien realiza la carga, su dni, apellido, nombre, edad y domicilio. Según el reglamento interno de la Facultad, para poder llevar a cabo el alta el sistema debe verificar que el nuevo agente no figure en la base de sumariados, de ser así se informa dicha situación y se cancela la carga. La base de sumariados es una base interna del sistema.

Además, según la ley 1231/6 de empleo, el sistema debe permitir asociar una obra social a un agente, para lo cual la secretaria deberá ingresar el dni del empleado. Luego el sistema debe consultar a un servidor si el agente es moroso. Para poder efectuar la consulta el sistema debe conectarse con el servidor y enviar el dni del empleado. En caso de morosidad el sistema deberá informar dicha situación permitiendo al empleado regularizar su situación en los próximos 30 días e imprimiendo un código de inicio de trámite. Si no es moroso el sistema le asocia la obra social e imprime un carnet. También se ha tenido una reunión con el jefe del área de comunicación visual, quien nos ha dado acceso al manual de estilo de la organización para que lo consultemos y respetemos cuestiones estéticas.

El sistema deberá permitir que el empleado avise la regularización de su deuda, para lo cual, existe una terminal electrónica, donde deberá ingresar su dni y código de inicio de trámite. Luego el sistema consultará al servidor de la obra social si efectivamente el agente dejó de ser moroso y de ser así le asignará la obra social imprimiendo un carnet. Si el empleado aún sigue siendo moroso se informará el error.

Suponga que el equipo de desarrollo tiene acceso a un sistema llamado Sigef para consultar su implementación dado que algunas funcionalidades son parecidas a las solicitadas.

---

### Actores
- Secretaria
- Empleado
- Servidor de la Obra Social

### Casos de Uso
- Alta Empleado
- Asociar Obra Social
- Validar Cliente
- Enviar Regulación

---

### Diagrama

- [Imagen Completa](/Practicas/Practica%203/Imagenes/11.jpg)

![](2023-05-04-13-45-19.png)

---

<div align="center">

### Alta Empleado

<table ><tr><td width="660"> 

**Nombre:** 
 
**Descripción:** 

**Actores:** 

**Precondiciones:** 

---

CURSO NORMAL<table> <tr><td>Acciones del actor</td> <td>Acciones del Sistema</td></tr>
<td width="320">  

Paso x:

</td><td width="320">

Paso x: 

</td></table>

---

**Curso alterno:**

**Postcondición:**

</table>

---
### Asociar Obra Social

<table ><tr><td width="660"> 

**Nombre:** 
 
**Descripción:** 

**Actores:** 

**Precondiciones:** 

---

CURSO NORMAL<table> <tr><td>Acciones del actor</td> <td>Acciones del Sistema</td></tr>
<td width="320">  

Paso x:

</td><td width="320">

Paso x: 

</td></table>

---

**Curso alterno:**

**Postcondición:**

</table>

---
### Validar Cliente

<table ><tr><td width="660"> 

**Nombre:** 
 
**Descripción:** 

**Actores:** 

**Precondiciones:** 

---

CURSO NORMAL<table> <tr><td>Acciones del actor</td> <td>Acciones del Sistema</td></tr>
<td width="320">  

Paso x:

</td><td width="320">

Paso x: 

</td></table>

---

**Curso alterno:**

**Postcondición:**

</table>

---
### Enviar Regulación

<table ><tr><td width="660"> 

**Nombre:** 
 
**Descripción:** 

**Actores:** 

**Precondiciones:** 

---

CURSO NORMAL<table> <tr><td>Acciones del actor</td> <td>Acciones del Sistema</td></tr>
<td width="320">  

Paso x:

</td><td width="320">

Paso x: 

</td></table>

---

**Curso alterno:**

**Postcondición:**

</table>


</div>
<img src= 'https://i.gifer.com/origin/8c/8cd3f1898255c045143e1da97fbabf10_w200.gif' height="20" width="100%">