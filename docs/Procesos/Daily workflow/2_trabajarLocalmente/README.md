# Trabajar localmente

Procedimiento a seguir para realizar cambios loclamente a un proyecto

## Índice

- [Requerimientos](#Requerimientos)
- [Procedimiento](#Procedimiento)
- [Siguientes pasos](#Siguientes-Pasos)

## Requerimientos

- Haber actualizado el repositorio local de acuerdo con la documentación: [Actualizar repositorio local](#).

## Procedimiento

*-- Como ejemplo contemplemos estar trabajando en un slider de fotos para la sección **Home** --*

1. Crear una nueva *branch* con un nombre que describa claramente los cambios a realizar. Usando el ejemplo: `git checkout -b slider_home`
2. Realiza los cambios al código que sean necesarios. Para compilar en tiempo real tus cambios a *js* o *sass*, utiliza el comando `npm run watch`.
3. Una vez terminados los cambios, detén el `watch` con `ctrl+z`. 
4. A continuación, utiliza `npm run production` para minificar tu *js* y *css*.
5. Revisa que todos los cambios estén funcionando adecuadamente.

## Siguientes pasos

- Procede a actualizar el repositorio remoto siguiendo la documentación: [Actualizar repositorio remoto](#).