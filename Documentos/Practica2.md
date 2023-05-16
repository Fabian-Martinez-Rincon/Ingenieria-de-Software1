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

---

## Nombre
**ID:** 

**TÍTULO:** 

**REGLAS DE NEGOCIO:** 

**CRITERIOS DE ACEPTACIÓN:** 

#### **Escenario 1:** título del criterio.
`Dado`

`Cuando` 

`Entonces` 



<img src= 'https://i.gifer.com/origin/8c/8cd3f1898255c045143e1da97fbabf10_w200.gif' height="20" width="100%">


**Para cada problema planteado realice las tarjetas completas de todas las historias de usuario identificadas**

<img src= 'https://i.gifer.com/origin/8c/8cd3f1898255c045143e1da97fbabf10_w200.gif' height="20" width="100%">

<div align = center>

## `Problema 1` Alquiler de mobiliario

</div>

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

## Reservar Alquiler

**ID:** Reservar Alquiler
 
**TÍTULO:** Como usuario quiero hacer una reserva de alquiler para poder vivir un tiempo

**REGLAS DE NEGOCIO:** Reservar Alquiler
- Incluye minimo 3 muebles
- Se abona el 20% del total con tarjeta de credito

**CRITERIOS DE ACEPTACIÓN:** 

#### **Escenario 1:** Reservar Exitosa

`Dado` que el alquiler tiene 3 muebles y se pago el 20% con una tarjeta de credito valida

`Cuando` el usuario ingresa 10-10-2010, La Plata, 3 dias, 3 muebles y los datos de una tarjeta de credito valida

`Entonces` el sistema emite un numero de reserva unico.

#### **Escenario 2:** Reservar Fallida por muebles insuficientes

`Dado` que el alquiler tiene 1 mueble y se pago el 20% con una tarjeta de credito valida

`Cuando` el usuario ingresa 05-05-2020, La Plata, 11 dias, 1 muebles y los datos de una tarjeta de credito valida

`Entonces` el sistema informa que el inmueble no cumple con los requisitos minimos

#### **Escenario 3:** Reserva Fallida por problemas con la tarjeta de credito

`Dado` que el alquiler tiene 5 muebles y se pago el 20% con una tarjeta invalida

`Cuando` el usuario ingresa 20-03-2015, Buenos Aires, 30 dias, 5 muebles y los datos de una tarjeta de credito invalida

`Entonces` el sistema informa que la tarjeta es invalida y no registra el pago

---

## Dar Alta Inmueble

**ID:** Dar alta inmueble
 
**TÍTULO:** Como encargado de departamento quiero dar alta un inmueble para que pueda ser alquilado

**REGLAS DE NEGOCIO:** 
- Codigo no registrado
- Se cargo en dolares

**CRITERIOS DE ACEPTACIÓN:** Dar alta inmueble

#### **Escenario 1:** Alta Exitosa

`Dado` que el codigo 0202 no esta registrado y el precio 10$ se cargo en dolares

`Cuando` el empleado de mesa ingresa 0202, Mesa, 1-1-2000, 20-20-2020, libre, 10$

`Entonces` el sistema registra el mueble en el sistema

#### **Escenario 2:** Alta Fallida por codigo ya existente

`Dado` que el codigo 1010 esta registrado y el precio 20$ se cargo en dolares

`Cuando` el empleado de mesa ingresa 1010, Ropero, 3-3-2003, 04-04-2004, de baja, 20$

`Entonces` el sistema informa que el codigo ya se encuentra registrado y no realiza el alta

#### **Escenario 3:** Alta Fallida por precio cargado en euros

`Dado` que el codigo 4040 no esta registrado y el precio 10$ se cargo en euros

`Cuando` el empleado de mesa ingresa 4040, Cama, 2-2-2002, 21-21-2021, alquilado, 30$

`Entonces` el sistema informa que el precio debe cargarse en dolares y no realiza el alta

---

## Pagar con tarjeta

**ID:** Pagar con tarjeta
 
**TÍTULO:** Como usuario quiero pagar con tarjeta para pode reservar un alquiler

**REGLAS DE NEGOCIO:** 

**CRITERIOS DE ACEPTACIÓN:** Pagar con tarjeta

#### **Escenario 1:** Pago exitoso

`Dado` que se pudo establecer conexión con el servidor del banco, el nro 123 de la tarjeta es valido y posee fondos suficientes

`Cuando` el cliente ingresa 123.

`Entonces` el sistema registra el pago

#### **Escenario 2:** Pago Fallido por falla con la conexión del banco

`Dado` que no se pudo establecer conexión con el banco

`Cuando` el cliente quiere pagar

`Entonces` el sistema informa que no se pudo establecer conexion con el banco

#### **Escenario 3:** Pago fallido por numero de tarjeta invalido

`Dado` que se pudo establecer conexión con el servidor del banco, el nro 777 de la tarjeta es invalido

`Cuando` el cliente ingresa 777.

`Entonces` el sistema informa que el nro de la tarjeta es invalido y no registra el pago

#### **Escenario 4:** Pago fallido por saldo insuficiente

`Dado` que se pudo establecer conexión con el servidor del banco, el nro 1010 de la terjeta es valido y no tiene fondos

`Cuando` el cliente ingresa 1010

`Entonces` el sistema informa que la tarjeta no tiene fondos suficientes y no registra el cobro



<img src= 'https://i.gifer.com/origin/8c/8cd3f1898255c045143e1da97fbabf10_w200.gif' height="20" width="100%">

<div align = center>

## `Problema 2` Posgrado

</div>



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

## Inscribir a carrera


**ID:** Inscribir a carrera
 
**TÍTULO:** Como usuario quiero inscribirme a una carrera para poder estudiar

**REGLAS DE NEGOCIO:** Inscribir a carrera
- Pago con tarjeta de credito

**CRITERIOS DE ACEPTACIÓN:** Inscribir a carrera

#### **Escenario 1:** Inscripción exitosa

`Dado` que las 10 cuotas no superan el maximo permitido y posee una tarjeta de credito valida

`Cuando` el usuario selecciona la carrera Filosofia, 10 y los datos de una tarjeta de credito valida

`Entonces` El sistema registra la inscripción del usuario e imprime dos comprobantes, uno de inscripcion y otro de pago

#### **Escenario 2:** Inscripción fallida por cuotas que superan el maximo

`Dado` que las 100 cuotas superan el maximo permitido y posee una tarjeta de credito valida

`Cuando` el usuario selecciona la carrera Ingenieria, 100 y los datos de una tarjeta de credito valida

`Entonces` El sistema informa que la cantidad de cuotas ingresadas es invalida

#### **Escenario 3:** Inscripción por problemas con la tarjeta

`Dado` que las 4 cuotas no superan el maximo permitido y posee una tarjeta de credito invalida

`Cuando` el usuario selecciona la carrera Aeronautica, 4 y los datos de una tarjeta de credito invalida

`Entonces` El sistema informa que hay problemas con el pago

---

## Alta carrera

**ID:** Alta carrera
 
**TÍTULO:** Como empleado administrativo quiero dar de alta la carrera para que los usuarios puedas inscribirse en ella

**REGLAS DE NEGOCIO:** 
- Nombre de la carrera no registrado
- La duración debe ser de no mas de 5 años

**CRITERIOS DE ACEPTACIÓN:** Alta carrera

#### **Escenario 1:** Alta de carrera exitosa.

`Dado` que el nombre Informatica no esta registrado, y la carrera dura 4 años que es menor de 5 años

`Cuando` el empleado administrativo ingresa Informatica, 4 años, 100$, 20 cuotas

`Entonces` El sistema da de alta la carrera

#### **Escenario 2:** Alta de carrera fallida por nombre ya registrado

`Dado` que el nombre Fisica esta registrado, y la carrera dura 3 años que es menor de 5 años

`Cuando` el empleado administrativo ingresa Fisica, 3 años, 1000$, 10 cuotas

`Entonces` El sistema informa que el nombre de la carrera ya se encuentra registrado

#### **Escenario 3:** Alta de carrera fallida por duración mayor a 5 años

`Dado` que el nombre Abogacia no esta registrado, y la carrera dura 40 años que es mayor de 5 años

`Cuando` el empleado administrativo ingresa Abogacia, 40 años, 1$, 2 cuotas

`Entonces` El sistema informa que la duración ingresada supera los 5 años

---

## Registrar Usuario

**ID:** Registrar Alumno
 
**TÍTULO:** Como alumno quiero registrarme para anotarme a una carrera

**REGLAS DE NEGOCIO:** 
- Nombre de usuario no registrado
- Contaseña con mas de 6 digitos 


**CRITERIOS DE ACEPTACIÓN:** 

#### **Escenario 1:** Registro exitoso

`Dado` que el usuario fabo no esta registrado y la contraseña kapo013 tiene mas de 6 digitos

`Cuando` el alumno ingresa Fabian, Martinez ,fabo, kapo013

`Entonces` el sistema registra al nuevo usuario

#### **Escenario 2:** Registro fallido por usuario ya existente

`Dado` que el usuario tomo esta registrado y la contraseña pepe555 tiene mas de 6 digitos

`Cuando` el alumno ingresa Tomas, Gomez, tomo, pepe555

`Entonces` el sistema Informa que el usuario ingresado ya existe

#### **Escenario 3:** Registro fallido por contraseña con menos de 6 digitos

`Dado` que el usuario messi no esta registrado y la contraseña 2023 tiene menos de 6 digitos

`Cuando` el alumno ingresa Lionel, Messi, messi, 2023

`Entonces` el sistema informa que la contraseña ingresada tiene menos de 6 digitos

---

## Iniciar Sesión

**ID:** Iniciar Sesión
 
**TÍTULO:** Como usuario quiero iniciar sesión para poder anotarme en alguna carrera

**REGLAS DE NEGOCIO:** 

**CRITERIOS DE ACEPTACIÓN:** Iniciar Sesión

#### **Escenario 1:** Inicio exitoso

`Dado` que el usuario fabo se encuentra registrado y la contraseña kapo013 es correcta

`Cuando` el usuario ingresa fabo, kapo013

`Entonces` el sistema realiza el inicio de sesión y habilita la inscripción a algunas carreras

#### **Escenario 2:** Inicio fallido por usuario no registrado

`Dado` que el usuario maradona no se encuentra registrado

`Cuando` el usuario ingresa maradona, cocacola21

`Entonces` el sistema informa que el usuario no se encuentra registrado y no realiza el inicio de sesión

#### **Escenario 3:** Inicio fallido por contraseña incorrecta

`Dado` que el usuario stalin se encuentra registrado y la contraseña presi19 es incorrecta

`Cuando` el usuario ingresa stalin, presi19

`Entonces` el sistema informa que la contraseña es incorrecta


---

## Cerrar Sesión

**ID:** Cerrar Sesión
 
**TÍTULO:** 

**REGLAS DE NEGOCIO:** 

**CRITERIOS DE ACEPTACIÓN:** Cerrar Sesión

#### **Escenario 3:** Cierre exitoso

`Dado` que el usuario tiene una sesión abierta

`Cuando` el usuario presiona el boton de cerrar sesión

`Entonces` el sistema cierra la sesión y deshabilita la inscripción a las carreras 


<img src= 'https://i.gifer.com/origin/8c/8cd3f1898255c045143e1da97fbabf10_w200.gif' height="20" width="100%">

<div align = center>

## `Problema 3` Contratos

</div>

![image](https://user-images.githubusercontent.com/55964635/232234621-77ecdb9f-55f2-4dab-8055-571bbdf9f69f.png)

---

### Roles
- Empleado de mesa de entrada
- Empleado de rendiciones

### Historias de Usuario
- Confeccionar minuta
- Aprobar minuta
- Imprimir Listado

---

## Confeccionar minuta

**ID:** Confeccionar minuta
 
**TÍTULO:** Como empleado de mesa quiero confeccionar una minuta para que pueda ser aprobada

**REGLAS DE NEGOCIO:**
- El monto no puede superar los $25000
- Duración maxima de 6 meses


**CRITERIOS DE ACEPTACIÓN:** 

#### **Escenario 1:** Confección exitosa

`Dado` que el monto $1000 no supera los $25000 y la duración de 3 meses no supera el maximo de 6 meses

`Cuando` el empleado de mesa ingresa Fabian, 777, temporal, 01-01-2001, 3 meses, $1000

`Entonces` el sistema confecciona la minuta y le asocia un numero automaticamente

#### **Escenario 2:** Confección fallida por monto superior a $25000

`Dado` que el monto $50000 supera los $25000 y duración 1 mes no supera el maximo de 6 meses

`Cuando` el empleado de mesa ingresa Tomas, 666, fijo, 10-10-2010, 1 mes, $50000

`Entonces` el sistema informa que el monto ingresado supera los $25000

#### **Escenario 3:** Confección fallida porque la duración excede los 6 meses 

`Dado` que el monto $500 no supera los $25000 y duración 10 meses supera el maximo de 6 meses

`Cuando` el empleado de mesa ingresa Franco, 1010, temporal, 11-11-2011, 10 meses, $500

`Entonces` el sistema informa que el la duración ingresada supera los 6 meses

---

## Aprobar minuta

**ID:** Aprobar minuta
 
**TÍTULO:** Como empleado de rendiciones quiero aprobar la minuta par poder hacer un contrato en un futuro

**REGLAS DE NEGOCIO:** 

- No se aprueba si tiene 3 contratos vigentes
- Cuit habilitado por el AFIP (esta habilitado si el servidor responde ante el token)

**CRITERIOS DE ACEPTACIÓN:** 

#### **Escenario 1:** Aprobación de minuta exitosa

`Dado` que la minuta 123 tiene 2 contratos vigentes que es menor a 3 contratos, se establecio conexión con el servidor y el cuit esta habilitado por el AFIP

`Cuando` el empleado de rendiciones ingresa 123

`Entonces` el sistema aprueba la minuta

#### **Escenario 2:** Aprobación fallida por tener 3 contratos vigentes

`Dado` que la minuta 666 tiene 3 contratos vigentes que es igual a 3 contratos, se establecio conexión con el servidor y el cuit esta habilitado por el AFIP

`Cuando` el empleado de rendiciones ingresa 666

`Entonces` el sistema informa que el usuario ya tiene tres contratos vigentes

#### **Escenario 3:** Aprobación fallida por falta de conexión

`Dado` que la minuta 4949 tiene 1 contrato vigentes que es menor a 3 contratos, no se establecio conexión con el servidor

`Cuando` el empleado de rendiciones ingresa 4949

`Entonces` el sistema informa que no se pudo establecer conexión


#### **Escenario 4:** Aprobación fallida por CUIT inhabilitado por el AFIP

`Dado` que la minuta 3131 tiene 1 contrato vigentes que es menor a 3 contratos, se establecio conexión con el servidor y el cuit esta inhabilitado por el AFIP

`Cuando` el empleado de rendiciones ingresa 3131

`Entonces` el sistema informa que el cuit se encuentra inhabilitado por el AFIP

---

## Imprimir Listado

**ID:** Imprimir listado
 
**TÍTULO:** Como empleado de rendiciones quiero imprimir el listado para poder darselo al jefe de departamento 

**REGLAS DE NEGOCIO:** 

**CRITERIOS DE ACEPTACIÓN:** Imprimir listado

**Escenario 1:** Impresión exitosa

`Dado` que el litado tiene minutas para mostrar

`Cuando` el empleado de rendiciones le da al boton "imprimir minutas"

`Entonces` el sistema imprime el listado 

#### **Escenario 2:** Impresión fallida por lista vacia

`Dado` que el listado no tiene minutas para mostrar

`Cuando` el empleado de rendiciones le da al boton "imprimir minutas"

`Entonces` el sistema informa que el listado se encuentra vacio

<img src= 'https://i.gifer.com/origin/8c/8cd3f1898255c045143e1da97fbabf10_w200.gif' height="20" width="100%">

<div align = center>

## `Problema 4` Venta de bebidas

</div>

![image](https://user-images.githubusercontent.com/55964635/232245201-80c3a9e9-1f85-4f5c-b3fb-02f6b06a0f46.png)
![image](https://user-images.githubusercontent.com/55964635/232245230-8f12ad19-a8dd-4c31-a99f-2de5db4ce65d.png)

---

### Roles
- Persona (no registrada)
- Usuario

### Historias de Usuario
- Registrar Persona
- Iniciar sesión
- Cerrar sesión
- Comprar Bebidas

---

## Registra Persona

**ID:** Registra Persona
 
**TÍTULO:** Como persona quiero registrarme para comprar bebidas

**REGLAS DE NEGOCIO:** 
- Mail no registrado
- Solo personas mayores de 18 años


**CRITERIOS DE ACEPTACIÓN:** 

#### **Escenario 1:** Registro exitoso

`Dado` que el mail menem@gmail.com no esta registrado y la persona tiene 90 años que es mayor de 18 años

`Cuando` la persona ingresa Calos, Menem, menem@gmail.com, 90 años

`Entonces` el sistema registra a la persona, genera una contraseña y la manda al mail ingresado

#### **Escenario 2:** Registro fallido por mail ya registrado

`Dado` que el mail pepe@gmail.com ya esta registrado y la persona tiene 30 años que es mayor de 18 años

`Cuando` la persona ingresa Pepe, ElSapo, pepe@gmail.com, 30 años

`Entonces` el sistema informa que el mail ya se encuentra registrado

#### **Escenario 3:** Registro fallido por persona menor de 18 años

`Dado` que el mail juansito@gmail.com no esta registrado y la persona tiene 10 años que es menor de 18 años

`Cuando` la persona ingresa Juan, Carosella, juansito@gmail.com, 10 años

`Entonces` el sistema muestra en pantalla la ley que impide la venta de bebidas alcoholicas a menores

---

## Iniciar sesión

**ID:** Iniciar Sesión
 
**TÍTULO:** Como usuario quiero iniciar sesión para poder comprar bebidas

**REGLAS DE NEGOCIO:** 

**CRITERIOS DE ACEPTACIÓN:** Iniciar Sesión

#### **Escenario 1:** Inicio exitoso

`Dado` que el usuario menem@gmail.com esta registrado y la contraseña xxxx es correcta

`Cuando` el usuario ingresa menem@gmail.com, xxxx

`Entonces` el sistema muestra un listado de bebidas

#### **Escenario 2:** Inicio fallido por mail no registrado

`Dado` que el usuario manolo@gmail.com no esta registrado

`Cuando` el usuario ingresa manolo@gmail.com

`Entonces` el sistema informa que el mail no se encuentra registrado

#### **Escenario 3:** Inicio fallido por contraseña incorrecta

`Dado` que el usuario diego@gmail.com esta registrado y la contraseña 20203 es incorrecta

`Cuando` el usuario ingresa diego@gmail.com, 20203

`Entonces` el sistema informa que la contraseña ingresada es incorrecta

---

## Cerrar sesión

**ID:** Cerrar Sesión
 
**TÍTULO:** Como usuario logueado quiero cerrar mi sesión para proteger mis datos

**REGLAS DE NEGOCIO:** 

**CRITERIOS DE ACEPTACIÓN:** 

**Escenario 1:** Cierre exitoso

`Dado` que el usuario tiene una sesión abierta

`Cuando` el usuario presiona el boton cerrar sesión

`Entonces` el sistema cierra la sesión y deshabilita las opciones de selección y compra de bebidas

---

## Comprar Bebidas 

**ID:** Comprar Bebidas
 
**TÍTULO:** Como usuario logueado quiero comprar bebidas para ir a una fiesta

**REGLAS DE NEGOCIO:** 
- Si es premium se le hace un descuento del 20%
- Si el monto es superior a $4500 se le hace un descuento del 10%

**CRITERIOS DE ACEPTACIÓN:** 

#### **Escenario 1:** Compra exitosa con 30% de decuento

`Dado` que el usuario messi@gmail.com es premium con 20% de descuento y su compra es de $50000 con 10% de descuento y hay stock de bebidas

`Cuando` el usuario selecciona las bebidas y le da al boton "comprar"

`Entonces` el sistema aplica un descuento del 30% sobre el total y registra la compra

#### **Escenario 2:** Compra exitosa con 20% de decuento

`Dado` que el usuario benzema@gmail.com es premium con 20% de descuento y su compra es de $50 sin 10% de descuento y hay stock de bebidas

`Cuando` el usuario selecciona las bebidas y le da al boton "comprar"

`Entonces` el sistema aplica un descuento del 20% sobre el total y registra la compra

#### **Escenario 3:** Compra exitosa con 10% de decuento

`Dado` que el usuario guardiola@gmail.com no es premium con 20% de descuento y su compra es de $20000 con 10% de descuento y hay stock de bebidas

`Cuando` el usuario selecciona las bebidas y le da al boton "comprar"

`Entonces` el sistema aplica un descuento del 10% sobre el total y registra la compra

#### **Escenario 4:** Compra exitosa sin descuentos

`Dado` que el usuario messi@gmail.com no es premium con 20% de descuento y su compra es de $2 sin 10% de descuento y hay stock de bebidas

`Cuando` el usuario selecciona las bebidas y le da al boton "comprar"

`Entonces` el sistema no aplica un descuento sobre el total y registra la compra

#### **Escenario 5:** Compra fallida por falta de stock

`Dado` que el usuario macalister@gmail.com es premium con 20% de descuento y su compra es de $50000 con 10% de descuento y no hay stock de bebidas

`Cuando` el usuario selecciona las bebidas y le da al boton "comprar"

`Entonces` el sistema informa que no hay stock de bebidas

<img src= 'https://i.gifer.com/origin/8c/8cd3f1898255c045143e1da97fbabf10_w200.gif' height="20" width="100%">

<div align = center>

#### `Problema 5` Casa de fotografía
</div>

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

## Registrar Persona

**ID:** Registrar Persona
 
**TÍTULO:** Como persona quiero registrame para poder subir fotos

**REGLAS DE NEGOCIO:** 
- nombre de usuario no registrado 

**CRITERIOS DE ACEPTACIÓN:** 

#### **Escenario 1:** Registro exitoso

`Dado` que el nombre de usuario manolo20 no esta registrado

`Cuando` la persona ingresa Manolo, Cuevas, manolo@gmail.com, 24 entre 51 y 50, manolo20, contraseña123

`Entonces` sistema realiza el registro del usuario y lo informa en pantalla

#### **Escenario 2:** Registro Fallido por usuario ya existente

`Dado` que el nombre de usuario vegeta666 esta registrado

`Cuando` la persona ingresa Vegeta, Sayan, vegeta@gmail.com, 1 entre 22 y 23, vegeta666, nameku1000

`Entonces` sistema informa que el usuario ya se encuentra registrado en el sistema

---

## Iniciar Sesión

**ID:** Iniciar Sesión
 
**TÍTULO:** Como usuario quiero iniciar sesión para poder comprar las fotos

**REGLAS DE NEGOCIO:** 

**CRITERIOS DE ACEPTACIÓN:** Iniciar Sesión

#### **Escenario 1:** Inicio Exitoso

`Dado` que el manolo20 se encuentra registrado y la contraseña contraseña123 es correcta

`Cuando` el usuario ingresa manolo20, contraseña123

`Entonces` el sistema realiza el inicio de sesión y habilita la opcion para subir imagenes y pagar

#### **Escenario 2:** Inicio Fallido por usuario no registrado

`Dado` que el goku50 no se encuentra registrado

`Cuando` el usuario ingresa goku50

`Entonces` el sistema informa que el usuario no se encuentra registrado

#### **Escenario 3:** Inicio Fallido por contraseña incorrecta

`Dado` que el manolo20 se encuentra registrado y la contraseña contraseña123 es in correcta

`Cuando` el usuario ingresa manolo20, contraseña123

`Entonces` el sistema informa que la contraseña es incorrecta

---

## Cerrar Sesión

**ID:** Cerrar Sesión
 
**TÍTULO:** Como usuario logueado quiero cerrar mi sesión para proteger mis datos

**REGLAS DE NEGOCIO:** 

**CRITERIOS DE ACEPTACIÓN:** 

#### **Escenario 1:** Cierre exitoso

`Dado` que el usuario tiene la sesión abierta

`Cuando` el usuario presiona el boton `cerrar sesión`

`Entonces` el sistema cierra la sesión y deshabilita las opciones para subir imagenes y pagar

---

## Pagar con tarjeta


**ID:** Pagar con tarjeta
 
**TÍTULO:** Como usuario quiero pagar con tarjeta para poder retirar las fotos

**REGLAS DE NEGOCIO:** 

**CRITERIOS DE ACEPTACIÓN:** 

#### **Escenario 1:** Pago exitoso

`Dado` que se pudo establecer conexión con el servidor, el nro de tarjeta 4342 es correcto y posee fondos suficientes 

`Cuando` el usuario ingresa 4342, 012, Fabian

`Entonces` el sistema registra el pago y retorna un nro para que pueda retirar las fotos

#### **Escenario 2:** Pago fallido por falta de conexión con el servidor

`Dado` que no se pudo establecer conexión con el servidor

`Cuando` el usuario intenta pagar

`Entonces` el sistema informa que no hay conexión con el banco

#### **Escenario 3:** Pago fallido por nro de tarjeta invalido

`Dado` que se pudo establecer conexión con el servidor, el nro de tarjeta 9578 no es correcto

`Cuando` el usuario ingresa 9578, 23, Jordan

`Entonces` el sistema informa que el nro de tarjeta es invalido

#### **Escenario 4:** Pago fallido por fondos insuficientes

`Dado` que se pudo establecer conexión con el servidor, el nro de tarjeta 8414 es correcto y no posee fondos suficientes 

`Cuando` el usuario ingresa 8414, 010, Messi

`Entonces` el sistema informa que la tarjeta no posee fondos suficientes

---

## Subir Foto


**ID:** Subir Foto
 
**TÍTULO:** Como usuario quiero subir foto para luego retirarla

**REGLAS DE NEGOCIO:** 
- Un maximo de 50 fotos
- Se suben de a una
- Se paga 15$ por foto con tarjeta de credito

**CRITERIOS DE ACEPTACIÓN:** 

#### **Escenario 1:** Subida exitosa

`Dado` que esta en la foto nro 20 que es menor al maximo de 50 y fueron una a la vez

`Cuando` el usuario sube perros.png

`Entonces` el sistema carga la foto 

#### **Escenario 2:** Subida fallida por cantidad excesiva de fotos

`Dado` que esta en la foto nro 50 que es igual al maximo de 50 y fueron una a la vez

`Cuando` el usuario sube gatos.png

`Entonces` el sistema informa que el usuario no puede subir mas de 50 imagenes 

#### **Escenario 3:** Subida fallida por subir mas de una foto a la vez

`Dado` que esta en la foto nro 20 que es menor al maximo de 50 y fueron dos a la vez

`Cuando` el usuario sube perros.png, gatos.png, ratas.png

`Entonces` el sistema informa que el usuario esta subiendo mas de una foto a la vez

---

## Retirar Foto

**ID:** Retirar Foto
 
**TÍTULO:** Como empleado quiero retirar las fotos para darselas al cliente

**REGLAS DE NEGOCIO:** 

**CRITERIOS DE ACEPTACIÓN:** 

#### **Escenario 1:** Retiro exitoso

`Dado` que el codigo 4321 esta cargado en el sistema

`Cuando` el empleado ingresa 4321

`Entonces` el sistema imprime las fotos 

#### **Escenario 2:** Retiro fallido por codigo inexistente

`Dado` que el codigo 6353 no esta cargado en el sistema

`Cuando` el empleado ingresa 6353

`Entonces` el sistema informa que el codigo ingresado no existe en el sistema

---


## Pagar Fotos
**ID:** Pagar Fotos

**TÍTULO:** Como usuario quier pagar fotos para poder retirarlas

**REGLAS DE NEGOCIO:** 
- Pagar 15$ por foto con tarjeta de credito 

**CRITERIOS DE ACEPTACIÓN:** 

#### **Escenario 1:** Pago exitoso
`Dado` que el usuario pepe tiene fotos previamente cargadas y posee una tarjeta de credito valida para pagar 15$ por foto

`Cuando` el usuario pepe presiona el boton "Pagar Fotos" e ingresa los datos de una tarjeta valida

`Entonces` El sistema registra el pago y le otorga al cliente un codigo para retirar las fotos

#### **Escenario 2:** Pago fallido por no tener fotos
`Dado` que el usuario manolo no tiene fotos previamente cargadas y posee una tarjeta de credito valida para pagar 15$ por foto

`Cuando` el usuario manolo presiona el boton "Pagar Fotos" e ingresa los datos de una tarjeta valida

`Entonces` El sistema informa que el usuario no tiene fotos cargadas

#### **Escenario 3:** Pago fallido por problemas con la tarjeta
`Dado` que el usuario juan tiene fotos previamente cargadas y posee una tarjeta de credito invalida para pagar 15$ por foto

`Cuando` el usuario juan presiona el boton "Pagar Fotos" e ingresa los datos de una tarjeta invalida

`Entonces` El sistema informa que hay problemas con el pago


<img src= 'https://i.gifer.com/origin/8c/8cd3f1898255c045143e1da97fbabf10_w200.gif' height="20" width="100%">

<div align = center>

## `Problema 6` Biblioteca 

</div>

![image](https://user-images.githubusercontent.com/55964635/232251137-9bbf9a21-f02d-4908-a670-8512253fcd11.png)

---

### Roles

- Alumno (No asociado)
- Socio
- Bibliotecario

### Historias de Usuario

- Registrar libro
- Asociar alumno
- Prestar libro
- Devolver libro

---

## Registrar libro


**ID:** Registrar Libro
 
**TÍTULO:** Como bibliotecaria quiero registrar un libro para que pueda ser prestado

**REGLAS DE NEGOCIO:** 


**CRITERIOS DE ACEPTACIÓN:** 

#### **Escenario 1:** Donación exitosa

`Dado` que el padre/madre dona un libro

`Cuando` la bibliotecaria ingresa los datos del ibro

`Entonces` el sistema registra el libro en el sistema

---

## Asociar alumno

**ID:** Asociar alumno
 
**TÍTULO:** Como alumno me quiero asociar para poder retirar libros

**REGLAS DE NEGOCIO:** 

**CRITERIOS DE ACEPTACIÓN:** 
- El alumno no debe estar registrado

#### **Escenario 1:** Asociación exitosa

`Dado` que es un alumno con dni 203200 entrega certificado de alumno regular y no esta registrado

`Cuando` la bibliotecaria ingresa 203200 

`Entonces` el sistema asocia al alumno y le otorga un carnet con un nro de socio

#### **Escenario 2:** Asociación fallida por alumno ya afiliado

`Dado` que es un alumno con dni 554234 entrega certificado de alumno regular y esta registrado

`Cuando` la bibliotecaria ingresa 203200 

`Entonces` el sistema informa que el alumno ingresado ya se encuentra registrado

#### **Escenario 3:** Asociación fallida por no entregar certificado

`Dado` que es un alumno con dni 12340 no entrega certificado de alumno regular

`Cuando` la bibliotecaria quiere asociar al alumno

`Entonces` la bibliotecaria le dice al niño que ya no joda

---

## Prestar Libro


**ID:** Prestar Libro
 
**TÍTULO:** Como bibliotecaria quiero prestar un libro para que el socio lo pueda leer

**REGLAS DE NEGOCIO:** 
- No posee mas de tres prestamos vigentes
- No debe tener prestamos vencidos
- Libro en buen estado

**CRITERIOS DE ACEPTACIÓN:** 

#### **Escenario 1:** Prestamo exitoso

`Dado` que posee 2 prestamos vigentes que es menor a 3 prestamos, no tiene prestamos vencidos y el libro "Harry Potter" esta en buen estado

`Cuando` la bibliotecaria ingresa el carnet 3123 y libro "Harry Potter"

`Entonces` el sistema registra el prestamo e incrementa los prestamos vigentes en uno

#### **Escenario 2:** Prestamo Fallido por poseer tres prestamos vigentes

`Dado` que posee 3 prestamos vigentes que es igual a 3 prestamos, no tiene prestamos vencidos y el libro "Pinocho" esta en buen estado

`Cuando` la bibliotecaria ingresa el carnet 3123 y libro "Pinocho"

`Entonces` el sistema informa que el socio ya posee tres prestamos vigentes y no registra el prestamo

#### **Escenario 3:** Prestamos fallido por tener prestamos vencidos

`Dado` que posee 1 prestamos vigentes que es menor a 3 prestamos, tiene prestamos vencidos y el libro "Blanca nieves" esta en buen estado

`Cuando` la bibliotecaria ingresa el carnet 3123 y libro "Blanca nieves"

`Entonces` el sistema informa que el socio tiene prestamos vencidos

#### **Escenario 4:** Prestamo fallido por libro en mal estado

`Dado` que posee 2 prestamos vigentes que es menor a 3 prestamos, no tiene prestamos vencidos y el libro "Harry Potter" esta en mal estado

`Cuando` la bibliotecaria ingresa el carnet 3123 y libroo "Harry Potter"

`Entonces` el sistema informa que el libro solicitado esta en mal estado

---

## Devolver Libro


**ID:** Devolver Libro
 
**TÍTULO:** Como socio quiero devolver un libro para poder recibir otros prestamos

**REGLAS DE NEGOCIO:** 
- Si el prestamo esta vencido, suspención por 15 dias

**CRITERIOS DE ACEPTACIÓN:** 

#### **Escenario 1:** Retorno exitoso

`Dado` que el prestamo no esta vencido

`Cuando` la bibliotecaria ingresa "Dragon Ball"

`Entonces` el sistema registra el retorno del libro

#### **Escenario 2:** Retorno exitoso con suspencion

`Dado` que el prestamo esta vencido

`Cuando` la bibliotecaria ingresa "Blanca nieves"

`Entonces` el sistema registra el retorno del libro, aumenta en uno los prestamos vencidos y suspende al socio por 15 dias


<img src= 'https://i.gifer.com/origin/8c/8cd3f1898255c045143e1da97fbabf10_w200.gif' height="20" width="100%">

<div align = center>

## `Problema 7` Mutual (Este enunciadado lo pase por arriba)

</div>


![image](https://user-images.githubusercontent.com/55964635/232254765-3caf2e2a-6204-4a5a-810b-913a45103127.png)

---

### Roles

- Persona (No afiliado)
- Afiliado

### Historias de Usuarios

- Afiliar persona
- Pagar con tarjeta
- Solicitar Ortodoncia
- Solicitar Plantillas
- Solicitar Anteojos
- Solicitar Internación
- Solicitar Consultas médicas

---

## Afiliar persona

**ID:** Persona
 
**TÍTULO:** Como persona quiero afiliarme para poder recibir prestaciones

**REGLAS DE NEGOCIO:** 
- El pago debe realizarse con tarjeta de credito


**CRITERIOS DE ACEPTACIÓN:** 

#### **Escenario 1:** Afiliación exitosa 

`Dado` que la persona Fabian Martinez no es afiliado y pago con una tarjeta de credito valida

`Cuando` la persona ingresa los datos de una tarjeta de credito valida

`Entonces` el sistema registra al afiliado y pasa a tener a cargo a su pareja e hijos(hasta que cumplan 18 años) y a cada uno se le otorga un numero de afiliado

#### **Escenario 2:** Afiliación fallida por persona ya afiliada 

`Dado` que la persona Tomas Martinez es afiliado y pago con una tarjeta de credito valida

`Cuando` la persona ingresa los datos de una tarjeta de credito valida

`Entonces` el sistema informa que la persona ya se encuentra registrada como afiliada

#### **Escenario 3:** Afiliación fallida por problemas con la tarjeta 

`Dado` que la persona Camila Martinez no es afiliado y pago con una tarjeta de credito invalida

`Cuando` la persona ingresa los datos de una tarjeta de credito invalida

`Entonces` el sistema informa que la tarjeta ingresada no es valida

---

## Pagar con tarjeta

**ID:** Pagar con tarjeta
 
**TÍTULO:** Como persona quiero pagar con tarjeta para poder afiliarme

**REGLAS DE NEGOCIO:** 

**CRITERIOS DE ACEPTACIÓN:** 

#### **Escenario 1:** Pago exitoso

`Dado` que se pudo establecer conexión con el servidor del banco, el nro de tarjeta 314 es valido y posee fondos suficientes 

`Cuando` la persona ingresa 314

`Entonces` El sistema registra el pago

#### **Escenario 2:** Pago fallido por falta de conexión con el servidor

`Dado` que no se pudo establecer conexión con el servidor del banco

`Cuando` la persona quiere pagar

`Entonces` el sistema informa que no se pudo establecer conexión con el banco y no realiza el pago

#### **Escenario 3:** Pago fallido por numero de tarjeta invalido

`Dado` que se pudo establecer conexión con el servidor del banco, el nro de tarjeta 6565 es invalido

`Cuando` la persona ingresa 6565

`Entonces` el sistema informa que el nro de tarjeta es invalido y no realiza el pago

#### **Escenario 4:** Pago fallido por fondos insuficientes

`Dado` que se pudo establecer conexión con el servidor del banco, el nro de tarjeta 8788 es valido y no posee fondos suficientes 

`Cuando` la persona ingresa 8788

`Entonces` el sistema informa que la tarjeta no tiene fondos suficientes y no realiza el pago

---

## Solicitar Ortodoncia

**ID:** Solicitar Ortodsoncia
 
**TÍTULO:** Como afiliado quiero solicitar ortodoncia para un chequeo

**REGLAS DE NEGOCIO:** 
- debe tener Pago asentado el mes anterior
- El prestamo solo se puede obtener una vez
- si es menor de 15 tienen necesita 9 meses de afiliado
- Presentar historia clinica 

**CRITERIOS DE ACEPTACIÓN:** 

#### **Escenario 1:** Solicitud exitosa

`Dado` que el afiliado Manolo pago el mes anterior, es la primera vez que recibe el prestamo, tiene 30 años que es mayor de 15 años y presenta la historia clinica

`Cuando` el afiliado solicita Ortodoncia

`Entonces` el sistema registra un turno para el afiliado y aumenta en uno los prestamos

#### **Escenario 2:** Solicitud fallida por falta de pago en el mes anterior

`Dado` que el afiliado Tomas no pago el mes anterior, es la primera vez que recibe el prestamo, tiene 32 años que es mayor de 15 años y presenta la historia clinica

`Cuando` el afiliado solicita Ortodoncia

`Entonces` el sistema informa que el afiliado no tiene asentado el pago del mes anterior

#### **Escenario 3:** Solicitud fallida porque ya recibio la prestación

`Dado` que el afiliado Scooby pago el mes anterior, no es la primera vez que recibe el prestamo, tiene 30 años que es mayor de 15 años y presenta la historia clinica

`Cuando` el afiliado solicita Ortodoncia

`Entonces` el sistema informa que su prestamo en ortodoncia ya fue utilizado

#### **Escenario 4:** Solicitud fallida por no presentar historia clinica

`Dado` que el afiliado Juan pago el mes anterior, es la primera vez que recibe el prestamo, tiene 5 años, 2 meses de afiliado y presenta la historia clinica

`Cuando` el afiliado solicita Ortodoncia

`Entonces` el sistema informa que el afiliado menor de 15 años debe tener como minimo 9 meses de afiliado


#### **Escenario 5:** Solicitud fallida por no presentar historia clinica

`Dado` que el afiliado Sergio pago el mes anterior, es la primera vez que recibe el prestamo, tiene 30 años que es mayor de 15 años y no presenta la historia clinica

`Cuando` el afiliado solicita Ortodoncia

`Entonces` el sistema informa que el afiliado debe presentar la historia clinica

---

## Solicitar Plantillas

**ID:** Solicitar Plantillas
 
**TÍTULO:** Como afiliado quiero solicitar plantillas para un chequeo

**REGLAS DE NEGOCIO:** 
- Tener pago el mes anterior
- Reciben como maximo 2 por año
- Presentar indicación profecional
- Presentar factura del comercio

**CRITERIOS DE ACEPTACIÓN:** Solicitar Plantillas

#### **Escenario 1:** Solicitud exitosa

`Dado` que el afiliado Juan tiene pago el mes anterior, lo solicito una vez en el año, presenta la indicación profecional y la facura del comercio

`Cuando` el afiliado solicita Plantillas

`Entonces` el sistema registra un turno para el afiliado

#### **Escenario 2:** Solicitud fallida por falta de pago

`Dado` que el afiliado Felipe no tiene pago el mes anterior, lo solicito una vez en el año, presenta la indicación profecional y la facura del comercio

`Cuando` el afiliado solicita Plantillas

`Entonces` el sistema informa que no se efectuo el pago del mes anterior

#### **Escenario 3:** Solicitud fallida por exceso de pedidos

`Dado` que el afiliado Nicolas tiene pago el mes anterior, lo solicito dos veces en el año, presenta la indicación profecional y la facura del comercio

`Cuando` el afiliado solicita Plantillas

`Entonces` el sistema informa que el afiliado ya solicito Plantillas dos veces en el año

#### **Escenario 4:** Solicitud fallida por no presentar la indicación

`Dado` que el afiliado Homero tiene pago el mes anterior, lo solicito una vez en el año, no presenta la indicación profecional y presento la facura del comercio

`Cuando` el afiliado solicita Plantillas

`Entonces` el sistema informa que el afiliado no presento la indicación profecional

#### **Escenario 5:** Solicitud fallida por no tener la factura del comercio

`Dado` que el afiliado Neimar tiene pago el mes anterior, lo solicito una vez en el año, presenta la indicación profecional y no tiene la facura del comercio

`Cuando` el afiliado solicita Plantillas

`Entonces` el sistema informa que el afiliado no tiene la factura del comercio


---

## Solicitar Anteojos

**ID:** Solicitar Anteojos
 
**TÍTULO:** Como afiliado quiero solicitar anteojos para poder ver mejor

**REGLAS DE NEGOCIO:**
- Tener pago el mes anterior
- Fecha de afiliación superior a 3 meses
- Un par cada 18 meses

**CRITERIOS DE ACEPTACIÓN:** 

#### **Escenario 1:** Solicitud exitosa

`Dado` que el afiliado Pepe tiene pago el mes anterior, tiene fecha de afiliacion de 4 meses y no solicito un par en los ultimo 18 meses

`Cuando` el afiliado solicita anteojos

`Entonces` el sistema reserva un turno para el afiliado

#### **Escenario 2:** Solicitud fallida por no tener pago el mes anterior

`Dado` que el afiliado Manuel no tiene pago el mes anterior, tiene fecha de afiliacion de 4 meses y no solicito un par en los ultimo 18 meses

`Cuando` el afiliado solicita anteojos

`Entonces` el sistema informa que el afiliado no tiene pago el mes anterior

#### **Escenario 3:** Solicitud fallida por tener fecha de afiliación menor a 3 meses

`Dado` que el afiliado Roberto tiene pago el mes anterior, tiene fecha de afiliacion de 2 meses y no solicito un par en los ultimo 18 meses

`Cuando` el afiliado solicita anteojos

`Entonces` el sistema informa que necesita minimo 3 meses de afiliacion para poder recibir el prestamo

#### **Escenario 3:** Solicitud fallida porque ya solicito un par en los ultimos 18 meses

`Dado` que el afiliado Pepe tiene pago el mes anterior, tiene fecha de afiliacion de 4 meses y solicito un par en los ultimo 18 meses

`Cuando` el afiliado solicita anteojos

`Entonces` el sistema informa que el afiliado ya solicito un prestamo de anteojos en los ultimos 18 meses

---

## Solicitar Internación

**ID:** Solicitar Internación
 
**TÍTULO:** Como afiliado quiero solicitar internación para un familiar

**REGLAS DE NEGOCIO:** 
- Tener pago el mes anterior

**CRITERIOS DE ACEPTACIÓN:** 

#### **Escenario 1:** Solicitud exitosa

`Dado` que el afiliado Cristian tiene pago el mes anterior

`Cuando` el afiliado solicita el prestamo

`Entonces` el sistema reserva un turno para el afiliado

#### **Escenario 2:** Solicitud fallida por no tener pago el mes anterior

`Dado` que el afiliado Koki no tiene pago el mes anterior

`Cuando` el afiliado solicita el prestamo

`Entonces` el sistema informa que no tiene pago el mes anterior


---

## Solicitar Consultas médicas

**ID:** Solicitar Consultas medicas
 
**TÍTULO:** Como afiliado quiero solicitar consultas medicas para poder hacerme un chequeo

**REGLAS DE NEGOCIO:** 
- Tener pago el mes anterior
- Hasta 2 por mes

**CRITERIOS DE ACEPTACIÓN:** 

#### **Escenario 1:** Solicitud exitosa

`Dado` que el afiliado Maradona tiene pago el mes anterior y solicito un par en el mes

`Cuando` el afiliado solicita prestamo

`Entonces` el sistema registra un turno para el afiliado

#### **Escenario 2:** Solicitud fallida por no tener pago el mes anterior

`Dado` que el afiliado Jorge no tiene pago el mes anterior y solicito un par en el mes

``Cuando`` el afiliado solicita prestamo

``Entonces`` el sistema informa que el afiliado no tiene asentado el pago del mes anterior

#### **Escenario 3:** Solicitud fallida por haber solicitado 2 pares en el ultimo mes

``Dado`` que el afiliado Luis tiene pago el mes anterior y solicito dos pares en el mes

``Cuando`` el afiliado solicita prestamo

``Entonces`` el sistema informa que el afiliado ya tiene dos pares solicitados en el ultimo mes

<img src= 'https://i.gifer.com/origin/8c/8cd3f1898255c045143e1da97fbabf10_w200.gif' height="20" width="100%">

<div align = center>

## `Problema 8` Teatro

</div>

![image](https://user-images.githubusercontent.com/55964635/232352219-2261f020-e05f-4ab6-9c10-570f306113c1.png)

---

### Roles

- Empleado/Espectador/usuario
- Vendedor de boleteria
- Administrador

### Historia de usuarios
- Seleccionar obra
- Reservar entrada Presencial
- Pagar con tarjeta
- Comprar entrada Online
- Comprar entrada Presencial
- Retirar entrada reservada
- Retirar entrada con codigo
- Administrar Programación de la sala

No se en donde meter que `las entradas caducan 3 horas antes del evento`

---

### Seleccionar Obra

**ID:** Mostrar Funciones
 
**TÍTULO:** Como empleado quiero mostrar las funciones para que el cliente pueda elegir

**REGLAS DE NEGOCIO:** 

**CRITERIOS DE ACEPTACIÓN:** Seleccionar Obra

#### **Escenario 1:** Muestra Exitosa

`Dado` que la pelicula "King Kong" tiene funciones disponibles

`Cuando` el empleado ingresa "King Kong"

`Entonces` el sistema muestra una lista de funciones disponibles 

#### **Escenario 2:** Muestra fallida por falta de funciones

`Dado` que la persona selecciona la pelicula "Duro de Matar" y no hay funciones disponibles

`Cuando` el empleado ingresa "Duro de Matar"

`Entonces` el sistema informa que hay funciones disponibles para esa pelicula

---

## Reservar entrada Presencial


**ID:** Reservar entrada Presencial
 
**TÍTULO:** como empleado quiero reservarle una entrada al espectador para que pueda ver la pelicula

**REGLAS DE NEGOCIO:** 
- Maximo 2 entradas
- Las entradas se reservan con 3 horas de anticipación como minimo

**CRITERIOS DE ACEPTACIÓN:** Reservar entrada Presencial

#### **Escenario 1:** Reserva exitosa

`Dado` que la persona Manolo tiene una entrada reservada y la reserva es dos dias antes del evento

`Cuando` el empleado ingresa 1-1-2001, 14:00, King Kong, Manolo, 12345

`Entonces` El sistema realiza la reserva de la entrada y aumenta en uno la cantidad de entradas del usuario

#### **Escenario 2:** Reserva fallida porque el usuario ya reservo dos entradas

`Dado` que la persona Quico tiene dos entradas reservadas y la reserva es dos dias antes del evento

`Cuando` el empleado ingresa 12-12-2012, 11:00, Harry Potter, Quico, 312312

`Entonces` el sistema informa que la persona ya tiene 2 entradas reservadas

#### **Escenario 3:** Reserva fallida porque el usuario reserva la entrada 1 hora antes del evento

`Dado` que la persona Bils no tiene entradas reservadas y la reserva es 1 (una) hora antes del evento

`Cuando` el empleado ingresa 31-11-2021, 16:00, Dragon Ball, Bils, 66666

`Entonces` el sistema informa que no se pueden reservar entradas 3 horas antes del evento.

---

## Comprar entrada Online

**ID:** Comprar entrada Online
 
**TÍTULO:** Como usuario quiero comprar una entrada online para ver una pelicula

**REGLAS DE NEGOCIO:** 
- El pago se realiza con tarjeta de credito

**CRITERIOS DE ACEPTACIÓN:** Comprar entrada Online

#### **Escenario 1:** Compra de entrada exitosa

`Dado` que el usuario Fabian posee una tarjeta de credito valida

`Cuando` el usuario selecciona una opcion, 10101, 20 , ingresa los datos de una tarjeta de credito valida y selecciona la opcion pagar

`Entonces` el sistema registra el pago y emite un codigo de compra para retirar las entradas en el cine

#### **Escenario 2:** Compra de entrada fallida por tarjeta invalida

`Dado` que el usuario Tomas no posee una tarjeta de credito valida

`Cuando` el usuario selecciona una opcion, 22222, 40, ingresa los datos de una tarjeta de credito invalida y selecciona la opcion pagar

`Entonces` el sistema informa que la tarjeta ingresada es invalida

---

## Pagar con tarjeta

**ID:** Pagar con tarjeta
 
**TÍTULO:** como persona quiero pagar con tarjeta para poder retirar mi entrada

**REGLAS DE NEGOCIO:** 

**CRITERIOS DE ACEPTACIÓN:** Pagar con tarjeta

#### **Escenario 1:** Paga exitosa

`Dado` que la conexión con el banco es exitosa, el nro de tarjeta 312 es valida , la tarjeta posee fondos suficientes y fecha de vencimiento el el 20-2-2060

`Cuando` la persona ingresa 312, 20-2-2060, 1

`Entonces` El sistema registra el pago

#### **Escenario 2:** Paga fallida por falta de conexión con el servidor del banco

`Dado` que la conexión con el banco no es exitosa

`Cuando` la persona intenta pagar

`Entonces` El sistema informa que no se pudo establecer conexión con el servidor del banco

#### **Escenario 3:** Paga fallida por nro de tarjeta invalido

`Dado` que la conexión con el banco es exitosa, el nro de tarjeta 222 es invalida

`Cuando` la persona ingresa 222, 25-12-2060, 4

`Entonces` El sistema informa que el nro de tarjeta es invalido y no registra el pago

#### **Escenario 4:** Paga fallida por no poseer fondos suficientes

`Dado` que la conexión con el banco es exitosa, el nro de tarjeta 444 es valida , la tarjeta no posee fondos suficientes y fecha de vencimiento el 20-2-2160

`Cuando` la persona ingresa 444, 20-2-2160, 7

`Entonces` El sistema informa que la tarjeta no posee fondos suficientes y no registra el pago

#### **Escenario 5:** Paga fallida por tarjeta vencida

`Dado` que la conexión con el banco es exitosa, el nro de tarjeta 555 es valida , la tarjeta posee fondos suficientes y vencimiento el 06-4-2065

`Cuando` la persona ingresa 555, 06-4-2065, 9

`Entonces` El sistema informa que la tarjeta se encuentra vencida y no registra el pago

---

## Comprar entrada Presencial

**ID:** Comprar entrada Presencial
 
**TÍTULO:** Como persona quiero comprar una entrada presencial para poder ver una pelicula

**REGLAS DE NEGOCIO:** 
- El pago se realiza con una tarjeta de credito

**CRITERIOS DE ACEPTACIÓN:** Comprar entrada Presencial

#### **Escenario 1:** Compra de entrada exitosa

`Dado` que el usuario Riquelme posee una tarjeta de credito valida

`Cuando` el usuario selecciona una opcion, 99919, 11 e ingresa los datos de una tarjeta de credito valida

`Entonces` el sistema registra el pago e imprime las entradas

#### **Escenario 2:** Compra de entrada fallida por tarjeta invalida

`Dado` que el usuario Pele no posee una tarjeta de credito valida

`Cuando` el usuario selecciona una opcion, 5432, 4 e ingresa los datos de una tarjeta de credito invalida

`Entonces` el sistema informa que la tarjeta ingresada es invalida

---

## Retirar entrada

**ID:** Retirar entrada 

**TÍTULO:** como persona quiero retirar mi entrada para poder ir a mirar la pelicula

**REGLAS DE NEGOCIO:** 
- Posee al menos una entrada
- Entrada no caducada

**CRITERIOS DE ACEPTACIÓN:** Retirar entrada 

#### **Escenario 1:** Retiro de entrada reservada exitosa

`Dado` que la persona Giorgio tiene 3 entradas de las cuales ninguna esta caducada y presenta el codigo 7777 valido

`Cuando` la persona ingresa Giorgio, 29139, 7777

`Entonces` El sistema imprime las entradas correspondientes y las libera

#### **Escenario 2:** Retiro de entrada sin codigo exitosa

`Dado` que la persona Vegeta tiene 3 entradas de las cuales ninguna esta caducada y no presenta el codigo

`Cuando` la persona ingresa Vegeta, 99885

`Entonces` El sistema imprime las entradas correspondientes

#### **Escenario 3:** Retiro fallido por no tener entradas

`Dado` que la persona ElRubius no tiene entradas

`Cuando` la persona ingresa ElRubius, 019192

`Entonces` El sistema informa que la persona no tiene entradas reservadas

#### **Escenario 4:** Retiro fallido por entradas caducadas

`Dado` que la persona Leo tiene 2 entradas de las cuales todas estan caducadas y presenta el codigo 6666 valido

`Cuando` la persona ingresa Leo, 12341, 6666

`Entonces` El sistema informa que las entradas se encuentran caducadas

#### **Escenario 5:** Retiro por codigo invalido

`Dado` que la persona Auron tiene 3 entradas de las cuales ninguna esta caducada y presenta el codigo 123111 invalido

`Cuando` la persona ingresa Auron, 3919239, 123111

`Entonces` El sistema informa que el codigo ingresado es invalido

---

## Administrar Programación de la sala

**ID:** Administrar Programación de la sala
 
**TÍTULO:** Como administrador quiero administrar la programación de la sala para cumplir con mi trabajo

**REGLAS DE NEGOCIO:** 

**CRITERIOS DE ACEPTACIÓN:** Administrar Programación de la sala

#### **Escenario 1:** Administración exitosa

`Dado` que el administrador tiene una distribución semanal

`Cuando` el administrador ingresa la distribución semanal

`Entonces` El sistema carga la administración semanal de las salas para la venta de entradas

#### **Escenario 2:** Administración fallida por falta de distribución

`Dado` que el administrador no tiene una distribución semanal

`Cuando` el administrador quiere actualizar la distribución semanal

`Entonces` El sistema no actualiza la distribución semanal

<img src= 'https://i.gifer.com/origin/8c/8cd3f1898255c045143e1da97fbabf10_w200.gif' height="20" width="100%">

<div align = center>

## `Problema 9` Pago Electrónico

</div>


`La verdad es que este enunciado es horrible, de momento no lo pienso hacer`



<img src= 'https://i.gifer.com/origin/8c/8cd3f1898255c045143e1da97fbabf10_w200.gif' height="20" width="100%">

<div align = center>

## `Problema 10` Un Aventón (Este esta mal)

</div>

![](2023-05-15-14-23-37.png)

---

### Roles
- Persona (Usuario no registrado)
- Usuario
- Chofer


### Historias de Usuario
- Registrar persona
- Alta viaje
- Postularse a un viaje

De este ejercicio tengo bastantes dudas la verdad

---

## Registrar Persona
 
**ID:** Registrar persona
 
**TÍTULO:** Como persona quiero registrarme para poder subir viajes

**REGLAS DE NEGOCIO:** 
- Correo electronico unico

**CRITERIOS DE ACEPTACIÓN:** Registrar persona

#### **Escenario 1:** Registro exitoso

`Dado` que el mail fabo@gmail.com es unico

`Cuando` la persona ingresa fabo19, fabo@gmail.com, cocacola10

`Entonces` el sistema registra a la persona 

#### **Escenario 2:** Registro fallido

`Dado` que el mail messi@gmail.com no es unico

`Cuando` la persona ingresa messi, messi@gmail.com, messi10

`Entonces` el sistema informa que la persona ya se encuentra registrada

---

## Alta viaje

**ID:** Alta viaje
 
**TÍTULO:** Como usuario autenticado quiero dar alta un viaje para salir con mis amigos

**REGLAS DE NEGOCIO:** 
- No se superpone con otro viaje
- Adeuda clasificaciones

**CRITERIOS DE ACEPTACIÓN:** Alta viaje

#### **Escenario 1:** Alta de viaje exitoso

`Dado` que el usuario fabo19 con un viaje el 01-01-2001 a las 19:00 no se superpone y no adeuda clasificaciones

`Cuando` el usuario ingresa 01-01-2001, 19:00, Camioneta

`Entonces` el sistema da de alta el viaje

#### **Escenario 2:** Alta de viaje fallida por superposición

`Dado` que el usuario giorgio69 con un viaje el 11-11-2011 a las 11:00 se superpone y no adeuda clasificaciones

`Cuando` el usuario ingresa 11-11-2011, 11:00, Remis

`Entonces` el sistema informa que el viaje se superpone con otra fecha

#### **Escenario 3:** Alta de viaje fallida por adeudar clasificaciones

`Dado` que el usuario rubiusOMG con un viaje el 07-07-2007 a las 17:00 no se superpone y adeuda clasificaciones

`Cuando` el usuario ingresa 07-07-2007, 17:00, Avion

`Entonces` el sistema informa que el usuario adeuda clasificaciones 

---

## Postularse a un viaje

**ID:** Postularse a un viaje
 
**TÍTULO:** Como usuario identificado quiero postularme a un viaje para hacer compañia 

**REGLAS DE NEGOCIO:** 

**CRITERIOS DE ACEPTACIÓN:** 

#### **Escenario 1:** Postulación exitosa

`Dado` que el usuario tiene una sesión abierta

`Cuando` se postula a un viaje

`Entonces` el sistema registra al postulado y lo notifica

<img src= 'https://i.gifer.com/origin/8c/8cd3f1898255c045143e1da97fbabf10_w200.gif' height="20" width="100%">

<div align = center>

## `Problema 11` Concursos

</div>

---

![](2023-05-15-14-24-38.png)


---

## Registrar Persona

**ID:** Registrar Persona
 
**TÍTULO:** Como persona quiero registrarme para poder inscribirme a un curso

**REGLAS DE NEGOCIO:** 
- Mail no registrado
- El dni no tiene que ser mayor de 55M
- El dni no tiene que ser menor de 12M


**CRITERIOS DE ACEPTACIÓN:** 

#### **Escenario 1:** Registro Exitoso

`Dado` que el usuario fabian@gmail.com no esta registrado, el dni 40M es mayor a 12M y menor a 55M

`Cuando` la persona ingresa 44M, Fabian, Martinez, fabian@gmail.com

`Entonces` El sistema manda un correo una contraseña asignada automaticamente

#### **Escenario 2:** Registro Fallido por mail registrado

`Dado` que el usuario juan@gmail.com esta registrado, el dni 45M es mayor a 12M y menor a 55M

`Cuando` la persona ingresa 45M, Juan, Carosella, juan@gmail.com

`Entonces` El sistema informa que el mail ya se encuentra registrado

#### **Escenario 3:** Registro Fallido por dni menor a 12M

`Dado` que el usuario messi@gmail.com no esta registrado, el dni 10M es menor a 12M y menor a 55M

`Cuando` la persona ingresa 10M, Lionel, Messi, messi@gmail.com

`Entonces` El sistema informa que el dni es menor de 12M

#### **Escenario 4:** Registro Fallido por dni mayor a 55M

`Dado` que el usuario pepe@gmail.com no esta registrado, el dni 400M es mayor a 12M y mayor a 55M

`Cuando` la persona ingresa 440M, Pepe, Zapo, pepe@gmail.com

`Entonces` El sistema informa que el dni es mayor de 55M


---

## Iniciar Sesión

**ID:** Iniciar Sesión
 
**TÍTULO:** Como Usuario quiero iniciar sesión para inscribirme a un concurso

**REGLAS DE NEGOCIO:** 

**CRITERIOS DE ACEPTACIÓN:** 

#### **Escenario 1:** Inicio Exitoso

`Dado` que el usuario fabian@gmail.com esta registrado y la contraseña omgCosa30 es correcta

`Cuando` el usuario ingresa fabian@gmail.com, omgCosa30 

`Entonces` El sistema inicia sesión y habilita las opciones para inscribirse a un concurso

#### **Escenario 2:** Inicio Fallido por usuario no registrado

`Dado` que el usuario carlos@gmail.com no esta registrado

`Cuando` el usuario ingresa carlos@gmail.com, casaRosada

`Entonces` El sistema informa que el usuario no se encuentra registrado

#### **Escenario 3:** Inicio Fallido por contraseña incorrecta

`Dado` que el usuario dios@gmail.com esta registrado y la contraseña "testigos" es incorrecta

`Cuando` el usuario ingresa dios@gmail.com, "testigos" 

`Entonces` El sistema informa que la contraseña es incorrecta.

---

## Cerrar Sesión

**ID:** Cerrar Sesión
 
**TÍTULO:** Como usuario logueado quiero cerrar sesión para conservar mis datos

**REGLAS DE NEGOCIO:** 

**CRITERIOS DE ACEPTACIÓN:** 

#### **Escenario 1:** Inicio Exitoso

`Dado` que el usuario fabian@gmail.com tiene una sesión abierta

`Cuando` el usuario presiona el boton "cerrar sesión"

`Entonces` El sistema cierra la sesión y deshabilita las opciones para la inscripción a los concursos

---

## Inscribirse a un concurso

**ID:** Inscribirse a un concurso
 
**TÍTULO:** Como usuario quiero inscribirme a un conscurso para participar

**REGLAS DE NEGOCIO:** 
- No se puede inscribir a mas de 3 concursos

**CRITERIOS DE ACEPTACIÓN:** 

#### **Escenario 1:** Inscripción exitosa

`Dado` que tiene 1 inscripción a un concurso que es menor al maximo de 3 concursos

`Cuando` el usuario selecciona el conscurso "Informatica"

`Entonces` El sistema acepta la inscripción, imprime comprobante y aumenta en uno la cantidad de inscripciones del usuario

#### **Escenario 2:** Inscripción fallida por tener 3 concursos

`Dado` que tiene 3 inscripciones a concursos que es igual al maximo de 3 concursos

`Cuando` el usuario selecciona el concurso "Gastronomia"

`Entonces` El sistema informa que esta inscripto al maximo de concursos permitido

---


## Imprimir Listado

**ID:** Imprimir Listado
 
**TÍTULO:** como jefe de area administrativa quiero imprimir el listado de los inscriptos a una materia para poder llevarlo al secretario administrativo

**REGLAS DE NEGOCIO:** 
- No se puede inscribir a mas de 3 concursos

**CRITERIOS DE ACEPTACIÓN:** 

#### **Escenario 1:** Inscripción exitosa

`Dado` que la materia Informatica tiene inscriptos para imprimir

`Cuando` el jefe de area administrativa selecciona informatica y presiona el boton imprimir inscriptos

`Entonces` El sistema imprime un listado con los inscriptos a esa materia



<img src= 'https://i.gifer.com/origin/8c/8cd3f1898255c045143e1da97fbabf10_w200.gif' height="20" width="100%">

<div align = center>

## `Problema 12` Créditos bancarios

</div>

![](2023-05-15-14-25-19.png)
![](2023-05-16-09-59-06.png)


## Solicitar un credito

**ID:** Solicitar un credito
 
**TÍTULO:** como cliente quiero solicitar un credito para solicitar un prestamo

**REGLAS DE NEGOCIO:** 
- El dni debe ser cliente del banco
- El monto no debe superar los 400.000$

**CRITERIOS DE ACEPTACIÓN:** 

#### **Escenario 1:** Solicitud exitosa

`Dado` que el dni 20321 es cliente del banco y el monto 20$ no supera los 400.000$

`Cuando` el cliente ingresa 20321, Fabian, Martinez, fabian@gmail.com, Personal, 20$

`Entonces` El sistema almacena el tramite e imprime un numero de comprobante para el cliente

#### **Escenario 2:** Solicitud fallida porque el dni no es cliente

`Dado` que el dni 54321 no es cliente del banco y el monto 200$ no supera los 400.000$

`Cuando` el cliente ingresa 54321, Tomas, Pompile, tomas@gmail.com,Personal, 200$

`Entonces` El sistema envia un correo un instructivo para hacerse cliente del banco

#### **Escenario 3:** Solicitud fallida porque el monto excede lo permitido

`Dado` que el dni 12345 es cliente del banco y el monto 2000.000$ no supera los 400.000$

`Cuando` el cliente ingresa 12345, Josue, Suarez, josu@gmail.com, Personal, 2000.000$

`Entonces` El sistema rechaza el inicio de tramite y muestra el mensaje "el monto solicitado excede el limite permitido"


---

## Consultar el estado

**ID:** Consultar el estado
 
**TÍTULO:** como usuario quiero consultar el estado para estar informado

**REGLAS DE NEGOCIO:** 
- tiene 3 intentos antes del bloqueo de ip

**CRITERIOS DE ACEPTACIÓN:** 

#### **Escenario 1:** Consulta exitosa

`Dado` que la ip no esta bloqueada, esta en el intento 0, el nro de comprobante 398129 es valido

`Cuando` el cliente ingresa 398129

`Entonces` El sistema retorna un informa con el estado del mismo

#### **Escenario 2:** Consulta fallida con nro invalido

`Dado` que la ip no esta bloqueada, esta en el intento 0 y el nro de comprobante 423789 es invalido

`Cuando` el cliente ingresa 423789

`Entonces` El sistema muestra "el tramite es inexistente" y aumenta los intentos en uno

#### **Escenario 3:** Consulta fallida por nro invalido

`Dado` que la ip no esta bloqueada, esta en el intento 2 y el nro de comprobante 123451 es invalido

`Cuando` el cliente ingresa 123451

`Entonces` El sistema muestra "el tramite es inexistente" y bloquea la ip

#### **Escenario 4:** Consulta fallida por bloqueo de IP

`Dado` que la ip esta bloqueada

`Cuando` el cliente quiere ingresar un nro de comprobante

`Entonces` El sistema informa "usted a excedido el numero de consultas inválida"

## Imprimir Listado

**ID:** Imprimir Listado
 
**TÍTULO:** como gerente quiero imprimir un listado de los creditos aprobados para estar informado

**REGLAS DE NEGOCIO:** 
- Las fechas deben ser validas

**CRITERIOS DE ACEPTACIÓN:** 

#### **Escenario 1:** Impresion exitosa

`Dado` que la fecha 12/3/2020 es valida y hay creditos aprobados para imprimir

`Cuando` el gerente ingresa 12/3/2020 y presiona el boton imprimir listado

`Entonces` El sistema muestra un listado con los creditos aprobados

#### **Escenario 2:** Impresion fallida por fecha invalida

`Dado` que la fecha 12/3/220 es invalida

`Cuando` el gerente ingresa 12/3/220 y presiona el boton imprimir listado

`Entonces` El sistema informa, las fehcas ingresadas no son validas

#### **Escenario 3:** Impresion fallida por lista vacia

`Dado` que la fecha 30/3/2020 es valida y no hay creditos aprobados para imprimir

`Cuando` el gerente ingresa 30/3/2020 y presiona el boton imprimir listado

`Entonces` El sistema informa que no hay creditos aprobados para mostrar

## Falta el iniciar sesión y cerrar sesión alta paja

<img src= 'https://i.gifer.com/origin/8c/8cd3f1898255c045143e1da97fbabf10_w200.gif' height="20" width="100%">

<div align = center>

## `Problema 12` Venta de libros

</div>

![](2023-05-16-09-59-36.png)

<img src= 'https://i.gifer.com/origin/8c/8cd3f1898255c045143e1da97fbabf10_w200.gif' height="20" width="100%">

<div align = center>

## `Problema 13` Manejo de tarjetas de crédito

</div>

![](2023-05-16-10-00-37.png)
Falta la otra pagina

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