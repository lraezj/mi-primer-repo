### **Básico GitGItHub**
 
## **5.	Crea un archivo llamado RECUPERACION.md donde expliques paso a paso:**

-	**Qué error simulaste.**
    - La eliminación del archivo creado "errores.sh" con `rm errores.sh`
-	**Qué comandos usaste para recuperar el archivo.**
    - Primero usamos el comando `git reflog` para ubicar el índice de la cabcera "HEAD", representando el commit previo a la eliminación del archivo.
	- Luego, con el índice "offset", ejecutamos `git reset --hard HEAD@{offset}` retornando así al commit previo a la eliminación y por ende el repositorio retrocede como un snapshot incluyendo el archivo eliminado.
-	**Qué aprendiste de la experiencia.**
    - Que existe la posibilidad que en la area de preparación (staging area), se pueda revertir cambios realizados en los archivos del repositorio pero igual queda un rastro de la actividad en el repositorio remoto y hasta local.

 