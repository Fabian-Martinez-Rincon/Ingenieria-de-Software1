<h1 align="center">  Practica 1</h1>
<p><img width="270" align='right' src="https://media.giphy.com/media/ddR31ZMLGH10k/giphy.gif"></p>

- [Obtención de los requerimientos](#obtención-de-los-requerimientos)
  - [Parte I Definiciones](#Parte-I-Definiciones-Requerimientos)
  - [Parte II Problemas](#Parte-II-Problemas-Requerimientos)
- [Entrevistas](#Entrevistas)
  - [Parte I Definiciones](#Parte-I-Definiciones-Entrevistas)
  - [Parte II Situaciones](#Parte-II-Situaciones-Entrevistas)
  - [Parte III Problemas](#Parte-III-Problemas-Entrevistas)
- [Cuestionarios](#Cuestionarios)
  - [Parte I Definiciones](#Parte-I-Definiciones-Cuestionarios)
  - [Parte II Soluciones](#Parte-II-Soluciones-Cuestionarios)

# `Obtención de los requerimientos`

---

## *Parte I Definiciones Requerimientos*

`1)` Definir brevemente que es un requerimiento

Es una característica del sistema o una descripción de algo que el sistema es capaz de hacer con el objetivo de satisfacer el propósito del sistema.

`2)` Defina requerimientos funcionales y no funcionales.

*Funcionales:*

- Describen una interacción entre el sistema y su ambiente. Cómo debe comportarse el sistema ante determinado estímulo.
- Describen lo que el sistema debe hacer o incluso cómo NO debe comportarse.
- Describen con detalle la funcionalidad del mismo
- Son independientes de la implementación de la solución
- Se pueden expresar de distintas formas
  
*No Funcionales:*

- Describen una restricción sobre el sistema que limita nuestras elecciones en la construcción de una solución al problema
- Requerimientos de producto:
  Especifican el comportamiento del producto(usabilidad, eficiencia, rendimiento, espacio, fiabilidad, portabilidad)
- Requerimientos organizacionales
  Se derivan de las políticas y procedimientos existentes en la organización del cliente y en la del desarrollador (entrega, implementación, estándares)
- Requerimientos externos 
  Interoperabilidad, legales, privacidad, seguridad, éticos

`3)` Defina que es un **stakeholder**.

El termino *stakeholder* se utiliza para referirse a cualquier persona o grupo que se verá afectado por el sistema, directa o indirectamente.

**Entre estos se encuentra**

- Usuarios finales
- Ingenieros
- Gerentes
- Expertos del dominio
- Diferentes versiones....


`4)` Defina las fuentes más importantes para la obtención de información.

**Métodos discretos**

- Muestreo de la documentación, los formularios y los datos existentes
- Investigación y visitas al sitio
- Observación del ambiente de trabajo

Los métodos discretos son menos perturbadores que otras formas de averiguar los requerimientos. \
Se consideran insuficientes para recopilar información cuando se utilizan por sí solos, por lo que deben utilizarse junto con uno o varios de los métodos.\
Utilizar diferentes métodos para acercarse a la organización es una práctica inteligente mediante la cual podrá formarse un panorama más completo de los requerimientos.


**Métodos iteractivos**

- Cuestionarios
- Entrevistas
- Planeación conjunta de Requerimientos (JRP o JAD)
- Lluvia de ideas

Hay métodos interactivos que pueden usarse para obtener los requerimientos de los miembros de la organización Aunque son distintos en su implementación, estos métodos tienen muchas cosas en común. La base es hablar con las personas en la organización y escuchar para comprender.


`5)` Indique los puntos de vista (de manera genérica) que se pueden reconocer en un proyecto de software.

Existen tres tipos genéricos de puntos de vista:
- `Interactuadores`: Representan a las personas u otros sistemas que interactúan directamente con el sistema. Pueden influir en los requerimientos del sistema de algún modo.
- `Indirecto:` Representan a los stakeholders que no utilizan el sistema ellos mismos pero que influyen en los requerimientos de algún modo.
- `Dominio:` Representan las características y restricciones del dominio que influyen en los requerimientos del sistema.


`6)` Enumere tres problemas de comunicación que pueden existir en la elicitación de requisitos.

**Limitaciones cognitivas (del desarrollador)**
- No conocer el dominio del problema.
- Hacer suposiciones sobre el dominio del problema.
- Hacer suposiciones sobre aspectos tecnológicos.
- Hacer simplificaciones excesivas.

**Conducta humana**

- Conflictos y ambigüedades en los roles de los participantes.
- Pasividad de clientes, usuarios o ingenieros de requisitos.
- Temor a que el nuevo sistema lo deje sin trabajo.

**Técnicos**

- Complejidad del dominio del problema.
- Complejidad de los requisitos.
- Múltiples fuentes de requisitos.
- Fuentes de información poco claras.


---

## *Parte II Problemas Requerimientos*

**a) Indicar para cada problema quienes podrían ser los Stakeholders, los puntos de vista y las fuentes de información.**

- `1)` En un sistema de registro de asistencia a través de técnicas biométricas (huella digital) de estudiantes
universitarios para la cátedra de Ingeniería I. Este sistema se alimentará de un listado otorgado por la oficina
de alumnos de la facultad. Además, necesita la autorización del Jefe de Trabajos Prácticos del turno
correspondiente para luego los alumnos poder registrar el presente. También, el profesor a cargo de la
materia podrá consultar y listar el estado de cada alumno perteneciente a su cátedra. El sistema sólo se
utilizará en el ámbito de la facultad de Informática y deberá adecuarse a la reglamentación sobre privacidad
de los datos en el ámbito de la misma.

`StakeHolders`: Estudiantes de la catedra de Ingenieria 1, el profesor a cargo.\
`Fuentes de información`: Listado otorgado por la oficina de alumnos de la facultad.\
`Puntos de vista`: Jefe de Trabajos Prácticos, reglamentación sobre privacidad de los datos.

- `2)` Se desea desarrollar un sistema para gestionar y administrar la atención de pacientes en una clínica privada
especializada en tratamientos alérgicos. Cuando un paciente nuevo es ingresado a la clínica el empleado
registra todos sus datos personales, posteriormente un enfermero registra los controles y realiza las
anotaciones habituales (temperatura, presión, peso, reacciones alérgicas etc.). Luego, el paciente es derivado
con alguno de los doctores de la clínica, quién registra qué tratamientos deberá realizar. El médico también
se encarga de registrar si el paciente debe quedar internado y debe mantener su historia clínica durante el
período que dure el tratamiento. Se sabe que el director de la clínica puede consultar las historias clínicas de
todos los pacientes. El sistema debe adecuarse a las normativas impuestas por el ministerio de salud de la
provincia de Bs As.

`StakeHolders`: Empleado, Enfermero, Paciente\
`Fuentes de información`: Datos personales registrados por un empleado.\
`Puntos de vista`: Director, normativas impuestas por el ministerio de salud de la provincia de Bs As.\

**b) Habiendo resuelto los problemas presentados, ¿por qué considera que los requerimientos de los distintos stakeholders podrían entrar en conflicto? UNLP – Facultad de Informática**

---

# `Entrevistas`

## Parte I Definiciones Entrevistas

- `1)` Describa qué tipo de información puede obtenerse en una entrevista.
- `2)` Enumere y describa brevemente las etapas de la preparación de una entrevista.
- `3)` Enumere y describa brevemente qué tipos de preguntas puede contener una entrevista. Detalle ventajas y desventajas de cada una.
- `4)` Enumere y describa brevemente qué tipo de estructuras y organización existen para el armado de una entrevista
- `5)` Analice un formato de la planilla adecuado al momento de armar una entrevista.
- `6)` Analice un formato de la planilla adecuado al momento de terminar una entrevista.

---

## Parte II Situaciones Entrevistas

### *Situación 1*

Tiene una entrevista con el gerente de ventas de una empresa el cual desea informatizar dicho sector pero no tuvo tiempo de preparar las preguntas por lo que le pidió a un nuevo empleado que le prepare algunas. Cuando las lee, se da cuenta que son inadecuadas. \
Lea las preguntas y vuelva a redactarlas de una manera más apropiada. Especifique por qué le parece inadecuada cada una de ellas.

- `a)` Sus subordinados me dijeron que la empresa no anda bien. ¿Es cierto?
- `b)` Soy nuevo en esto. ¿Qué he dejado afuera?
- `c)` ¿Estará usted de acuerdo con los demás gerentes de ventas, respecto a que computarizar las ventas mensuales y luego realizar un análisis de la tendencia tendría usted grandes mejoras?
- `d)` ¿No habrá una mejor manera de hacer proyecciones de sus ventas, que ese procedimiento anticuado que usted utiliza?


### *Situación 2*

Apenas ha entrado a la oficina de su entrevistado se da cuenta que él no ha dejado de revisar papeles, mirar el reloj y hacer llamadas telefónicas. Usted supone que se siente nervioso porque está atrasado con otro trabajo que tiene que terminar.

- `a)` Explique brevemente cómo resolvería tal situación.
- `b)` Qué opciones propone para el caso en que la entrevista no pueda reprogramarse.

 
### *Situación 3*

El siguiente es el primer informe de una entrevista realizada por uno de los miembros de su equipo de análisis de sistemas:

“En mi opinión, el resultado de la entrevista fue muy bueno. El entrevistado me permitió hablar con él durante una
hora y media. Me relató toda la historia del negocio, que fue muy interesante. También mencionó que las cosas no
han cambiado desde que él ha estado en la empresa, hace aproximadamente 16 años. En breve nos reuniremos
nuevamente para terminar la entrevista, pues, no tuvimos tiempo para analizar las preguntas que preparé “.

- `a)` Lea atentamente el informe de la entrevista y explique qué sensación le deja dicho informe.
- `b)` Indique si existe información que es irrelevante en el informe.
- `c)` Mencione tres sugerencias que le haría a su compañero de equipo para que realizara una mejor entrevista la próxima vez.

---

### Parte III Problemas Entrevistas

### *Problema 1*

Preparar una entrevista para obtener los requerimientos del siguiente problema:

Se desea desarrollar un sistema que permita compartir un vehículo para un viaje. La idea es que cuando una persona tiene que realizar un viaje lo publique en la aplicación. Luego el resto de los usuarios se postulan para acompañarla y el chofer podrá seleccionar quienes viajan. El objetivo es abaratar costos y evitar congestiones en el tránsito.

### *Problema 2*

Preparar una entrevista para obtener los requerimientos del siguiente problema:\
CookBooks es un negocio pequeño manejado por una pareja jubilada. Hasta este momento, Cookbooks ha vendido sus libros sólo a través de pedidos por correo. Los dueños ahora quieren desarrollar un sistema en línea para vender libros de cocina difíciles de conseguir y agotados a través de internet.\
Los visitantes podrán hojear diferentes libros de cocina, pero tendrán que crear una cuenta del cliente antes de poder hacer una compra. Los pagos se aceptarán sólo en línea con una tarjeta de crédito reconocida

---

# `Cuestionarios`

## Parte I Definiciones Cuestionarios

- `1)` Describa qué tipo de información se busca mediante la aplicación de cuestionarios.
- `2)` Describa bajo qué circunstancia considera apropiado utilizar cuestionarios.
- `3)` Describa los dos tipos de cuestionarios.

## Parte II Soluciones Cuestionarios

### *Solución 1*

Alguien nuevo en el centro de cómputo de un gimnasio que tiene varias sucursales, viene con muchas ganas de
mejorar las cosas que ve dentro del mismo. Dicho centro está desarrollando un sistema en red que usarán todas las
sucursales.\
Dado el siguiente cuestionario verifique si es necesario reescribir las preguntas, justifique.

<table>

<td>

### Cuestionario 1

¡Urgente! Complételo y devuélvalo de manera inmediata, sino su cheque de pago será retenido
hasta que devuelva el presente.
- `1)` En pocas palabras indique qué problemas ha tenido el actual centro de cómputo.
- `2)` ¿Habrá alguien que piense de la misma manera que usted? Enumere sus nombres.
- `3)` ¿Cuántas PC fallaron en estos últimos 6 meses?
- `4)` ¿Cuál es el problema más grande que enfrenta al comunicar sus problemas al centro de
cómputo?

</td>
</table>

### *Solución 2*

El siguiente es un cuestionario diseñado por un empleado de una empresa textil que se especializa en fabricar medias para hombres. Este empleado lo escribió en calidad de gerente de la oficina que tiene a cargo la propuesta de compra / implementación de un nuevo sistema de cómputos.

<table><td>

¡Hola a todos los empleados!
Según los rumores, estamos tras una nueva computadora. Aquí hay algunas preguntas para que reflexionen.

- `a)` ¿Cuánto tiempo ha usado la computadora vieja?_______________________
- `b)` ¿Con que frecuencia se descompone?_______________________________
- `c)` ¿Quién la repara?________________________________________________
- `d)` ¿Cuándo fue la ultima vez que usted sugirió una mejora al sistema de cómputos y esta
se puso en práctica? ¿De qué se trató?________________
- `e)` ¿Cuándo fue la última vez que usted sugirió una mejora al sistema de cómputos y
nadie la usó? ¿De que se trató?___________________________
- `f)` ¿Usted utiliza una pantalla o una impresora, o ambas?___________________
- `g)` ¿Qué tan rápido escribe en la computadora?___________________________
- `h)` ¿Cuántas personas necesitan acceder a la base de datos regularmente en su sucursal?
¿Hay alguien que actualmente no utilice la computadora y que le gustaría
hacerlo?_________________________________________________

</td></table>

- `a)` Reformule o elimine las preguntas que considere inapropiadas.
- `b)` Realice una crítica sobre el diseño y el estilo en cuanto a espacio en blanco, espacio para las respuestas, facilidad para responder, etc.
- `c)` Escriba el cuestionario nuevamente, teniendo en cuenta lo respondido en los puntos a y b.
UNLP – Facultad de Informática'