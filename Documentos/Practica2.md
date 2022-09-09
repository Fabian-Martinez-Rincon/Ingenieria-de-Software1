<h2 align="center">  Ingeniería de Software I
Práctica 2 – Historias de Usuario</h2>

Para cada Historia de Usuario se deben indicar los siguientes ítems:

<table><tr><td> Formato </td> </tr>
<tr><td>

**ID:** Identificador unívoco de la historia expresado como texto generalmente de la forma \<verbo> \<sustantivo>
 
**TÍTULO:** Descripción de la historia de la forma: **Como** \<rol> **quiero** \<algo> **para poder** \<beneficio>

**REGLAS DE NEGOCIO:** Conjunto de reglas, normas, políticas, leyes, etc. que condicionan el modo de operación (Requisitos no funcionales)

**CRITERIOS DE ACEPTACIÓN:** Criterios por los cuales una historia cumple con las expectativas del cliente.\
El formato es el siguiente:

- **Escenario 1:** título del criterio.\
    Dato \<un contexto inicial>
Cuando \<ocurre un evento>,
Entonces <garantiza uno o más resultados>
- **Escenario 2:** título del criterio.\
    Dato \<un contexto inicial>
Cuando \<ocurre un evento>,
Entonces <garantiza uno o más resultados>
- **Escenario N:** título del criterio.\
    Dato \<un contexto inicial>
Cuando \<ocurre un evento>,
Entonces <garantiza uno o más resultados>
...


</td></tr></table>

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

**Para cada problema planteado realice las tarjetas completas de todas las historias de usuario identificadas**



## `Problema 1` Alquiler de mobiliario

Suponga que trabaja en una consultora la cual ha sido recientemente contactada por una empresa de alquiler de mobiliario
para eventos para la realización de una app.
De las diferentes entrevistas se ha obtenido la siguiente información:
El gerente nos dijo que resulta fundamental tener una aplicación móvil que nos permita manejar la agenda de la empresa,
sabiendo qué disponibilidad tenemos y permitiendo que nuestros clientes alquilen a través de la app. Para esta primera
versión de la app, el gerente nos pidió que sea posible dar de alta los diferentes mobiliarios, así como la posibilidad de que
los usuarios puedan realizar una reserva de alquiler desde sus dispositivos. Para el detalle de cómo se realiza la carga de
los muebles, el gerente nos sugirió hablar con el encargado del departamento de mobiliario. El encargado de mobiliario
nos comentó que de cada mueble se debe cargar código de inventario, tipo de mueble, fecha de creación, fecha de último
mantenimiento, estado (libre, de baja, alquilado) y el precio de alquiler. Además, no pueden existir códigos repetidos y por
el contrato de la franquicia, el precio debe cargarse en dólares. Para que el encargado pueda dar de alta el mobiliario debe
autenticarse en el sistema. El registro de los usuarios de carga no debe modelarse.
El encargado del departamento de alquileres no comentó acerca de las reservas de los alquileres. Por una política
comercial de la marca una reserva tiene que incluir como mínimo 3 muebles. La reserva debe tener una fecha, lugar del
evento, cantidad de días y mobiliario junto a su cantidad. Para realizar una reserva se debe abonar el 20% del total del
alquiler. El pago de la reserva se realiza únicamente con tarjeta de crédito validando número de tarjeta y fondos a través de
un servicio del banco. Luego de efectuado el pago, se emite un número de reserva único que será luego utilizado por el
cliente para hacer efectivo el alquiler.

## `Problema 2` Posgrado

Suponga que trabaja en el área de sistemas de la Facultad de Informática y se le solicitó la automatización del pago de
carreras de posgrado. Inicialmente se coordinó una reunión con el director del posgrado y se obtuvo la siguiente
información:
Ya que no se desea seguir cobrando el dinero en la secretaría, es necesario que los alumnos puedan pagar las carreras vía
web. Como el director de posgrado no realiza tareas administrativas nos recomendó hablar con el secretario académico.
De la entrevista con el secretario académico se obtuvo la siguiente información:
Es necesario cargar las carreras a un sistema. En esta primera versión del sistema sólo se nos pidió esta funcionalidad, sin
la modificación ni eliminación. De cada carrera se conoce: nombre de la carrera (no puede repetirse), duración en años (a
partir de la consulta del estatuto de posgrado se obtuvo que como máximo son 5 años), costo y cantidad máxima de cuotas
para el pago. La carga de las carreras no la realiza el secretario académico sino un empleado administrativo.
Al preguntarle por la dinámica del sistema, el secretario académico nos derivó con el jefe del área administrativa, con el
cual hicimos otra entrevista y pudimos obtener la siguiente información:
El requerimiento fue que el alumno ingrese a la web de posgrado y pueda registrarse ingresando: nombre, apellido,
nombre de usuario (único) y contraseña (más de 6 dígitos). Cualquier alumno previamente registrado, puede iniciar sesión con su nombre de usuario y contraseña, habilitándose la inscripción a alguna de las carreras. Para ejemplificar esta
funcionalidad nos otorgaron acceso al sistema SIGEF, el cual realiza funcionalidades similares para las carreras de grado.
Para inscribirse, el alumno deberá seleccionar la carrera, ingresar la cantidad de cuotas a pagar, ingresar el número de
tarjeta y, en caso de que la tarjeta sea válida y tenga fondos, se hará efectivo el cobro y la inscripción. La tarjeta de crédito
se valida a través de un servicio del banco con el cual la universidad tiene convenio. Luego de efectuado el cobro, el
sistema debe imprimir dos comprobantes, uno de inscripción y otro de pago. La única forma que tiene el alumno de pagar
es con tarjeta de crédito

## `Problema 3` Contratos

Suponga que trabaja en un grupo en el área de sistemas de una organización y está por comenzar un nuevo proyecto para
desarrollar un sistema que depende del departamento contable.
El sistema deberá administrar los contratos realizado con terceros. En una de las reuniones con el jefe de departamento
nos dijo que él no usará el sistema pero que recibirá listados del personal contratado ya que deberá firmarlos para
elevarlos a las autoridades.
Para obtener más información generamos una reunión con el empleado de mesa de entradas. Nos contó que el problema
que tienen actualmente es que realizan todas las minutas a mano por lo cual desean automatizar esta tarea. Las minutas
son el paso previo a un contrato. Para confeccionar una minuta, el empleado de mesa de entradas debe ingresar nombre y
número de CUIT de una persona a contratar, tipo de contrato, fecha de comienzo, duración y monto, a lo que el sistema le
asociará un número de minuta automáticamente. Nos recomendó leer la reglamentación vigente acerca de contratos de la
que obtuvimos que los montos de los mismos no pueden superar los $25.000 y que la duración debe ser como máximo de
6 meses.
Una vez confeccionada la minuta por parte del empleado de mesa de entradas, la misma queda pendiente de aprobación.
El que puede aprobar una minuta es el empleado de rendiciones. Realizamos una reunión con él y nos contó que su tarea
consiste en evaluar las minutas para determinar su aprobación. También nos dijo que en otro trabajo que tiene usan un
sistema llamado MiMiNuTa al que nos puede dar acceso para ver como hacen esa tarea. Después del análisis de este
sistema, se concluyó que para aprobar una minuta necesitaría ingresar un número de minuta y que el sistema muestre los
datos de la misma para poder aprobarla. Nos dijo que no puede aprobar la minuta si la persona a contratar tiene 3 contratos
vigentes (minutas aprobadas) ni tampoco si el CUIT de la persona a contratar está inhabilitado por la AFIP. Actualmente
se comunica telefónicamente con la AFIP para realizar esta verificación, pero sabe que ésta provee un servicio para
aplicaciones que permite hacer la verificación en línea. Esto último nos obligó a generar una reunión con el administrador
de servidores de la AFIP. Nos dijo que para poder conectarnos con un servidor de la AFIP, el sistema debe mandar un
token (código que identificará de manera única a nuestra aplicación) y CUIT, si el token es correcto, el servidor responde
si el CUIT está habilitado o no.
Por último el empleado de rendiciones será el responsable de imprimir los listados con las minutas aprobadas, es decir, un
listado con el personal contratado para poder dárselo al jefe de departamento para que lo firme.

## `Problema 4` Venta de bebidas

Se desea modelar un sistema para el manejo de venta de bebidas alcohólicas en linea. Para poder empezar a comprar en el
sitio, es necesario que las personas se registren ingresando nombre, apellido, mail (será utilizado como nombre de usuario
por lo tanto debe ser único) y edad. Solo se permite que se registren al sitio personas mayores a 18 años, de lo contrario el
sistema debe mostrar en pantalla el texto de la ley que impide la venta de bebidas alcohólicas a menores. Si el registro es
exitoso el sistema genera una contraseña que es enviada al mail ingresado en el registro.
Para comprar el usuario debe iniciar sesión y una vez logueado el sistema muestra una lista de bebidas, una vez que el
usuario selecciona todos los productos que desea comprar, si el usuario es premium se le hace un descuento del 20% y se informa en pantalla el total menos el 20%. Ademas si el usuario seleccionó productos por un monto superior a los $4500
se le hace un 10% de descuento y se informa en pantalla el total menos el 10%. Tenga en cuenta que si el usuario es
premium y compra por un monto superior a $4500 se deben aplicar ambos descuentos

## `Problema 5` Casa de fotografía

Se desea desarrollar un sistema para la impresión de fotos para una casa fotográfica. Los clientes pueden subir sus
fotos, pagar por internet y luego ser retiradas personalmente por el local.
Para subir las fotos la persona debe registrarse en el sitio, ingresando sus datos personales, nombre, apellido, email,
domicilio, nombre de usuario y contraseña.
Una vez autenticado, el usuario puede subir un máximo de 50 fotos para ser impresas. Las fotos se ingresan de a
una. Una vez subidas, el usuario debe abonar el monto total (el valor de cada foto es de $15). El pago se realiza con
tarjeta de crédito, ingresando los datos de la misma (número de tarjeta, código de seguridad y nombre del titular), la
cual debe ser validada a través del sistema del banco. Una vez que se realiza el pago se le otorga al cliente un código
único que le servirá posteriormente para retirar las fotos.
Un cliente debe acercarse a la sucursal para retirar las fotos enviadas previamente. Para esto debe presentar el
código único a un empleado. Este registra el código, la fecha de retiro y entrega las fotos al cliente.

## `Problema 6` Biblioteca


La biblioteca de una escuela primaria realiza su trabajo de forma manual y requiere un sistema informático que
automatice su funcionamiento.
La bibliotecaria recibe libros por donaciones de los padres de los chicos que asisten a la escuela. De un mismo libro
se pueden tener varios ejemplares.
Para que un alumno pueda asociarse debe presentar el DNI y certificado de alumno regular. Una vez asociado, se le
otorga un carnet con su correspondiente número de socio.
Los préstamos se realizan exclusivamente a socios habilitados, que no posean más de tres préstamos vigentes y no
tengan préstamos vencidos. La bibliotecaria presta libros que se encuentren en buen estado. Cuando un libro se
encuentra deteriorado ya no se presta.
Cuando el socio retorna un libro se verifica si el préstamo se encuentra vencido. En este caso, la bibliotecaria
suspende al socio, que por 15 días no podrá solicitar nuevos préstamos.

## `Problema 7` Mutual

Una mutual necesita automatizar el manejo de las prestaciones que ofrece a sus afiliados.
Una persona puede afiliarse sólo si posee una tarjeta de crédito para que se pueda hacer el pago de la cuota mensual
automáticamente. Una vez que la persona se ha afiliado, puede pasar a tener a cargo a su pareja e hijos (hasta 18 años,
luego es dado de baja). A cada uno se le otorga un número de afiliado.
Las prestaciones que brinda, siempre y cuando esté asentado el pago del mes anterior al que es solicitado, son:
-Ortodoncia: Se reconoce sólo una y a los afiliados menores de 15 años que estén afiliados desde al menos
nueve meses. Debe presentarse historia clínica elaborado por el profesional.
-Plantillas: A cualquier afiliado, hasta dos por año calendario. Debe presentarse la indicación del profesional y
factura del comercio que la confeccionó.
-Anteojos: A cualquier afiliado con fecha de afiliación superior a tres meses, un par cada 18 meses.
-Internación: A cualquier afiliado, sin límite.
-Consultas médicas: A cualquier afiliado, hasta 2 por mes.

## `Problema 8` Teatro

Se desea modelar un sistema de gestión de ventas de entradas para un teatro. Las personas compran sus entradas a
través de una página web, o personalmente.
El sistema permite, sólo de modo personal en el teatro, la reserva de entradas de forma gratuita. El empleado debe
ingresar los datos de la obra (fecha, hora, y nombre) junto el nombre y DNI del espectador. En este caso, sólo se podrá
reservar hasta 2 entradas. Las entradas reservadas no compradas caducarán tres horas antes del evento. Para seleccionar
el nombre de la obra, el sistema muestra una grilla de funciones disponibles para que el usuario seleccione una.
Para comprar una entrada vía web, el sistema muestra la grilla de funciones disponibles. El usuario selecciona una
opción, ingresa su DNI, la cantidad de lugares solicitados y selecciona la opción “pagar”. El pago se realiza con tarjeta de
crédito. Para esto debe ser autorizada a través del sistema del banco. Este pide el número de tarjeta, vencimiento, y
código de seguridad. Verifica todos los campos y autoriza la compra. Autorizada la tarjeta, se emite un código de compra
con el que el cliente podrá retirar sus entradas en la boletería del cine.
Para comprar una entrada personalmente, el vendedor de la boletería solicita los datos de la función al cliente,
procediendo de un modo similar a la compra web, con la diferencia que en este caso no se muestra el código de compra
sino que se imprimen directamente la/s entrada/s. El pago es unicamente con tarjeta de crédito, igual que en el caso
anterior.
Para retirar las entradas reservadas previamente, el empleado solicita nombre y DNI del espectador, el sistema
valida que la persona posea entradas reservadas, y que no estén caducas. El resto del procedimiento se realiza igual que
la compra de entradas descriptas anteriormente.
Cuando una persona llega con el código de compra, el vendedor debe ingresar el código para que el sistema, luego
de verificarlo, imprima las entradas correspondientes.
Además se desea administrar la programación de las salas. El administrador ingresa la distribución semanal de las
obras en las salas de manera que se encuentre disponible para la realización de la venta de entradas

## `Problema 9` Pago Electrónico

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

## `Problema 10` Un Aventón

Se desea desarrollar un sistema que permita compartir un vehículo para un viaje. La idea es que cuando una persona
tiene que realizar un viaje lo publique en la aplicación. Luego, el resto de los usuarios se postulan para acompañarla y el
chofer podrá seleccionar quienes viajan. El objetivo es abaratar costos y evitar congestiones en el tránsito. El sistema es
gratuito.
Para utilizar el sistema, una persona debe registrarse y estar correctamente identificado antes de poder utilizarlo. Al
registrarse, se pide un nombre de usuario, un correo electrónico y una contraseña. No puede haber dos correos
electrónicos iguales en el sistema. Una vez autenticado, podrá dar de alta diferentes viajes, identificando la fecha, hora y
el automóvil que utilizará. Los diferentes viajes que una persona publique no pueden superponerse. Un usuario que
adeuda calificaciones tampoco podrá publicar un viaje.
Cualquier usuario identificado podrá postularse a un viaje. Luego, el usuario dueño del viaje podrá aceptar o
rechazar los candidatos para que realicen el viaje con él.
En el sistema existe una política de reputaciones que permiten a los usuarios conocer la opinión del resto sobre los
viajes realizados. Luego de terminado un viaje, tanto el piloto como los copilotos que viajaron deberán calificarse entre
sí. El piloto califica a todos sus copilotos. Cada copiloto califica al piloto del viaje. Las calificaciones podrán ser positivas
(suma un punto de reputación) o negativas (restan un punto de reputación)

## `Problema 11` Concursos

Suponga que el área para la cual trabaja fue contactada para implementar un sistema para el manejo de concursos de los
docentes de la Facultad de Informática.
El docente que quiera inscribirse a un concurso deberá registrarse previamente en el sistema. Para esto deberá ingresar
los siguientes datos: Dni, nombre, apellido y dirección de mail. Una vez completado los datos el sistema mandará a la
casilla de correo ingresada la contraseña asignada automáticamente. El mail debe ser único y será utilizado como
nombre de usuario. Según el estatuto de la UNLP los dni permitidos para concursar son aquellos menores a 55 millones y
mayores a 12 millones.
Una vez registrado el docente puede inscribirse al concurso, para lo cual, una vez que haya ingresado al sistema, deberá
seleccionar la materia a la cual desea inscribirse. Según el reglamento interno de la Facultad de informática que nos
facilitó el jefe del área de personal, el docente no podrá inscribirse a más de 3 concursos. Cuando el docente acepta la
inscripción el sistema deberá imprimir un comprobante.
Por último, para cumplir con la ordenanza número 123/19 de la UNLP, el jefe del área de concursos, el cual ya cuenta con
un nombre de usuario y contraseña, deberá poder imprimir un listado con los inscriptos a una materia determinada para
poder enviar dicho listado al secretario administrativo quien lo firma y eleva al decano de la Facultad. Suponga que el
sistema Siu-Guarani realiza una tarea similar a la solicitada y que puede consultar su implementación y registros.

## `Problema 12` Créditos bancarios

Se desea modelar mediante historias de usuario el manejo de créditos otorgados por un banco a sus clientes.
Los clientes que desean pedir un crédito, deben iniciar un trámite a través de un sitio web del banco ingresando dni,
nombre, apellido, mail, tipo de crédito (personal, vivienda, etc.) y monto solicitado. El sistema acepta el inicio de trámite
si el dni ingresado corresponde a un cliente del banco y si el crédito solicitado no supera los $400.000. En caso de que no
sea cliente del banco el sistema deberá enviar un correo electrónico al email ingresado con un instructivo para hacerse
cliente del banco. Si el monto supera los $400.000 el sistema rechaza el inicio de trámite y muestra el mensaje “El monto solicitado excede el límite permitido”. Si los datos son correctos, el sistema almacena el trámite para que sea analizado
por el área económica e imprime un número de comprobante para el cliente.
Por otro lado, los clientes pueden consultar el estado de un trámite, para esto es necesario que se ingrese un número de
comprobante. Si el número de comprobante es válido, el sistema retorna un informe con el estado del mismo, de lo
contrario mostrará un mensaje “trámite inexistente”. Si el cliente ingresa tres veces un código inexistente el sistema
bloquea la ip (dirección de red de la máquina que efectúa la consulta) del cliente por 24 horas mostrando un mensaje
“Usted ha excedido el número de consultas inválidas”.
Por último, el gerente del banco puede pedir un listado de créditos aprobados entre fechas. Si las fechas ingresadas son
válidas, el sistema mostrará un listado con los créditos aprobados, de lo contrario mostrará un mensaje “las fechas
ingresadas no son válidas”. El sistema utiliza un sistema de autenticación general del banco, por lo que no es necesario
modelar el iniciar y cerrar sesión. Si no hay créditos aprobados para las fechas ingresadas el sistema mostrará el siguiente
mensaje: ”No hay créditos aprobados en las fechas ingresadas”.

## `Problema 12` Venta de libros

Una nueva empresa de venta de libros en línea está diseñando su sitio web. Cualquier visitante puede acceder a su
catálogo de libros y navegar los distintos libros que se encuentren en él y solo los usuarios registrados pueden realizar
compras.
Para poder comprar los libros se necesita un usuario registrado. El proceso de registro se realiza en dos pasos. En el
primer paso el sistema requiere Nombre, Apellido, DNI y cuenta de correo electrónico (que no exista en el sistema) y una
clave de 6 caracteres para darlo de alta de forma parcial. En este proceso el sistema debe generar un código de 16 dígitos
y enviarlo por correo para que luego el visitante confirme la cuenta. Como segundo paso el visitante debe entrar a la
página de confirmación e ingresar su dirección de correo y el código de 16 dígitos. Si estos datos son correctos el sistema
lo registra definitivamente como usuario.
Una vez registrado, para autenticarse, el sistema requiere el correo del usuario y la clave de 6 caracteres.
Para realizar la compra de un libro el sistema pide ingresar el ISBN del mismo y muestra al usuario la portada con una
descripción del libro y la opción “Comprar”. Cuando el usuario selecciona “Comprar” se le pide los datos de la tarjeta:
Apellido, Nombre, Nro de tarjeta. Es importante tener en cuenta que por disposición del Banco Central solo el titular de
la tarjeta puede realizar la compra, por lo que el nombre y apellido registrado debe coincidir con el de la tarjeta.
Realizada esta verificación se procede a enviar los datos al servidor de la tarjeta para realizar el cobro. Si todo es correcto
se genera un enlace de descarga al correo del usuario

## `Problema 13` Manejo de tarjetas de crédito

La gerencia del banco donde trabajamos nos pide realizar un subsistema para el manejo de las tarjetas de crédito SIVA.
El sistema podrá ser operado únicamente por el personal de área comercial y por el gerente de la sucursal. En ambos
casos las funcionalidades solo serán habilitadas con autenticación previa.
El registro del personal en el sistema no es necesario implementarlo, ya que las credenciales son obtenidas del sistema
central del banco. Entonces, para autenticarse, el usuario debe ingresar sus credenciales (las mismas que usa para otros
servicios del banco) y estas son corroboradas por el sistema del banco central (al cual nos comunicamos por intranet),
enviándonos un token de autenticación válido en caso de ser correctas. Una vez autenticado, todo el personal debe poder dar de alta una nueva tarjeta y dar de baja una existente. Para dar de
alta se requiere nombre completo, DNI y CUIT del titular. Luego, se debe seleccionar un tipo de tarjeta (Básica o Gold).
Para dar de alta la tarjeta la persona debe ser cliente del banco y no podrá darse de alta una tarjeta si la persona es
morosa en el sistema SIVA (externo al banco). Para esto, nuestro sistema debe comunicarse con el SIVA y verificar la
morosidad de la persona con el DNI. En el mismo momento, el sistema SIVA nos dará un número de tarjeta nuevo.
Para dar de baja una tarjeta, simplemente se debe ingresar el número de tarjeta y el sistema la debe eliminar de la base
de datos del banco.
El gerente, además, podrá pedir un listado de las operaciones realizadas entre dos fechas. Para esto el sistema le pedirá
que ingrese ambas fechas y le mostrará un listado. No debe ser posible ingresar fechas futuras al presente, ni tampoco
que la fecha de inicio sea mayor a la fecha de fin

## `Problema 13` Manejo de canchas de tenis


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

## `Problema 14` Procesamiento de imágenes

Se desea modelar un sub-sistema de procesamiento de imágenes astronómicas para un observatorio. El objetivo del
sub-sistema será cargar una imagen, que un usuario experto la analice y recorte ciertas áreas de interés.
Para poder usar el sistema, el operario debe autenticarse. Para esto, el sub-sistema se conecta al sistema general del
observatorio (no administrado por nosotros) para validar las credenciales (nombre de usuario y contraseña). De ser
correctas, el sistema de autenticación retorna un token indicando la autenticación correcta. Al terminar de usar el
sistema, el usuario debe cerrar la sesión.
Una vez autenticado, el operario debe poder hacer dos operaciones principales: cargar una imagen nueva y recortar
áreas de interés. Para cargar una nueva imagen, el sistema debe mostrar una serie de archivos posibles donde el usuario
debe seleccionar el deseado. El sistema no debe mostrar como opciones imágenes que tengan menos de 2Megapixeles
de resolución. Una vez seleccionada la imagen, el sistema debe mostrar la opción de visualizarla en escala de grises o a
color. El usuario puede seleccionar la opción que quiera.
Para recortar áreas de interés, debe haber previamente cargada una imagen. No se podrán recortar más de 4 áreas. El
sistema dejará al usuario que marque consecutivamente cada área de interés. Si algún área se superpone con otra el
sistema debe notificarlo como un error. Una vez seleccionadas las áreas, el sistema almacena en disco los resultados.
Por último, debe existir un usuario supervisor, que además de las funcionalidades del operario, también podrá pedir un
listado de las últimas imágenes procesadas. El supervisor debe poder seleccionar entre qué fechas mostrar el listado.
Luego el sistema mostrará una debajo de la otra todas las imágenes procesadas. Por cuestiones de visualización, el
sistema no debe permitir mostrar más de 20 imágenes a la vez.