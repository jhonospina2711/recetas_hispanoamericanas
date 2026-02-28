## 6. Crear y extraer etiquetas

## Cree una etiqueta anotada para el último commit.

`git tag -a v1.0 -m 'Receta brasileña: Arrolladitos'`

![alt text](image.png)

## Liste las etiquetas del repositorio.

`git tag`

![alt text](image-1.png)

## Consulte la etiqueta creada en el primer punto.

`git show v1.0`

#3.Consulte la etiqueta creada en el primer punto.

![alt text](image-2.png)
#Este comando muestra toda la información relacionada con la etiqueta: su autor, la fecha, el commit correspondiente y una previsualización de los archivos involucrados.

## Elimine la etiqueta v1.0

`git tag -d v1.0 //la opción -d indica que se hará un delete de la etiqueta`

![alt text](image-3.png)

## 7. Comparar ramas

# Ejecute el siguiente comando para comparar dos ramas:

`git diff --name-status master..Brasil //la opción --name--status permite consultar el nombre de los archivos y su estado (Delete, Add or Modified)`

![alt text](image-4.png)
# El comando anterior permite comparar master con respecto a Brasil. Note que los archivos marcados con la letra A corresponden a los agregados en la sección anterior y el archivo marcado con la letra M corresponde al modificado.
# Este comando tiene muchas variaciones dependiendo de lo requerido.
# En el caso de querer consultar las diferencias incluyendo el contenido de los archivos implicados, utilice el comando:

`git diff master..Brasil`

# Si desea consultar el nombre y cantidad de archivos modificados, así como la cantidad de líneas insertadas o eliminadas, utilice el comando:

`git diff --stat master..Brasil //la opción --stat permite consultar la cantidad de archivos modificados y la cantidad de cambios`