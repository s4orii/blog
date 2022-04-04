# Reparar ModuleNotFoundError: No module named


Muchas veces a la hora de ejecutar un exploit , un programa o un simple _script_ nos a pasado que *python*
arroje un error por el modulo que se desea usar.
 
![error](/assets/img/errorinpy/nomodule.png)

Lo más lógico sería ir a google a buscar el error y encontrar en diversos sitios americanos como repararlo.
pero para ahorrar ese tiempo valioso , lo resumiré en un post _(Específicamente este.)_

# Solución 1
Harémos lo más lógico. En el buscador adaptaremos nuestra busqueda a ___'' [Nombre del modulo] python [Version de python]''___
en este caso usare de ejemplo el de el error de la primera foto , el modulo _requests_

![solu1](/assets/img/errorinpy/formato.png)

y entraremos donde este nuestro paquete junto a su version y la web ___- PyPI___

![solu2](/assets/img/errorinpy/ejemplo.png)

y tal como dice el sitio , lo instalaremos con _pip_ y su correspondiente sintaxsis.

![solu3](/assets/img/errorinpy/solucion1.png)

# Solucion 2

Si lo previamente mostrado no dio frutos entorno a nuestro error , haremos lo siguiente.
Buscaremos el _git_ o _github_ de nuestro modulo, siguiendo el ejemplo previo , buscaremos el git de requests.

![xd](/assets/img/solu2/busqueda.png)

![ft2](/assets/img/solu2/github.png)

Una vez dentro del repositorio lo clonaremos con la sintaxis: 
>git clone https://github.com/psf/requests.git 

El enlace para  copiarlo es obtenido del mismo repositorio , en una cuadrado verde donde dice _code_.


![ft3](/assets/img/solu2/clonar.png)

Una vez clonado , nos moveremos dentro del repositorio
>cd requests

y haremos una instalacion con el _setup_ que viene en el mismo repositorio , lo instalaremos con la version de python a la cual querramos instalarle el _modulo_ con el siguiente comando.
>**Python3**


>sudo python3 setup.py install


>**Python2** 


>sudo python2 setup.py install

y ya se te instalara el modulo en tu python de version 3 _(o 2)_

![ft4](/assets/img/solu2/python3.png)

y listo! , ya puedes reventar ese el RCE con tu exploit en python3 :).



_-s4ori_

