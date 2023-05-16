# Parciales

## Primera Fecha
![primera Fecha](https://github.com/Fabian-Martinez-Rincon/Fabian-Martinez-Rincon/assets/55964635/6c0c0493-3d85-492f-89e6-c59e37372872)

![Parcial Colores](https://github.com/Fabian-Martinez-Rincon/IS1/assets/55964635/8e1ee15d-40ee-4e31-9592-3418bf4009a9)


### Roles
- Persona (Usuario no registrado)
- Visitante
- Usuario

### Casos de Uso

- `Nombre` Registro primer paso
- `Descripción` Este cu describe como una persona realiza el primer paso en su registro
- `Actores` Persona
- `Precondición` -
- `Curso Normal`

<table> <tr><td>Acciones del actor</td> <td>Acciones del Sistema</td></tr>
<td width="320">  

Paso 1: La persona selecciona la opción "Registro Primer Paso"

Paso 3: La persona ingresa datos solicitados 

</td><td width="320">

Paso 2: El sistema solicita nombre, apellido, dni, correo electronico y contraseña

Paso 4: El sistema verifica que el correo no este registrado

Paso 5: El sistema valida que la contraseña tenga al menos 6 caracteres

Paso 6: El sistema da de alta al usuario de forma parcial, genera un codigo de 16 digitos y lo envia al correo

</td></table>

---

## Segunda Fecha
  ![2](https://github.com/Fabian-Martinez-Rincon/Fabian-Martinez-Rincon/assets/55964635/a3c06772-cd17-4beb-8f19-b4d44f2df60a)


![Parcial 1Colores](https://github.com/Fabian-Martinez-Rincon/Fabian-Martinez-Rincon/assets/55964635/b61a35eb-39c5-448d-b06c-08434e5dfd08)


### Actores

- Persona(Usuario no registrado)
- Usuario

### Historias de Usuario
- Registrar persona
- Solicitar Turno
- Iniciar Sesión
- Cerrar Sesión

---

### Regitrar persona

- `ID` Registrar Persona
- `Titulo` Como persona quiero registrarme para poder solicitar turnos
- `Reglas de negocio`
  - Mail no registrado
  - Solo personas mayores de edad (18 años)

`Criterios de aceptación` : Registrar Persona
- `Escenario 1` Registro exitoso
  - `Dado` que el mail juan@gmail.com no esta registrada y tiene edad 20 años que es mayor de edad
  - `Cuando` la persona ingresa Juan, Carosella, juan@gmail.com, 20 años, 1 y 60.
  - `Entonces` El sistema registra al nuevo usuario, genera una contraseña y la manda al mail ingresado
- `Escenario 2` Registro fallido por mail ya registrado
  - `Dado` que el mail martin@gmail.com esta registrada y tiene edad 20 años que es mayor de edad
  - `Cuando` la persona ingresa Martin, Suarez, martin@gmail.com, 20 años, 1 y 44.
  - `Entonces` El sistema informa que la persona ya se encuentra registrada
- `Escenario 3` Registro fallido por ser menor de edad
  - `Dado` que el mail messi@gmail.com no esta registrada y tiene edad 10 años que es menor de edad
  - `Cuando` la persona ingresa Messi, Messi, messi@gmail.com, 10 años, 10 y 60.
  - `Entonces` El sistema informa que la persona es menor de edad

---

### Solicitar Turno

- `ID` Solicitar Turno
- `Titulo` Como usuario loguead quiero solicitar un turno para 
- `Reglas de negocio`
  - La cancha debe estar disponible
  - La fecha con dos dias de anticipación

`Criterios de aceptación`: 
- `Escenario 1` Solicitud exitosa
  - `Dado` que la cancha Roja esta disponible y la fecha 1/1/2024 se hizo con dos dias de anticipación
  - `Cuando` el usuario ingresa Roja, 1/1/2024, 14:00
  - `Entonces` El sistema asigna un turno al usuario e informa "Su turno ha sido registrado con exito"
- `Escenario 2` Solicitud fallida por cancha no disponible
  - `Dado` que la cancha Azul no esta disponible y la fecha 3/3/2025 se hizo con dos dias de anticipación
  - `Cuando` el usuario ingresa Azul, 3/3/2025, 11:00
  - `Entonces` El sistema asigna un turno al usuario e informa "Su turno ha sido registrado con exito"
- `Escenario 3` Solicitud fallida por fecha no reservada con dos dias de anticipación
  - `Dado` que la cancha Verde esta disponible y la fecha 1/12/2023 se hizo con un dia de anticipación
  - `Cuando` el usuario ingresa Verde, 1/12/2023, 19:00
  - `Entonces` El sistema informa que el turno debe solicitarse con dos dias de anticipación


---

### Iniciar Sesión
- `ID` Iniciar Sesión
- `Titulo` Como persona quiero iniciar sesión para poder solicitar turnos
- `Reglas de negocio`
  - Tiene 3 intentos antes de ser bloqueada

`Criterios de aceptación` : Iniciar Sesión

- `Escenario 1` Inicio exitoso
  - `Dado` dado que el mail juan@gmail.com esta registrado, esta en el intento 1, y la contraseña 123456 es correcta
  - `Cuando` el usuario ingresa juan@gmail.com, 123456
  - `Entonces` El sistema inicia la sesión y habilita la solicitud de turnos
- `Escenario 2` Inicio fallido mail no registrado
  - `Dado` dado que el mail martin@gmail.com no esta registrado
  - `Cuando` el usuario ingresa martin@gmail.com
  - `Entonces` El sistema informa que el usuario no se encuentra registrado
- `Escenario 3` Inicio fallido por contraseña incorrecta
  - `Dado` dado que el mail carlos@gmail.com esta registrado, esta en el intento 1, y la contraseña 7777777 es incorrecta
  - `Cuando` el usuario ingresa carlos@gmail.com, 7777777
  - `Entonces` el sistema incrementa en un intento e informa que la contraseña es incorrecta
- `Escenario 4` Inicio fallido por contraseña incorrecta
  - `Dado` dado que el mail pedro@gmail.com esta registrado, esta en el intento 3, y la contraseña 666666 es incorrecta
  - `Cuando` el usuario ingresa pedro@gmail.com, 666666
  - `Entonces` el sistema bloquea la cuenta e informa que la contraseña es incorrecta
- `Escenario 5` Inicio fallido por cuenta bloqueada
  - `Dado` dado que el mail manolo@gmail.com esta registrado y tiene la cuenta bloqueada
  - `Cuando` el usuario ingresa manolo@gmail.com
  - `Entonces` el sistema informa que la cuenta fue bloqueada

---

### Cerrar Sesión
- `ID` Cerrar Sesión
- `Titulo` Como usuario logueado quiero iniciar sesión para poder guardar mis datos
- `Reglas de negocio`

`Criterios de aceptación`: Cerrar Sesión
- `Escenario 1` Cierre exitoso
  - `Dado` que el usuario felix@gmail.com tiene una sesión abierta
  - `Cuando` el usuario presiona el boton "cerrar sesión"
  - `Entonces` El sistema cierra la sesión y bloquea las opciones para solicitar turnos

---

### Tercera Fecha
![tercera Fecha](https://github.com/Fabian-Martinez-Rincon/Fabian-Martinez-Rincon/assets/55964635/13dd77c6-cece-4afc-bdc5-2d159e461742)

