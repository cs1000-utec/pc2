# Gitflow

Meta: Utilizar `git` para ingresar código a un repositorio siguiendo la aún muy utilizada estrategia para manejo de branches conocida como [Gitflow](https://www.atlassian.com/git/tutorials/comparing-workflows/gitflow-workflow).

Pasos a seguir:

- Crear un repositorio e inicializarlo con un archivo README.md

- Tener creados/crear un branch `main` y un branch `development`.

- Asignar permisos a todos los integrantes (desde ahora conocido como equipo) menos a uno de ellos (desde ahora conocido como colaborador externo).

- Cada miembro del equipo debe crear un archivo `.md` en el cual hablen sobre un tema de programación de su elección, para ello deberá realizar los siguientes pasos:

  - Crear un Issue describiendo el cambio que realizaran.

  - Crear un branch con la extensión `feature/numerodeissues-detalles-del-cambio`. Por ejemplo: `feature/1-computer-vision`.

  - \* Agregar su archivo `.md` a dicho branch.

  - Crear un pull requests para que incluyan su branch a `development`.

  - Conseguir que el team apruebe el pull request y mergearlo a `development`.

- El colaborar externo debe realizar algo similar:

  - Crear un Issue describiendo el cambio que realizaran.

  - Realizar un fork del repositorio.
  
  - \* Agregar en su fork el nuevo archivo `.md`

  - Crear un pull requests para que incluyan su cambio en el branch `development`.

  - Conseguir que el team apruebe el pull request y mergearlo a `development`.

- Una vez que se mergearon todos los cambios, crear un branch `release/0.0.1` el cual nazca de `development`.

- Verificar que están todos los archivos en el branch `release/0.0.1`.

- Hacer un pull request para mergear `release/0.0.1` en `main`.

*Los puntos que empiezan con \* **deben** ser realizados desde el terminal. Anotar los comandos utilizados para ello.*

## Presentacion (3 mins)

- Explicar el flujo realizado y la ventaja del uso de branches y pull requests.

- Explicar el historial de commits del proyecto.

- Indicar los comandos utilizados para agregar los archivos a su propio branch desde el terminal y la manera en que crearon los branches, fork y pull request.