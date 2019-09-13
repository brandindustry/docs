# Actualizar repositorio local

Procedimiento para obtener cambios del repositorio remoto y poder trabajar localmente.

## Índice

- [Requerimientos](#Requerimientos)
- [Procedimiento](#Procedimiento)
- [Siguientes pasos](#Siguientes-Pasos)

## Requerimientos

- Tener el repositorio clonado
- Tener dado de alta el repositorio remoto como `git remote`
- Estar ubicado en el folder raíz del repositorio local
- Contar con la carpeta `scripts`

## Procedimiento

1. Obtén los cambios más recienes hechos al código usando `git pull origin master`
2. Obtén los datos más recienes guardados en la base de datos usando `scripts/pull_db.sh`
3. Obtén los *assets* más recientes usando `scripts/pull_assets.sh`

## Siguientes pasos

- Si no hay errores en ninguno de los pasos del procedimiento, procede a trabajar en los cambios de acuerdo a la documentación: [Trabajar localmente](../2_trabajarLocalmente/README.md).