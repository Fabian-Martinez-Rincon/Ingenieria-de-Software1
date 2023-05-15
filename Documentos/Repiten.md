


## Estas son las historias que son iguales en todos los ejercicios

---

## Pagar con Tarjeta


**ID:** Pagar con tarjeta
 
**TÍTULO:** Como usuario quiero pagar con tarjeta para pode reservar un alquiler

**REGLAS DE NEGOCIO:** 

- Numero de tarjeta valido
- Tiene fondos suficientes

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


---

### Registrar Usuario

**ID:** Registrar Alumno
 
**TÍTULO:** Como alumno quiero registrarme para tener una cuenta

**REGLAS DE NEGOCIO:** 
- Nombre de usuario unico
- Contaseña con mas de 6 digitos (Esta puede variar)


**CRITERIOS DE ACEPTACIÓN:** 

#### **Escenario 1:** Registrar Alumno

`Dado` que el usuario fabo es unico y la contraseña kapo013 tiene mas de 6 digitos

`Cuando` el alumno ingresa fabo, kapo013

`Entonces` el sistema registra al usuario

#### **Escenario 2:** Registro fallido por usuario ya existente

`Dado` que el usuario tomo no es unico y la contraseña pepe555 tiene mas de 6 digitos

`Cuando` el alumno ingresa tomo, pepe555

`Entonces` el sistema Informa que el usuario ingresado ya existe, y no realiza el registro

#### **Escenario 3:** Registro fallido por contraseña con menos de 6 digitos

`Dado` que el usuario messi es unico y la contraseña 2023 tiene menos de 6 digitos

`Cuando` el alumno ingresa messi, 2023

`Entonces` el sistema informa que la contraseña ingresada tiene menos de 6 digitos y no realiza el registro

---

### Iniciar Sesión

**ID:** Iniciar Sesión
 
**TÍTULO:** Como usuario quiero iniciar sesión para poder entrar en mi cuenta

**REGLAS DE NEGOCIO:** 

**CRITERIOS DE ACEPTACIÓN:** Iniciar Sesión

#### **Escenario 1:** Inicio exitoso

`Dado` que el usuario fabo se encuentra registrado y la contraseña kapo013 es correcta

`Cuando` el usuario ingresa fabo, kapo013

`Entonces` el sistema realiza el inicio de sesión y habilita sus respectivas opciones


#### **Escenario 2:** Inicio fallido por usuario no registrado

`Dado` que el usuario maradona no se encuentra registrado

`Cuando` el usuario ingresa maradona, cocacola21

`Entonces` el sistema informa que el usuario no se encuentra registrado y no realiza el inicio de sesión

#### **Escenario 3:** Inicio fallido por contraseña incorrecta

`Dado` que el usuario stalin se encuentra registrado y la contraseña presi19 es incorrecta

`Cuando` el usuario ingresa stalin, presi19

`Entonces` el sistema informa que la contraseña es incorrecta y no realiza el inicio de sesión

---

### Cerrar Sesión

**ID:** Cerrar Sesión
 
**TÍTULO:** 

**REGLAS DE NEGOCIO:** Cerrar Sesión

**CRITERIOS DE ACEPTACIÓN:** 

**Escenario 1:** Cierre exitoso

`Dado` que el usuario tiene una sesión abierta

`Cuando` el usuario aprieta el boton de cerrar su sesión

`Entonces` el sistema cierra la sesión y deshabilita sus respectivas opciones 

---
