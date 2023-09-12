# ¿Qué es un changelog?

Un changelog es un archivo que contiene una lista *ordenada cronológicamente*
de los cambios *notables* para cada versión de un proyecto.

# ¿Por qué mantener un changelog?

Para que sea más fácil para los usuarios y colaboradores ver exactamente qué
cambios notables se han realizado entre cada lanzamiento (o versión) del proyecto.

Los usuarios del software, ya sean consumidores finales o desarrolladores,
son seres humanos que se preocupan por lo que hay en el
software. Cuando el software cambia, la gente quiere saber por qué y cómo. 
Ayuda a los usuarios a decidir si actualizar o no a una nueva versión del software.
Ayuda a los desarrolladores a rastrear los cambios que se han realizado en el software
y les facilita la resolución de problemas cuando algo sale mal.

En el caso particular del Bootcamp WebDev de Laboratoria, mantener un changelog
para cada proyecto que desarrolles, tiene los siguientes objetivos:
- Identificar los avances sprint a sprint en tu proyecto
- Identificar los aprendizajes sprint a sprint por tu proyecto
- Evaluar la calidad y utilidad de los mensajes de tus commits

# ¿Qué formato debo usar para el Changelog de un proyecto de Laboratoria?

En primer lugar, debes crear un archivo `CHANGELOG.md` en la raíz de tu proyecto.

Luego, al terminar cada sprint, antes de la ceremonia de _Sprint Review_, deberás agregar una nueva entrada
al inicio del archivo con los avances y aprendizajes del último sprint, usando el siguiente formato:

```
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
y `<date>` por la fecha de liberacion en formato YYYY-MM-DD.

# Ejemplo

En el archivo [EXAMPLE.md](./EXAMPLE.md) encontrarás un changelog de ejemplo.


