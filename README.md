<h1 align="center"> 🖥️ Ingenieria de Software 1</h1>

- [Aprovanto historias de usuario](#aprobar-historias-de-usuario)

## Aprobar Historias de Usuario

### Ejercicio 1) Alquiler de mobiliario
- Reservar Alquiiler
    - Minimo 3 muebles
    - Pago con tarjeta de crédito valida
- Alta mueble
    - Un mueble no puede estar registrado dos veces
- Pagar con tarjeta de credito
    - Abonar el 20% total del alquiler

### Ejercicio 2) Postgrado

- Cargar Carrera
    - Nombre Unico
    - Maximo 5 años de duración
- Registrar Alumno
    - Usuario Unico
    - Contraseña mayor a 6 digitos
- Iniciar Sesión
    - Usuario existente //Hace falta poner esto?
- Cerrar Sesión
- Inscripción alumno registrado al curso
    - Pagar con tarjeta de credito valida
- Pagar con tarjeta de credito

### Ejercicio 3) Contratos

- Confecciónar minuta
    - Monto no puede superar los $25.000
    - Duración maxima 6 meses
- Aprobar Minuta
    - Menos de 3 minutas aprobadas
    - Cuit habilitado por la AFIP 
    - Establecer conexión con servidor de AFIP

### Ejercicio 4) Venta de bebidas
- Registrar Persona
    - Persona mayor de 18 años
    - Mail no registrado
- Iniciar Sesión
- Cerrar Sesión
- Seleccionar bebida
    - Tener Stock
- Descontar 20% compra
    - Ser usuario premium
- Descontar 10% compra
    - Comprar monto superior a $4500

### Ejercicio 5) Casa de fotografia
- Registrar Persona
    - Nombre de usuario unico
- Iniciar Sesión
- Cerrar Sesión
- Subir Foto
    - Maximo 50 fotos subidas
    - Subir fotos de a una
- Pagar foto
- Registrar Codigo
    - Codigo Único

### Ejercicio 6) Biblioteca

- Registrar Libro
- Asociar alumno
    - Certificado alumno regular
- Prestar Libro
    - Ser socio
    - No posea mas de tres prestamos vigentes
    - No tenga prestamos vencidos
    - Libro en buen estado
- Retornar Libro
    - Préstamo no vencido


### Ejercicio 7) Mutual
- Afiliar Persona
    - Tarjeta de crédito valida
- Prestar Ortodoncia
    - Pago mes anterior
    - El prestamo es una vez por afiliado
    - Menor a 15 años
    - Con menos de 9 meses de antiguedad
    - Presentar historia crinica elaborada por el profecional
- Presentar plantillas
    - Pago el mes anterior
    - Prestación cada 2 años
    - Presentar indicación del profecional
    - Presentar factura comercio que la confecciono
- Prestar anteojos
    - Prestar anteojos
    - Prestación cada 18 meses
    - Afiliado con al menos 3 meses de antiguedad
- Prestar Internación
    - Pago el mes anterior
- Consultas medicas
    - Pago el mes anterior
    - Prestación cada 2 meses

### Ejercicio 8) Teatro
- Reservar entrada
    - 2 entradas por persona (maximo)
    - Se podra reservar hasta 3 horas antes del evento
- Comprar entrada Web
    - Pagar con tarjeta de credito valida
- Comprar entrada personalmente
    - Pagar con tarjeta de credito valida
- Retirar entrada reservada // Como dice que el proceso se realiza igual el las compras, yo lo dejo asi
    - Pagar con tarjeta de credito valida
    - Entrada reservada no caducada 
- Pagar entrada
- Retirar compra Online
- Administrar funcion

### Ejercicio 9) Pago electrónico
- Recuperar datos  
    - Conexión central de cobro
- Verificar vencimiento
    - Si la factura no esta vencida, informar monto original
    - Si la factura en 1ra fecha, cobro monto original mas recargo
    - Si la factura esta vencida en 2da fecha no se puede cobrar por ese mismo motivo
- Registrar cobro
    - Conexión centrar de cobro
    - Clave maestra valida
    - Enviar transacción una sola vez
- Mostrar estadistica
    - Clave maestra valida
- Conexión central de cobro


### Ejercicio 10) Un Aventón
- Registra Persona
    - Mail Unico
- Iniciar Sesion
- Cerrar Sesion
- Publicar Viaje
- Aceptar candidato
- Calificar Usuario

### Ejercicio 11) Concursos
- Registrar Persona
    - Mail Unico
    - Dni menor a 55M y mayor a 12M
- Iniciar Sesión
- Cerrar Sesion
- Inscribir Usuario
    - Docente no puede inscribirse en más de 3 cursos
- Listar inscriptos


### Ejercicio 12) Creditos Bancarios
- Iniciar Tramite
- Consultar estado
    - Si el cliente ingresa 3 veces un codigo inexistente el sistema bloquea la ip
- Listar créditos


### Ejercicio 13) Venta de libros
- Registrar usuario
    - El correo electronico único
    - Clave de 6 caracteres
- Confirmar Usuario
    - Codigo de 16 digitos valido
- Iniciar Sesion
- Cerrar Sesión
- Ingresar ISBN
- Comprar Libro
    - Tarjeta valida
- Pagar compra
### Ejercicio 14) 
- Autenticar Usuario
    - Credenciales correctas
    - Conexión sistema del Banco Central
- Alta tarjeta
    - Persona que quiere la tarjeta debe ser cliente del banco
    - Conexion exitosa con el sistema SIVA
- Baja tarjeta
- Listar operaciones
    - No pueden ingresarse fechas futuras al presente
    - La fecha de inicio no puede ser mayor a la de fin

### Ejercicio 15)
- Registrar Persona
    - Mail Unico
    - Edad mayor a 18 años
- Iniciar Sesión
    - Si un usuario falla 3 veces su cuenta es bloqueada
- Cerrar sesión
- Solicitar turno
    - Turno registrado con 2 o más dias de la fecha en que se solicita

### Ejercicio 16)
- Autenticar usuario
    - Conexión con el sistemas general del observatorio
- Cerrar Sesión
- Cargar Imagen
    - Solo se pueden cargar imágenes mayores o iguales a 2 Megapixeles
- Recortar área de interes
    - No se pueden superponer con otra del sistema
    - No se podrán recortar mas de 4 áreas
- Listar Imagenes
    - Nose puede mostrar mas de 20 imagenes a la vez
    