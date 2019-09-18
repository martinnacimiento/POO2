# GEAS

## Grupo: Los 4 Fantásticos

1. Añais, Raul Alejandro
2. Nacimiento, Francisco Martin
3. Potocki, Joaquín
4. Silveira Do Santo, Facundo Omar
 
## Visión 

Gestión automatizada de alumnos de la escuela secundaria EPET Nro 38, localizada en la ciudad de San Pedro, Misiones. El sistema permitirá a los usuarios (Docentes, preceptores y directivos), automatizar las actividades repetitivas y ahorrar tiempo. Estas actividades están centradas en la gestión de los legajos, los libros de evaluacion, gestionar pases, promover alumnos y generar el LUA (Legajo Unico del Alumno), con los reportes de novedades sobre las altas, bajas y pases de alumnos.

## Lista de características

1. Inscribir Alumno.
2. Gestionar legajos. 
3. Imprimir libretas. 
4. Tomar Asistencias.
5. Generar Libro de evaluación.
6. Promover alumnos.
7. Cargar Notas.
8. Enviar Reportes de asistencias a los padres. 
9. Generar LUA.
10. Gestionar los pases.


## Análisis de Dominio

...

## Bocetos de Interfaz de Usuario


![alt text](https://github.com/cbiale/POO2/blob/master/iteraci%C3%B3n_1/oop.png "Pantalla 1")

Pantalla 1

## Casos de Uso

### Actores

1. Preceptor: Es el encargado de la gestion administrativa de los alumnos.
2. Docente: Es el encargado de Calificar a un alumno y entregar planilla de notas de su materia.

...

_Por cada caso de uso especificar_

__Inscribir Alumno__

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

__Titulo del Caso de Uso__

__Actores__: Especificar actores

__Objetivo__: Especificar objetivos

__Flujo Principal__:

1. ...
2. ...
3. ...

_De ser necesario especificar flujos alternativos_

## Arquitectura

- ...
- ...
- ...
- ...
