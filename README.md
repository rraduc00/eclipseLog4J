# eclipseLog4J
# @Author:  Razvan Raducu X5526828C
# Git repository url: https://github.com/rraduc00/eclipseLog4J.git
Repositorio para la práctica de integración de eclipse, log4j, github...

Después de intalar el IDE Eclipse tal y como viene indicado en la página, me encuentro que no tengo el plugin de Git aunque sí debería. Para instalarlo en Eclipse he hecho lo siguiente:
  Con Eclipse abierto: Help > Install new software
  He añadido la siguiente dirección: http://download.eclipse.org/egit/updates/
  He seleccionado todo ya que esto instalará JGit y EGit
  Cuando la instalación acaba me pide reiniciar eclipse y así lo he hecho.

Incorporar GIT.
	Lo primero que he hecho ha sido crear el projecto java en Eclipse y seguir los pasos que vienen indicados en la sección 6 de la práctica.
		1. Crearemos el proyecto
		2. Crear una carpeta lib y añadir los jar que se utilizaron en la práctica de
		Log4J
		3. Añadir los fuentes que se utilizaron en la práctica correspondiente
		(respetando los paquetes)
		4. Añadir el fichero log4j2.xml en un directorio creado para el proyecto y
		denominado <etc>
		5. Informar a tu proyecto que tiene que utilizar librerías extras disponibles
		en lib. Botón secundario sobre tu proyecto, Java Build Path, pestaña
		Libraries, Add external Jars.
		6. Informar al compilador que tiene que utilizar el fichero de configuración
		disponible en etc: Run As> run configurations> pestaña classpath>
		Seleccionar User Entries > Advanced > Add folder > seleccionar la
		carpeta <etc>
	Acto seguido, lo que he hecho ha sido cambiar a la vista git. Window > Perspective > Other Perspective > Other > Git
  	Acto seguido, he clonado el repositorio del enlace mencionado arriba. Clone a Git repositoy 
  	He indicado la ulr, next. No son necesarias credenciales puesto que el repositorio es público.
  	Acto seguido le he indicado la/s rama/s que quiero importar, en este caso sólo una, master.
  	Acto seguido he compartido mi proyecyo eclipse con ese repostorio. Para ello, click derecho en el proyecto. Team > Share Project > y he seleccionado el repositorio al que se lo he querido compartir puesto que, al clonarlo, ya lo tengo en local.
  	Con esto ya tengo el proyecto incorporado a eclipse y sincronizado con github. Mientras estoy escribiendo este readme (ya desde eclipse) voy a hacer un commit para guardar los cambios. Para ello desde el package explorer y habiendo guardado los resultados doy click derecho al proyecto > Team > Commit, añado todos los parámetros necesarios, como por ejemplo el mensaje y "Commit and Push"
  	Para hacer el commit hay que primero "stagear" los cambios. Lo que viene siendo hacer add desde la línea de comandos. Para ello hay que seleccionar el/los archivo/s que se quieran añadir en el commit and push y añadirlos al index.
