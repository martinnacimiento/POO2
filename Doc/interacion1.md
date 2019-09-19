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


![alt text](https://github.com/Nacimiento98/POO2/blob/master/Imagenes/IMG_20190919_151337669.jpg "Pantalla 1")

Pantalla 1

![alt text](https://github.com/Nacimiento98/POO2/blob/master/Imagenes/IMG_20190919_150015857.jpg "Pantalla 2")

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

__Imprimir novedades__

__Actores__: Director

__Objetivo__: Generar un documento con las novedades que serán enviados al consejo de educación dos veces al año


__Flujo Principal__:

1. Este C.U comienza cuando el director selecciona la opción “ver novedades”.
2. El sistema muestra una pantalla con todas las novedades.
3. El director podrá realizar un filtrado por fecha, tipo de novedad, curso,etc.
4. El sistema mostrará aquellas novedades que cumplan con el filtro.
5. El director presionara el botón generar PDF.
6. El sistema generará un PDF con todos los datos generados.

__Generar legajo__

__Actores__: Preceptor

__Objetivo__: Gestionar legajo para cada alumno que ya esté pre inscripto en el sistema

__Flujo Principal__:

1. Este C.U comienza cuando el actor selecciona la opción “gestionar legajo” 
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

- ...
- ...
- ...
- ...
