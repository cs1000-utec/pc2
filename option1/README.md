# Gitflow

Opción 1

## Objetivo

Utilizar `git` para ingresar código a un repositorio siguiendo la aún muy utilizada estrategia para manejo de branches conocida como [Gitflow](https://www.atlassian.com/git/tutorials/comparing-workflows/gitflow-workflow).

## Pasos a seguir

### Preparación

- Crear un repositorio e inicializarlo con un archivo README.md

- Tener creados/crear un [branch](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-and-deleting-branches-within-your-repository#creating-a-branch) `main` y un branch `development`.

- Asignar permisos a todos los integrantes (desde ahora conocido como **equipo**) menos a uno de ellos (desde ahora conocido como **colaborador externo**).

### Pasos a realizar por el *Equipo*

- Cada miembro del equipo debe crear un archivo `.md` en el cual hablen sobre un tema de Computer Science de su elección (e.g. computer vision, AI, NLP, etc...), para ello deberá realizar los siguientes pasos:

  - Crear un [Issue](https://docs.github.com/en/issues/tracking-your-work-with-issues/creating-an-issue#creating-an-issue-from-a-repository) describiendo el cambio que realizaran.

  - Crear un branch con la extensión `feature/numerodeissues-detalles-del-cambio`. Por ejemplo: `feature/1-computer-vision`.

  - Agregar su archivo `.md` a dicho branch. (Este paso debe necesariamente ser desarrollado desde el terminal)

  - Crear un [pull requests](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request) para que incluyan su branch a `development`.

  - Conseguir que todos los miembros del **equipo** aprueben el pull request y mergearlo a `development`.

### Pasos a realizar por el *Colaborador Externo*

- El colaborador externo debe realizar algo similar:

  - Crear un Issue describiendo el cambio que realizaran.

  - Realizar un [fork](https://docs.github.com/en/get-started/quickstart/fork-a-repo) del repositorio.
  
  - Agregar en su fork el nuevo archivo `.md`. (Este paso debe necesariamente ser desarrollado desde el terminal)

  - Crear un pull request para que incluyan su cambio en el branch `development`.

  - Conseguir que el todo los miembros del **equipo** apruebe el pull request y mergearlo a `development`.

## Testing release

- Una vez que se mergearon todos los cambios, crear un branch `release/0.0.1` el cual nazca de `development`.

## Final release

- Verificar que están todos los archivos en el branch `release/0.0.1`.

- Hacer un pull request para mergear `release/0.0.1` en `main`.

- Todos los miembros del **equipo** deben aprobar el pull request y mergear a `main`.

*Anotar los comandos utilizados para las operaciones que realice desde el terminal.*

## Presentacion (3 mins)

- Dar una breve explicación:
  - Branches
  - Fork
  - Pull requests

- Explicar el historial de commits del proyecto detallando lo utilizado en cada parte.

## Información adicional para el README

Incluir en el README.md del proyecto captura(s) de pantalla de:

- Historial de commits
- Comandos que usaron desde el terminal