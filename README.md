# Creación y sincronización de repositorios con Git y GitHub

## Datos del estudiante

- **Nombre:** Oskar Tadeo Alvarez Nájera
- **Matrícula:** 2630002
- **Nombre de la práctica:** Creación y sincronización de repositorios con Git y GitHub

## Objetivo de la práctica

Aprender a utilizar **Git** para crear y administrar repositorios, así como enviar los archivos de un repositorio local a **GitHub** y realizar modificaciones desde GitHub para después sincronizarlas nuevamente con el repositorio local.

## Comandos de Git utilizados

Durante la práctica se utilizaron diferentes comandos básicos de Git para crear, modificar y sincronizar el repositorio.

| Comando | Función |
|---|---|
| `git init` | Crea un nuevo repositorio local de Git. |
| `git status` | Muestra el estado actual de los archivos del repositorio. |
| `git add .` | Agrega todos los archivos modificados al área de preparación. |
| `git commit -m "mensaje"` | Guarda los cambios realizados en el repositorio con un mensaje. |
| `git branch -M main` | Cambia el nombre de la rama actual a `main`. |
| `git remote add origin URL` | Vincula el repositorio local con un repositorio remoto de GitHub. |
| `git push -u origin main` | Envía los cambios del repositorio local a GitHub. |
| `git pull origin main` | Descarga y combina los cambios realizados en GitHub con el repositorio local. |
| `git clone URL` | Crea una copia local de un repositorio existente en GitHub. |
| `git log` | Muestra el historial de cambios y commits del repositorio. |

## Explicación breve de la función de cada comando

### `git init`

Se utiliza para iniciar un repositorio de Git dentro de una carpeta local.

```bash
git init
```

### `git status`

Permite conocer qué archivos han sido modificados, agregados o están pendientes de guardar.

```bash
git status
```

### `git add .`

Agrega los archivos y cambios al área de preparación antes de realizar un commit.

```bash
git add .
```

### `git commit`

Guarda los cambios en el historial del repositorio.

```bash
git commit -m "Primer commit"
```

### `git branch -M main`

Establece el nombre de la rama principal como `main`.

```bash
git branch -M main
```

### `git remote add origin`

Permite conectar el repositorio local con un repositorio creado en GitHub.

```bash
git remote add origin URL_DEL_REPOSITORIO
```

### `git push`

Envía los commits del repositorio local hacia GitHub.

```bash
git push -u origin main
```

### `git pull`

Descarga los cambios que existen en GitHub y los integra en el repositorio local.

```bash
git pull origin main
```

### `git clone`

Permite descargar un repositorio que ya existe en GitHub y crear una copia local.

```bash
git clone URL_DEL_REPOSITORIO
```

### `git log`

Muestra los commits realizados anteriormente y permite consultar el historial del proyecto.

```bash
git log
```

## Explicación de cómo se creó el repositorio local

Primero se creó una carpeta para almacenar los archivos de la práctica. Después se abrió una terminal dentro de dicha carpeta y se utilizó el comando `git init` para convertirla en un repositorio local.

```bash
git init
```

Posteriormente se agregaron los archivos al área de preparación utilizando:

```bash
git add .
```

Después se creó el primer commit para guardar los cambios:

```bash
git commit -m "Primer commit"
```

De esta manera se creó el repositorio local y se registró la primera versión del proyecto.

## Explicación de cómo se vinculó el repositorio local con GitHub

Después de crear el repositorio local, se creó un repositorio nuevo en GitHub.

Para conectar ambos repositorios se utilizó el comando:

```bash
git remote add origin URL_DEL_REPOSITORIO
```

Después se estableció la rama principal como `main`:

```bash
git branch -M main
```

Finalmente, se enviaron los archivos del repositorio local a GitHub mediante:

```bash
git push -u origin main
```

Con esto, el repositorio local quedó vinculado con el repositorio remoto de GitHub.

## Explicación de la sincronización Local → GitHub

Para enviar los cambios realizados en el equipo local hacia GitHub, primero se modificaron o agregaron los archivos necesarios.

Después se utilizó:

```bash
git add .
```

Para preparar los cambios.

Posteriormente se creó un commit:

```bash
git commit -m "Actualización de archivos"
```

Finalmente, los cambios fueron enviados a GitHub con:

```bash
git push
```

El proceso básico puede representarse de la siguiente manera:

```text
Repositorio Local
       |
       | git add
       v
Área de preparación
       |
       | git commit
       v
Historial de Git
       |
       | git push
       v
     GitHub
```

## Explicación de la sincronización GitHub → Local

Cuando se realizan cambios directamente desde GitHub, estos cambios deben descargarse al repositorio local para mantener ambos repositorios actualizados.

Para realizar esta sincronización se utiliza:

```bash
git pull origin main
```

Este comando descarga los cambios realizados en el repositorio remoto y los integra en la copia local.

El proceso puede representarse de la siguiente manera:

```text
     GitHub
       |
       | git pull
       v
Repositorio Local
```

De esta forma, el repositorio local puede mantenerse actualizado con los cambios realizados desde GitHub.

## Descripción de los archivos contenidos en el repositorio

El repositorio contiene los archivos utilizados durante la práctica de Git y GitHub.

| Archivo | Descripción |
|---|---|
| `README.md` | Contiene la información de la práctica, los comandos utilizados y las explicaciones del proceso. |
| Otros archivos de la práctica | Contienen los ejercicios o actividades realizadas durante la práctica. |

Los archivos pueden modificarse localmente y posteriormente sincronizarse con GitHub mediante los comandos de Git.

## Conclusión personal sobre lo aprendido

Durante esta práctica aprendí a utilizar Git para crear y administrar un repositorio local y posteriormente conectarlo con GitHub. También aprendí a utilizar comandos básicos como `git init`, `git add`, `git commit`, `git push` y `git pull`.

Comprendí que Git permite llevar un historial de los cambios realizados en un proyecto, mientras que GitHub permite almacenar el repositorio en línea y trabajar con él desde diferentes lugares. La práctica también me ayudó a entender la diferencia entre enviar cambios del repositorio local a GitHub y descargar cambios de GitHub al repositorio local.

En conclusión, Git y GitHub son herramientas útiles para organizar proyectos, guardar versiones de los archivos y mantener sincronizados los cambios.
