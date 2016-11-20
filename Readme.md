## Tarea.

#### Arquitectura Model View Presenter y como se diferencia del Model View Controller.

Model view controller (MVC) es un patrón que permite desacoplar la implementación de las vistas de la implementación lógica de negocio de nuestro modelo.

En éste patrón hay tres componentes importantes: Modelo, Vista y controlador.
El modelo es el encargado de encapsular y mantener la lógica de negocio lo que tiene que hacer nuestra aplicación.
La vista es la encargada de renderizar los layouts creados en xml.
La función del controlador es intercambiar mensajes entre la vista y el modelo, típicamente se utiliza una subclase de Activity, Fragment y un service como controlador.

Una mala aplicación de MVC comienza cuando decidimos usar un activity o un fragment como un controlador, ya que las actividades y fragmentos forman parte de la vista dentro de MVC.

Es por ello que se introduce el MVP que es un patrón derivado de MVC comúnmente usado en la construcción de interfaces gráficas, que debemos considerar y tener en mente es que el MVP no es un patrón de arquitectura, es decir sólo se encarga de implementar la lógica de la capa de presentación.


#### 

