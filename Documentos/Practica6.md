<div align="center">

[![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/Nomadiix/IS1)
[![GitHub stars](https://img.shields.io/github/stars/Nomadiix/IS1)](https://github.com/FabianMartinez1234567/IS1/stargazers/)
[![GitHub repo size in bytes](https://img.shields.io/github/repo-size/Nomadiix/IS1)](https://github.com/Nomadiix/IS1)
 </div>
 
<h1 align="center"> 🕸️ Practica 5</h1>
<div align="center">
<img src="https://media.giphy.com/media/XG0tayFvL5MoSJ4OVw/giphy.gif"/>
</div>

---

- [Ejercicio 1 ]()
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
- [Ejercicio 13]()
- [Ejercicio 14]()
- [Ejercicio 15]()
- [Ejercicio 16]()
- [Ejercicio 17]()

<img src= 'https://i.gifer.com/origin/8c/8cd3f1898255c045143e1da97fbabf10_w200.gif' height="20" width="100%">

## Ejercicio 1

Pedrito está decidiendo que sistema operativo instalar en la computadora de su hermana que se inscribió en la carrera Lic. en Sistemas. Si su hermana va a usar la computadora para jugar le instalará Windows, de lo contrario le instalará Linux. Además, en el caso de instalar Windows, debe evaluar qué antivirus instalar. Si su hermana le comenta que no tiene dinero deberá instalarle un antivirus libre, en cambio, si la hermana le dice que tiene dinero le instalará un antivirus con licencia. Por último, deberá evaluar si la hermana va a programar en Python. 

En este caso deberá instalarle el paquete Anaconda

<img src= 'https://i.gifer.com/origin/8c/8cd3f1898255c045143e1da97fbabf10_w200.gif' height="20" width="100%">

## Ejercicio 2

Se desea modelar mediante una tabla de decisión el siguiente problema:

Pedro tiene que cambiar su compu y está evaluando qué hacer. Si a Pedro le toman su máquina como parte de pago y la compu a comprar sale menos de 15 mil entonces la comprará en efectivo. Si cuesta más de 15 mil y le toman su compu, entonces la pagará en cuotas. Además, si supera los 25 mil, le pedirá plata a su mamá. En el caso que no le tomen su computadora como parte de pago pagará en cuotas y le pedirá plata a su mamá sin importar el valor de la máquina a comprar.

<img src= 'https://i.gifer.com/origin/8c/8cd3f1898255c045143e1da97fbabf10_w200.gif' height="20" width="100%">

## Ejercicio 3

Una entidad financiera tiene como servicio a sus clientes el otorgamiento de créditos. Si el cliente tiene una antigüedad mayor o igual a dos años, se considera su valor promedio de movimientos mensuales para optar a un crédito, de la siguiente forma: si su promedio es mayor o igual a $ 60.000, puede optar por un crédito máximo de 1 millón de pesos. Si su promedio es inferior a $ 60.000 pero igual o superior a $ 40.000, puede optar a un crédito máximo de $ 70.000. Si su promedio es inferior a $ 40.000, el máximo al que puede optar es $ 50.000. En cualquiera de estos casos, el cliente elige el número de cuotas hasta un máximo de 120.

Si la antigüedad del cliente es inferior a 2 años, el cliente solo puede acceder a un crédito de máximo $50.000, y además debe pagar un interés adicional. En este caso, además, debe considerarse que si el promedio mensual del cliente es inferior a $ 40.000 puede solicitar un máximo de 12 cuotas, y si es superior o igual a $ 40.000, el máximo de cuotas es 20

<img src= 'https://i.gifer.com/origin/8c/8cd3f1898255c045143e1da97fbabf10_w200.gif' height="20" width="100%">

## Ejercicio 4

Dado el siguiente enunciado y la solución propuesta:
- a. Identifique y corrija los siguientes errores:
    - i. Errores en las acciones.
    - ii. Errores en las reglas.
    - iii. Errores de marcado.
- b. Sobre la tabla resultante del inciso a) realice, si es posible, la reducción de la tabla.

Una clínica privada ubicada en la ciudad de La Plata realiza diferentes estudios a los docentes de la Facultad de Informática. A todos los docentes se le realiza un estudio de rutina. Si el docente es menor  de 25 años, además se le realiza un estudio de fuerza. A los docentes mayores de 40 años además, se les realiza un estudio de corazón.  Si el docente es diplomado y es mayor de 40 años, se le paga un plus en el sueldo

| Condiciones  | R1 | R2 | R3 | R4 | R5 | R6 | R7 | R7 |
| ------------- | ------------- | ------------- | ------------- | ------------- | ------------- | ------------- | ------------- | ------------- |
| Edad <= 40 | V  | V  | V  | V  | F  | F  | F  | F  |
| Es diplomado | V  | V  | F  | F  | V  | V  | F  | F  |
| Edad <= 25 | V  | F  | V  | F  | V  | F  | V  | F  |
| Acciones |   |   |   |   |   |   |   |   |
| Estudio del Corazón y examen de rutina  |  |   |   |   | X  | X  | X  | X  |
| Paga Plus |   |   |   |   | X  | X  |   |   |
| Estudio de fuerza | X  |   | X  |   |   |   |   |   |

<img src= 'https://i.gifer.com/origin/8c/8cd3f1898255c045143e1da97fbabf10_w200.gif' height="20" width="100%">

## Ejercicio 5

Dado el siguiente enunciado y las soluciones propuestas:

- `a)` Indique en cuál de las tres soluciones están correctamente identificadas las condiciones y acciones.
- `b)` En la solución del inciso anterior identificada como correcta, marque las acciones correspondientes.
- `c)` Sobre la tabla resultante del inciso `b)` realizar, de ser posible, la reducción correspondiente.

Se desea desarrollar un sistema de autoayuda para una pinturería. Los clientes ingresan su inquietud al sistema web y el sistema debe ayudar a decidir qué tipo de pintura utilizar.

Si lo que se va a pintar es una pared, entonces se deberá utilizar pintura tipo Látex y previamente se le aplicará enduido. Para pintar otras superficies se usará Pintura Sintética y se recomendará comprar además un diluyente especial. Si la pared que se va a pintar está en el exterior se recomendará Pintura Látex Exterior, caso contrario será Pintura Látex Interior.  Por último, en caso que lo que se desea pintar esté en mal estado, deberá aplicarse primero un fondo blanco.

### Solución propuesta 

| First Header  | Second Header | Second Header | Second Header | Second Header | Second Header | Second Header | Second Header | Second Header |
| ------------- | ------------- | ------------- | ------------- | ------------- | ------------- | ------------- | ------------- | ------------- |
| Content Cell  | Content Cell  | Content Cell  | Content Cell  | Content Cell  | Content Cell  | Content Cell  | Content Cell  | Content Cell  |
| Content Cell  | Content Cell  | Content Cell  | Content Cell  | Content Cell  | Content Cell  | Content Cell  | Content Cell  | Content Cell  |

<img src= 'https://i.gifer.com/origin/8c/8cd3f1898255c045143e1da97fbabf10_w200.gif' height="20" width="100%">

## Ejercicio 6

<img src= 'https://i.gifer.com/origin/8c/8cd3f1898255c045143e1da97fbabf10_w200.gif' height="20" width="100%">

## Ejercicio 7

<img src= 'https://i.gifer.com/origin/8c/8cd3f1898255c045143e1da97fbabf10_w200.gif' height="20" width="100%">

## Ejercicio 8

<img src= 'https://i.gifer.com/origin/8c/8cd3f1898255c045143e1da97fbabf10_w200.gif' height="20" width="100%">

## Ejercicio 9

<img src= 'https://i.gifer.com/origin/8c/8cd3f1898255c045143e1da97fbabf10_w200.gif' height="20" width="100%">

## Ejercicio 10

<img src= 'https://i.gifer.com/origin/8c/8cd3f1898255c045143e1da97fbabf10_w200.gif' height="20" width="100%">

## Ejercicio 11

<img src= 'https://i.gifer.com/origin/8c/8cd3f1898255c045143e1da97fbabf10_w200.gif' height="20" width="100%">

## Ejercicio 12

<img src= 'https://i.gifer.com/origin/8c/8cd3f1898255c045143e1da97fbabf10_w200.gif' height="20" width="100%">

## Ejercicio 13

<img src= 'https://i.gifer.com/origin/8c/8cd3f1898255c045143e1da97fbabf10_w200.gif' height="20" width="100%">

## Ejercicio 14

<img src= 'https://i.gifer.com/origin/8c/8cd3f1898255c045143e1da97fbabf10_w200.gif' height="20" width="100%">

## Ejercicio 15

<img src= 'https://i.gifer.com/origin/8c/8cd3f1898255c045143e1da97fbabf10_w200.gif' height="20" width="100%">

## Ejercicio 16

<img src= 'https://i.gifer.com/origin/8c/8cd3f1898255c045143e1da97fbabf10_w200.gif' height="20" width="100%">

## Ejercicio 17

<img src= 'https://i.gifer.com/origin/8c/8cd3f1898255c045143e1da97fbabf10_w200.gif' height="20" width="100%">
