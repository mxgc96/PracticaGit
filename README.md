# PracticaGit

Cada estudiante debe crear su propio archivo dentro de este repositorio.

**Requisito:** haber aceptado la invitación como colaborador de este repositorio

---

## Paso 1. Crear una carpeta de prácticas y abrir la terminal (Git Bash) ahí

En el escritorio (o donde prefieras), crear una carpeta llamada, por ejemplo, `practicas-git`. Entrar a esa carpeta, clic derecho dentro de ella **Git Bash Here**.

## Paso 2. Crear la carpeta de esta práctica

```
mkdir Practica1
```

## Paso 3. Entrar a esa carpeta

```
cd Practica1
```

## Paso 4. Clonar este repositorio dentro de "Practica1"

```
git clone https://github.com/mxgc96/PracticaGit.git .
```

El punto final (`.`) al terminar el comando es importante: le dice a Git que clone el repositorio directamente dentro de la carpeta `Practica1` en la que ya estás, en vez de crear una carpeta nueva adentro.

**Aquí puede abrirse una ventana del navegador pidiendo iniciar sesión en GitHub o vincular tu cuenta**, es la forma en que Git confirma que tienes permiso de colaborador sobre este repositorio. Inicia sesión con tu propia cuenta de GitHub y continúa.

## Paso 5. Confirmar tu identidad

Solo si no realizaron este paso en la instalación

```
git config --global user.name "Tu Nombre Apellido"
git config --global user.email "tucorreo@ejemplo.com"
```

(el mismo correo con el que te agregaron como colaborador)

## Paso 6. Crear tu archivo con la primera línea

```
echo Primera linea en git > practica_1_nombre.txt
```

## Paso 7. Primer commit

```
git add practica_1_nombre.txt
git commit -m "Primer commit: primera linea"
```

## Paso 8. Agregar la segunda línea

```
echo Segunda linea en git >> practica_1_nombre.txt
```

(`>>` agrega la línea al final sin borrar la primera — un solo `>` la habría reemplazado por completo)

## Paso 9. Segundo commit

```
git add practica_1_nombre.txt
git commit -m "Segundo commit: segunda linea"
```

## Paso 10. Traer los cambios de tus compañeros antes de subir los tuyos

```
git pull
```

Si se abre una ventana de texto pidiendo un mensaje de "merge commit", no hay que escribir nada: guardar y cerrar tal cual. Git combina los archivos automáticamente porque cada quien creó uno distinto.

## Paso 11. Subir tus cambios (push)

```
git push
```

## Paso 12. Verificar en GitHub

Recarga esta página del repositorio en el navegador y confirma que tu
archivo `practica_1_nombre.txt` aparece en la lista, con tus dos commits en
el historial (pestaña **Commits**).
