<div align="center">

[![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/Nomadiix/IS1)
[![GitHub stars](https://img.shields.io/github/stars/Nomadiix/IS1)](https://github.com/FabianMartinez1234567/IS1/stargazers/)
[![GitHub repo size in bytes](https://img.shields.io/github/repo-size/Nomadiix/IS1)](https://github.com/Nomadiix/IS1)
</div>

<h1 align="center"> 🖥️ Ingenieria de Software 1</h1>
<div align="center">
<img src="https://media.giphy.com/media/3ohze1y2AJUOHiid8I/giphy.gif"/>
</div>

<img src= 'https://i.gifer.com/origin/8c/8cd3f1898255c045143e1da97fbabf10_w200.gif' height="20" width="100%">

- [📖 Resumen Teorico 1ra AE](/Documentos/Teoria/Teoria.md)
- [📖 Resumen Teorico 2da AE](/Documentos/Teoria/Teoria2.md)
- [📋 Practica 1 Full Teoria](/Documentos/Practica1.md)
- [👤 Practica 2 Historias de Usuario](/Documentos/Practica2.md)
- [👥 Practica 3 Casos de Uso](/Documentos/Practica3.md)
- [📊 Practica 4 Diagramas de Transición de Estado](/Documentos/Practica4.md)
- [🕸️ Practica 5 Redes de Petri](/Documentos/Practica5.md)
- [📋 Practica 6 Tablas de Desición](/Documentos/Practica6.md)

<img src= 'https://i.gifer.com/origin/8c/8cd3f1898255c045143e1da97fbabf10_w200.gif' height="20" width="100%">

## Parciales

### Primera Fecha
![primera Fecha](https://github.com/Fabian-Martinez-Rincon/Fabian-Martinez-Rincon/assets/55964635/6c0c0493-3d85-492f-89e6-c59e37372872)



---

### Segunda Fecha
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
- `Titulo` Como usuario quiero solicitar un turno para 
- `Reglas de negocio`

`Criterios de aceptación` : 
- `Escenario 1` 
  - `Dado` 
  - `Cuando` 
  - `Entonces` 
---

### Iniciar Sesión
- `ID` Iniciar Sesión
- `Titulo` Como persona quiero iniciar sesión para poder solicitar turnos
- `Reglas de negocio`
  - Tiene 3 intentos antes de ser bloqueada

#### `Criterios de aceptación` : Iniciar Sesión

`Escenario 1` Inicio exitoso
- `Dado` dado que el mail juan@gmail.com esta registrado, esta en el intento 1, y la contraseña 123456 es correcta
- `Cuando` el usuario ingresa juan@gmail.com, 123456
- `Entonces` El sistema inicia la sesión y habilita la solicitud de turnos

`Escenario 2` Inicio fallido mail no registrado
- `Dado` dado que el mail martin@gmail.com no esta registrado
- `Cuando` el usuario ingresa martin@gmail.com
- `Entonces` El sistema informa que el usuario no se encuentra registrado

`Escenario 3` Inicio fallido por contraseña incorrecta
- `Dado` dado que el mail carlos@gmail.com esta registrado, esta en el intento 1, y la contraseña 7777777 es incorrecta
- `Cuando` el usuario ingresa carlos@gmail.com, 7777777
- `Entonces` el sistema incrementa en un intento e informa que la contraseña es incorrecta

`Escenario 4` Inicio fallido por contraseña incorrecta
- `Dado` dado que el mail pedro@gmail.com esta registrado, esta en el intento 3, y la contraseña 666666 es incorrecta
- `Cuando` el usuario ingresa pedro@gmail.com, 666666
- `Entonces` el sistema bloquea la cuenta

`Escenario 5` Inicio fallido por cuenta bloqueada
- `Dado` dado que el mail manolo@gmail.com esta registrado y tiene la cuenta bloqueada
- `Cuando` el usuario ingresa manolo@gmail.com
- `Entonces` el sistema informa que la cuenta fue bloqueada

---

### Cerrar Sesión
- `ID` Cerrar Sesión
- `Titulo`
- `Reglas de negocio`

---

### Tercera Fecha
![tercera Fecha](https://github.com/Fabian-Martinez-Rincon/Fabian-Martinez-Rincon/assets/55964635/13dd77c6-cece-4afc-bdc5-2d159e461742)

