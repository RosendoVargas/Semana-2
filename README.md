# Semana-2
Resumen
# Exploración de los servicios de Azure Compute
Objetivos:
Una vez que haya completado este módulo, podrá describir las ventajas y el uso de:
- Azure Virtual Machines
- Azure App Service
- Azure Container Instances
- Azure Kubernetes Service
- Azure Functions
- Azure Virtual Desktop
# Introducción a los servicios de Azure Compute
Azure Compute es un servicio de informática a petición para ejecutar aplicaciones basadas en la nube. Se proporcionan recursos informáticos como:
- Discos
- Procesadores
- Memoria 
- Redes y Sistemas Operativos

Los recursos están disponibles a petición y normalmente pueden estar disponibles en minutos o incluso en segundos. Solo se paga por los recursos que se usan y solo durante el tiempo que se usan.

Azure también tiene muchos servicios que pueden ejecutar máquinas virtuales (VM). Cada servicio proporciona opciones distintas en función de los requisitos. Algunos de los servicios más destacados son los siguientes:
- Azure Virtual Machines
- Azure Container Instances
- Azure App Service
- Azure Functions (o informática sin servidor)

- Máquinas virtuales: Las máquinas virtuales son emulaciones de software de equipos físicos. Incluyen un procesador virtual, memoria, almacenamiento y recursos de red. Hospedan un sistema operativo, y se puede instalar y ejecutar software, al igual que en un equipo físico. Al utilizar un cliente de escritorio remoto, puede usar y controlar la máquina virtual como si se estuviera sentado delante de ella.
- Conjuntos de escalado de máquinas virtuales: Con un recurso de Azure Compute que puede usar para implementar y administrar un conjunto de máquinas virtuales idénticas. No es necesario el aprovisionamiento previo de las máquinas virtuales. Por este motivo, es más sencillo compilar servicios a gran escala cuyo destino sean las cargas de trabajo en contenedores, de macroproceso y macrodatos. El proceso puede ser manual, automatizado o una combinación de ambos.
- Containers y Kubernetes:Son recursos de Azure Compute que puede usar para implementar contenedores y administrarlos. Los contenedores son entornos de aplicación ligeros y virtualizados. Están diseñados para crearse, escalarse horizontalmente y detenerse dinámicamente de forma rápida.
- App Service: Con Azure App Service puede compilar, implementar y escalar de forma rápida aplicaciones de API, móviles y web de nivel empresarial que se pueden ejecutar en cualquier plataforma. 
- Funciones: Functions es una opción ideal si le preocupa solo el código que ejecuta el servicio y no la infraestructura o la plataforma subyacente.
# Decisión de cuándo usar Azure Virtual Machines
Gracias a Azure Virtual Machines, puede crear y utilizar máquinas virtuales en la nube. Estas máquinas virtuales proporcionan una infraestructura como servicio (IaaS) en forma de un servidor virtualizado y se pueden usar de muchas formas
Las máquinas virtuales son una opción ideal cuando se necesita lo siguiente:

- Control total sobre el sistema operativo (SO).
- Capacidad de ejecutar software personalizado.
- Usar configuraciones de hospedaje personalizadas.
Una máquina virtual de Azure le ofrece la flexibilidad de la virtualización sin necesidad de adquirir y mantener el hardware físico que ejecuta la máquina virtual. Todavía se necesita configurar, actualizar y mantener el software que se ejecuta en la máquina virtual.
# Ejemplos de cuándo usar máquinas virtuales

Durante las pruebas y el desarrollo. Las máquinas virtuales proporcionan una manera rápida y sencilla de crear distintas configuraciones de sistema operativo y de aplicación. El personal encargado de las pruebas y del desarrollo puede eliminar fácilmente las máquinas virtuales cuando ya no las necesite.
- Durante las pruebas y el desarrollo. Las máquinas virtuales proporcionan una manera rápida y sencilla de crear distintas configuraciones de sistema operativo y de aplicación
- Al ejecutar aplicaciones en la nube. La capacidad de ejecutar determinadas aplicaciones en la nube pública, en lugar de crear una infraestructura tradicional para ejecutarlas, puede proporcionar importantes beneficios económicos.
- A la hora de extender el centro de recursos a la nube. Una organización puede extender las capacidades de su propia red local mediante la creación de una red virtual en Azure y al agregar máquinas virtuales a esa red virtual.
- Durante la recuperación ante desastres. Igual que con la ejecución de ciertos tipos de aplicaciones en la nube y con la ampliación de una red local a la nube, se puede obtener un ahorro considerable en costos mediante el uso de un enfoque basado en IaaS para la recuperación ante desastres.
# Traslado a la nube con máquinas virtuales
Las máquinas virtuales también son una opción excelente cuando se mueve de un servidor físico a la nube (también conocido como Lift-and-shift). Puede crear una imagen del servidor físico y hospedarla en una máquina virtual con pocos o ningún cambio. Al igual que un servidor físico local, las máquinas virtuales requieren mantenimiento. Por tanto, debe actualizar el sistema operativo y su software.
# Escalado de máquinas virtuales en Azure
Se pueden ejecutar máquinas virtuales únicas para pruebas, desarrollo o tareas secundarias. También se pueden agrupar las máquinas virtuales para proporcionar alta disponibilidad, escalabilidad y redundancia.
Estas características son:

- Conjuntos de escalado de máquinas virtuales
- Azure Batch
# ¿Qué son los conjuntos de escalado de máquinas virtuales?
- Los conjuntos de escalado de máquinas virtuales permiten crear y administrar un grupo de máquinas virtuales idénticas, de carga equilibrada. 
- Los conjuntos de escalado le permiten administrar, configurar y actualizar de forma centralizada un gran número de máquinas virtuales en cuestión de minutos para proporcionar aplicaciones altamente disponibles. 
# ¿Qué es Azure Batch?
Azure Batch permite trabajo por lotes paralelos a gran escala y de informática de alto rendimiento (HPC) con la capacidad de escalar a decenas, cientos o miles de máquinas virtuales.

Cuando esté listo para ejecutar un trabajo, Batch:

- Iniciará un grupo de máquinas virtuales de proceso de forma automática.
- Instalará aplicaciones y datos de almacenamiento provisional.
- Ejecutará trabajos con tantas tareas como tenga.
- Identificará errores.
- Reordenará la cola de trabajo.
- Reducirá verticalmente el grupo a medida que se complete el trabajo.
Puede haber situaciones en las que se necesite potencia informática sin procesar o potencia de cálculo a nivel de superequipo. Azure proporciona estas capacidades.

# Decisión de cuándo usar Azure App Service}
App Service permite crear y hospedar aplicaciones web, trabajos en segundo plano, back-ends móviles y API RESTful en el lenguaje de programación que prefiera, sin tener que administrar la infraestructura. Ofrece escalado automático y alta disponibilidad. App Service es compatible con Windows y Linux, y permite implementaciones automatizadas desde GitHub, Azure DevOps o cualquier repositorio Git para admitir un modelo de implementación continua.
# Costos de Azure App Service
El plan de App Service determina la cantidad de hardware dedicado al host. Por ejemplo, el plan determina si el hardware es dedicado o compartido y cuánta memoria se le reserva. Incluso hay un nivel gratuito que puede usar para hospedar sitios pequeños y con poco tráfico.
# Tipos de servicios de aplicaciones
- Aplicaciones web
App Service incluye compatibilidad completa para hospedar aplicaciones web mediante ASP.NET, ASP.NET Core, Java, Ruby, Node.js, PHP o Python. Puede elegir Windows o Linux como sistema operativo del host.

- Aplicaciones de API
Al igual que al hospedar un sitio web, puede compilar API web basadas en REST mediante el lenguaje y el marco que prefiera. Se obtiene compatibilidad completa con Swagger y la posibilidad de empaquetar y publicar la API en Azure Marketplace. Las aplicaciones producidas se pueden consumir desde cualquier cliente basado en HTTP o HTTPS.

- Trabajos web
Se puede usar la característica WebJobs para ejecutar un programa (.exe, Java, PHP, Python o Node.js) o un script (.cmd, .bat, PowerShell o Bash) en el mismo contexto que una aplicación web, aplicación de API o aplicación móvil. Los puede programar o ejecutar un desencadenador. Los trabajos web suelen usarse para ejecutar tareas en segundo plano como parte de la lógica de aplicación.

- Aplicaciones móviles
Use la característica Mobile Apps de App Service a fin de compilar rápidamente un back-end para aplicaciones iOS y Android. Con unos pocos clics en Azure Portal, puede realizar lo siguiente:

      - Almacenar los datos de aplicaciones móviles en una base de datos SQL basada en la nube.
      - Autenticar a clientes con proveedores sociales comunes, como MSA, Google, Twitter y Facebook.
      - Enviar notificaciones de inserción.
      - Ejecutar lógica de back-end personalizada en C# o Node.js.
 # Decisión de cuándo usar Azure Container Instances o Azure Kubernetes Service
 Los contenedores son una excelente opción si quiere ejecutar varias instancias de una aplicación en un solo equipo host.
 # ¿Qué son los contenedores?
 Los contenedores son un entorno de virtualización. Al igual que la ejecución de varias máquinas virtuales en un solo host físico, se pueden ejecutar varios contenedores en un solo host físico o virtual. Las máquinas virtuales parecen ser una instancia de un sistema operativo que se puede conectar y administrar, sin embargo los contenedores son ligeros y están diseñados para crearse, escalarse horizontalmente y detenerse de forma dinámica. Con los contenedores, puede reiniciar rápidamente en caso de bloqueo o interrupción del hardware. Uno de los motores de contenedor más populares es Docker, que es compatible con Azure.
 # Administrar contenedores
 Los contenedores se administran a través de un orquestador de contenedores, que puede iniciar, detener y escalar horizontalmente las instancias de la aplicación, según sea necesario. Hay dos maneras de administrar los contenedores basados en Microsoft y Docker en Azure: Azure Container Instances y Azure Kubernetes Service (AKS).
 - Azure Container Instances: ofrece la forma más rápida y sencilla de ejecutar un contenedor en Azure, sin tener que administrar ninguna máquina virtual o adoptar ningún servicio adicional.
 - Azure Kubernetes Service: La tarea de automatizar y administrar una gran cantidad de contenedores (y de interactuar con ellos) se conoce como orquestación. Azure Kubernetes Service es un servicio completo de orquestación para contenedores con arquitecturas distribuidas y grandes volúmenes de contenedores.
# Uso de contenedores en las soluciones
Los contenedores se usan normalmente para crear soluciones mediante una arquitectura de microservicios. Esta arquitectura es donde se dividen las soluciones en partes más pequeñas e independientes. Por ejemplo, se puede dividir un sitio web en un contenedor que hospeda el front-end, otro que hospeda el back-end y un tercero para el almacenamiento. De esta forma, puede separar partes de la aplicación en secciones lógicas que se pueden mantener, escalar o actualizar independientemente.

Imagine que el back-end de su sitio web ha alcanzado el límite de su capacidad, pero el front-end y el almacenamiento no están sobrecargados. Podría:

- Escalar el back-end por separado para mejorar el rendimiento.
- Decidir utilizar un servicio de almacenamiento diferente.
- Reemplazar el contenedor de almacenamiento sin que ello afecte al resto de la aplicación.

# Decisión de cuándo usar Azure Function
En otras palabras, para una gran cantidad de tiempo, la aplicación espera una entrada determinada antes de realizar cualquier procesamiento. Para reducir los costos, se quiere evitar el tener que pagar por el tiempo que la aplicación espera la entrada. Teniendo esto en cuenta, ha decidido investigar Azure Functions para ver si puede ser de ayuda.

La informática sin servidor es la abstracción de los servidores, la infraestructura y los sistemas operativos. Con la informática sin servidor, Azure se encarga de administrar la infraestructura de servidor, así como de la asignación y desasignación de recursos según la demanda. La infraestructura no es responsabilidad del usuario. El escalado y el rendimiento se controlan automáticamente. Solo se le cobrarán los recursos exactos que use. Tampoco hay ninguna necesidad de reservar capacidad.

La informática sin servidor incluye la abstracción de servidores, un escalado controlado por eventos y la microfacturación:

- Abstracción de servidores: la informática sin servidor abstrae los servidores en los que se ejecuta. Nunca se reservan instancias de servidor de forma explícita. La plataforma las administra de forma automática. Cada ejecución de función puede ejecutarse en una instancia de proceso diferente. 
- Escalado controlado por eventos: la informática sin servidor es una opción excelente para las cargas de trabajo que responden a eventos entrantes. Los eventos incluyen desencadenadores mediante lo siguiente:

(Temporizadores, por ejemplo, si una función tiene que ejecutarse todos los días a las 10:00 UTC.
HTTP, por ejemplo, escenarios de API y webhook.
Colas, por ejemplo, con procesamiento de pedidos.
Y mucho más.)
- Microfacturación: la informática tradicional factura para un bloque de tiempo, como el pago de una tarifa mensual o anual, para el hospedaje de sitios web. Este método de facturación es práctico, pero no siempre es rentable. Incluso si el sitio web de un cliente solo recibe una visita al día, este sigue pagando por tenerlo disponible durante todo el día. 

Azure tiene dos implementaciones de proceso sin servidor:

- Azure Functions: las funciones pueden ejecutar código en prácticamente cualquier lenguaje moderno.
- Azure Logic Apps: las aplicaciones lógicas están diseñadas en web y pueden ejecutar lógica desencadenada mediante servicios de Azure sin escribir código.

# Azure Functions
El uso de Azure Functions es ideal si le preocupa solo el código que ejecuta el servicio, pero no la infraestructura o la plataforma subyacentes. Las funciones se usan normalmente cuando se debe realizar un trabajo en respuesta a un evento (a menudo a través de una solicitud REST), un temporizador o un mensaje de otro servicio de Azure, y cuando ese trabajo puede completarse rápidamente, en segundos o en menos tiempo.

Las funciones escalan automáticamente según la demanda, para que sean una opción sólida cuando la demanda es variable.

# Azure Logic Apps
Las aplicaciones lógicas son similares a las funciones. Ambas permiten desencadenar lógica basada en un evento. Cuando las funciones ejecutan código, las aplicaciones lógicas ejecutan flujos de trabajo diseñados para automatizar escenarios empresariales y compilados a partir de bloques lógicos predefinidos.

# Decisión de cuándo usar Azure Virtual Desktop
Esta tarea normalmente requeriría la configuración de varios equipos PC nuevos con todas las herramientas de desarrollo necesarias para el nuevo equipo. Después, tendría que enviarlos a los desarrolladores correspondientes. El tiempo de adquisición, configuración y envío de cada uno de estos equipos sería costoso. Además, los nuevos desarrolladores tienen sus propios dispositivos informáticos que ejecutan una combinación de sistemas operativos Windows, Android y macOS.

# ¿Qué es Azure Virtual Desktop?
Azure Virtual Desktop es un servicio de virtualización de escritorios y aplicaciones que se ejecuta en la nube. Permite que los usuarios usen una versión hospedada en la nube de Windows desde cualquier ubicación. Azure Virtual Desktop funciona en dispositivos como Windows, Mac, iOS, Android y Linux. Funciona con aplicaciones que se pueden usar para acceder a aplicaciones y escritorios remotos. También puede usar la mayoría de los exploradores modernos para acceder a experiencias hospedadas en Azure Virtual Desktop.
# ¿Por qué debería usar Azure Virtual Desktop?
- Proporción de la mejor experiencia de usuario
- Aumento de la seguridad
# ¿Cuáles son algunas de la principales características de Azure Virtual Desktop?
- Administración simplificada
Azure Virtual Desktop es un servicio de Azure, por lo que resultará familiar para los administradores de Azure. Utilice Azure AD y RBAC para administrar el acceso a los recursos
- Administración del rendimiento
Azure Virtual Desktop ofrece opciones para equilibrar la carga de los usuarios en los grupos de hosts de máquinas virtuales. Los grupos de hosts son colecciones de máquinas virtuales con la misma configuración asignada a varios usuarios. Para obtener el mejor rendimiento, puede configurar el equilibrio de carga para que se produzca cuando los usuarios inicien sesión (modo de amplitud).
- Implementación de sesión múltiple de Windows 10
Azure Virtual Desktop permite usar la sesión múltiple de Windows 10 Enterprise, el único sistema operativo basado en cliente de Windows que permite varios usuarios simultáneos en una sola máquina virtual. 

# ¿Cómo puede reducir costos con Azure Virtual Desktop?
- Traiga sus propia licencias
Azure Virtual Desktop está disponible sin costo adicional si tiene una licencia de Microsoft 365 válida. Pague solo por los recursos de Azure que usa en Azure Virtual Desktop.
- Ahorre en costos de proceso
Compre licencias de Azure Reserved Virtual Machine Instances de un año o de tres años para ahorrar hasta un 72 %, en comparación con los precios de pago por uso. Puede pagar una reserva por adelantado o mensualmente.
