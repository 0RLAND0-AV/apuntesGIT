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
Comando Git: $git init < nuevoProyecto > 
              $cd nuevoProyecto  
### ¿Como iniciar un proyecto ya creado?  
Comando Git: git < directorio del proyecto >  
              $git init   
### LOS 3 ESTADOS DE GIT:  
Modified:Cuando modificamos  
Staged: Preparamos los cambios a guardar  
Commited: Cuando guardamos los cambios  
### Comandos GIT para de los estados  
Comando Git: $git status    //Muestra el estado de tu repositorio local  
              $git add < archivo modificado > //Lo agrega al area Staged  
              $git commit  
### ¿Que es un commit?
Sirven para guardar los cambios que se han producido en el repositorio.  Creas un punto de restauracion  
Comando Git: $git commit -m < Comentarios del cambio hechos en el fichero >    
### OTROS COMANDOS  
Comando Git: $git log //Para ver el historial de cambios  
              $git commit -amend -m < Comentarios > //Cambia el commit inicial (REVISAR)  
### ¿QUE ES HEAD?  
Es un puntero, te indica en que version estas  
Comando Git: $git checkout < ID de la anteriro version >  

  
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
Comando Git: $git branch < miPrimeraRama >
### ¿Como moverse entre ramas?
Comando Git: $git switch < ramaObjetivo > //Rama a la que nos queremos mover  
             $git checkout -b main < ramaObjetivo > //Rama a la que nos queremos mover  
### FUSIONAR RAMAS
Cuando creas ramas tienes dos opciones:  
Se fucionan todas las ramas o bifurcaciones al main.  
O se quedan en el olvido.  
### ¿Como fusionar ramas?
Comando Git: $git merge < ramaActual > //Cuando ejecutas estre comando, entonces fusionas la "ramaActual" al main(REVISAR)  
Ejemplo fusionando rama login:  
  $git merge login  
### COMANDO PARA SINCRONIZAR TU RAMA EN LA NUBE
Comando Git: $git push  
### ¿PORQUE ELIMINAMOS LAS RAMAS?
Para ahorrar espacio seas mamon xd.  
Por buenas practicas.  
Las ramas deben tener un solo proposito y una vida corta.  
### ¿Como eleiminar ramas?
Comando Git: $git branch -d < ramaEliminar >  
              $git branch -D < ramaEliminar > //Esto cuando la rama se la hace a las dificiles, Fuerza Bruta.  
### CONFLICTOS EN GIT  
Ocurren cuando al tratar de fusionar 2 ramas ambas presentan diferentes codigos en la misma linea (REVISAR).  
GIT  no es capaz de determinar que cambios es el que tiene que prevalecer una vez ocurra la FUSION.  
### Como abortar/cancelar un merge  
Comando Git: $git merge -abort  
## CLASE 02/05/2024  
### GITHUB  
### ¿Que es Git-Hub?¿Y para que sirve?  
GitHub es una plataforma de desarrollo colaborativo basada en Git que permite a los desarrolladores almacenar, gestionar y compartir su código y proyectos de software  
Un repositorio remoto en Git, como el que ofrece GitHub, es simplemente una copia de tu repositorio local que se almacena en un servidor remoto. Esto permite a los desarrolladores colaborar en proyectos, sincronizar cambios entre diferentes máquinas y mantener un historial completo de cambios para el proyecto. Los repositorios remotos como GitHub son fundamentales para el trabajo colaborativo y la distribución de software de código abierto.(Copiado de ChatGPT)
### SECCIONES DE GITHUB  
1.	Repositorios: Esta sección es donde se almacena todo el código de un proyecto. Los repositorios pueden ser públicos (visibles para todos) o privados (sólo visibles para los colaboradores autorizados). Cada repositorio contiene el historial completo de cambios, ramas y archivos del proyecto.  
2.	Issues: Las issues se utilizan para realizar un seguimiento de tareas, errores o mejoras propuestas en un proyecto. Cada issue puede tener etiquetas, asignaciones, comentarios y un estado (abierto, cerrado, etc.).  
3.	Pull Requests (solicitudes de extracción): Las pull requests se utilizan para proponer cambios en un repositorio. Cuando alguien envía una pull request, está proponiendo que se añadan los cambios que ha hecho en una rama de su repositorio al repositorio principal. Otros colaboradores pueden revisar los cambios, hacer comentarios y aprobar la pull request antes de fusionar los cambios en el repositorio principal.  
4.	Acciones (Actions): GitHub Actions te permite automatizar tu flujo de trabajo desde la gestión de compilaciones y pruebas hasta la implementación y entrega de tu código en cualquier lugar.  
5.	Proyectos: Los proyectos te permiten organizar y priorizar tu trabajo en GitHub. Puedes crear tableros personalizados con tarjetas que representan tareas, problemas o pull requests, y mover las tarjetas a través de columnas para realizar un seguimiento del progreso.  
6.	Wiki: Algunos repositorios tienen un wiki donde se pueden documentar detalles importantes del proyecto, como tutoriales, guías de instalación o especificaciones técnicas.  
7.	Pulse (Insights): La pestaña Pulse proporciona una visión general del estado y la actividad de tu repositorio, incluyendo gráficos de contribuciones, problemas abiertos y pull requests.  
8.	Configuración (Settings): En la configuración del repositorio, puedes gestionar la configuración general, como la colaboración, las notificaciones, las ramas predeterminadas, las acciones de GitHub, etc.
### PULL REQUEST  
¿Qué son los forks y los pull requests?   
Fork consiste en crear una copia personal de un repositorio existente. Esto permite a los desarrolladores trabajar en el código sin afectar el repositorio original. Las forks son útiles para:  
Probar cambios: Puedes experimentar con nuevas ideas y cambios en tu fork sin afectar la versión principal del código.  
Colaborar: Puedes compartir tu fork con otros desarrolladores para que puedan aportar sus ideas y sugerencias.  
Contribuir a proyectos de código abierto: Puedes crear un fork de un proyecto de código abierto y enviar un pull request para que tus cambios se integren en el repositorio principal.  
Pull requests (solicitudes de extracción) son una forma de proponer cambios a un repositorio existente. Una vez que hayas realizado tus cambios en tu fork, puedes crear un pull request. El pull request notificará a los mantenedores del repositorio original sobre tus cambios e iniciará un proceso de revisión. Los mantenedores pueden revisar tu código, proporcionar comentarios y decidir si desean fusionar tus cambios en el repositorio principal.  
### COMANDOS VISTOS EN CLASE  
Comando Git: $git push origin main //Envia los cambios del main al repositorio remoto(main)  
             $git remote -v //Ver los repositorios remotos enlazados  
              $git branch -a //Muestra las ramas remotas y locales  
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
Comando Git: git init < nuevoProyecto >    
              $cd nuevoProyecto  
### ¿Como iniciar un proyecto ya creado?  
Comando Git: git < directorio del proyecto >.    
              $git init 
### LOS 3 ESTADOS DE GIT:  
Modified:Cuando modificamos  
Staged: Preparamos los cambios a guardar  
Commited: Cuando guardamos los cambios  
### Comandos GIT para de los estados  
Comando Git: $git status    
              $git add < archivo modificado > //Lo agrega al area Staged  
              $git commit  
### ¿Que es un commit?
Sirven para guardar los cambios que se han producido en el repositorio.  Creas un punto de restauracion  
Comando Git: $git commit -m < Comentarios del cambio hechos en el fichero >    
### OTROS COMANDOS  
Comando Git: $git log //Para ver el historial de cambios  
              $git commit -amend -m < Comentarios > //Cambia el commit inicial (REVISAR)  
### ¿QUE ES HEAD?  
Es un puntero, te indica en que version estas  
Comando Git: $git checkout < ID de la anteriro version >  

  
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
Comando Git: $git branch < miPrimeraRama >
### ¿Como moverse entre ramas?
Comando Git: $git switch < ramaObjetivo > //Rama a la que nos queremos mover  
             $git checkout -b main < ramaObjetivo > //Rama a la que nos queremos mover  
### FUSIONAR RAMAS
Cuando creas ramas tienes dos opciones:  
Se fucionan todas las ramas o bifurcaciones al main.  
O se quedan en el olvido.  
### ¿Como fusionar ramas?
Comando Git: $git merge < ramaActual > //Cuando ejecutas estre comando, entonces fusionas la "ramaActual" al main(REVISAR)  
Ejemplo fusionando rama login:  
  $git merge login  
### COMANDO PARA SINCRONIZAR TU RAMA EN LA NUBE
Comando Git: $git push  
### ¿PORQUE ELIMINAMOS LAS RAMAS?
Para ahorrar espacio seas mamon xd.  
Por buenas practicas.  
Las ramas deben tener un solo proposito y una vida corta.  
### ¿Como eleiminar ramas?
Comando Git: $git branch -d < ramaEliminar >  
              $git branch -D < ramaEliminar > //Esto cuando la rama se la hace a las dificiles, Fuerza Bruta.  
### CONFLICTOS EN GIT  
Ocurren cuando al tratar de fusionar 2 ramas ambas presentan diferentes codigos en la misma linea (REVISAR).  
GIT  no es capaz de determinar que cambios es el que tiene que prevalecer una vez ocurra la FUSION.  
### Como abortar/cancelar un merge  
Comando Git: $git merge -abort  
## CLASE 02/05/2024  
### GITHUB  
### ¿Que es Git-Hub?¿Y para que sirve?  
GitHub es una plataforma de desarrollo colaborativo basada en Git que permite a los desarrolladores almacenar, gestionar y compartir su código y proyectos de software  
Un repositorio remoto en Git, como el que ofrece GitHub, es simplemente una copia de tu repositorio local que se almacena en un servidor remoto. Esto permite a los desarrolladores colaborar en proyectos, sincronizar cambios entre diferentes máquinas y mantener un historial completo de cambios para el proyecto. Los repositorios remotos como GitHub son fundamentales para el trabajo colaborativo y la distribución de software de código abierto.(Copiado de ChatGPT)
### SECCIONES DE GITHUB  
1.	Repositorios: Esta sección es donde se almacena todo el código de un proyecto. Los repositorios pueden ser públicos (visibles para todos) o privados (sólo visibles para los colaboradores autorizados). Cada repositorio contiene el historial completo de cambios, ramas y archivos del proyecto.  
2.	Issues: Las issues se utilizan para realizar un seguimiento de tareas, errores o mejoras propuestas en un proyecto. Cada issue puede tener etiquetas, asignaciones, comentarios y un estado (abierto, cerrado, etc.).  
3.	Pull Requests (solicitudes de extracción): Las pull requests se utilizan para proponer cambios en un repositorio. Cuando alguien envía una pull request, está proponiendo que se añadan los cambios que ha hecho en una rama de su repositorio al repositorio principal. Otros colaboradores pueden revisar los cambios, hacer comentarios y aprobar la pull request antes de fusionar los cambios en el repositorio principal.  
4.	Acciones (Actions): GitHub Actions te permite automatizar tu flujo de trabajo desde la gestión de compilaciones y pruebas hasta la implementación y entrega de tu código en cualquier lugar.  
5.	Proyectos: Los proyectos te permiten organizar y priorizar tu trabajo en GitHub. Puedes crear tableros personalizados con tarjetas que representan tareas, problemas o pull requests, y mover las tarjetas a través de columnas para realizar un seguimiento del progreso.  
6.	Wiki: Algunos repositorios tienen un wiki donde se pueden documentar detalles importantes del proyecto, como tutoriales, guías de instalación o especificaciones técnicas.  
7.	Pulse (Insights): La pestaña Pulse proporciona una visión general del estado y la actividad de tu repositorio, incluyendo gráficos de contribuciones, problemas abiertos y pull requests.  
8.	Configuración (Settings): En la configuración del repositorio, puedes gestionar la configuración general, como la colaboración, las notificaciones, las ramas predeterminadas, las acciones de GitHub, etc.
### PULL REQUEST  
***¿Qué son los forks y los pull requests?***  
Fork consiste en crear una copia personal de un repositorio existente. Esto permite a los desarrolladores trabajar en el código sin afectar el repositorio original. Las forks son útiles para:  
Probar cambios: Puedes experimentar con nuevas ideas y cambios en tu fork sin afectar la versión principal del código.  
Colaborar: Puedes compartir tu fork con otros desarrolladores para que puedan aportar sus ideas y sugerencias.  
Contribuir a proyectos de código abierto: Puedes crear un fork de un proyecto de código abierto y enviar un pull request para que tus cambios se integren en el repositorio principal.  
Pull requests (solicitudes de extracción) son una forma de proponer cambios a un repositorio existente. Una vez que hayas realizado tus cambios en tu fork, puedes crear un pull request. El pull request notificará a los mantenedores del repositorio original sobre tus cambios e iniciará un proceso de revisión. Los mantenedores pueden revisar tu código, proporcionar comentarios y decidir si desean fusionar tus cambios en el repositorio principal.  
### COMANDOS VISTOS EN CLASE  
Comando Git: $git push origin main //Envia los cambios del main al repositorio remoto(main)  
             $git remote -v //Ver los repositorios remotos enlazados  
              $git branch -a //Muestra las ramas remotas y locales  
               $git fetch //Actualiza tu repositorio local en base al repositorio remoto  
                $git remote remote prune origin //Elimina las ramas remotas de tu repo local  
## CLASE 06/05/2024  
### COMANDO GIT PUSH
En resumen el push sirve para enviar los cambios al repositorio remoto
1.    git push origin <branch>   : Envía los cambios de la rama local a la rama correspondiente en el repositorio remoto  origin .
2.    git push -u origin <branch>   : Configura la rama remota como la rama de seguimiento de la rama local especificada.
3.    git push origin --delete <branch>   : Elimina la rama especificada del repositorio remoto.
4.    git push --force   : Fuerza el envío de cambios al repositorio remoto, útil cuando se reescribe la historia del repositorio local.
### COMANDO GIT PULL
1.   git pull: El comando básico para obtener los últimos cambios del repositorio remoto y fusionarlos en tu rama local.
2.   git pull --rebase: Similar a git pull, pero reescribe el historial de commits local para que sea lineal. Útil para evitar conflictos de merge.
3.   git pull <remote-name> <branch-name>: Permite especificar el repositorio remoto y la rama específica desde la que se desea extraer e integrar los cambios.
4.   git pull --force: Fuerza la actualización local, incluso si hay conflictos de merge sin resolver. Úsalo con precaución.
5.   git pull --all: Obtiene e integra los cambios de todas las ramas remotas en tu repositorio local.
6.   git pull --prune: Elimina las ramas remotas que ya no existen en el repositorio remoto.
7.   



