# ¿Qué es un changelog?

Un changelog es un archivo que contiene una lista *ordenada cronológicamente*
de los cambios *notables* para cada versión de un proyecto.

# ¿Por qué mantener un changelog?

Para que sea más fácil para las usuarias y colaboradoras ver exactamente qué
cambios notables se han realizado entre cada lanzamiento (o versión) del proyecto.

Las usuarias del software, ya sean consumidoras finales o desarrolladoras,
son seres humanos que se preocupan por lo que hay en el
software. Cuando el software cambia, la gente quiere saber por qué y cómo. 
Ayuda a las usuarioa a decidir si actualizar o no a una nueva versión del software.
Ayuda a las desarrolladoras a rastrear los cambios que se han realizado en el software
y les facilita la resolución de problemas cuando algo sale mal.

En el caso particular del Bootcamp WebDev de Laboratoria, mantener un changelog
para cada proyecto que desarrolles, tiene los siguientes objetivos:
- Que identifiques los avances sprint a sprint en tu proyecto
- Que identifiques los aprendizajes sprint a sprint por tu proyecto
- Que evalúes la calidad y utilidad de los mensajes de tus commits

# ¿Qué formato debo usar para el Changelog de un proyecto de Laboratoria?

En primer lugar, debes crear un archivo `CHANGELOG.md` en la raíz de tu proyecto.

Luego, al terminar cada sprint, antes de la ceremonia de _Sprint Review_, deberás agregar una nueva entrada
al inicio del archivo con los avances y aprendizajes del último sprint, usando el siguiente formato:

```md
## <version> - <date>

### Sprint learnings

En esta sección enumera los aprendizajes del sprint.

### Added

En esta sección especifica las funcionalides que agregaste.

### Changed

En esta sección detalla los cambios que hiciste a funcionalides ya existentes.

### Fixed

En esta sección describe los _bugs_ solucionados.

### Removed

En esta sección incluye las funcionalidades eliminadas.

```
En el formato anterior, deberás reemplazar `<version>` por el número de la nueva versión liberada
por ejemplo 1.0.1 y `<date>` por la fecha de liberacion en formato YYYY-MM-DD por ejemplo 2023-09-20.

El número de versión deberá usar el estándar de [Semantic Versioning](https://semver.org/),
que estable que:

>Dado un número de versión MAYOR.MENOR.PARCHES, incrementa lo siguiente:
>
>    MAYOR versión cuando realizas cambios incompatibles en la API
>
>    MENOR versión cuando agregas funcionalidad de manera compatible hacia atrás
>
>    PARCHES versión cuando realizas correcciones de errores compatibles hacia atrás

# Consulta de commits en el sprint

Puedes ejecutar el siguiente comando para consultar los mensajes de los commits que haz hecho
en los últimos 7 días en todas las ramas en tu repositorio y con ello construir tu changelog:

``git log --all --since='7 days ago' --oneline --format="* %h %s (%an) %as"``

El resultado de este comando podrá verse como lo siguiente:

>* 4a87adb refactor in request hook (Carlos Gonzalez) 2023-09-19
>* 388f431 README improvements (Sergio Sinuco) 2023-09-19
>* 509bcf8 Adjust readme with images and components description, adjusted some types and params (Kvn Alvarado) 2023-09-18

# Ejemplo

En el archivo [EXAMPLE.md](./EXAMPLE.md) encontrarás un changelog de ejemplo.


