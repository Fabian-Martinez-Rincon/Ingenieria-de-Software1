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

## Primera Fecha

<img src="https://github.com/Fabian-Martinez-Rincon/Fabian-Martinez-Rincon/assets/55964635/e584be28-12fb-4f8f-9811-a3bc7cb31559" alt="Parcial1">

## Listar Noticias

**ID:** Listar Noticias

**TÍTULO:** Usuario o persona quiero ver las noticias para estar informado

**REGLAS DE NEGOCIO:** 
- El token es valido

**CRITERIOS DE ACEPTACIÓN:** 

#### **Escenario 1:** Listado exitoso

`Dado` que se establecio conexión con el servidor, el token en valido y hay noticias para mostrar

`Cuandod` el usuario o la persona le dan al boton "listar noticias"

`Entonces` el sistema informa el listado de noticias en pantalla

#### **Escenario 2:** Listado fallido por fallas en la conexión

`Dado` que no se establecio conexión con el servidor

`Cuandod` el usuario o la persona quiere "listar noticias"

`Entonces` el sistema informa que no se pudo establecer la conexión

#### **Escenario 3:** Listado fallido por token invalido

`Dado` que se establecio conexión con el servidor, el token en invalido

`Cuandod` el usuario o la persona le dan al boton "listar noticias"

`Entonces` el sistema informa que el token es invalido


#### **Escenario 4:** Listado fallido por falta de noticias

`Dado` que se establecio conexión con el servidor, el token en valido y no hay noticias para mostrar

`Cuandod` el usuario o la persona le dan al boton "listar noticias"

`Entonces` el sistema informa que no hay noticias para listar

---

## Acceder detalle

**ID:** Acceder detalle

**TÍTULO:** Como usuario logueado quiero acceder al detalle de una noticias para estar informado

**REGLAS DE NEGOCIO:**
- Solo se permite el acceso a 5 noticias por dia

**CRITERIOS DE ACEPTACIÓN:** 

#### **Escenario 1:** Listado exitoso

`Dado` que el usuario fabo@gmail.com tiene 0 accesos a detalles que es menor al 5 a los 5 permitidos

`Cuandod` el usuario preciona el boton "ver detalles"

`Entonces` el sistema muestra el detalle de la noticia y aumenta en 1 los detalles visos

#### **Escenario 2:** Acceso fallido

`Dado` que el usuario fabo@gmail.com tiene 5 accesos a detalles que es igual al 5 a los 5 permitidos

`Cuandod` el usuario preciona el boton "ver detalles"

`Entonces` el sistema informa que que ya no puede ver los detalles de las noticias por el resto del dia


## Iniciar Sesión

**ID:** Iniciar Sesión

**TÍTULO:** Como usuario quiero iniciar sesión para poder acceder a los detalles

**REGLAS DE NEGOCIO:**
- Tiene 3 intentos de autentificación antes de ser bloqueado

**CRITERIOS DE ACEPTACIÓN:** 

#### **Escenario 1:** Inicio exitoso

`Dado` que el usuario fabo@gmail.com esta registrado, no esta bloqueado, esta en el intento 1, y la contraseña pepe30 es correcta

`Cuandod` el usuario ingresa fabo@gmail.com, pepe30

`Entonces` el sistema inicia la sesión del usuario y habilita las opciones para el acceso a los detalles

#### **Escenario 2:** Inicio fallido por usuario no registrado

`Dado` que el usuario leo@gmail.com no esta registrado

`Cuandod` el usuario ingresa leo@gmail.com, mundial10

`Entonces` el sistema informa que el usuario no se encuentra registrado

#### **Escenario 3:** Inicio fallido por usuario bloqueado

`Dado` que el usuario hitler@gmail.com esta registrado y esta bloqueado

`Cuandod` el usuario ingresa hitler@gmail.com, horno666

`Entonces` el sistema informa que el usuario se encuentra bloqueado

#### **Escenario 4:** Inicio fallido por contraseña incorrecta

`Dado` que el usuario maradona@gmail.com esta registrado, no esta bloqueado, esta en el intento 1, y la contraseña mundial86 es incorrecta

`Cuandod` el usuario ingresa maradona@gmail.com, mundial86

`Entonces` el sistema informa que la contraseña es incorrecta y aumenta en 1 los intentos

#### **Escenario 5:** Inicio fallido por contraseña incorrecta

`Dado` que el usuario diego@gmail.com esta registrado, no esta bloqueado, esta en el intento 3, y la contraseña rosa10 es incorrecta

`Cuandod` el usuario ingresa fabo@gmail.com, rosa10

`Entonces` el sistema informa que la contraseña es incorrecta y bloquea la cuenta

---

## Cerrar sesión

**ID:** Cerrar Sesión

**TÍTULO:** Como usuario con una sesión abierta cerrar mi sesión para proteger mis datos

**REGLAS DE NEGOCIO:**

**CRITERIOS DE ACEPTACIÓN:** 

#### **Escenario 1:** Cierre exitoso

`Dado` que el usuario tiene una sesión abierta

`Cuandod` el usuario presiona el boton "cerrar sesión"

`Entonces` el sistema cierra la sesión y deshabilita las opciones para el acceso a las noticias

---

## Registrar Persona

**ID:** Registrar Persona

**TÍTULO:** Como usuario quiero registrarme para poder acceder a los detalles

**REGLAS DE NEGOCIO:**
- Mail no registrado
- Solo personas mayores de edad (18 años)

**CRITERIOS DE ACEPTACIÓN:** 

#### **Escenario 1:** Registra exitoso

`Dado` que el usuario fabian@gmail.com no esta registrado, tiene 20 años que es mayor de edad

`Cuandod` la persona ingresa Fabian, Martinez, 20 años, fabian@gmail.com

`Entonces` el sistema registra al usuario y manda una contraseña aleatoria al mail

#### **Escenario 2:** Registro fallido mail ya registrado

`Dado` que el usuario lucas@gmail.com esta registrado, tiene 22 años que es mayor de edad

`Cuandod` la persona ingresa Lucas, Benitez, 22 años, lucas@gmail.com

`Entonces` el sistema informa que el mail ya se encuentra registrado

#### **Escenario 3:** Registro fallido por ser menor de edad 

`Dado` que el usuario julian@gmail.com no esta registrado, tiene 10 años que es menor de edad

`Cuandod` la persona ingresa Julian, Lopez, 10 años, julian@gmail.com

`Entonces` el sistema informa que la persona es menor de edad



