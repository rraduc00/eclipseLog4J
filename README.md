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
  Para incorporar git a eclipse primero he cambiado la vista. Window > Perspective > Other Perspective > Other > Git
  Acto seguido, he clonado el repositorio del enlace mencionado arriba. Clone a Git repositoy 
  He indicado la ulr, next. No son necesarias credenciales puesto que el repositorio es público.
  Acto seguido le he indicado la/s rama/s que quiero importar, en este caso sólo una, master.
  Acto seguido lo he importado a Eclipse. Para ello desde la perspectiva de git, click derecho en el repositorio > Import projects > Import as a general project.
  Con esto ya tengo el proyecto incorporado a eclipse. Mientras estoy escribiendo este readme (ya desde eclipse) voy a hacer un commit para guardar los cambios. Para ello desde el package explorer y habiendo guardado los resultados doy click derecho al proyecto > Team > Commit, añado todos los parámetros necesarios, como por ejemplo el mensaje y "Commit and Push"
  Para hacer el commit hay que primero "stagear" los cambios. Lo que viene siendo hacer add desde la línea de comandos. Para ello hay que seleccionar el/los archivo/s que se quieran añadir en el commit and push y añadirlos al index.
