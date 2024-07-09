                              CREACION BASE PARA UNA APP DE RESERVAS DE CLASES DE PILATES

Problema:
Estudio de Pilates necesita el desarrollo de una base de datos para una aplicación donde sus alumnos puedan reservar sus clases. Requiere agendar la reserva de turnos con el fin de poder llevar el registro de turnos disponibles por horarios.

Descripción del Problema:
Actualmente la reserva de clases es realizada de forma manual, las alumnas solicitan el turno mediante el WhatsApp del estudio y son anotadas en una hoja Google Sheets que es compartida a las profesoras para que estén informadas de las alumnas que asistirán a su clase, luego las profesoras envían la confirmación de las asistencias a la administración para que puedan llevar el control.
1.	Tipo Reserva: Es importante poder clasificar las reservas según su tipo, ya sea una reserva de clase privada, duo o grupal.
2.	Tipo Clase: Se requiere poder clasificar el tipo de clase que tomara el alumno, ya sea actual o por recuperación.
3.	Disponibilidad de Reformer: La base de datos debe permitirnos registrar la disponibilidad de reformer por horario, es decir, si el equipo está ocupado o disponible.
4.	Registro de Reservas: Se requiere un sistema que pueda registrar de manera detallada cada reserva realizada, incluyendo la fecha y hora de la clase, el alumno que la realizó, el profesor que dicta la clase y el tipo de clase.

Objetivo:
Diseñar e implementar una base de datos relacional que abarque todas las necesidades para el proceso de reserva de clases del estudio de pilates. Esta base de datos deberá ser eficiente, exponencial y fácil de mantener, permitiendo una administración precisa de todas las reservas.
Descripción de la Base de Datos - Gestión de Reservas en Restaurantes
Esta base de datos está diseñada administrar las reservas en un estudio de pilates, así como la información relacionada con alumnos, profesoras, tipos de reserva, entre otros. A continuación se detallan los elementos principales de la base de datos:

Tablas:

1.RESERVA: Registra la reserva realizada por el alumno

o	Atributos: IDRESERVA, IDALUMNO, IDEQUIPO, IDPROFESOR, IDTIPORESERVA, FECHA, HORA.

2.ALUMNO: Almacena información sobre los datos de los alumnos que realizan reservas.

o	Atributos: IDALUMNO, NOMBRE, FECHA_DE_NACIMIENTO, TELEFONO, CORREO.

3.PROFESOR:Contiene información sobre datos de los profesores encargados de dictar la clase.

o	Atributos: IDPROFESOR, IDTIPOCLASE, IDNIVELCLASE, NOMBRE, TELEFONO, CORREO.

4.TIPORESERVA: Define los tres tipos de reserva (Privada, Duo, Grupal).

o	Atributos: IDTIPORESERVA, TIPO.

5.TIPOCLASE:Contiene registro del tipo de la clase (Actual, Recuperación).

o	Atributos: IDTIPODECLASE, IDPROFESOR, FECHA, HORA.

6.NIVELCLASE: Contiene registro del nivel de la clase (Básico, Intermedio y Avanzado).

o	Atributos: IDNIVELCLASE, IDPROFESOR, IDTIPOCLASE, FECHA, HORA.

7.EQUIPO: Contiene información sobre los equipos disponibles en cada horario.

o	Atributos: IDEQUIPOS, IDPROFESOR, DISPONIBLE.

Problemática Resuelta:
Esta base de datos permite administrar de manera eficiente el proceso de reserva en un estudio de pilates, desde la información de los alumnos y profesores hasta la disponibilidad de equipos y el registro de reservas. Algunos aspectos que aborda incluyen:

•	Registro de los alumnos en los horarios requeridos.

•	Clasificación de las reservas según su tipo y clase.

•	Gestión de la disponibilidad de equipos por horario.

En resumen, esta base de datos proporciona una estructura para organizar y administrar de manera eficiente el proceso de reservas en el estudio de pilates, contribuyendo un mejor servicio para el alumno.



