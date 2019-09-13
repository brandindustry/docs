# Actualizar repositorio remoto

Procedimiento para actualizar el repositorio remoto con los nuevos cambios .

## Índice

- [Requerimientos](#Requerimientos)
- [Procedimiento](#Procedimiento)

## Requerimientos

- Haber llevado a cabo **todos** los pasos en la documentación: [Trabajar localmente](#).

## Procedimiento

*-- Como ejemplo contemplemos estar trabajando en un slider de fotos para la sección **Home** --*

1. Una vez probado todo, utiliza `git add .` para agregar los cambios realizados.
2. Utiliza `git commit -m 'slider home listo'` para fijarlos.
3. Envía los cambios a una *branch* remota con `git push origin slider_home`.
4. Cambia de *branch* a la principal (`master`) utilizando `git checkout master`.
5. Envía los cambios al `master` del repositorio remoto con `git push origin master`.