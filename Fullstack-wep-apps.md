# <center/>Build and deploy fullstack web apps with NodeJS, React, Redux, Express, and MongoDB.


### Recursos del curso:

    1. Udemy Discussion Threads
    2. Google
    3. Stackoverflow
    4. Kreic

### Diagramas:

    1. Bajemos el archivo y lo extraemos en algún lado de nuestra computadora.
    2. Visitar diagrams.net
    3. Clickear en "Open Existing Diagram" y lo buscamos dentro de nuestra computadora.
    4. Seleccionamos "Open From DEvice" y utilizamos el file explorer para seleccionar el archivo del diagrama de nuestra computadora.

#
# <center/>Feedback Collection Application

Vamos a targetear **Product Managers** o **Startups** y lo que vamos a hacer es *automatizar el proceso de mejora de ellas*, enviar en masa e-mails en busqueda de feedback y extrapolarlos para que de una manera más fácil podamos ver los resultados y así, posteriormente mejorar la aplicación o el servicio.

Esta aplicación va a tener que resolver **cómo** vamos a envíar en masa los e-mails, o si vamos a trabajar con **direcciones** de los clientes deberíamos de tener un sistema de creación de cuentas, lo que *significaría que necesitamos autentificación*.

Uno pensaría que basta de los diagramas, que empecemos a codear un poco pero, es importante ver el diagrama para entender al máximo lo que tenemos que hacer, cada paso.

#

Cuando un cliente entra a nuestra página web tenemos que resolver, cómo es qué se registran en nuestro sitio, necesitamos que de algúna forma, se identifiquen y que asociemos cierto tipo de cuenta a esos usuarios, normalmente esto se resuelve con ***Google OAuth***, **Google OAuth** es el cartelito que vemos que dice "Sign Up with Google", en muchas páginas webs.

Luego de que ellos loggean a la página web, vamos a pedirles que agreguen un poco de dinero para poder envíar los correos, esto lo vamos a hacer a través de Stripe, no vamos a utilizar un modelo de suscripción, vamos a **utilizar un modelo de créditos**, en el cual el usuario agrega créditos a su cuenta, y de ahí los puede utilizar para mandar "x" cantidad de e-mails.

Cuando agregan créditos a su cuenta, ellos tienen la opción de crear una nueva **"campaign"**, esencialmente ***van a tener la posibilidad de crear una campaña*** para decir: *"Quiero mandar "x" cantidad de e-mails para recolectar feedback sobre "z" cosa."*

Ese usuario va a escribir una lista de todos los clientes del cual él quiere recibir feedback, para dejarlo claro: el *usuario* en este caso son los *Product Managers*, *Startups*, ellos tienen los e-mails de las personas que utilizan su aplicación.

Una vez de que el usuario **nos provee** una lista de e-mails, que puede variar de **n** a **n.length - 1**, vamos a crear un e-mail *que vamos a mandar a toda la lista que anteriormente nos dieron*.

Esos *"surveyees"* van a recibir un e-mail con un **link**, el cual van a clickear para hacer el feedback que el *usuario quiere recibir*.

Posteriormente vamos a *tabular* toda esa información.

Por último, *vamos a entregar esa información al usuario que nos contrató para la recolección de feedback*, para que ellos puedan ver la **información que les interesa**.

Es por esto, que debemos de *tener* **nuestro diagrama** y **entender con fácilidad** qué es lo que vamos a escribir, ya que cuando estemos codificando, <u>todo se va a ir a la mierda, muy rápido</u>.

![02, Diagram]("E:\Enzo\Enoch\javascript\Images\02-diagram.png")