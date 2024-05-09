# APUNTES GIT
apuntes del curso GIT de la SCESI
## CLASE 01/05/2024
#### ¿QUE ES UNA RAMA?
Son una instantanea(SnapShot) de la division del estado del codigo.
Es un apuntador al ultimo commit
Son como nuna calle que parte de una avenida principal.
#### ¿PARA QUE SIRVEN LAS RAMAS?
Trabajo colaborativo
Desarrollo no lineal y colaborativo
Cada integrante del Equipo trabaja una parte y luego lo pueden juntar todo en uno.
### ¿COMO CREAR RAMAS?
Comando Git: $git branch "miPrimeraRama"
### ¿COMO MOVERSE ENTRE RAMAS?
Comando Git: $git switch "ramaObjetivo" //Rama a la que nos queremos mover  
             $git checkout -b main "ramaObjetivo" //Rama a la que nos queremos mover  
### FUSIONAR RAMAS
Cuando creas ramas tienes dos opciones:  
Se fucionan todas las ramas o bifurcaciones al main.  
O se quedan en el olvido.  
### ¿COM0 FUSIONAR RAMAS?
Comando Git: $git merge "ramaActual" //Cuando ejecutas estre comando, entonces fusionas la "ramaActual" al main(REVISAR)  
Ejemplo fusionando rama login:  
  $git merge login  
### COMANDO PARA SINCRONIZAR TU RAMA EN LA NUBE
Comando Git: $git push  
### ¿PORQUE ELIMINAMOS LAS RAMAS?
Para ahorrar espacio seas mamon xd.  
Por buenas practicas.  
Las ramas deben tener un solo proposito y una vida corta.  

