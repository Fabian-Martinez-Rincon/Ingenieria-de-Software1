<div align="center">

[![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/Nomadiix/IS1)
[![GitHub stars](https://img.shields.io/github/stars/Nomadiix/IS1)](https://github.com/FabianMartinez1234567/IS1/stargazers/)
[![GitHub repo size in bytes](https://img.shields.io/github/repo-size/Nomadiix/IS1)](https://github.com/Nomadiix/IS1)
 </div>
 
<h1 align="center"> 📊 Practica 4</h1>
<div align="center">
<img src="https://media.giphy.com/media/Wz8BcbiANKcXF5Jy6S/giphy.gif"/>
</div>

---

- [Ejercicio 1]()
- [Ejercicio 2]()
- [Ejercicio 3]()
- [Ejercicio 4]()
- [Ejercicio 5]()
- [Ejercicio 6]()
- [Ejercicio 7]()
- [Ejercicio 8]()
- [Ejercicio 9]()
- [Ejercicio 10]()
- [Ejercicio 11]()
- [Ejercicio 12]()

---

Se detallan a continuación los pasos a seguir para realizar la construcción de un DTE:

- `1)` Identificar todos los estados del sistema y representarlos como cajas. Los nombres de los estados se escriben en gerundio.
- `2)` Desde el estado inicial (único), comenzar a identificar los cambios del sistema que lo llevan de un estado a otro y representarlos con flechas (transiciones) que van desde el estado origen al estado destino.
- `3)` Analizar, para cada transición, el evento, condiciones y las acciones para pasar de un estado a otro.
- `4)` Verificación de Consistencia: una vez dibujado el DTEdebemos verificar que se cumplan las siguientes condiciones.
    - a. Se han definido todos los estados.
    - b. Se pueden alcanzar todos los estados.
    - c. Se puede salir de todos los estados.
    - d. En cada estado, el sistema responde a todas las condiciones posibles (Normales y Anormales). No debería haber transiciones recurrentes (mismo estado origen y destino) sin acciones.

---

## Ejercicio 1.

Dado el siguiente diagrama que representa el funcionamiento de una Licuadora, corrija los errores existentes. La licuadora tiene 2 velocidades y sólo dos botones: uno para aumentar la velocidad y otro para disminuirla. La licuadora se apaga con el botón disminuir estando en la primera velocidad.

![image](https://user-images.githubusercontent.com/55964635/223026391-d12f9f54-2c4d-4ca1-b28b-ad048ca16744.png)

## Ejercicio 2. Complete el siguiente diagrama DTE que ilustra el comportamiento de una máquina de gaseosas, en base al siguiente enunciado:

La máquina se activa cuando el usuario ingresa una moneda. Todos los productos tienen el mismo valor. Las monedas son ingresadas de a una y cada una es validada en ese mismo momento, en base a su tamaño, peso y espesor mediante un dispositivo específico. Al mismo tiempo se valida el monto ingresado. Si alguna moneda no es válida, se retorna al usuario, y continúa el proceso normalmente. Como siguiente paso, el usuario debe seleccionar un producto. Si no hay stock de dicho producto entonces debe retornar las monedas y mostrar un mensaje informando tal situación. Si hay stock, se entrega el producto, y en caso de que se haya ingresado un monto superior, la máquina retorna el vuelto correspondiente. El usuario puede cancelar en cualquier momento, dando por finalizado todo el proceso.

![image](https://user-images.githubusercontent.com/55964635/223026577-7a8c1362-22ac-4b1d-8ffc-8db59f5507ff.png)

## Ejercicio 3.

Se desea modelar con un DTE el acceso a una caja fuerte, la cual posee un código de seguridad con una longitud desconocida. La caja presenta un teclado numérico y un botón “aceptar”. Si el código es incorrecto el sistema debe terminar indicando un error.

Analice las siguientes soluciones y discuta las diferencias.

![image](https://user-images.githubusercontent.com/55964635/223027130-a805c235-e534-45ec-b0c2-9104a04016b5.png)

## Ejercicio 4. Realizar el DTE para modelar un turbo ventilador.

Considere un sistema de control de un turbo ventilador que posee tres niveles de velocidad. Para ir de un nivel a otro, ya sea anterior o posterior, se debe girar una perilla en forma secuencial. Inicialmente el ventilador se encuentra apagado. Girando la perilla en el sentido de las agujas del reloj se enciende y se aumenta la velocidad, mientras que girando la perilla en el sentido contrario se disminuye. El ventilador puede ser apagado girando hacia la izquierda en el nivel 1 o hacia la derecha en el nivel 3.

## Ejercicio 5. Modelar mediante un DTE el ingreso del personal a una empresa.

Para ello existe una máquina en donde un empleado debe registrar el presente. Para iniciar el registro se selecciona la opción “Registrar Asistencia”. Luego, se habilitan dos opciones posibles para registrar su presente: mediante su tarjeta o su huella dactilar.

Si el empleado selecciona “registro por tarjeta”, debe pasar la tarjeta por un lector. Si la tarjeta es válida se habilita un teclado virtual donde debe proceder a ingresar un código de 4 dígitos, en el caso de que la tarjeta fuese inválida se informa el error. Para el ingreso de los 4 dígitos se tienen sólo 3 intentos, pasados los 3 intentos se anula la operación y se retorna la tarjeta.

Si opta por registrar el presente mediante la huella dactilar sólo debe apoyar el dedo en el scanner.

En cualquiera de los 2 casos si el ingreso es exitoso se muestra en el display la fecha y el horario de entrada y un mensaje de éxito, caso contrario, se visualiza un mensaje de error y se emite un pitido.


## Ejercicio 6. Se desea modelar el funcionamiento de un personaje para un juego electrónico.

El personaje es un guardia medieval de un castillo. Su objetivo es vigilar el castillo y eliminar enemigos que puedan aparecer.

El personaje comienza su ronda de vigilancia cuando es creado por el sistema, con el 100% de energía. El modo normal del personaje es vigilar el castillo, mientras no detecte un enemigo. Al detectar uno, el personaje pasa a modo combate. Si el enemigo está fuera del castillo, el personaje saca su arco y flecha. Si el enemigo está dentro del castillo, el personaje saca su espada. Durante el combate, el personaje puede recibir “golpes”, reduciendo su energía 10% por cada uno. Si el personaje gana el combate, recupera el 50% de energía y vuelve con su ronda de vigilancia. Pero si pierde energía hasta quedarse con el 20%, entonces el personaje comienza a huir del enemigo, guardando su arma. Durante la huida el personaje puede seguir recibiendo “golpes”, hasta quedarse sin energía y morir, quedando fuera del juego. Cuando pierde de vista al enemigo, el personaje deja de huir y vuelve con su ronda de vigilancia, ganando un 30% de energía.

## Ejercicio 7. Modelar mediante un DTE el sistema de voto electrónico para la facultad de informática.

El sistema cuenta con 2 terminales: la mesa de autoridades y la urna electrónica.

Cuando un alumno se presenta a votar, le entrega la documentación a la autoridad de la mesa y el encargado del manejo del sistema selecciona la opción ‘Nuevo Votante’. No todos los alumnos tienen su huella dactilar registrada por lo que el sistema presenta 2 opciones: identificación por huella e identificación por número de alumno.

En el caso de que se seleccione la opción identificación por huella se procede a la lectura de la huella del alumno. Si la huella no es identificada por el sistema se cancela la operación. Si la huella es detectada correctamente y el alumno no votó se habilita la urna electrónica que es donde el alumno emite su voto.

En el caso de que se seleccione identificación por número de alumno, el sistema solicita que se ingrese el legajo y luego se continúa con el mismo procedimiento de emisión de voto. Si el legajo no es reconocido por el sistema es informado y se cancela la operación. Para ambos casos, una vez identificado el alumno, si el mismo ya emitió su voto el sistema muestra un mensaje y cancela la operación.

Una vez iniciada la votación, se habilita la pantalla y se muestran las opciones para elegir el tipo de votación: “boleta completa” o “cortar boleta”. Si pasan 30 segundos y el votante no ha decidido su tipo de votación, la maquina emitirá un cartel de alerta donde indica que debe realizar la elección correspondiente, el cartel se mantendrá en pantalla hasta que el votante decida su tipo de votación.

Una vez elegido el tipo de votación, se pasará a elegir la agrupación a votar, para ello la máquina oculta las opciones anteriores y muestra un listado de los partidos disponibles. Si se eligió cortar boleta, el votante deberá elegir dos agrupaciones, caso contrario, elige solo una agrupación.

Una vez emitido el voto, es decir, que seleccionó la/s agrupación/es correspondiente/s, se oculta el listado, se muestra en toda la pantalla la opción/es elegida/s, se muestra un botón para confirmar y se muestra otro
botón para cancelar. Si confirma el voto, el mismo se envía a imprimir, se muestra un mensaje éxito, envía un mensaje a la mesa de autoridades y finaliza la sesión. Si cancela se muestra un mensaje de cancelación y finaliza la sesión