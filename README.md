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
#ATENCIÓN

  	Los pasos que he mencionado anteriormente no han resultado satisfactorios pues el preoyecto seguía teniendo errores ya que las librerías no eran reconocidas por eclipse. Pongo a continuación los pasos que he realizado. Esta información la he encontrado en internet así que la pegaré tal y como está, original y en inglés. Aquí el enlace. http://syncor.blogspot.com.es/2013/09/getting-started-with-log4j-2-in-eclipse.html
  	
###Set up the log4j 2 library
These steps only needs to be done once for all the projects in your workspace.

Download the framework and unzip it. You can put it anywhere it’s easily accessible from Eclipse. I just decided to use the Program Files/Java folder under Windows.
Type “user” into Quick Access and select the User/Libraries Java Build Path option under preferences.
Click the New… button on the right (see the blue A in image below)
In the User library name: text box provide a name like log4j 2
Highlight the newly added name and click the Add External JARS… button (see the blue B in the image).
In the resulting dialog select the log4j-api-2.0*.jar and the log4j-core-2.0*.jar  files as shown in the image. The * will have the current suffix for your files which will likely be different from those shown as the product is currently in late beta.  Click the Open button to select the files and close the dialog.
Click OK to dismiss the Preferences dialog

###Add the Library to the ClassPath for your project
Right Click on your Project and Select Properties… to launch the Properties for your project

Select the Java Build Path Item and Select the Libraries tab
Click the Add Library… button
Select User Library and click on Next
Select the log4j library and click on Finish

###Set up your Run Configuration
You’ll do this step once for each run or debug configuration. We need to make the xml configuration file available when running our project. From the Run menu select Run Configurations… In the dialog switch to the Classpath tab and follow these steps (see the image).

Select the User Entries.
Click the Advanced… button.
In the resulting dialog select the Add Folders radio button.
Click OK.
This will launch a dialog allowing you to select a folder from your workspace; open up the current project.
Select the Log4j2 folder you created.
Click the OK button and close any dialogs just opened.

#Y ahora sí doy por finalizada la práctica. Este será el README que entregue en agora.
