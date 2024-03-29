﻿# GEAS

## Grupo: Los 4 Fantásticos

1. Añais, Raul Alejandro
2. Nacimiento, Francisco Martin
3. Potocki, Joaquín
4. Silveira Do Santo, Facundo Omar
 
## Visión 

Gestión automatizada de alumnos de la escuela secundaria EPET Nro 38, localizada en la ciudad de San Pedro, Misiones. El sistema permitirá a los usuarios (Docentes, preceptores y directivos), automatizar las actividades repetitivas y ahorrar tiempo. Estas actividades están centradas en la gestión de los legajos, los libros de evaluacion, gestionar pases, promover alumnos y generar el LUA (Legajo Unico del Alumno), con los reportes de novedades sobre las altas, bajas y pases de alumnos.

## Lista de características

1. Inscribir Alumnos.
2. Gestionar Legajos. 
3. Imprimir Libretas. 
4. Tomar Asistencias.
5. Generar Libros de Evaluación.
6. Promover Alumnos.
7. Cargar Notas.
8. Enviar Reportes de Asistencias a los Padres. 
9. Generar LUA.
10. Gestionar Pases.


## Análisis de Dominio


__Inscribir Alumnos:__ Se toman los datos y documentos que alumno vaya trayendo a la escuela para su pre-inscripción.
__Gestionar Legajos:__ Se trata de un CRUD de los alumnos y sus tutores, esta inscripción es la oficial de alumno a la escuelo.
__Imprimir Libretas:__ Una vez cerrado cada trimestre se imprimirá un documento con las notas correspondientes a cada alumno.
__Generar Libro de Evaluación:__ Es el resumen de las notas de los alumnos de un curso en particular y sus materias. Por cada curso habrá un libro de evaluación, 5 libros de evaluación por año, 3 de los trimestres y dos por instancias de recuperatorios.
__Promover Alumnos:__  Cada cierre de ciclo si el alumno cumple con las condiciones preestablecidas será promovido al siguiente curso, en caso de que no cumpla las condiciones será promovido a los recuperatorios de diciembre o marzo según corresponda y si no logra cumplir con las condiciones de promoción recurrirá el año. 
__Enviar Reportes de Asistencias a los Padres:__
__Generar LUA:__El documento que se le manda al consejo de educación de la provincia, tiene datos que son requeridos por el consejo, tiene un formato a seguir, tiene fechas estipuladas de envíos, tiene información sobre pases de los alumnos y bajas.
__Gestionar Pases:__En este proceso hay una constancia de pase (un documento) para decir las escuela que viene el estudiante.

__Diccionario
__Legajo:__ Son los datos de los alumnos y tutores. 
__Libreta:__ Es un documento oficial de comunicación entre la escuela y el tutor, puede tener cualquier formato y queda como criterio de la escuela. (El orden de las materias es importante, según el libro matriz).
__Documentos de novedades:__ Es el documento que tiene la información de alumnos que se fueron e ingresaron a la escuela junto con datos de sus tutores, este documento se envía al consejo de educación es determinadas fechas.

## Bocetos de Interfaz de Usuario


![alt text](https://github.com/Nacimiento98/POO2/blob/master/Imagenes/IMG_20190919_151337669.jpg "Pantalla 1 C.U preinscripcion")

Pantalla 1

![alt text](https://github.com/Nacimiento98/POO2/blob/master/Imagenes/IMG_20190919_150015857.jpg "Pantalla 2 C.U novedades")

## Casos de Uso

### Actores

1. Preceptor: Es el encargado de la gestion administrativa de los alumnos.
2. Docente: Es el encargado de Calificar a un alumno y entregar planilla de notas de su materia.

...

_Por cada caso de uso especificar_

__Inscribir Alumnos__

__Actores__: Preceptor

__Objetivo__: Cargar datos de alumnos y tutores

__Flujo Principal__:

1. Este caso de uso comienza cuando el Preceptor selecciona la opcion inscribir Alumno.
2. El sistema mostrará una pantalla de carga de datos.
3. El preceptor completa los campos y selecciona la opcion "guardar" o "guardar y continuar" o "descartar".
4. El sistema verifica que los campos obligatorios esten cargados y termina el caso de uso.

_Flujos alternativos_

3.1. Si el actor Selecciona la opcion guardar se realiza el paso 4 y finaliza el caso de uso.
3.2. Si el actor Selecciona la opcion guardar y continuar se realiza el paso 4, se guarda un nuevo alumno y se vuelve al paso 2.
3.3. Si el actor Selecciona la opcion descartar no se realiza ningun cambio y finaliza el caso de uso.

__Imprimir Novedades__

__Actores__: Director

__Objetivo__: Generar un documento con las novedades que serán enviados al consejo de educación dos veces al año


__Flujo Principal__:

1. Este caso de uso comienza cuando el director selecciona la opción “ver novedades”.
2. El sistema muestra una pantalla con todas las novedades.
3. El director podrá realizar un filtrado por fecha, tipo de novedad, curso,etc.
4. El sistema mostrará aquellas novedades que cumplan con el filtro.
5. El director presionara el botón generar PDF.
6. El sistema generará un PDF con todos los datos generados.

__Generar Legajo__

__Actores__: Preceptor

__Objetivo__: Gestionar legajo para cada alumno que ya esté pre inscripto en el sistema

__Flujo Principal__:

1. Este caso de uso comienza cuando el actor selecciona la opción “gestionar legajo” 
2. El sistema mostrará una pantalla en la cual podrá realizar búsqueda de alumnos por 3. distintos criterios o un alumno en particular.
4. El actor seleccionará un alumno de la lista o el alumno buscado.
5. El sistema mostrará por pantalla los datos de dicho alumno permitiendo al actor modificar los datos del alumno.
6. El actor podrá visualizar o modificar los datos, en caso de modificarlos el actor elige la opción “guardar” y da fin al caso de uso.

Titulo del Caso de Uso

Actores : Especificar actores

Objetivo : Especificar objetivos

Director de Flujo :

...
...
...
De ser necesario especificar cambios alternativos

## Arquitectura
La arquitectura propuesta para el sistema es Modelo, Vista y Controlador (MVC).

__Herramientas
- Editor de Texto: Visual Studio Code.
- Gestor de Paquetes: Maven.
- Framework Back-End: Javalin.
- Framework Front-End: Vue.js.
- Librerías para el Fron-End: Vuetify.
- Control de Versiones: Git y GitHub.
- Base de Datos: MariaDB.
- ...
