<div align="center">

[![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/Nomadiix/IS1)
[![GitHub stars](https://img.shields.io/github/stars/Nomadiix/IS1)](https://github.com/FabianMartinez1234567/IS1/stargazers/)
[![GitHub repo size in bytes](https://img.shields.io/github/repo-size/Nomadiix/IS1)](https://github.com/Nomadiix/IS1)
 </div>
<h1 align="center"> 📋 Teoria 2da AE</h1>
<div align='center'>

[Practica 1 | Teoria](/Documentos/Practica1.md)<br>
[Practica 2 | Historias de Usuario](/Documentos/Practica2.md)<br>
[Practica 3 | Casos de Uso](/Documentos/Practica3.md)<br>
[Practica 4 | DTE](/Documentos/Practica4.md)<br>
[Practica 5 | Redes de Petri](/Documentos/Practica5.md)<br>
[Practica 6 | Tablas de Desición](/Documentos/Practica6.md)
</div>

<img src= 'https://i.gifer.com/origin/8c/8cd3f1898255c045143e1da97fbabf10_w200.gif' height="20" width="100%">

- [Qué es un proceso de software?](#qué-es-un-proceso-de-software)
- [Qué es un modelo de proceso de Software?](#qué-es-un-modelo-de-proceso-de-software)
- [Cuáles son los atributos de un buen software?](#cuáles-son-los-atributos-de-un-buen-software)
- [Requerimientos](#requerimientos)
  - [Funcionales](#requerimientos-funcionales)
  - [No Funcionales](#requerimientos-no-funcionales)
- [Ingeniería de Requerimientos](#ingeniería-de-requerimientos)
  - [Estudio de Viabilidad](#estudio-de-viabilidad)
  - [Obtención y Análisis de Requerimientos](#obtención-y-análisis-de-requerimientos)
  - [Especificación de Requerimientos](#especificación-de-requerimientos)
  - [Validación de Requerimientos](#validación-de-requerimientos)
- [Técnicas de especificación de Requerimientos](#técnicas-de-especificación-de-requerimientos)
  - [Estaticas](#estáticas)
    - [Referencia indirecta](#referencia-indirecta-ecuaciones-implícitas)
    - [Relaciones de recurrencia](#relaciones-de-recurrencia)
    - [Definición axiomática](#definición-axiomática)
    - [Expresiones regulares](#expresiones-regulares)
    - [Abstracciones de datos](#abstracciones-de-datos)
  - [Dinamicas](#dinámicas)
    - [Tablas de Desición](#tablas-de-decisión)
    - [Historias de Usuario]()
    - [Casos de Uso]()
    - [Maquinas de Estado Finito]()
    - [Diagramas de Transición y Estado (DTE)]()
    - [Redes de Petri]()


<img src= 'https://i.gifer.com/origin/8c/8cd3f1898255c045143e1da97fbabf10_w200.gif' height="20" width="100%">

## Qué es un proceso de software?

Es un conjunto de actividades y resultados asociados que producen un producto de software

Actividades fundamentales de los procesos
- Especificación del software
- Desarrollo del software
- Validación del software
- Evolución del software

Los IS son los responsables de realizar estas actividades

---

### Qué es un modelo de proceso de software

Es una descripción simplificada de un proceso de software que presenta una visión de ese proceso. Estos modelos pueden incluir actividades que son partes de los procesos y productos de software, y el papel de las personas involucradas.

La mayoría de los modelos de proceso de software se basan en uno de los siguientes modelos generales o paradigmas
- **Modelo en cascada**: Representa las actividades anteriores y las representa como fases de proceso separadas.
- Especificación de requerimientos, diseño, implantación, etc.
- **Desarrollo iterativo**: Un sistema inicial se desarrolla rápidamente a partir de una especificación abstracta. Éste se refina basándose en las peticiones del cliente.
- **IS basada en componentes**: Esta técnica supone que las partes ya existen. El proceso se enfoca en la integración de las partes.

---

### Cuáles son los atributos de un buen software?


Los productos de software tiene un cierto número de atributos asociados que
reflejan su calidad. Estos atributos reflejan su comportamiento durante su ejecución y la estructura y organización de los programas fuentes en la documentación asociada

Los atributos básicos son
- **Mantenibilidad** Posibilidad de modificaciones ante los cambios del negocio
- **Confiabilidad** Fiabilidad, seguridad, no debe causar daños físico o económicos ante fallas
- **Eficiencia** Hacer un uso apropiado de los recursos
- **Usabilidad** Fácil de usar sin esfuerzo adicional

---

## Requerimientos

Un requerimiento (o requisito) es una característica del sistema o una descripción de algo que el sistema es capaz de hacer con el objeto de satisfacer el propósito del sistema

Impacto de los errores en la etapa de requerimientos

El software resultante puede no satisfacer a los usuarios. Las interpretaciones múltiples de los requerimientos pueden causar desacuerdos entre clientes y desarrolladores. Puede gastarse tiempo y dinero construyendo el sistema erróneo

- **0.1** Requerimientos 
- **0.5** Diseño 
- **1.0** Codificación 
- **2.0** Pruebas de Unidad
- **5.0** Pruebas ded Aceptación
- **20.0** Mantenimiento

---

### Tipos de Requerimientos
#### Requerimientos Funcionales

- Describen una interacción entre el sistema y su ambiente. Cómo debe comportarse el sistema ante determinado estímulo.
- Describen lo que el sistema debe hacer, o incluso cómo NO debe comportarse.
- Describen con detalle la funcionalidad del mismo.
- Son independientes de la implementación de la solución.
- Se pueden expresar de distintas formas

#### Requerimientos no funcionales

Describen una restricción sobre el sistema que limita nuestras elecciones en la construcción de una solución al problema
- **Del Producto** Especifican el comportamiento del producto (usabilidad, eficiencia, rendimiento, espacio, fiabilidad, portabilidad).
- **Organizacionales** Se derivan de las políticas y procedimientos existentes en la organización del cliente y en la del desarrollador (entrega, implementación, estándares).
- **Externos** Interoperabilidad, legales, privacidad, seguridad, éticos
- **Del dominio** Reflejan las características y restricciones del dominio de la aplicación del sistema. Pueden ser funcionales o no funcionales y pueden restringir a los anteriores. Como se especializan en el dominio son complicados de interpretar.
- **Por Prioridad**
  - Que deben ser absolutamente satisfechos
  - Que son deseables pero no indispensables
  - Que son posibles, pero que podrían eliminarse
- **Del Usuario**
  - Son declaraciones en lenguaje natural y en diagramas de los servicios que se espera que el sistema provea y de las restricciones bajo las cuales debe operar.
  - Pueden surgir problemas por falta de claridad, confusión de requerimientos, conjunción de requerimientos.
  - **Del Sistema**
    - Establecen con detalle los servicios y restricciones del sistema.
    - Es difícil excluir toda la información de diseño (arquitectura inicial, interoperabilidad con sistemas existentes, etc.)

---

## Ingeniería de Requerimientos

La ingeniería de requerimientos es la disciplina para desarrollar una especificación completa, consistente y no ambigua, la cual servirá como base para acuerdos comunes entre todas las partes involucradas y en donde se describen las funciones que realizará el sistema


> **Ingeniería de requerimientos** es el proceso por el cual se transforman los requerimientos declarados por los clientes, ya sean hablados o escritos, a especificaciones precisas, no ambiguas, consistentes y completas del comportamiento del sistema, incluyendo funciones, interfaces, rendimiento y limitaciones

También es el proceso mediante el cual se intercambian diferentes puntos de vista para recopilar y modelar lo que el sistema va a realizar. Este proceso utiliza una combinación de métodos, herramientas y actores, cuyo producto es un modelo del cual se genera un documento de requerimientos.”

“Ingeniería de requerimientos” es un enfoque sistémico para recolectar, organizar y documentar los requerimientos del sistema; es también el proceso que establece y mantiene acuerdos sobre los cambios de requerimientos, entre los clientes y el equipo del proyecto”

Importancia
- Permite gestionar las necesidades del proyecto en forma estructurada
- Mejora la capacidad de predecir cronogramas de proyectos
- Disminuye los costos y retrasos del proyecto
- Mejora la calidad del software
- Mejora la comunicación entre equipos
- Evita rechazos de usuarios finales.

---

### Estudio de Viabilidad

Principalmente para sistemas nuevos

A partir de una descripción resumida del sistema se elabora un informe que recomienda la conveniencia o no de realizar el proceso de desarrollo

Responde a las siguientes preguntas:
- ¿El sistema contribuye a los objetivos generales de la organización?( Si no contribuye, entonces no tiene un valor real en el negocio )
- ¿El sistema se puede implementar con la tecnología actual?
- ¿El sistema se puede implementar con las restricciones de costo y tiempo?
- ¿El sistema puede integrarse a otros que existen en la organización?

Una vez que se ha recopilado toda la información necesaria para contestar las preguntas anteriores se debería hablar con las fuentes de información para responder nuevas preguntas y luego se redacta el informe, donde debería hacerse una recomendación sobre si debe continuar o no el desarrollo.

---

### Obtención y Análisis de Requerimientos

Propiedades de los Requerimientos
- **Necesario**: Su omisión provoca una deficiencia.
- **Conciso**: Fácil de leer y entender
- **Completo**: No necesita ampliarse
- **Consistente**: No contradictorio con otro
- **No ambiguo**: Tiene una sola implementación
- **Verificable**: Puede testearse a través de inspecciones, pruebas, etc.

---

### Especificación de Requerimientos

Objetivos
- Permitir que los desarrolladores expliquen cómo han entendido lo que el cliente pretende del sistema
- Indicar a los diseñadores qué funcionalidad y características va a tener el sistema resultante
- Indicar al equipo de pruebas qué demostraciones llevar a cabo para convencer al cliente de que el sistema que se le entrega es lo que había pedido.

Mas caracteristicas

- Rastreable
- Independiente del diseño
- Anotada
- Concisa
- Organizada
- Utilizable en operación y mantenimiento
- Correcta
- No ambigua
- Completa
- Verificable
- Consistente
- Comprensible por los consumidores
- Modificable

Tipos de Documentos

- **`Documento de definición de requerimientos`** Listado completo de todas las cosas que el cliente espera que haga el sistema propuesto
- **`Documento de especificación de requerimientos`** Definición en términos técnicos
- **`Documento de especificación de requerimientos de Software IEEE Std. 830-1998 (SRS)`**
  - **Objetivo** Brindar una colección de buenas prácticas para escribir especificaciones de requerimientos de software (SRS). Se describen los contenidos y las cualidades de una buena especificación de requerimientos.

Aspectos básicos de una especificación de requerimientos

- **`Funcionalidad`** ¿Qué debe hacer el software?
- **`Interfaces Externas`** ¿Cómo interactuará el software con el medio externo (gente, hardware, otro software)?
- **`Rendimiento`** Velocidad, disponibilidad, tiempo de respuesta, etc.
- **`Atributos`** Portabilidad, seguridad, mantenibilidad, eficiencia
- **`Restricciones de Diseño`** Estándares requeridos, lenguaje, límite de recursos, etc.

---

### Validación de Requerimientos

Es el proceso de certificar la corrección del modelo de requerimientos contra las intenciones del usuario.

Trata de mostrar que los requerimientos definidos son los que estipula el sistema. Se describe el ambiente en el que debe operar el sistema.

Es importante, porque los errores en los requerimientos pueden conducir a grandes costos si se descubren más tarde

Definición de la IEEE
- **`Validación`** Al final del desarrollo evaluar el software para asegurar que el software cumple los requerimientos
- **`Verificación`** Determinar si un producto de software de una fase cumple los requerimientos de la fase anterior

Sobre estas definiciones:
- la validación sólo se puede hacer con la activa participación del usuario
- **`Validación`** hacer el software correcto
- **`Verificación`** hacer el software correctamente

¿Es suficiente validar después del desarrollo del software?
- La evidencia estadística dice que NO
- Cuanto más tarde se detecta, más cuesta corregir (Boehm)
- Bola de nieve de defectos
- Validar en la fase de especificación de requerimientos puede ayudar a evitar costosas correcciones después del desarrollo

¿Contra qué se verifican los requerimientos?
- No existen **los requerimientos de los requerimientos**
- No puede probarse formalmente que un Modelo de Requerimientos es correcto. Puede alcanzarse una convicción de que la solución especificada en el modelo de requerimientos es el correcto para el usuario.

Comprenden
- Verificaciones de validez (para todos los usuarios)
- Verificaciones de consistencia (sin contradicciones)
- Verificaciones de completitud (todos los requerimientos)
- Verificaciones de realismo (se pueden implementar)
- Verificabilidad (se puede diseñar conjunto de pruebas)

Técnicas de validación
- Pueden ser manuales o automatizadas
- Revisiones de requerimientos (formales o informales)
  - **`Informales`** Los desarrolladores deben tratar los requerimientos con tantos stakeholders como sea posible.
  - **`Formal`** El equipo de desarrollo debe conducir al cliente, explicándole las implicaciones de cada requerimiento
- Antes de una revisión formal, es conveniente realizar una revisión informal.

Construcción de prototipos

Generación de casos de prueba

---

# Técnicas de Especificación de Requerimientos

## Estáticas
Se describe el sistema a través de las entidades u objetos, sus atributos y sus relaciones con otros. No describe como las relaciones cambian con el tiempo.

Cuando el tiempo no es un factor mayor en la operación del sistema, es una descripción útil y adecuada.
  - Referencia indirecta
  - Relaciones de recurrencia
  - Definición axiomática
  - Expresiones regulares
  - Abstracciones de datos
  - Otras…

---

### Referencia indirecta (ecuaciones implícitas)

- Descripción del sistema con una referencia indirecta al problema y su solución.
- Se define **`QUÉ`** se hace, no **`CÓMO`**.
- Ejemplo: sistema que resuelva `k` ecuaciones con `n` incógnitas => NO se declara el método de resolución, puede NO existir la solución.

---

### Relaciones de recurrencia

- Descripción del sistema mediante una función que define su valor en función de términos anteriores.
- Ejemplo: Expresar la serie de Fibonacci
- F(0) = 1
- F(1) = 1
- F(n+1) = F(n) + F(n-1)

---

### Definición axiomática
- Se definen las propiedades básica de un sistema a través de operadores y axiomas (debe ser un conjunto completo y consistente)
- Se generan teoremas a través del comportamiento del sistema y se demuestran
- Ejemplos: Sistemas expertos, Definición de TADs, etc.

---

### Expresiones regulares

Se define un alfabeto y las combinaciones permitidas. Cuando un sistema procesa un conjunto de cadenas de datos, permite definir las cadenas de datos aceptables

Alfabeto
- ÁTOMOS: (símbolos básicos) a,b,c.
- ALTERNACIÓN: (a|b) = {a,b}
- COMPOSICIÓN: (ab) = {ab}
- ITERACIÓN: (a)*={e,a,aa..} (a)+= {a,aa,...}

Se definen las combinaciones válidas
- (a(b|c)) = {ab,ac}
- (a(b|c))+ = {ab,ac,abac,acab...}

---

### Abstracciones de datos

- Para aquellos sistemas en los que los datos determinan las clases de acciones que se realizan (importa para qué son).
- Se categorizan los datos y se agrupan los semejantes.
- El diccionario contiene los TIPOS DE DATOS (clases) y los DATOS (objetos).
- Se organizan de tal manera de aprovechar las características compartidas.

---

## Dinámicas

- Se considera un sistema en función de los cambios que ocurren a lo largo del tiempo.
- Se considera que el sistema está en un estado particular hasta que un estímulo lo obliga a cambiar su estado.
  - Tablas de decisión
  - Diagramas de transición de estados
  - Tablas de transición de estados
  - Diagramas de persianas
  - Diagramas de transición extendidos
  - Redes de Petri
  - Casos de Uso
  - Historias de Usuario
  - DFD/DFC
  - Otras…

---

## Tablas de Decisión

Es una herramienta que permite presentar de forma concisa las reglas lógicas que hay que utilizar para decidir acciones a ejecutar en función de las condiciones y la lógica de decisión de un problema específico

Describe el sistema como un conjunto de:

- Posibles **`CONDICIONES`** satisfechas por el sistema en un momento dado
- **`REGLAS`** para reaccionar ante los estímulos que ocurren cuando se reúnen determinados conjuntos de condiciones y
- **`ACCIONES`** a ser tomadas como un resultado.

Construiremos las tablas con:
- condiciones simples y acciones simples
- Las condiciones toman sólo valores Verdadero o Falso
- Hay **`2N`** Reglas donde N es la cantidad de condiciones

![](2023-05-09-13-06-12.png)

¿Cómo se llena la tabla?
- A partir de un enunciado se debe:
- Identificar las condiciones y las acciones.
- Completar la tabla teniendo en cuenta:
  - Si hay condiciones que son opuestas, debe colocarse una de ellas porque por la negativa se “obtendrá” la otra. (Si son n condiciones excluyentes, colocar n-1 en la tabla).
  - Las condiciones deben ser atómicas.
- Se construyen las reglas

Modelizar el problema de remisión de mercadería con las siguientes consideraciones

> Si el comprador no es cliente se imprime un mensaje de aviso y no se remite.
> Si no hay stock y el comprador es cliente no se remite.
> Si hay stock y el comprador es cliente se remite

Identificar las condiciones y las acciones

- Especificaciones completas
- Aquellas que determinan acciones (una o varias) para todas las reglas posibles.
- Especificaciones redundantes
- Aquellas que marcan para reglas que determinan las mismas condiciones acciones iguales.
- Especificaciones contradictorias
- Aquellas que especifican para reglas que determinan las mismas condiciones acciones
distintas

![](2023-05-10-13-05-19.png)

Redundancia y Contradicción

![](2023-05-10-13-06-35.png)

Reducción de Complejidad (Redundancia)
- Combine las reglas en donde sea evidente que una alternativa no representa una diferencia en el resultado.
- El guión [—] significa que la condición 2 puede ser S o N, y que aún así se realizará la acción.

![](2023-05-10-13-08-14.png)

![](2023-05-10-13-08-53.png)

## Historias de Usuario

- Una historia de usuario es una representación de un requisito de software escrito en una o dos frases utilizando el lenguaje común del usuario.
- Son utilizadas en las metodologías de desarrollo ágiles para la especificación de requisitos
- Acompañadas de las discusiones con los usuarios y las pruebas de validación
- Debe ser limitada, esta debería poderse escribir sobre una nota adhesiva pequeña.
- Son una forma rápida de administrar los requisitos de los usuarios sin tener que elaborar gran cantidad de documentos formales y sin requerir de mucho tiempo para administrarlos.
- Permiten responder rápidamente a los requisitos cambiantes

Generalmente se espera que la estimación de tiempo de cada historia de usuario se sitúe entre unas 10 horas y un par de semanas
- Estimaciones mayores a dos semanas son indicativo de que la historia es muy compleja y debe ser dividida en varias historias.

Al momento de implementar las historias, los desarrolladores deben tener la posibilidad de discutirlas con los clientes.
Si bien el estilo puede ser libre, la historia de usuario debe responder a tres preguntas: 
- **¿Quién se beneficia?** El Rol
- **¿qué se quiere?** La Historia
- **¿cuál es el beneficio?** Esto es parte del cliente

Ejemplos

- Como (rol) quiero (algo) para poder (beneficio).
- Como usuario registrado deseo loguearme para poder poder empezar a utilizar la aplicación.

### Características
- **`Independientes unas de otras`** De ser necesario, combinar las historias dependientes o buscar otra forma de dividir las historias de manera que resulten independientes.
- **`Negociables`** La historia en si misma no es lo suficientemente explícita como para considerarse un contrato, la discusión con los usuarios debe permitir esclarecer su alcance y éste debe dejarse explícito bajo la forma de pruebas de validación.
- **`Valoradas por los clientes o usuarios`** Los intereses de los clientes y de los usuarios no siempre coinciden, pero en todo caso, cada historia debe ser importante para alguno de ellos más que para el desarrollador.
▪ **`Estimables`** Un resultado de la discusión de una historia de usuario es la estimación del tiempo que tomará completarla. Esto permite estimar el tiempo total del proyecto.
- **`Pequeñas`** Las historias muy largas son difíciles de estimar e imponen restricciones sobre la planificación de un desarrollo iterativo. Generalmente se recomienda la consolidación de historias muy cortas en una sola historia.
- **`Verificables`** Las historias de usuario cubren requerimientos funcionales, por lo que generalmente son verificables. Cuando sea posible, la verificación debe automatizarse, de manera que pueda ser verificada en cada entrega del proyecto.

