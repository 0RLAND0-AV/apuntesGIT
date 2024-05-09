# APUNTES GIT
apuntes del curso GIT de la SCESI
## CLASE 29/04/2024
### ¿QUE ES GIT?
Es un control de versiones distribuido.  
Te registra los cambios que haya en el codigo.  
Te permite tener un Historico.  
### ¿QUE ES UN REPOSITORIO?
Es como un directorio(CARPETA).  
Hay repositorio Local o Remoto  
Son donde se almacenan las diferentes versiones de los ficheros de un proyecto y el historico de cambios realizados.  
### INICIAR EN GIT  
### ¿Como crear e iniciar un proyecto?//Repositorio  
Comando Git: $git init <nuevoProyecto>    
              $cd nuevoProyecto  
### ¿Como iniciar un proyecto ya creado?  
Comando Git: $git <directorio del proyecto>    
              $git init 
### LOS 3 ESTADOS DE GIT:  
Modified:Cuando modificamos  
Staged: Preparamos los cambios a guardar  
Commited: Cuando guardamos los cambios  
### Comandos GIT para de los estados  
Comando Git: $git status  
              $git add <archivo modificado> //Lo agrega al area Staged  
              $git commit  
### ¿Que es un commit?
Sirven para guardar los cambios que se han producido en el repositorio.  Creas un punto de restauracion  
Comando Git: $git commit -m <Comentarios del cambio hechos en el fichero>  
### OTROS COMANDOS  
Comando Git: $git log //Para ver el historial de cambios  
              $git commit -amend -m <Comentarios> //Cambia el commit inicial (REVISAR)  
### ¿QUE ES HEAD?  
Es un puntero, te indica en que version estas  
Comando Git: $git checkout <ID de la anteriro version>  

  
## CLASE 01/05/2024  
### ¿QUE ES UNA RAMA?  
Son una instantanea(SnapShot) de la division del estado del codigo.  
Es un apuntador al ultimo commit  
Son como nuna calle que parte de una avenida principal.  
### ¿Para que sirven las ramas?  
Trabajo colaborativo  
Desarrollo no lineal y colaborativo  
Cada integrante del Equipo trabaja una parte y luego lo pueden juntar todo en uno.  
### ¿Como crear ramas?
Comando Git: $git branch "miPrimeraRama"
### ¿Como moverse entre ramas?
Comando Git: $git switch "ramaObjetivo" //Rama a la que nos queremos mover  
             $git checkout -b main "ramaObjetivo" //Rama a la que nos queremos mover  
### FUSIONAR RAMAS
Cuando creas ramas tienes dos opciones:  
Se fucionan todas las ramas o bifurcaciones al main.  
O se quedan en el olvido.  
### ¿Como fusionar ramas?
Comando Git: $git merge "ramaActual" //Cuando ejecutas estre comando, entonces fusionas la "ramaActual" al main(REVISAR)  
Ejemplo fusionando rama login:  
  $git merge login  
### COMANDO PARA SINCRONIZAR TU RAMA EN LA NUBE
Comando Git: $git push  
### ¿PORQUE ELIMINAMOS LAS RAMAS?
Para ahorrar espacio seas mamon xd.  
Por buenas practicas.  
Las ramas deben tener un solo proposito y una vida corta.  
### ¿Como eleiminar ramas?
Comando Git: $git branch -d <ramaEliminar>  
              $git branch -D <ramaEliminar> //Esto cuando la rama se la hace a las dificiles, Fuerza Bruta.  
### CONFLICTOS EN GIT  
Ocurren cuando al tratar de fusionar 2 ramas ambas presentan diferentes codigos en la misma linea (REVISAR).  
GIT  no es capaz de determinar que cambios es el que tiene que prevalecer una vez ocurra la FUSION.  
### Como abortar/cancelar un merge  
Comando Git: $git merge -abort  
