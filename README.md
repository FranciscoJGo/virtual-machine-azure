# Virtual Machine Azure AZ-900

Guia para crear una Máquina Virtual dentro de Azure utilizando sus recursos para configurarla

Antes de iniciar tenemos que ir al [Portal de Azure](https://portal.azure.com/)

## Paso 1
En el menu lateral seleccionamos la opcion de "maquinas virtuales" si en la barra de busqueda ponemos "maquinas virtuales"
![Menu lateral](/images/image1.png)

## Paso 2
Una vez dentro de damos seleccionamos al apartado "crear" y nos desplegara sus opciones de estas elegimos "Maquina virtual de Azure"
![Menu de Maquinas Virtuales](/images/image2.png)

## Paso 3
* Revisamos que la susbripción es de tipo "student"
* Creamos un grupo de recurso, que es el contenedor logico que almacena nuestros recursos (para utilizar los recursos de azure tienes que estar dentro de un grupo de recursos para poder utilizarlo). Lo nombramos como "Direccion-de-desarrollo".
* Nombramos a nuestra Maquina Virtual como "MV-01"
* Seccionamos nuestra region en este caso (US) Central US
* Las opciones de disponibilidad son para tener una copia de seguridad en otro centro de datos en dado lugar que presente una falla, pero como es una prueba no se necesita.
* La seguridad se mantiene en "Estandar".
* Para la imagen que es nuestro sistema operativo que usara nuestra VM hay una gran cantidad para elegir segun nuestras necesidades, aqui usamos: Windows Server 2019 Datacenter - Gen2. 
![Menu de Maquinas Virtuales](/images/image3.png)

* Seleccionamos un tamaño para nuestra VM (maquina virtual) considerando nuestro credito o presupuesto y requrimientos. Usamos la que nos muestra por defectos pero podemos utilizar mas accediendo a pestaña y podemos ver mas opciones y diferentes precios.
![Tamaño de Maquinas Virtuales](/images/image4.png)

* Le damos un nombre de usuario y una constraseña.
![Usuario y contraseña](/images/image5.png)

* Aceptamos para usar una licencia de Windows Server existente.
![Licencias](/images/image6.png)

## Pestaña:Disks(Discos)
* El tamaño de la máquina virtual determina el tipo de almacenamiento que puede usar y la cantidad de datos que permiten los discos.
* Para este apartado vamos a dejar todo con la opcion predeterminada que nos da azure.
![Almacenamiento](/images/image7.png)

## Pestaña:Networking(Redes)
* Puede controlar los puertos y la conectividad entrante y saliente con reglas de grupos de seguridad o bien aplicar una solución de equilibrio de carga ya existente.
* De igual manera vamos a dejar con la opcion predeterminada que nos da azure que son la Red virtual, Subred y IP pública.
![Almacenamiento](/images/image8.png)

## Pestaña:Management(Administración)
* Igualmente usamos las opciones predeterminadas de Azure.
![Almacenamiento](/images/image9.png)

## Pestaña:Advanced(Opciones avanzadas)
* Usamos las opciones predeterminadas por Azure.
![Almacenamiento](/images/image10.png)

## Pestaña:Tags(Etiquetas)
Los etiquetas nos ayudan a llevar un mejor de los recursos que usamos en azure. Podemos agregar detalles del recurso, como quien lo usa, que area de la empresa y su finalidad.
![Almacenamiento](/images/image11.png)

## Pestaña:Review+Create(Revisar y Crear)
Revisamos el resumen de las caracteristicas de nuestra Maquina Virtual y si todo esta en orden le damos continuar. Nos aparece una notificacion de Validación superada que quiere decir que nuestra maquina virtual si se puede crear.
![Validación superada](/images/image12.png)
* Y despues le damos click en crear
![Crear](/images/image13.png)
* No muestra una notificacion de se completó la implementación y ver más detalles sobre la implementación.
![Implentaicion completada](/images/image14.png)
* Despues seleccionamos "ir al recurso"
![Ir al recurso](/images/image15.png)
* Exploramos nuestra maquina virtual, para eso presionamos en "conectar y despues elegimos 'RDP'".
![Conectar RDP](/images/image16.png)

## Paso 5
* Descargamos el archivo 'RDP' y lo abrimos.
![Descargar archivo RDP](/images/image17.png)

## Paso 6
* Nos abrira una ventana y nos preguntara si queremos concectar y le decimos que si
![Ventana emergente](/images/image18.png)

## Paso 8
* Le damos en mas opciones y usar otra cuenta
![Mas opciones](/images/image19.png)

## Paso 9
* Insertamos el usuario y contraseña que usamos para crear la maquina virtual.
![Mas opciones](/images/image20.png)

## Paso 10
* Volvera a salir una ventana emergente donde preguntara si nos queremos conectar, ya que es la primera vez que lo hacemos. Y seleccionamos que "si"
![Conectar](/images/image21.png)

## Paso 11
* Vista de nuestra maquina virtual en la que podemos realizar cualquier cosa con ella.
 Nota: aunque apaguemos la maquina virtual azure sigue cobrando el uso del disco duro porque se sigue utilizando y ocupando espacio en azure.
![Conectar](/images/image22.png)

## Paso 12
* Cerramos y desconectamos la maquina virtual
![Desconectar](/images/image23.png)

## Paso 13
Eliminar la VM:
* Ir al portal de Azure y seleccionamos 'grupo de recursos'.
![Portal y grupo de recurso](/images/image24.png)
* Seleccionas nuestro grupo de recursos "Dirección-de-desarrollo" y seleccionamos "Eliminar grupo de recursos"
![Eliminar grupo de recurso](/images/image25.png)
* Escribimos el nombre de nuestro recurso para eliminarlo lo hacemos varias veces y esperamos un rato porque se tarda un momento en mostrarse los cambios.
![Eliminar grupo de recurso](/images/image26.png)
* De igual manera eliminamos nuestro grupo de recursos 'NetworkWatcherRG' el cual se encarga de vigilar la red del grupo de recursos.
![Eliminar NetworkWatcherRG](/images/image27.png)

## Nota:
Es importante mantener limpia nuestra area de grupos de recursos para evitar cargos mientras no estemos utilizando.
![Grupo de Recursos Limpio](/images/image28.png)


Redes:
* GitHub: [Francisco J Gonzalez](https://github.com/FranciscoJGo)

