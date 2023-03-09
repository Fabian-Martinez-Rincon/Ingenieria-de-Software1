<div align="center">

[![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/Nomadiix/IS1)
[![GitHub stars](https://img.shields.io/github/stars/Nomadiix/IS1)](https://github.com/FabianMartinez1234567/IS1/stargazers/)
[![GitHub repo size in bytes](https://img.shields.io/github/repo-size/Nomadiix/IS1)](https://github.com/Nomadiix/IS1)
 </div>
 
<h1 align="center"> 🕸️ Practica 5</h1>
<div align="center">
<img src="https://media.giphy.com/media/XG0tayFvL5MoSJ4OVw/giphy.gif"/>
</div>

<img src= 'https://i.gifer.com/origin/8c/8cd3f1898255c045143e1da97fbabf10_w200.gif' height="20" width="100%">

<div align='center'>

[Practica 1 | Teoria](/Documentos/Practica1.md)<br>
[Practica 2 | Historias de Usuario](/Documentos/Practica2.md)<br>
[Practica 3 | Casos de Uso](/Documentos/Practica3.md)<br>
[Practica 4 | DTE](/Documentos/Practica4.md)<br>
[Practica 5 | Redes de Petri](/Documentos/Practica5.md)<br>
[Practica 6 | Tablas de Desición](/Documentos/Practica6.md)
</div>

<img src= 'https://i.gifer.com/origin/8c/8cd3f1898255c045143e1da97fbabf10_w200.gif' height="20" width="100%">

- [Ejercicio 1 Fabrica de papas](#ejercicio-1-fabrica-de-papas)
- [Ejercicio 2 Fabrica de vinos](#ejercicio-2-fabrica-de-vinos)
- [Ejercicio 3 Peluquería](#ejercicio-3-peluquería)
- [Ejercicio 4 Estación de servicio](#ejercicio-4-estación-de-servicio)
- [Ejercicio 5 Voto electrónico](#ejercicio-5-voto-electrónico)
- [Ejercicio 6 Puente](#ejercicio-6-puente)
- [Ejercicio 7 Puesto de trabajo](#ejercicio-7-puesto-de-trabajo)
- [Ejercicio 8 Alfajores](#ejercicio-8-alfajores)
- [Ejercicio 9 Mobiliaria](#ejercicio-9-mobiliaria)
- [Ejercicio 10 Juego en la escuela](#ejercicio-10-juego-en-la-escuela)
- [Ejercicio 11 Fábrica de pastas](#ejercicio-11-fábrica-de-pastas)
- [Ejercicio 12 Recital](#ejercicio-12-recital)
- [Ejercicio 13 Aserradero](#ejercicio-13-aserradero)
- [Ejercicio 14 Legalización de documentos](#ejercicio-14-legalización-de-documentos)
- [Ejercicio 15 VTV](#ejercicio-15-vtv)

<img src= 'https://i.gifer.com/origin/8c/8cd3f1898255c045143e1da97fbabf10_w200.gif' height="20" width="100%">

## Ejercicio 1 Fabrica de papas

Se desea modelar con Redes de Petri el funcionamiento de una fábrica de papas bastón crudas.

Las papas llegan de a una y se depositan en un contenedor común. El primer paso es pasar la papa por una máquina que
quita la cáscara. Esta máquina solo puede atender de a una papa a la vez. Las papas peladas son depositadas en un
contenedor común a la espera de la próxima etapa. La cáscara por su parte, es depositada en un basurero general.

Luego, cada papa cruda debe ser cortada. Para esto, la papa pasa por una máquina que corta las papas en 9 bastones.
Esta máquina solo puede procesar una papa a la vez. Una vez cortados, los bastones de papas son agrupados de a 10
para ser envasados. Esto lo realiza una máquina que solo procesa una bolsa por vez. Por último, las bolsas son
depositadas en un contenedor común para ser distribuidas.

<img src= 'https://i.gifer.com/origin/8c/8cd3f1898255c045143e1da97fbabf10_w200.gif' height="20" width="100%">

## Ejercicio 2 Fabrica de vinos

Modelar con una Red de Petri el funcionamiento del sector de empaquetado de una fábrica de vinos.

Los vinos llegan por dos canales distintos (vino blanco y vino tinto) y son depositados en un contenedor distinto para
cada tipo de vino. Luego, debe haber 3 vinos de cada tipo para poder armar una caja. La caja puede armarse por
cualquiera de los dos operarios disponibles, quienes trabajan de forma separada y solo pueden armar una caja a la vez.
Una vez finalizado el empaquetado la caja es enviada al depósito para ser despachadas

<img src= 'https://i.gifer.com/origin/8c/8cd3f1898255c045143e1da97fbabf10_w200.gif' height="20" width="100%">

## Ejercicio 3 Peluquería

Dos peluqueros trabajan en una peluquería. La peluquería cuenta con una sala de espera con sólo 3 sillas para que los
clientes esperen por ser atendidos. Cuando alguno de los peluqueros se libera atiende a uno de los clientes de cualquiera
de las sillas para cortarle el cabello, liberando la silla de la sala de espera, para que se siente un nuevo cliente. Una vez
que terminó de cortarle el cabello el peluquero es liberado y puede atender a otro cliente. Finalmente los clientes deben pasar por la caja en la cual se atiende a un cliente por vez. Cuando llegan clientes y las tres sillas están ocupadas deben
formar una única fila en la puerta de la peluquería

<img src= 'https://i.gifer.com/origin/8c/8cd3f1898255c045143e1da97fbabf10_w200.gif' height="20" width="100%">

## Ejercicio 4 Estación de servicio

Una estación de servicio cuenta con tres surtidores con sus respectivos empleados (uno por surtidor) y dos cobradores (los empleados de los surtidores no pueden cobrar).

Cuando los autos llegan, forman fila en cualquiera de los surtidores. Una vez que se terminó de cargar combustible al
auto, se libera el surtidor y se pasa al sector de pago. En este sector cualquiera de los cobradores le cobra al conductor
del auto. Si no hay cobradores libres, debe esperar a que uno se libere. Cuando el cobrador termina, el auto se retira de
la estación y el cobrador queda libre para atender a un nuevo auto.

<img src= 'https://i.gifer.com/origin/8c/8cd3f1898255c045143e1da97fbabf10_w200.gif' height="20" width="100%">

## Ejercicio 5 Voto electrónico

Modelar una elección mediante voto electrónico, para ello se disponen de dos mesas y dos terminales de voto (una para cada mesa). A medida que los votantes llegan, forman una única fila y luego son derivados indistintamente a la mesa 1 o a la mesa 2. En cada mesa hay una autoridad para atender y tomar los datos del votante. Cada mesa atiende de a un votante a la vez. Una vez que la autoridad le tomó los datos, el votante pasa a votar a la terminal electrónica de la mesa correspondiente. Una vez que el votante emitió su voto, debe pasar a firmar que efectivamente votó, en ese mismo instante puede ingresar otra persona a la mesa. Luego, el votante que estaba firmando se retira

<img src= 'https://i.gifer.com/origin/8c/8cd3f1898255c045143e1da97fbabf10_w200.gif' height="20" width="100%">

## Ejercicio 6 Puente

- a) Modelar el pasaje de vehículos a través de un puente el cual posee una sola mano por donde pasan los vehículos. El máximo permitido es de 3 vehículos por vez.
- b) Agregar al modelo anterior una segunda mano. Los vehículos pueden ingresar al puente por cualquiera de las dos manos y en cada puede haber un máximo de 3 vehículos a la vez.
- c) Agregar al modelo anterior la restricción de que sólo puede haber 4 vehículos en total sobre el puente

<img src= 'https://i.gifer.com/origin/8c/8cd3f1898255c045143e1da97fbabf10_w200.gif' height="20" width="100%">

## Ejercicio 7 Puesto de trabajo

Un puesto de trabajo recibe pedidos de dos líneas de montaje distintas. El puesto procesa los pedidos y los deriva indistintamente por uno de sus dos canales. Se procesa/deriva de a un pedido por vez.

Si el pedido es enviado a través del canal 1, se lo deposita en una cinta transportadora que lo conduce al sector de pedidos anulados, en donde un empleado les coloca el sello de anulado, se sabe que el empleado puede sellar de un pedido por vez. Una vez sellado se lo envía a un depósito de pedidos descartados, donde finalmente son retirados del puesto de trabajo.

Si el pedido es enviado a través del canal 2, se lo deposita en un contenedor que tiene una capacidad máxima de 4 pedidos. Cuando el contenedor está lleno se envían los 4 pedidos al sector de logística, donde serán finalmente despachados simultáneamente.

<img src= 'https://i.gifer.com/origin/8c/8cd3f1898255c045143e1da97fbabf10_w200.gif' height="20" width="100%">

## Ejercicio 8 Alfajores

Se desea modelar utilizando una Red de Petri el funcionamiento de una fábrica artesanal de alfajores. Esta cuenta con 3 líneas de producción, que recibe pedidos independientes, para producir alfajores con diferentes rellenos y coberturas (dulce de leche con chocolate, dulce de leche con merengue y fruta con merengue).

Cada línea de fabricación tiene un empleado que arma de a un alfajor por vez. Luego, el alfajor queda a la espera para su posterior embalaje. Una vez terminados los alfajores, deben empaquetarse en una caja de 6 unidades, con 2 alfajores decada sabor, ya que la fábrica vende únicamente este tipo de formato.

Finalmente se envía la caja al sector de almacenamiento

<img src= 'https://i.gifer.com/origin/8c/8cd3f1898255c045143e1da97fbabf10_w200.gif' height="20" width="100%">

## Ejercicio 9 Mobiliaria

Una distribuidora mobiliaria de la ciudad recibe pedidos de muebles desarmados y empaquetados, los cuales deben ser armados y ensamblados para su posterior envío y entrega a domicilio.

Los pedidos ingresan a la distribuidora por una línea única de montaje y luego son derivados al puesto A o al puesto Bque posee dicha distribuidora. Allí los pedidos son analizados. Cada puesto atiende un pedido por vez. 

Luego, los pedidos pasan al depósito del sector de ensamblado para su armado y embalaje. Se sabe que en este sector hay un conjunto de empleados que trabajan juntos y van tomando los pedidos del depósito y pueden, como máximo, armar y embalar 3 pedidos simultáneamente. Una vez que el pedido está listo se lo pasa al sector de envíos en donde se esperan 5 pedidos para armar un lote que será cargado en el camión de reparto para su posterior entrega.

<img src= 'https://i.gifer.com/origin/8c/8cd3f1898255c045143e1da97fbabf10_w200.gif' height="20" width="100%">

## Ejercicio 10 Juego en la escuela

Modelar un juego en donde participan los alumnos/as de una escuela. Para comenzar el juego, se realizan dos filas pertenecientes a dos equipos, el equipo A por un lado y el equipo B por otro. Para el inicio del juego se necesitan de 6 alumnos/as, 3 del equipo A y 3 del equipo B. Una vez finalizado el juego, participan los siguientes 6 alumnos y así sucesivamente

<img src= 'https://i.gifer.com/origin/8c/8cd3f1898255c045143e1da97fbabf10_w200.gif' height="20" width="100%">

## Ejercicio 11 Fábrica de pastas

Se desea modelar mediante una red de Petri el funcionamiento de una fábrica de pastas. La fábrica cuenta con dos líneas de producción independientes, en una se realizan canelones y en la otra se realizan sorrentinos. Por cada una de las líneas llegan porciones de masa. Existen 3 empleados que se encargan de estirar las masas y pueden trabajar en cualquiera de las dos líneas.

Una vez estiradas las masas pasan a los sectores de corte respectivos. En el caso de los canelones, de una masa se obtienen 3 canelones. En el caso de los sorrentinos, de una masa se obtienen 6 sorrentinos. En cada sector se corta de a una masa por vez.

Luego de cortadas las masas cada unidad obtenida en el corte pasa al sector de relleno. En cada sector hay una máquina que realiza esta tarea. La máquina de sorrentinos rellena tres sorrentinos al mismo tiempo, mientras que la máquina de canelones solo rellena de a uno. Finalizado el relleno, las pastas ya están listas para ser guardarlas en cajas. En el caso de los sorrentinos se arman cajas de 6 sorrentinos y en el caso de los canelones las cajas contienen 3 unidades. Una vez armadas las cajas se despachan

<img src= 'https://i.gifer.com/origin/8c/8cd3f1898255c045143e1da97fbabf10_w200.gif' height="20" width="100%">

## Ejercicio 12 Recital

Se desea modelar utilizando una Red de Petri el ingreso de personas a un recital. Las personas pueden llegar desde doscalles diferentes. En cada calle hay cuatro inspectores quienes realizan revisiones. Cada revisión la realizan dos inspectores al mismo tiempo, y sólo pueden revisar de a una persona a la vez. Una vez que las personas son revisadas pueden ingresar al recital por cualquiera de las tres puertas (existe una única cola para las tres puertas). En cada puerta hay un detector de metales por el cual puede pasar de a una persona por vez. Por último, las personas se ubican en alguno de los dos sectores disponibles para el recital

<img src= 'https://i.gifer.com/origin/8c/8cd3f1898255c045143e1da97fbabf10_w200.gif' height="20" width="100%">

## Ejercicio 13 Aserradero

Se desea modelar con una Red de Petri el funcionamiento de un aserradero. Al lugar llegan troncos de árboles en bruto
por dos puertas distintas. Cada tronco debe ser primero inspeccionado individualmente. Esta tarea la realiza un inspector
especializado, habiendo un inspector por puerta.

Luego, los troncos pasan al único sector de corte del aserradero. En este sector se cortan los troncos de a uno. Por cada tronco se generan cuatro tablones y cuatro desperdicios (sobrantes que no se usan). Los desperdicios van a parar a un contenedor para luego ser desechados.

Cada tablón debe pasar a alguno de los dos sectores de cepillado del aserradero, donde se cepilla de a un tablón por vez. Luego, pasan al sector de empaquetado donde se agrupan de a 6 tablones, para luego ser despachados

<img src= 'https://i.gifer.com/origin/8c/8cd3f1898255c045143e1da97fbabf10_w200.gif' height="20" width="100%">

## Ejercicio 14 Legalización de documentos

Se desea modelar el funcionamiento de un proceso de legalización de documentos.

Los documentos llegan de a uno a la oficina y deben ser triplicados en una de las dos fotocopiadoras existentes. Una vez elegida la fotocopiadora, se solicita al encargado de esa fotocopiadora, las tres copias del documento. La fotocopiadora sólo imprime de a una copia por vez. Hasta no terminar las 3 copias, el empleado no puede recibir nuevos documentos. Al terminar las tres copias de un documento, deben empaquetarse juntas para ser derivadas al sector de asuntos legales. En ese momento, se libera el encargado de la fotocopiadora para recibir nuevos documentos.

<img src= 'https://i.gifer.com/origin/8c/8cd3f1898255c045143e1da97fbabf10_w200.gif' height="20" width="100%">

## Ejercicio 15 VTV

Dado el siguiente enunciado y la solución propuesta:

Identifique cual es la solución correcta. Para aquellas soluciones que crea incorrectas, explique cuáles son los errores que hacen a dicha solución errónea.

Se desea modelar la atención de vehículos en un centro gratuito para realizar la verificación técnica vehicular (vtv).

Los vehículos llegan al centro de verificación e ingresan por cualquiera de los tres accesos disponibles y aguardan en su fila correspondiente para ser atendidos. En cada uno de estos accesos existe una cabina con un solo empleado en donde se solicita la documentación de la persona y del vehículo a verificar. Se atiende de a uno a la vez.

Una vez presentada la documentación, los vehículos pasan a un sector común, formando una única fila, en donde aguardan a ser evaluados.

Un detalle importante es que en el sector común hay capacidad para que esperen solamente 8 vehículos. En caso de que se complete dicho sector se deberá detener la atención en las tres cabinas de ingreso, hasta que alguno de los 8 vehículos inicie su evaluación.

Para ser evaluados, el centro de verificación posee dos puestos distintos de evaluación donde los vehículos van pasando de a uno y son testeados. Para cada puesto se requieren dos empleados que van realizando las anotaciones necesarias del test del vehículo. Un vehículo puede pasar indistintamente por cualquiera de ambos puestos. Una vez que el vehículoes evaluado, los empleados del puesto correspondiente le entregan el informe al dueño del vehículo y la documentación correspondiente. Luego los vehículos se retiran del centro de verificación por una única salida.

### **Solución Propuesta 1**

<img src='https://user-images.githubusercontent.com/55964635/223319687-42eaaeb8-42bf-491e-bad1-182c464f2e92.png'>

### **Solución Propuesta 1**

<img src='https://user-images.githubusercontent.com/55964635/223319806-cd8dabda-edca-47cc-ba55-15b012d8860d.png'>

### **Solución Propuesta 1**

<img src='https://user-images.githubusercontent.com/55964635/223319890-1c0da23a-2442-45ef-8aca-64b0396f20d6.png'>

<img src= 'https://i.gifer.com/origin/8c/8cd3f1898255c045143e1da97fbabf10_w200.gif' height="20" width="100%">
