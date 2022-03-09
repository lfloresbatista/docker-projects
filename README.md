# docker-projects

Estos son algunos de los proyectos en los que he trabajado con docker, mayormente han sido gracias a la contribucion de otros techs, con algunos cambios mios, de igual forma dejare link de las referencias que utilice. 

Espero que los disfruten y le pueda servir a aquel que esta en busca de conocimiento y es muy importante compartir entre todos.

|| These are some of the projects in which I worked with docker, mostly thanks to the contribution of other techs, with some changes of mine, in the same way I will leave a link of the references that I use.

I hope you enjoy them and can serve those who are in search of knowledge and it is very important to share with everyone.


<h2>Contenido</h2>

<h3>
  1. <a href=https://github.com/lfloresbatista/docker-projects/tree/main/NginX-LetsEncrypt-Mysql>Nginx + Let's Encrypt + Mysql</a>
</h3>
   <br>
   <strong>Descp:</strong> Este yaml es buenisimo si lo que quieres es tener un servidor proxy que diriga la solicitud hacia el contenedor especifico, sin tener que estar creando o modificando todo cada que creas un contenedor, ya que la imagen de <b>jwilder</b> lo hace, conectandose al sock de docker y creandolo, adicional se conecta al volumen de CA de letsencrypt en read-only.
   <br>
   <br>
   <b>Mis practicas y comentarios :</b> Bueno despues de varios labs, me dije cada vez que cree un contenedor de servicio para mis usuarios, como wordpress, nextcloud, etc, tengo que modificar el docker compose (bueno el stack porque utilizo portainer, luego mas adelante agrego algo de ello) entonces me dije mejor los contendores que trabajan en background, que a mis usuarios no les interesa, por lo menos no los de IT, los voy a tirar afuera de este yaml, Porque? sencillo si yo necesito destruir uno, no necesito reiniciar mis servicios como el proxy, letsencrypt y mysql, basta con crear la base de datos desde el exec de docker o el cli de portainer, su usuario para esa app especifica y apuntarle los puertos virtuales para mi proxy y me CA, asi que si yo basicamente lo que hago es esos contenedores los corro fuera o por decirlo fuera del yaml donde estan estas app principales.
   


