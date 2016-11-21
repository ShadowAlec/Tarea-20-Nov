## Tarea.

#### Arquitectura Model View Presenter y como se diferencia del Model View Controller.

Model view controller (MVC) es un patrón que permite desacoplar la implementación de las vistas de la implementación lógica de negocio de nuestro modelo.

En éste patrón hay tres componentes importantes: Modelo, Vista y controlador.
El modelo es el encargado de encapsular y mantener la lógica de negocio lo que tiene que hacer nuestra aplicación.
La vista es la encargada de renderizar los layouts creados en xml.
La función del controlador es intercambiar mensajes entre la vista y el modelo, típicamente se utiliza una subclase de Activity, Fragment y un service como controlador.

Una mala aplicación de MVC comienza cuando decidimos usar un activity o un fragment como un controlador, ya que las actividades y fragmentos forman parte de la vista dentro de MVC.

Es por ello que se introduce el MVP que es un patrón derivado de MVC comúnmente usado en la construcción de interfaces gráficas, que debemos considerar y tener en mente es que el MVP no es un patrón de arquitectura, es decir sólo se encarga de implementar la lógica de la capa de presentación.

![mvp](images/mvp.png)

* M: El modelo es el proveedor de datos que queremos en la vista.
* V: Una view dentro de MVP no representa una vista del SDK de android (Android class View), es decir no es un TextView, ni un button ni un layout. Una view representa una abstracción de lo que se puede hacer con la vista, normalmente se asocia a una interface para representar la funcionalidad de una vista. La parte importante está en una Activity o un fragmento tienen la responsabilidad únicamente de implementar la interface View y conectar las acciones del ususario con el presenter.

* Presenter: En este patrón	 es el encargafo de coordinar la implementación de la vista y el modelo, actualiza la vista y actúa sobre los eventos de un usuario que se envían por la vista. El presenter también recupera los datos del modelo y los prepara para su visualización.

#### Investigar más a detalle la arquitectura CLEAN.

La arquitectura Clean fue propuesta por Robert Cecil Martin (El tío Bob) y es algo de lo que se ha hablado bastante en los últimos años dentro de la comunidad de Android.
Surge con la problemática de que en un framework se encuentra más código que lo representa, en lugar del problema que está resolviendo, es decir, la idea es centrarse en lo que tiene que hacer la aplicación como tal y es por ello que dice que debemos de pensar en él framework como el mecanismo de paso de mensajes hacia nuestro software, el cual se debe mirar como una herramienta o plugin de lo que queremos realizar.

El tío Bob menciona que más que una arquitectura, es una serie de reglas que se deben cumplir para que una arquitectura sea considerada "clean".

Tiene la siguiente estructura.
![Clean Architecture](images/clean_archi.png)


Lo único que nos dice es que hay que respetar la regla de dependencia "Dependency rule." que establece que "El código fuente sólo puede apuntar hacia adentro".

##### Entities (Entidades).

Son aquellos objetos que van a representar los actores importantes de la lógica de negocio de nuestra aplicación.

##### Use cases (Casos de uso).

Están muy relacionados con las entidades y son los encargados de implementar lógica de negocio de nuestra aplicación, ya que van a orientar todas aquellas interacciones del flujo de datos y entidades dejando al framework fuera de todo esto (En nuestro caso el sdk android), también  se conocen como interactores.

##### Interface adapters (Adaptdores de interfaz).

Convierten los datos en el formato más conveniente para los casos de uso y entidades. 

##### Frameworks and drivers.
Aquí es donde residen los detalles y todo ese conjunto de plataformas externas y herramientas como puede ser la UI, Web, DB, dispositivos, etc. generalmente sólo se deben comunicar con el siguiente círculo a su interior


![android clean architecture](images/android_archi.png)




