# Guía para utilizar un repositorio
Este documento tiene la intención de dar una guía basica sobre como manejar un repositorio. Cada equipo podra seguir esta guía o adecuarla segun necesite.
## 1. Ramas principales
Se tendran 2 ramas: `master` y `dev`. La rama `master` tendra el codigo que se vera en el sitio en producción y `dev` en el ambiente de desarrollo.

## 2. Ramas secundarias
Por cada tarea, corrección o funcionalidad, se debera crear la rama desde `master`.
```
git checkout master
git checkout -b NUEVA_RAMA
```

### 2.1. Nombres para ramas secundarias
Esto es a criterio del equipo pero se sugiere usar el siguiente formato:
- Para una nueva vista o funcionalidad: `feat/login_page`.
- Para corregir un error: `fix/update_error_message`.

## 3. Commits semanticos
Se debera usar commits semanticos, parecidos a lo que se menciona en este [articulo](https://gist.github.com/joshbuchea/6f47e86d2510bce28f8e7f42ae84c716) pero con algunas variaciones segun acuerde el equipo.

### 3.1. Estructura de un commit
No se esta tomando en scope y todo se debera escribir en letras minusculas.
- Nueva vista o funcionalidad `feat: add login page`.
- Agregar una corrección `fix: update email error message`.
- Agregar o actualizar documentación o comentarios: `docs: add login endpoint doc`.
- Refactorizar una función: `refactor: update authentication method`.
- Agregar o actualizar configuraciones para deployment, building, etc: `chore: add circle ci`.
- Agregar o actualizar tests: `test: add test for authentication endpoint`.
