# Repositorio Ejercicio-git-branch
## Paso 1
Crear este repositorio ejercicio-git-branch

## Paso 2
Realizar clonación del repositorio.

```code
bae2@jpexposito-VirtualBox:~/Documentos$ git clone https://github.com/GabrielHerreraGanzo/ejercicio-git-branch.git
Clonando en 'ejercicio-git-branch'...
remote: Enumerating objects: 3, done.
remote: Counting objects: 100% (3/3), done.
remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
Recibiendo objetos: 100% (3/3), listo.
```
## Paso 3
Crear una nueva branch o rama para los nuevos cambios que vas a introducir.

**Utilizando:** git branch ejercicio1-branch **Y después utilizo:** git checkout  ejercicio1-branch
```code
bae2@jpexposito-VirtualBox:~/Documentos/ejercicio-git-branch$ git branch ejercicio1-branch
bae2@jpexposito-VirtualBox:~/Documentos/ejercicio-git-branch$ git checkout  ejercicio1-branch
Cambiado a rama 'ejercicio1-branch'
```
## Paso 4
Añado esta clase al repositorio:

```java
public class Ejercicio1 {
     public static void main(String[] args) {
         System.out.println("Ejercicio 1 realizado.");
     }
 }
```

## Paso 5
Realizar commit de los cambios:

```code
bae2@jpexposito-VirtualBox:~/Documentos/ejercicio-git-branch$ git commit -m "Creo un Branch e incluyo el Ejercicio1.java"
[ejercicio1-branch fea53b7] Creo un Branch e incluyo el Ejercicio1.java
 1 file changed, 10 insertions(+), 1 deletion(-)
```

## Paso 6 
Subo los cambios al repositorio. **Utilizando:** git push origin ejercicio1-branch

```code
bae2@jpexposito-VirtualBox:~/Documentos/ejercicio-git-branch$ git push origin ejercicio1-branch
Username for 'https://github.com': GabrielHerreraGanzo
Password for 'https://GabrielHerreraGanzo@github.com': 
Enumerando objetos: 8, listo.
Contando objetos: 100% (8/8), listo.
Compresión delta usando hasta 4 hilos
Comprimiendo objetos: 100% (4/4), listo.
Escribiendo objetos: 100% (6/6), 1023 bytes | 511.00 KiB/s, listo.
Total 6 (delta 1), reusados 0 (delta 0), pack-reusados 0
remote: Resolving deltas: 100% (1/1), done.
remote: 
remote: Create a pull request for 'ejercicio1-branch' on GitHub by visiting:
remote:      https://github.com/GabrielHerreraGanzo/ejercicio-git-branch/pull/new/ejercicio1-branch
remote: 
To https://github.com/GabrielHerreraGanzo/ejercicio-git-branch.git
 * [new branch]      ejercicio1-branch -> ejercicio1-branch
```

## Paso 7
Fusionar la nueva branch (ejercicio1-branch) con la main.

Cambio al main y luego fuisono la rama.

```code
bae2@jpexposito-VirtualBox:~/Documentos/ejercicio-git-branch$ git checkout main
Cambiado a rama 'main'
Tu rama está actualizada con 'origin/main'.
bae2@jpexposito-VirtualBox:~/Documentos/ejercicio-git-branch$ git merge ejercicio1-branch
Actualizando 3ebbb08..b26e012
Fast-forward
 README.md | 60 +++++++++++++++++++++++++++++++++++++++++++++++++++++++++++-
 1 file changed, 59 insertions(+), 1 deletion(-)
```
Subo los cambios con git push

```code
bae2@jpexposito-VirtualBox:~/Documentos/ejercicio-git-branch$ git push origin main
Username for 'https://github.com': GabrielHerreraGanzo
Password for 'https://GabrielHerreraGanzo@github.com': 
Enumerando objetos: 5, listo.
Contando objetos: 100% (5/5), listo.
Compresión delta usando hasta 4 hilos
Comprimiendo objetos: 100% (2/2), listo.
Escribiendo objetos: 100% (3/3), 503 bytes | 503.00 KiB/s, listo.
Total 3 (delta 1), reusados 0 (delta 0), pack-reusados 0

remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/GabrielHerreraGanzo/ejercicio-git-branch.git
   3ebbb08..229b1b0  main -> main
```



