
- [Condiciones](/Documentos/Condiciones.md)
- [Practica 1](/Documentos/Practica1.md)
- [Practica 2](/Documentos/Practica2.md)

**Clase 1 Conceptos de Ingenieria de software**
- [Software](#software)
    - [Naturaleza](#naturaleza)
    - [Que es?](#que-es)
    - [Caracteristicas](#caracteristicas)
    - [Tipos de productos](#tipos-de-productos)
- [Ingenieria de Software](#ingenieria-de-software)
    - [Que es?](#que-es-la-is)
    - [Conocimientos que debe tener un IS](#conocimientos-que-debe-tener-un-is)
- [Tecnicas de Comunicacion](#tecnicas-de-comunicacion)
    - [Introduccion](#introduccion)
    - [Requerimientos](#requerimientos)
    - [StakeHolder](#stakeholder)
    - [Puntos de Vista](#puntos-de-vista)
    - [Elicitacion de Requerimientos](#elicitacion-de-requerimientos)
    - [Recopilacion de informacion]()
        - [Metodos discretos](#metodos-discretos)
        - [Metodos interactivos](#metodos-interactivos)

**Clase 2 Requerimientos**

- [Proceso](#que-es-un-proceso)
- [Modelo de Proceso](#que-es-un-modelo-de-proceso-de-software)
- [Requerimientos](#requerimientos-2)
- [Tipos](#tipos)
- [Ingenieria de Requerimientos](#ingenieria-de-requerimientos)
- [Estudio de Viabilidad](#estudio-de-viabilidad)
- [Especificacion de Requerimientos](#especificacion-de-requerimientos)
- [Validacion de requerimientos](#validacion-de-requerimientos)
- [Tecnicas de Especificacion de Requerimientos](#tecnicas-de-especificacion-de-requerimientos)
- [Historias de usuario](#historias-de-usuario)

**Clase 3 Requerimientos II**

- [Casos de Uso]()


---

# Clase 1 Conceptos de Ingenieria de software

## Naturaleza

- Producto (Y su documentacion asociada)
- Transformador de informacion, factor predominante
- Vehiculo de entrega de Producto
    - Base para control de computos
    - Sistemas operativos
        - Comunicacion
        - Creacion y control de otros programas

## Que es?

Intrucciones (programas de computo), procedimientos, reglas, sdocumentacion y datos asociados que forman parte de las operaciones de un sistema de computación(IEEE)

## Caracteristicas

- Elemento logico
- Se desarrolla, no se fabrica
- No se desgasta

## Tipos de productos
- **Personalizados:** Sistemas requeridos por un cliente en particular
- **Genericosa:** Sistemas aislados producidos por organizaciones desarrolladoras de software y que se venden en un mercado abierto.

```
Cada vez mas sistemas son construidos por un producto generico como base que 
luego es adaptado a los requerimientos del cliente
```

## Clasificacion

- De sistemas
- De aplicacion
- Cientifico y de ingenieria
- Empotrado
- De linea de productos
- Aplicaciones web
- De inteligencia artificial

## Ingenieria de Software

A medida que los usuarios adoptan nuevas tecnologias, parte del trabajo consiste en integrar los sistemas tradicionales con los nuevos para asegurar un contexto util.

Debemos estar concientes de que al integrar tecnologias se ven afectados todos los tipos de usuarios y el sistema

Que hacer? Ingenieria de Software

## Que es la IS? 

Diciplina de la ingenieria que comprende todos los aspectos de la produccion de software desde las etapas iniciales de la especificacion del sistema incluyendo la evolucion de este, luego que se comienza a ejecutar.

- `Diciplina de software:` Se encarga de que nuestros objetivos funcionen. Se aplican teorias, metodos, y herramientas.

- `Aspectos de produccion:` No solo comprende los procesos tecnicos del desarrollo de software, sino tambien se realizan actividades como la gestion de proyectos y el desarrollo de herramientas, metodos y teorias de apoyo a la produccion de software.

La IEEE define a la ingenieria de software como:

- `1)` El uso de metodos sistematicos, diciplinados y cuantificables para el desarrollo, operacion y mantenimiento de software
- `2)` El estudio de tecnicas relacionas con 1

**Usa metodos sistematicos cuantificables**

La cuantificacion rigurosa de recursos, procesos y productos es una precondicion para optimizar productividad y calidad. La "metrificacion" t el control estadistico de procesos son claves en IS.

**Dentro de tiempos y costos estimados**

Un ingeniero de Software debe cumplir contratos en tiempo y costos como es normal en obras de ingenieria. Ello presupone la capacidad de medir, estimar, planificar y administrar proyectos

**Para el "Desarrollo, operacion y mantenimiento"**

La IS se ocupa de todo el ciclo de vida de un producto, desde su etapa inicial de planificacion y analisis de requerimientos hasta la estrategia para determinar cuanto y como debe ser retirado de servicio


## Conocimientos que debe tener un IS

El ingeniero debe conocer:

- **Las tecnologias y productos:**
    - Sistemas operativos, lenguajes, base de datos, sistemas generadores de interfaces, bibliotecas de codigo.
- **Tecnicas de administracion de proyectos:**
    - planificacion, analisis de riesgos, control de calidad, seguimiento de proyectos, control de subcontratistas, etc.

```
En los ultimos anios se observa una especializacion de los ingenieros de 
software por dominio de aplicacion o por actividad
```

**Responsabilidad profesional y etica**

La ingenieria de software se desarrolla en un marco economico, social y legal
- Los IS deben aceptar responsabilidades ,as amplias que las responsabilidades tecnicas.

No debe utilizar su capacidad y habilidades de forma deshonesta, o de forma que deshonre la profesio.

- `Confidencialidad:` Respetar la confidencialidad de sus empleados y clientes.
- `Competencia:` No falsificar el nivel de competencia y aceptar responsabilidades fuera de su capacidad
- `Derechos de la propiedad intelectual:`Conocer las leyes vigentes sobre las patentes y copyright
- `Uso inapropiado de las computadoras:` No debe utilizar sus habilidades tecnicas para utilizar de forma inapropiada otras computadoras


```
Existen diferentes organizaciones como ACM o IEEE que sugieren 
diferentes codigos de etica a respetar
```


## Tecnicas de comunicacion


### Introduccion

- Al iniciar un proyecto cual es la primera actividad?\
Saber lo que el usuario quiere, como lo quierem cuando y porque.

Tenemos que Comunicarnos.

**La comunicacion**

- La comunicacioon es la base para la obtencion de las necesidades del cliente.
- Es la principal fuente de error
- Al hablar de necesidades, en terminos mas tecnicos, estamos hablando de **requerimientos**

## Requerimientos
Es una caracteristica del sisterma o una descripcion de algo que el sistema es capaz de hacer con el objeto de satisfacer el proposito del sistema.

**Definicion IEE-std-610**
- Condicion o capacidad que necesita el usuario para resolver un problema o alcanzar un objetivo.
- Condicion o capacidad que debe satisfacer o poseer un sistema o una componente de un sistema para satisfacer un contrato, un estandar, una especificacion u otro.
- Representacion documentada de una condicion o capacidad como en 1 o 2.


## StakeHolder

El termino **stakeholder** se utiliza para referirse a cualquier persona o grupo que se vera afectado por el sistema, directa o indirectamente.

Entre los stakeholders se encuentran:
- Usuarios finales
- Ingenieros
- Gerentes
- Expertos del dominio
- Diferentes viciones

## Puntos de Vista

Existen tres tipos genericos de puntos de vista:
- De los **interactuadores:** representan a las personas u otros sistemas que interactuan directamente con el sistema. Pueden influir  en los requerimientos del sistema de algun modo.
- **Indirecto:** representan a los stakeholders que no utilizan el sistema ellos mismo pero influyen en los requerimientos de algun modo.
- Del **dominio:** representan las caracteristicas y restricciones del dominio que influyen en los requerimientos del sistema.

Su identificacion puede ser dificil, los mas especificos son:

- Los proveedores de servicios al sistema, los receptores de servicios del sistema.
- Los sistemas que deben interactuar.
- Las regulaciones que deben interactuar.
- Las regulaciones y estandares a aplicar.
- Las fuentes de requerimientos.
- Los puntos de vista de las personas que lo van a desarrollar, administrar y mantener.
- Puntos de vista del marketing y otros que generan requerimientos sobre las caracteristicas del sistema.

## Elicitacion de requerimientos

Es el proceso de adquirir ('eliciting') todo el conocimiento relevante necesario para producir un modelo de los requerimientos de un dominio de problema.

**Objetivos**
- Conocer el dominio del problema para poder comunicarse con clientes y usuarios y entender sus necesidades.
- Conocer el sistema actual (manual o informatizado).
- Identificar las necesidades, tanto explicitas como implicitas, de clientes y usuarios y expectativos sobre el sistema a desarrollar.

La elicitacion de requerimientos es una actividad principalmente de caracter social, mucho mas que tecnologico.

Los problemas que se plantean son por tanto de naturaleza psicologica y social, mas que tecnicos.

Nota: Requerimientos = Requisitos

**Problemas de comunicacion**

- Dificultad para expresar claramente las necesidades
- No ser conscientes de sus propias necesidades
- No entender como la tecnologia puede ayudar
- Miedo a parecer incompetentes por ignorancia tecnologica
- No tomar deciciones por no poder prever las consecuencias, no entender las alternativas o no tener una vision global.
- Cultura y vocabulario diferentes
- Intereses distintos en el sistema a desarrollar
- Medios de comunicacion inadecuados (diagramas que no entienden los clientes y usuarios)
- Conflictos personales o politicos


**Limitaciones cognitivas (del desarrollador)**
- No conocer el dominio del problema
- Hacer suposiciones sobre el dominio del problema.
- Hacer suposiciones sobre aspectos tecnologicos.
- Hacer simplificaciones excesivas.

**Conducta humana**
- Conflictos y ambuguedades en los roles de los participantes
- Pasividad de clientes, usuarios o ingenieros de requisitos.
- Temor a que el nuevo sistema lo deje sin trabajo

**Tecnicos**
- Complejidad del dominio del problema.
- Complejidad de los requisitos
- Multiples fuentes de requerimientos
- Fuerntes de informacion poco claras.


Recopilacion de informacion:

- **Metodos discretos:**
    - Muestreo de la documentacion, los formularios y los datos existentes
    - Investigacion y visitas al lugar
    - Observacion del ambiente de trabajo
- **Metodos interactivos:**
    - Cuestionarios
    - Entrevistas
    - Planeacion conjunta de Requerimientos (JRP o JAD)
    - Lluvia de Ideas

## Metodos discretos

Los metodos discretos son menos perturbadores que otras formas de averiguar los requerimientos

Se considedran insuficientes para recopilar informacion cuando se utilizan por si solos, por lo que deben utilizarse junto con uno o varios de los metodos.

Utilizar diferentes metodos para acercarse a la organizacion es una practica inteligente mediante la cual podra formarse un panorama mas completo sobre los requerimientos

- Muestreo de la documentacion, los formularios y los datos existentes.
- Investigacion y visitas al sitio
- Observacion del ambiente de trabajo

### **Muestreo de la documentacion, los formularios y los datos existentes**

Recoleccion de hechos a partir de la documentacion existentes

Que tipo de documentos pueden enseniar algo acerca del sistema?
- Organigrama (identificar el propietario, usuario claves)
- Memos, notas internas, minutas, registros contables.
- Solicitudes de proyectos de sistema de informacion anteriores

Permiten conocer el historial que origina el proyecto.

**Recoleccuib de hechos a partir de la documentacion existente**

Documenteos que describen la funcionalidad del negocio que esta siendo analizada.
- Declaracion de la mision y plan estrategico de la organizacion
- Objetivos formales del departamento en cuestion
- Politicas, restricciones, procedimientos operativos.
- Base de Datos
- Sistemas en funcionamiento

Documentacion de sistemas anteriores
- Diagramas
- Diccionario o Repositorios de proyecto
- Documentos de dusenio
- Manuales de operacion y/o entrenamiento

**Investigacion y visitas al sitio**
- Investigar el dominio
- Patrones de soluciones (mismo problema en otra organizacion)
- Revistas especializadas
- Buscar problemas similares en internet
- Consultar otras organizaciones

### Observascion del ambiente de trabajo.
- El analista se convierte en observador de las personas y actividades con el objeto de aprender acerca del sistema.
- Lineamientos de la observacion:
    - Determinar quien y cuando sera observado
    - Obtener el permiso de la persona y explicar el porque sera observado.
    - Mantener bajo perfil
    - Tomar nota de lo observado
    - Revisar las notas con la persona apropiada.
    - No interrumpir a la persona en su trabajo

**Ventajas:**
- Datos confiables 
- El analista puede ver exactamente lo que se hace (tareas dificiles de explicar con palabras)
- Analisis de disposiciones fisicas, transito, iluminacion, ruido.
- Economica en comparacion con otras tecnicas

**Desventajas:**
- La gente se siente incomoda siendo observada
- Algunas actividades del sistema pueden ser realizadas en horarios incomodos
- Las tareas estan sujetas a interrupciones
- Tener en cuenta que la persona observada puede estar realizando las tareas de la forma 'correcta' y no como lo hace habitualmente.


## Metodos interactivos

Hay metodos interactivos que pueden usarse para obtener los requerimientos de los miembros de la organizacion aunque son distintos en su implementacion, estos metodos tienen muchas cosas en comun. La base es hablar con las personas en la organizacion y escuchar para comprender.

Cada uno cuenta con su propio proceso establecido

- Cuestionarios
- Entrevistas
- Planeacion conjunta de Requerimientos
- Lluvia de Ideas

### Cuestionarios

Documentacion que permite al analista recabar informacion y opiniones de los encustados
- Recolectar hechos de un gran numero de personas
- Detectar un sentimiento generalizado
- Detectar problemas entre usuarios
- Cuantificar respuestas

**Ventajas**
- Respuesta rapida
- Economicos
- Anonimos
- Estructurados de facil analisis

**Desventajas**
- Numero bajo de respuestas
- No responde a todas las preguntas
- Preguntas rigidas
- No se puede realizar el analisis corporal
- No se pueden aclarar respuestas incompletas

**Tipos de Preguntas**
- **Abiertas:**
    - Son las que dejan abiertas todas las posibles opciones de respuesta.
- **Cerradas:**
    - Limitan o cierran las opciones de respuesta disponibles

**Tipo de informacion obtenida**
- **Actitud:** Lo que las personas dicen que quieren
- **Creencias:** Lo que las personas creen que es verdad
- **Comportamiento:** Lo que realmente hacen
- **Caracteristicas:** De las personas o cosas

Cuando usar cuestionarios?
- Las personas estan dispersas geograficamente
- Muchas personas involucradas
- Queremos obtener opiniones generales
- Queremos identificar problemas generales


## Entrevistas

- Tecnica de explotacion mediante la cual el analista de sistemas recolecta informacion de las personas a traves de la interaccion cara a cara.
- Es una conversacion con un proposito especifico, que se basa en un formato de preguntas y respuestas en general.
- Conocer opiniones y sentimientos del entrevistado

**Ventaja**
- El entrevistador se siente incluido en el proyecto
- Es posible obtener una retroalimentacion del encuestado
- Es posible adaptar las preguntas de acuerdo al entrevistado`
- Informacion no verbal observando las acciones y expresiones del entrevistado.

**Desventaja**
- Costosas
- Tiempo y recursos humanos
- Las entrevistas dependen en gran parte de las habilidades del entrevistador
- No aplicable a distancia

**Tipos de entrevistas**

- **Estructuradas (Cerradas)**
    - El encuestador tienen un conjunto especifico de preguntas para hacerselas al entrevistado` 
    -  Se dirige al usuario sobre un requerimiento puntual
    -  No permite adquirir un amplio conocimiento del dominio
- **No estructuradas (Abiertas)**
    - El encuestador lleva a un tema en general
    - Sin preparacion de preguntas especificas.
    - Iniciar con preguntas que no dependan del contexto, para conocer el problema, la genete involucrada, etc.

**Tipos de Preguntas**
- **Abiertas:** Permiten al encuestado responder de cualquier manera
- **Cerradas:** Las respuesta son directas, cortas o de seleccion especifica.
- **Sondeo:** Permite obtener mas detalle sobre un tema puntual

**Preguntas Abiertas:**
- **Ventajas:**
    - Revelan nueva linea de preguntas 
    - Hacen mas interesante la entrevista
    - Permiten espontaneidad
- **Desventajas:**
    - Pueden dar muchos detaller irrelevantes 
    - Se puede perder el control de la entrevista`
    - Parece que el entrevistador no tiene los objetivos claros

**Preguntas Cerradas:**
- **Ventajas:**
    - Ahorran tiempo.
    - Se mantiene mas facil el control de la entrevista
    - Se consiguen datos relevantes
- **Desventajas:**
    - Pueden aburrir al encuestado 
    - No se obtienen detalles

**Preparacion Previa (Kendall)**

- **Leer los antecedentes**
    - Poner atencion en el lenguaje. Buscar un vocabulario en comun. Imprescindible para poder entender al entrevistado.
- **Establecer los objetivos de la entrevista**
    - Usando los antecedentes. Los directivos suelen proporcionar una vision general, mientras que los futuros usuarios una mas detallada.
- **Seleccionar los entrevistados**
    - Se debe minimizar el numero de entrevisdtas
    - Los entrevistados deben conocer con antelacion el objetivo de la entrevista y las preguntas que se le van a hacer.
- **Planificacion de la entrevista y preparacion del entrevistado**
    - Establecer fecha, hora, lugar y duracion de cada entrevista de acuerdo con el entrevistado.
- **Seleccion del tipo de preguntas a usar y su estructura**

### **Como conducir la entrevista**
- **Seleccion del entrevistado**
    - Segun el requerimiento a analizar
    - Conocer sus fortalezas, prejuicios y motivaciones
        - Armar la entrevista en base a las caracteristicas de la persona
    - Hacer una cita (ano llegar sin avisar)
    - Respetar el horario de trabajo
    - Establecer la duracion de la entrevista 
        - Cuanto mayor es el cargo de la entrevista menor tiempo se debe utilizar
    - Obtener el permiso del supervisor o jefe.
    - La entrevista es personal y debe realizarse en un lugar privado
- **Preparacion de la entrevista**
    - Informar al entrevistado el tema de tratar antes de la reunion 
    - Definir un 'Guion de Entrevista'
    - Se debe evitar preguntas sesgadas o con intencion, amenazantes o criticas
    - Usar lenguaje claro y conciso
    - No incluir opinion como parte de la pregunta
    - Evitar realizar preguntas largas y complejas
- **Conduccion de la entrevista**
    - Respete el horario y los tiempos definidos 
    -  Si es una sala de reunion llegue antes para asegurar las condiciones de la misma
    -  Inicie la entrevista saludando, presentandose y agradeciendo la atencion
    -  Mencione el proposito de la misma y la duracion
    -  Escuche con atencion y observe al entrevistado, tome nota de las respuestas verbales y no verbales
    -  Concluya la entrevista expresando su agradecimiento
    -  Haga una breve conclusion de la entrevista para ganar la confianza del entrevistado

**Debe**
- Vestirse adecuadamente
- Ser cortes
- Escuchar cuidadosamente
- Mantener el control
- Observar los gestos
- Ser paciente
- Mantener al entrevistado en calma
- Mantener el autocontrol
- Terminar a tiempo

**Evite**
- Suponer que una respuesta no lleva a ningun lado
- Revelar pistas
- Usar jerga
- Revelar sesgos personales
- Hablar en lugar de escuchar
- Suponer cualquier cosa acerca del tema o del entrevistado
- Uso de grabadores (senial de debilidad de escuchar)


**Seguimiento de la entrevista**\
Enviar al entrevistado un resumen de la entrevista, permitiendo aclarar cualquier cosa que no se haya entendido durante la entrevista.

**Como escuchar**\
Saber escuchar es la parte mas importante del proceso de una entrevista, se debe diferenciar entre oir y escuchar
- Llegue con actitud positiva
- Haga que la otra persona se tranquilice
- Haga ver que esta escuchando lo que dice
- Haga preguntas sobre lo que dice
- No haga suposiciones
- Tome nota


### Planeacion Conjunta de Requerimientos
Proceso mediante el cual se conducen reuniones de grupo altamente estructurados con el proposito de analizar problemas y definir requerimientos.
- Requiere de extenso entrenamiento
- Reduce el tiempo de expotacion de requerimientos
- Amplia particion de los integrantes
- Se trabaja sobre lo que se va generando
- Alguna bibliografia la mencionada como JAD (Joint Aplication Design)

**Ventajas**
- Ahorro de tiempo
- Usuarios involucrados
- Desarrollos creativos

**Desventajas**
- Es dificil organizar los horarios de los involucrados
- Es complejo encontrar un grupo de participantes integrados y oganizados

**Como planear las sesiones de JRP**
- Seleccion de una ubicacion para las sesiones de JRP
- Seleccion de los participantes
- Preparar la agenda 

**Beneficios del JRP**
- JRP involucra activamente a los usuarios y la gerencia en el proyecto de desarrollo
- JRP reduce el tiempo de la etapa de requerimientos
- Si se incorporan prototipos, los mismos ya confirman el disenio del sistema.


### Lluvia de Ideas

- Tecnica para generar ideas al alantar a los participantes para que ofrezcan tantas ideas como sea posible en un corto tiempo sin ningun analisis hasta que se hayan agotado las ideas.
- Se promueve el desarrollo de ideas creativas para obtener soluciones
- Se realizan reuniones del equipo involucrado en la resolucion del problema, conducidas por un director.
- Los principios en los que se basa esta tecnica son
    - Cuantas mas ideas se sugieren, mejores resultados se conseguiran
    - La produccion de ideas en grupos puede ser mas efectiva que la individual
    - Las ideas de una persona pueden hacer que aparezan otras por 'acontagio'
    - A veces las mejores ideas aparecen tarde
    - Es mejor elegir sobre una variedad de soluciones
- Incluye una serie de fases de aplicacion
    - Descubrir hechos, Producir ideas, Descubrir soluciones
- Clave para resolver la falta de consenso entre usuarios
- Es util combinarlo con la toma de decisiones
- Ayuda a entender el dominio del problema
- Encara la dificultad del usuario para transmitir
- Ayuda a entender (al usuario y al analista)


---

# Clase 2 Requerimientos

## Que es un proceso?

Es un conjunto de actividades y resultados asociados que producen un producto de software

Pasos que deberia seguir: `Idea`, `Disenio`, `Pruebas`, `Fabricacion`, `Mercado`

Actividades fundamentales de los procesos
- Especificacion del software
- Desarrollo del software
- Validacion del software
- Evolucion del software

Los IS son los responsables de realizar estas actividades

## Que es un modelo de proceso de software?

Es una representacion simplificada de un proceso de software que presenta una vision de este proceso.

Estos modelos pueden incluir actividades que son partes de los procesos y productos de software, y el papel de las personas involucradas.

La mayoria de los modelos de proceso de software se basan en uno de los siguientes modelos generales o paradigmas.

- **Modelo en cascada:** Las etapas se representan cayendo en cascada. Cada etapa de desarrollo se debe completar antes que comience la siguiente.
- **Desarrollo iteractivo:** Un sistema inicial se desarrolla rapidamente a partir de una especificacion abstracta. Este se refina basandose en las peticiones del cliente.
- **Desarrollo basado en componentes:** Esta tecnica supone que las partes ya existen. El proceso se enfoca en la integracion de las partes.

Mas adelante se ven los procesos mas detallados


## Requerimientos 2
Un requerimiento es una caracteristica del sistema o una descripcion de algo que el sistema es capaz de hacer con el objetivo de satisfacer el proposito del sistema

Impacto de los errores en la etapa de requerimientos
- El software resultante puede no satisfacer a los usuarios
- Las interpretaciones multiples de los requerimientos pueden causar desacuerdos entre clientes y desarrolladores
- Puede gastarse tiempo y dinero construyendo el sistema erroneo

## Tipos

- **Requerimientos funcionales:**
    - Describen una interaccion entre el sistema y su ambiente. Como debe comportarse el sistema ante determinado estimulo.
    - Describen lo que el sistema debe hacer, o incluso como NO debe comportarse.
    - Describen con detalle la funcionalidad del mismo
    - Son independientes de la implementacion de la solucion.
    - Se pueden expresar de distintas formas
- **Requerimientos no funcionales:**
    - Describen una `restriccion` sobre el sistema que limita nuestras elecciones en la construccion de una solucion al problema.
    - Requerimientos del producto
        - Especifican el comportamiento del producto(usabilidad, eficiencia, rendimiento, espacio, fiabilidad, portabilidad)
    - Requerimientos organizacionales
        - Se derivan de las politicas y procedimientos existentes en la organizacion del cliente y en la del desarrollador (entrega, implementacion, estandares)
    - Requerimientos externos
        - Interoperabilidad, legales, privacidad, seguridad, eticos.


**Requerimientos no funcionales**

- Del producto
    - De usabilidad
    - De eficiencia
        - De rendimiento
        - De espacio
    - De fiabilidad
    - De portabilidad
- Organizacionales
    - De entrega
    - De implementacion
    - De estandares
- Externos
    - Interoperabilidad
    - Eticos
    - Legistaltivos
        - De privacidad
        - De seguridad

**Otras clasificaciones**

- **Requerimientos del dominio**\
    Reflejan las caracteristicas y restricciones del dominio de la aplicacion del sistema. Pueden ser funcionales o no funcionales y pueden restringir a los anteriores. Como se especializan en el dominio son complicados de interpretar.
- **Requerimientos por Prioridad**
    - Que deben ser absolutamente satisfechos
    - Que son deseables pero no indispensables
    - Que son posibles, pero que podrian eliminarse
- **Requerimientos del Usuario**
    - Son declaraciones en lenguaje natural y en diagramas de los servicios que se espera que el sistema provea y de las restricciones bajo las cuales debe operar
    - Pueden surgir problemas por falta de claridad, confusion de requerimientos, conjuncion de requerimientos.
- **Requerimientos del Sistema**
    - Establecen con detalle los servicios y restricciones del sistema
    - Es dificil excluir toda la informacion de disenio(arquitectura inicial, Interoperabilidad con sistemas existentes, etc)



## Ingenieria de Requerimientos

Es el proceso por el cual se transforman los requerimientos declarados por los clientes, ya sean hablados o escritos, a especificaciones precisas, no ambiguas, consistentes y completas del comportamiento del sistema, incluyendo funciones, interfaces, rendimiento y limitaciones

La ingenieria de requerimientos es la diciplina para desarrollar una especificacion completa, consistente y no ambigua, la cual servira como base para acuerdos comunes entre todas las partes involucradas y en donde se describen las funciones que realizara el sistema.

Tambien es el proceso mediante el cual se intercambian diferentes puntos de vista para recopilar y modelar lo que el sistema va a realizar. Este proceso utiliza una combinacion de metodos, herramientas y actores, cuyo producto es un modelo del cual se genera un documento de requerimientos.

Tambien es un enfoque sistematico para recolectar, organizar y documentar los requerimientos del sistema; es tambien el proceso que establece y mantiene acuerdos sobre los cambios de requerimientos, entre los clientes y el equipo del proyecto.

**Importancia**
- Permite gestionas las necesidades del proyecto en forma estructurada
- Mejora la capacidad de predecir cronogramas de proyectos
- Disminuye los costos y retrasos del proyecto`
- Mejora la calidad del software
- Mejora la comunicacion entre equipos
- Evita rechazos de usuarios finales

## Estudio de Viabilidad

Principalmente para sistemas nuevos.

A partir de una descripcion resumida del sistema se elabora un informe que recomienda la conveniencia o no de realizar el proceso de desarrollo

Responde las siguientes preguntas:
- El sistema contribuye a los objetivos generales de la organizacion?(Si no contribuye, entonces no tiene un valor real en el negocio)
- El sistema se puede implementar con la tecnologia actual?
- El sistema se puede implementar con las restricciones de costo y tiempo?
- El sistema puede integrarse a otros que existen en la organizacion?


Una vez que se ha recopilado toda la informacion necesaria para contestar las preguntas anteriores se deberia hablar con las fuentes de informacion para responder nuevas preguntas y luego se redacta el informe, donde deberia hacerse una recomendacion sobre si debe continuar o no el desarrollo.

## Especificacion de Requerimientos
- **Necesario:** Su omision provoca una deficiencia
- **Conciso:** Facil de leer y entender
- **Completo:** No necesita ampliarse
- **Consistente:** No contradictorio con otro
- **No ambiguo:** Tiene una sola implementacion
- **Verificable:** Puede testearse a traves de inspecciones, pruebas, etc

Objetivos
- Permitir que los desarrolladores expliquen como han entendido lo que el cliente pretende del sistema
- Indicar a los diseniadores que funcionalidad y caracteristicas va a tener el sistema resultante
- Indicar al equipo de pruebas que demostraciones llevar a cabo poara convercer al cliente de que el sistema que se le entrega es lo que habia pedido.

| Especificaciones de requerimientos| | 
| -- | -- |
| - Correcta | Rasteable |
| - No ambigua | Independiente del disenio |
| - Verificable | Anotada |
| - Completa | Concisa |
| - Consistente | Organizada |
| - Comprensible por los consumidores | Utilizable en operacion y mantenimiento |
| Modificable |  |

- Documento de definicion de requerimientos\
    Listado completo de todas las cosas que el cliente espera que haga el sistema
- Documento de especificacion de requerimientos\
    Definir en terminos tecnicos
- Documento de especificacion de requerimientos de Software IEEE Std 830 - 1998 (SRS)
- Aspectos basicos de una especificacion de requerimientos
    - **Funcionalidada:** Que debe hacer el sosftware?
    - **Interfaces Externas:** Como interactua el software con el medio externo?
    - **Rendimiento:** Velocidad, disponibilidad, tiempo de respuesta, etc
    - **Atributos:**
    - **Atributos:** Portabilidad, seguridad, mantenibilidad, eficiencia
    - **Restricciones de Disenio:** Estandares requeridos, lenguaje, limite de recursos, etc

**Usuarios de un documento de requerimientos**
- **`Clientes del sistema:`** Especifican los requerimientos y los leen para comprobar que cubren sus necesidades. Los clientes especifican los cambios a los requerimientos
- **`Administradores:`** Usan el documento de requerimientos para planear una cotizacion para el sistema y el proceso de desarrollo del sistema
- **`Ingenieros del sistema:`** Usan los requerimientos para entender que sistema debe desarrollarse.
- **`Ingenieros de prueba del sistema:`** Usan los requerimientos para desarrollar pruebas de validacion para el sistema
- **`Ingenieros de mantenimiento del sistema:`** Usan los requerimientos para comprender el sistema y las relaciones entre sus componentes.

## Validacion de requerimientos

Es el proceso de certificar la correcion del modelo de requerimientos contra las intenciones del usuario

Trata de mostrar que los requerimientos definidos son los que estipula el sistema. Se describe el ambiente en el que debe operar el sistema.

Es importante, porque los errores en los requerimientos pueden conducir a grandes costos si se descubren mas tarde

- **Validacion:** Al final del desarrollo evaluar el software para asegurar que el software cumple los requerimientos
- **Verificacion:** El software cumple los requerimientos correctamente

Sobre estas definiciones
- La validacion solo se puede hacer con la activa participacion del usuario
- Validacion: hacer el software correcto
- Verificacion: hacer el software correctamente

**Es suficiente validar despues del desarrollo de software?**
- La evidencia estadistica dice que NO
- Cuanto mas tarde se detecta, mas cuesta corregir (Boehm)
- Bola de nieve de defectos
- Validar en la fase de especificacion de requerimientos puede ayudar a evitar costosas correcciones despues del desarrollo

**Contra que se verifican los requerimientos?**
- No existen 'los requerimientos de los requerimientos'
- No puede probarse formalmente que un Modelo de Requerimientos es correcto. Puede alcanzarse una conviccion de que la solucion especificada en el modelo de requerimientos es el correcto para el usuario.

Comprenden
- Verificaciones de validez (para todos los usuarios)
- Verificaciones de consistencia (sin contradicciones)
- Verificaciones de completitud (todos los requerimientos`)
- Verificaciones de realismo (se pueden implementar)
- Verificaciones (se puede diseniar conjunto de pruebas)

### Tecnicas de Validacion

Pueden ser manuales o automatizadas
- Revisiones de requerimientos (formales o informales)
    - Informales: Los desarrolladores deben tratar los requerimientos con tantos stakeholders como sea posible`
    - Formal: El equipo de desarrollo debe conducir al cliente, explicandole las explicaciones de cada requerimiento
- Antes de una revision formal, es conveniente realizar una revision informal
- Contruccion de prototipos
- Generacion de casos de prueba


## Tecnicas de Especificacion de Requerimientos

**Estaticas**

Se describe el sistema a traves de las entidades u objetos, sus atributos y sus relaciones con otros. No describe como las relaciones cambian con el tiempo. 
Cuando el tiempo no es un factor mayor en la operacion del sistema, es una descripcion util adecuada.

Ejemplos: Referencia indirecta, Relaciones de recurrencia, Definicion axiomatica, Expresiones regulares, Abstracciones de datos, entre otras.

**Dinamica**

Se considera un sistema en funcion de los cambios que ocurren a lo largo del tiempo.

Se considera que el sistema esta en un estado particular hasta que un estimulo lo obliga a cambiar su estado.

Ejemplos: Tablas de decision, Diagramas de transicion de estados, Tablas de transicion de estados, Diagramas de persianas, Diagramas de transicion extendidos, Redes de Petri, entre otras.

## Historias de usuario

Son utilizadas en las metodologias de desarrollo agiles (XP, SCRUM, etc) para las especificaciones de requerimientos

Acompaniadas de las discusiones con los usuarios y las pruebas de validacion

```
Una historia de usuario es una representacion de un requerimiento de 
software escrito en una o dos frases utilizando el lenguaje comun del usuario 
```


**Debe ser limitada,** esta deberia poder escribirse sobre una nota adhesiva pequenia

Son **una forma rapida de administrar los requisitos** de los usuarios sin tener que elaborar gran cantidad de documentos formales y sin requerir de mucho tiempo para administrarlo

Permiten **responder rapidamente a los requisitos cambiantes**

Al momento de implementar las historias, los desarrolladores deben tener la posibilidad de **discutirlas con los clientes.**

Generalmente se espera que la **estimacion de tiempo** de cada historia de usuario se situe entre unas **10 horas y un par de semanas**

Estimaciones **mayores a dos semanas** son indicativo de que la historia es muy compleja y debe ser **dividida en varias historias**

Si bien el estilo puede ser libre, la historia de usuario debe responder a tres preguntas:
- **Quien se beneficia?**
- **Que se quiere?**
- **Cual es el beneficio?**

Esquema

- Como (**rol**) quiero (**algo**) para poder (**beneficio**)

Ejemplos
- Como **`usuario registrado`** deseo loguearme para poder **`empezar a utilizar la aplicacion`**
- Como **`secretaria`** quiero poder imprimir el listado de turnos asignados en una fecha determinada y **`guardar la informacion de los mismos`**
- Como `Cliente`, quiero `suscribirme por medio del sitio web` y `obtener un nuevo plan de TV por clable`
- Como `Vendedor`, quiero `registrar los productos y cantidades que me solicita un cliente` para `crear un pedido de venta`
- Como `Analista de compras`, quiero `que el sistema notifique via correo electronico a los preveedores` para `avisar que se ha desviado una cotizacion de licitacion`


### Caracteristicas
- **Independientes unas de otras:** De ser necesario, combinar las historias dependientes o buscar otra forma de dividir las historias de manera que resulten independientes.
- **Negociables:** La historia en si misma no es lo suficientemente explicita como para considerarse un contrato, la discusion con los usuarios debe permitir esclarecer su alcance y este debe dejarse explicito bajo la forma de pruebas de validacion.
- **Valoradas por los clientes o usuarios:** Los intereses de los clientes y de los usuarios no siempre coinciden, pero en todo caso, cada historia debe ser importante para alguno de ellos mas que para el desarrollador.
- **Estimables:** Un resultado de la discusion de una historia de usuario es la estimacion del tiempo que tomara completarla. Esto permite estimar el tiempo total del proyecto.
- **Pequenias:** Las historias muy largas son dificiles de estimar e imponen restricciones sobre la planificacion de un desarrollo iteractivo. Generalmente se recomienda la consolidacion de historias muy cortas en una sola historia
- **Verificables:** Las historias de usuario cubren requerimientos funcionales, por lo que generalmente son verificables. Cuando sea posible, la verificacion debe automatizarse, de manera que pueda ser verificada en cada entrega del proyecto

Un criterio de aceptacion es el criterio por el cual se define si una historia de usuario fue desarrollada segun la expectativa del Product Manager (Como representante de los criterios del cliente) y se si puede dar como hecha.

Deben ser definidos durante la etapa inicial antes de la codificacion, acompanian a la historia de usuario, porque complementan la historia de usuario y ayudan al equipo de desarrollo a entender mejor como se espera que el producto se comporte.

Los criterios de aceptacion son utilizados para expresar el resultado de las conversaciones del cliente con el desarrollador. El cliente deberia ser quien las escriba mas que el desarrollador.

Representan el inicio de la definicion del como. No estan diseniados para ser tan detallados como una especificacion de disenio tradicional.

Si una historia de usuario tiene mas de 4 criterios de acecptacion, debe evaluarse subdividir la historia.

Puede aniadirse un numero de escenario para identificar al criterio, asociado a la historia de usuario en cuestion.

### Beneficios
- Al ser muy corta, esta representa requisitos del modelo de negocio que pueden implementarse rapidamente (dias o semanas)
- Necesitan poco mantenimiento
- Mantienen una relacion cercana con el cliente
- Permiten divir los proyectos en pequenias entregas
- Permite estimar facilmente el esfuerzo de desarrollo
- Es ideal para proyectos con requisitos volatiles o no muy claros.

### Limitadores

- Sin criterios de aceptacion pueden quedar abiertas a distintas interpretaciones haciendo dificil utilizarlas como base para un contrato
- Se requiere un contacto permanten con el cliente durante el proyecto lo cual puede ser dificil o costoso
- Podria resultar dificil escalar a proyectos grandes
- Requiere desarrolladores muy competentes

### Epicas

Se denomina Epica a un conjunto de Historias de usuario que se agrupan por algun denominador comun

---

# Clase 3

## Casos de Uso

### Definicion
Proceso de modelado de las 'funcionalidades' del sistema en termino de los eventos que interactuan entre los usuarios y el sistema.

Tienen sus origenes en el modelo orientado a objetos (Jacobson 1992) pero su eficiencia en modelado de requerimientos hizo que se independice de la tecnica de diseño 


