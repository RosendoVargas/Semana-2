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

# Exploración de los servicios de red de Azure
# Introducción
Supongamos que su empresa, Tailwind Traders, ha migrado algunas aplicaciones a la nube y está diseñando otras aplicaciones nuevas. Los servidores que hospedan los datos de clientes y productos de Tailwind Traders residen en Silicon Valley. Su empresa también tiene varias sucursales ubicadas en diferentes regiones geográficas. Como parte de la estrategia de migración, su empresa debe determinar el enfoque correcto para configurar su infraestructura de red.
# Aspectos básicos de Azure Virtual Network
Tailwind Traders tiene un centro de datos local que va a mantener, pero quiere usar Azure para descargar los picos de tráfico mediante máquinas virtuales (VM) hospedadas en Azure. Quiere mantener el esquema de direcciones IP y los dispositivos de red existentes, y asegurarse de que todas las transferencias de datos sean seguras.
# ¿Qué son las redes virtuales de Azure?
Las redes virtuales de Azure permiten a los recursos de Azure, como las máquinas virtuales, las aplicaciones web y las bases de datos, comunicarse entre sí, con los usuarios de Internet y con los equipos cliente en el entorno local.

Las redes virtuales de Azure proporcionan las importantes funcionalidades de red siguientes:

- Aislamiento y segmentación: Virtual Network permite crear varias redes virtuales aisladas. Al configurar una red virtual, se define un espacio de direcciones IP privadas con intervalos de direcciones IP públicas o privadas.
- Comunicación con Internet: Una máquina virtual en Azure se puede conectar a Internet de forma predeterminada. Puede habilitar las comunicaciones entrantes desde Internet si define una dirección IP pública o un equilibrador de carga público. 
- Comunicación entre los recursos de Azure: Le interesará habilitar los recursos de Azure para que se comuniquen entre sí de forma segura. Puede hacerlo de dos maneras:

   Redes virtuales Las redes virtuales no solo pueden conectar máquinas virtuales, sino también otros recursos de Azure, como App Service Environment para Power Apps, Azure Kubernetes Service y conjuntos de escalado de máquinas virtuales de Azure.
   Puntos de conexión de servicio Puede usar los puntos de conexión de servicio para conectarse a otros tipos de recursos de Azure, como cuentas de almacenamiento y bases de datos SQL de Azure. Este enfoque permite vincular varios recursos de Azure con las redes virtuales para mejorar la seguridad y proporcionar un enrutamiento óptimo entre los recursos.
   
- Comunicación con recursos locales: Las redes virtuales de Azure permiten vincular entre sí los recursos del entorno local y dentro de la suscripción de Azure. De hecho, puede crear una red que abarque tanto el entorno local como el entorno en la nube; Redes privadas virtuales de punto a sitio, Redes virtuales privadas de sitio a sitio y Azure ExpressRoute

- Enrutamiento del tráfico de red: De forma predeterminada, Azure enruta el tráfico entre las subredes de todas las redes virtuales conectadas, las redes locales e Internet. También puede controlar el enrutamiento e invalidar esa configuración del siguiente modo: Tablas de rutas, rotocolo de puerta de enlace de borde.

- Filtrado del tráfico de red: Grupos de seguridad de red Un grupo de seguridad de red es un recurso de Azure que puede contener varias reglas de seguridad de entrada y salida. y Aplicaciones virtuales de red Una aplicación virtual de red es una máquina virtual especializada que se puede comparar con un dispositivo de red protegido. 

- Conexión de redes virtuales: Puede vincular redes virtuales entre sí mediante el emparejamiento de red virtual. El emparejamiento permite que los recursos de cada red virtual se comuniquen entre sí. Estas redes virtuales pueden estar en regiones distintas, lo que permite crear una red global interconectada con Azure.

# Configuración de Azure Virtual Network
Puede crear y configurar instancias de Azure Virtual Network desde Azure Portal, Azure PowerShell en el equipo local o Azure Cloud Shell.
# Creación de una red virtual
Cuando se crea una red virtual de Azure, se configuran algunas opciones básicas. Tendrá la posibilidad de configurar opciones avanzadas, como varias subredes, protección contra denegación de servicio distribuido (DDoS) y puntos de conexión de servicio.
Configurará las opciones siguientes para una red virtual básica:
- Nombre de red
- Espacio de direcciones
- Suscripción
- Grupo de recursos
- Ubicación
- Subred
- Protección contra DDoS
- Puntos de conexión de servicio

# Definición de opciones de configuración adicionales
Después de crear una red virtual, puede definir más opciones. Entre ellas se incluyen las siguientes:

- Grupo de seguridad de red Los grupos de seguridad de red tienen reglas de seguridad que permiten filtrar el tipo de tráfico de red que puede entrar o salir de las interfaces de red y las subredes de red virtual. Cree el grupo de seguridad de red por separado. Después, asócielo con la red virtual.
- Tabla de rutas Azure crea automáticamente una tabla de rutas para cada subred de una red virtual de Azure y agrega las rutas predeterminadas del sistema a la tabla. Puede agregar tablas de rutas personalizadas para modificar el tráfico entre las redes virtuales.

# Configuración de redes virtuales
Después, puede revisar y cambiar la configuración en paneles secundarios adicionales. Esta configuración incluye:

- Espacios de direcciones: puede agregar espacios de direcciones adicionales a la definición inicial.
- Dispositivos conectados: use la red virtual para conectar las máquinas.
- Subredes: puede agregar subredes adicionales.
- Emparejamientos: vincule las redes virtuales mediante organizaciones de emparejamiento.

Las redes virtuales son mecanismos eficaces y muy configurables para conectar las entidades de Azure. Puede conectar los recursos de Azure entre sí o a los recursos del entorno local. Puede aislar, filtrar y enrutar el tráfico de red. Azure le permite aumentar la seguridad donde considere que es necesario.

# Aspectos básicos de Azure VPN Gateway
Las redes privadas virtuales usan un túnel cifrado en otra red. Normalmente, se implementan para conectar entre sí dos o más redes privadas de confianza a través de una red que no es de confianza (normalmente, la red pública de Internet). El tráfico se cifra mientras viaja por la red que no es de confianza para evitar ataques de interceptación o de otro tipo.

# Puertas de enlace de VPN
Una puerta de enlace de VPN es un tipo de puerta de enlace de red virtual. Las instancias de Azure VPN Gateway se implementan en instancias de Azure Virtual Network y habilitan la conectividad siguiente:

- Conectar los centros de datos locales a redes virtuales a través de una conexión de sitio a sitio.
- Conectar los dispositivos individuales a redes virtuales a través de una conexión de punto a sitio.
- Conectar las redes virtuales a otras redes virtuales a través de una conexión entre redes.

Al implementar una instancia de VPN Gateway, especifique el tipo de red privada virtual, es decir, basada en directivas o basada en rutas. La principal diferencia entre estos dos tipos de VPN es cómo se especifica el tráfico que se va a cifrar. 

# Redes privadas virtuales basadas en directivas
Las instancias de VPN Gateway basadas en directivas especifican de forma estática la dirección IP de los paquetes que se deben cifrar a través de cada túnel. Este tipo de dispositivo evalúa cada paquete de datos en función de los conjuntos de direcciones IP para elegir el túnel a través del cual se va a enviar el paquete.

Entre las características clave de las instancias de VPN Gateway basadas en directivas en Azure se incluyen:
- Compatibilidad solo con IKEv1.
- Uso del enrutamiento estático, en el que las combinaciones de prefijos de dirección de ambas redes controlan cómo se cifra y descifra el tráfico a través del túnel VPN. 
- Las redes privadas virtuales basadas en directivas se deben usar en escenarios específicos que las necesiten, por ejemplo, para ofrecer compatibilidad con dispositivos de red privada virtual locales heredados.

# Redes privadas virtuales basadas en rutas
Si la definición de las direcciones IP que están detrás de cada túnel es demasiado compleja, se pueden usar puertas de enlace basadas en rutas. Con las puertas de enlace basadas en rutas, los túneles IPSec se modelan como una interfaz de red o una interfaz de túnel virtual. 
El enrutamiento IP (ya sean rutas estáticas o protocolos de enrutamiento dinámico) decide cuál de estas interfaces de túnel se va a usar al enviar cada paquete. Las redes privadas virtuales basadas en rutas son el método preferido para conectar dispositivos locales. Son más resistentes a los cambios de la topología, como la creación de subredes.
Si necesita alguno de los siguientes tipos de conectividad, use una instancia de VPN Gateway basada en rutas:

- Conexiones entre redes virtuales
- Conexiones de punto a sitio
- Conexiones de varios sitios
- Coexistencia con una puerta de enlace de Azure ExpressRoute

Entre las características clave de las instancias de VPN Gateway basadas en rutas en Azure se incluyen:

- Compatibilidad con IKEv2
- Uso de selectores de tráfico universales (comodín)
- Puede usar protocolos de enrutamiento dinámico, donde las tablas de enrutamiento y reenvío dirigen el tráfico a diferentes túneles IPSec. En este caso, las redes de origen y destino no se definen estáticamente como en las VPN basadas en directivas o incluso en las VPN basadas en rutas con enrutamiento estático.

# Implementación de instancias de VPN Gateway
Antes de implementar una instancia de VPN Gateway, necesitará algunos recursos de Azure y locales.

# Recursos de Azure necesarios
Se necesitarán estos recursos de Azure para poder implementar una instancia de VPN Gateway operativa:
- Red virtual. Implemente una red virtual que tenga suficiente espacio de direcciones para la subred adicional que necesitará para la instancia de VPN Gateway.
- GatewaySubnet. Implemente una subred llamada GatewaySubnet para la instancia de VPN Gateway. Use al menos una máscara de dirección /27 con el fin de asegurarse de que proporciona suficientes direcciones IP en la subred para un crecimiento futuro.
- Dirección IP pública. Cree una dirección IP pública dinámica de SKU básico si usa una puerta de enlace que no tenga en cuenta la zona. Esta dirección proporciona una dirección IP pública enrutable como destino para el dispositivo VPN local. 
- Puerta de enlace de red local. Cree una puerta de enlace de red local para definir la configuración de la red local; por ejemplo, dónde y a qué se conectará la instancia de VPN Gateway. 
- Puerta de enlace de red virtual. Cree la puerta de enlace de red virtual para enrutar el tráfico entre la red virtual y el centro de datos local u otras redes virtuales.
- Conexión. Cree un recurso de conexión para crear una conexión lógica entre la instancia de VPN Gateway y la puerta de enlace de red local.

       La conexión se realiza a las direcciones IPv4 del dispositivo VPN local, tal como define la puerta de enlace de red local.
       La conexión se realiza desde la puerta de enlace de red virtual y la dirección IP pública asociada.
       
# Recursos locales necesarios
Para conectar el centro de datos a una instancia de VPN Gateway, se necesitarán los siguientes recursos locales:

- Un dispositivo VPN que admita instancias de VPN Gateway basadas en directivas o en rutas.
- Una dirección IPv4 de acceso público (enrutable por Internet).

# Escenarios de alta disponibilidad
 
- Configuración de activo-en espera: De forma predeterminada, las instancias de VPN Gateway se implementan como dos instancias en una configuración de activo-en espera, incluso si solo ve un recurso de VPN Gateway en Azure. Cuando el mantenimiento planeado o la interrupción imprevista afectan a la instancia activa, la instancia en espera asume de forma automática la responsabilidad de las conexiones sin ninguna intervención del usuario. 
- Activo/activo: Al incorporar compatibilidad con el protocolo de enrutamiento de BGP, también puede implementar puertas de enlace VPN en una configuración del tipo activo/activo. En esta configuración, se asigna una IP pública única a cada instancia. Después, se crean túneles independientes desde el dispositivo local a cada dirección IP. 
- Conmutación por error de ExpressRoute: Otra opción de alta disponibilidad consiste en configurar una instancia de VPN Gateway como una ruta segura de conmutación por error para las conexiones ExpressRoute. Los circuitos ExpressRoute tienen resistencia integrada. Sin embargo, no son inmunes a los problemas físicos que afectan a los cables que entregan conectividad ni a las interrupciones que afectan a la ubicación completa de ExpressRoute. 
- Puertas de enlace con redundancia de zona: En las regiones que admiten zonas de disponibilidad, se pueden implementar puertas de enlace VPN y ExpressRoute en una configuración con redundancia de zona.

# Aspectos básicos de Azure ExpressRoute

ExpressRoute le permite ampliar las redes locales a la nube de Microsoft mediante una conexión privada con la ayuda de un proveedor de conectividad. Con ExpressRoute, puede establecer conexiones con servicios en la nube de Microsoft, como Microsoft Azure y Microsoft 365.

La conectividad puede ser desde una red de conectividad universal (IP VPN), una red Ethernet de punto a punto o una conexión cruzada virtual a través de un proveedor de conectividad en una instalación de ubicación compartida. Las conexiones de ExpressRoute no pasan por la red pública de Internet. Esto permite a las conexiones de ExpressRoute ofrecer más confiabilidad, más velocidad, latencia coherentes y mayor seguridad que las conexiones normales a través de Internet. Para información sobre cómo conectar la red a Microsoft mediante ExpressRoute, consulte ExpressRoute connectivity models (Modelos de conectividad de ExpressRoute).

Como parte de su trabajo para Tailwind Traders, debe comprender qué es Azure ExpressRoute y cómo se integra con las redes locales y de Azure. En esta unidad, conocerá las ventajas que proporciona ExpressRoute en comparación con otras opciones de conectividad de sitio a sitio. Como resultado, observará si ExpressRoute puede proporcionar a la empresa el mejor rendimiento de red posible.

A lo largo de esta unidad, nos centraremos en dos niveles diferentes del modelo de interconexión de sistemas abiertos (OSI):

- Nivel 2 (L2): se trata del nivel de vínculo de datos, que proporciona una comunicación de nodo a nodo entre dos nodos de la misma red.
- Nivel 3 (L3): se trata del nivel de red, que proporciona el direccionamiento y enrutamiento entre los nodos de una red de varios nodos.
 
# Características y ventajas de ExpressRoute
El uso de ExpressRoute como servicio de conexión entre Azure y las redes locales tiene varias ventajas.

- Conectividad de nivel 3 entre su red local y Microsoft Cloud a través de un proveedor de conectividad. La conectividad puede ser desde una red de conectividad universal (IP VPN), una red Ethernet de punto a punto, o una conexión cruzada virtual a través de un intercambio de Ethernet.
- Conectividad de servicios en la nube de Microsoft en todas las regiones dentro de la región geopolítica.
- Conectividad global a los servicios de Microsoft en todas las regiones con el complemento ExpressRoute Premium.
- Enrutamiento dinámico entre la red y Microsoft a través de BGP.
- Redundancia integrada en todas las ubicaciones de configuración entre pares para una mayor confiabilidad.
- El tiempo de actividad de conexión SLA.
- Compatibilidad con QoS de Skype para la empresa.

# Conectividad de nivel 3
ExpressRoute proporciona conectividad de nivel 3 (nivel de dirección) entre la red local y la nube de Microsoft a través de asociados de conectividad. Estas conexiones pueden ser de una red punto a punto o universal. También puede tratarse de conexiones cruzadas virtuales a través de un intercambio.
# Redundancia integrada
Cada proveedor de conectividad usa dispositivos redundantes para garantizar que las conexiones establecidas con Microsoft tengan alta disponibilidad. Puede configurar varios circuitos para complementar esta característica. Todas las conexiones redundantes se configuran con conectividad de nivel 3 para cumplir los Acuerdos de Nivel de Servicio.
# Conectividad con los Servicios en la nube de Microsoft
ExpressRoute permite el acceso directo a los siguientes servicios en todas las regiones:

- Microsoft Office 365
- Microsoft Dynamics 365
- Servicios de proceso de Azure, como Azure Virtual Machines
- Servicios en la nube de Azure, como Azure Cosmos DB y Azure Storage

Office 365 se creó para tener acceso a él de forma segura y fiable a través de Internet. Por este motivo, se recomienda utilizar ExpressRoute en escenarios concretos. La sección "Más información" al final de este módulo incluye un vínculo sobre el uso de ExpressRoute para acceder a Office 365.

# Conectividad local con Global Reach de ExpressRoute
Puede permitir que Global Reach de ExpressRoute intercambie datos entre los sitios locales si conecta los diferentes circuitos ExpressRoute. Por ejemplo, supongamos que tiene un centro de datos privado en California conectado a ExpressRoute en Silicon Valley. Tiene otro centro de centros privado en Texas conectado a ExpressRoute en Dallas.
# Enrutamiento dinámico
ExpressRoute usa el protocolo de enrutamiento Protocolo de puerta de enlace de borde (BGP). BGP se usa para intercambiar rutas entre las redes locales y los recursos que se ejecutan en Azure. Este protocolo permite el enrutamiento dinámico entre la red local y los servicios que se ejecutan en la nube de Microsoft.
# Modelos de conectividad de ExpressRoute
ExpressRoute admite tres modelos que puede usar para conectar la red local con la nube de Microsoft:

- Ubicación de CloudExchange
- Conexión Ethernet de punto a punto
- Conexión universal

# Coubicación en un intercambio en la nube
Normalmente, los proveedores de coubicación pueden ofrecer conexiones de nivel 2 y nivel 3 entre la infraestructura, que puede encontrarse en las instalación de la coubicación, y la nube de Microsoft. 
# Conexión Ethernet de punto a punto
Las conexiones de punto a punto proporcionan conectividad de nivel 2 y nivel 3 entre el sitio local y Azure. Puede conectar sus oficinas o centros de datos a Azure mediante vínculos de punto a punto. 
# Redes universales
Con la conectividad universal, puede integrar la red de área extensa (WAN) con Azure si proporciona conexiones a las oficinas y los centros de datos. Azure se integra con la conexión WAN para proporcionarle una conexión, como la que tendría entre el centro de datos y las sucursales.
Con las conexiones universales, todos los proveedores de WAN ofrecen conectividad de nivel 3. 
# Consideraciones sobre la seguridad
Con ExpressRoute los datos no viajan a través de la red pública de Internet y, por tanto, no se exponen a los posibles riesgos asociados a las comunicaciones de Internet. ExpressRoute es una conexión privada de la infraestructura local a la infraestructura de Azure. Incluso si tiene una conexión ExpressRoute, las consultas de DNS, la comprobación de la lista de revocación de certificados y las solicitudes de Azure Content Delivery Network se siguen enviando a través de la red pública de Internet.

# Exploración de los servicios de Azure Storage!!!

# Introducción

Supongamos que su empresa, Tailwind Traders, tiene una serie de folletos de productos, hojas de datos, imágenes de productos y otros archivos relacionados con el marketing, las ventas y el soporte técnico. En el pasado, su empresa ha hospedado estos archivos en servidores web independientes en su centro de datos.

Su empresa ahora está en proceso de migrar sus aplicaciones a la nube y su equipo de desarrollo actualmente está diseñando nuevas aplicaciones. Su director tecnológico (CTO) quiere migrar todos los archivos de marketing, ventas y soporte técnico a la nube con el fin de aprovechar la distribución geográfica de los archivos. Esta migración también reduce el número de servidores físicos que mantiene su empresa en su centro de datos. Como parte de la estrategia de migración, debe determinar el enfoque correcto para su infraestructura de almacenamiento basado en la nube.

# Aspectos básicos de la cuenta de Azure Storage

El director tecnológico (CTO) de su empresa, Tailwind Traders, ha encargado a su equipo la tarea de migrar todos los archivos a la nube. El equipo ha elegido Azure Storage, que es un servicio que puede usar para almacenar archivos, mensajes, tablas y otros tipos de información. Los clientes como sitios web, aplicaciones móviles, aplicaciones de escritorio y muchos otros tipos de soluciones personalizadas pueden leer y escribir datos en Azure Storage. Azure Storage también se usa en máquinas virtuales de infraestructura como servicio y en servicios en la nube de plataforma como servicio.

Una cuenta de almacenamiento proporciona un espacio de nombres único para los datos de Azure Storage, al que se puede acceder desde cualquier lugar del mundo a través de HTTP o HTTPS. Los datos de esta cuenta son seguros, de alta disponibilidad, duraderos y escalables de forma masiva.

# Aspectos básicos de Disk Storage

Disk Storage proporciona discos para Azure Virtual Machines. Las aplicaciones y otros servicios pueden acceder a estos discos y usarlos cuando sea necesario, igual que se haría en escenarios locales. Disk Storage permite que los datos se almacenen de forma persistente y que se acceda a ellos desde un disco duro virtual conectado.

Los discos tienen diferentes tamaños y niveles de rendimiento, desde unidades de estado sólido (SSD) a unidades de disco duro (HDD) giratorias tradicionales, con diferentes niveles de rendimiento. Puede usar discos SSD y HDD estándar para cargas de trabajo menos críticas, discos SSD Premium para aplicaciones de producción críticas y Ultra Disks para cargas de trabajo con un uso intensivo de datos como SAP HANA, bases de datos de nivel superior y cargas de trabajo con mucha actividad de transacciones. Azure han ofrecido durabilidad de nivel empresarial de forma coherente para los discos de infraestructura como servicio (IaaS), con una tasa de error anualizada del 0 % líder del sector.

# Aspectos básicos de Azure Blob Storage

Azure Blob Storage es una solución de almacenamiento de objetos para la nube. Puede almacenar grandes cantidades de datos, como datos de texto o binarios. Azure Blob Storage es no estructurado, lo que significa que no hay ninguna restricción en cuanto a los tipos de datos que puede contener. Blob Storage puede administrar miles de cargas simultáneas, cantidades enormes de datos de vídeo, archivos de registro en constante crecimiento y es accesible desde cualquier lugar con conexión a Internet.
Los blobs no están limitados a formatos de archivo comunes. Un blob podría contener gigabytes de datos binarios transmitidos desde un instrumento científico, un mensaje cifrado para otra aplicación o datos en un formato personalizado para una aplicación que se está desarrollando. Una ventaja del almacenamiento en blobs con respecto al almacenamiento en disco es que no requiere que los desarrolladores piensen en discos o los administren; los datos se cargan como blobs y Azure se encarga de las necesidades de almacenamiento físico.

Blob Storage resulta ideal para lo siguiente:

- Visualización de imágenes o documentos directamente en un explorador.
- Almacenamiento de archivos para acceso distribuido.
- Streaming de audio y vídeo.
- Almacenamiento de datos para copia de seguridad y restauración, recuperación ante desastres y archivado.
- Almacenamiento de datos para el análisis en local o en un servicio hospedado de Azure.
- Almacenamiento de hasta 8 TB de datos para máquinas virtuales.

Los blobs se almacenan en contenedores, lo que ayuda a organizar los blobs en función de sus necesidades empresariales.

En el diagrama siguiente se muestra cómo puede usar las cuentas, los contenedores y los blobs de Azure.
![image](https://user-images.githubusercontent.com/92233744/137811284-fe4b8a85-f5b1-4345-b7ec-70452b211d5c.png)

# Aspectos básicos de Azure Files

Azure Files ofrece recursos compartidos de archivos totalmente administrados en la nube a los que se puede acceder mediante los protocolos del Bloque de mensajes del servidor y Network File System (versión preliminar). Los recursos compartidos de Azure se pueden montar simultáneamente en implementaciones de Windows, Linux y macOS en la nube o locales. Las aplicaciones que se ejecutan en máquinas virtuales o servicios en la nube de Azure pueden montar un recurso compartido de almacenamiento de archivos para acceder a datos de archivos, del mismo modo que una aplicación de escritorio montaría un recurso compartido SMB normal. 

Use Azure Files para las siguientes situaciones:

- Muchas aplicaciones locales usan recursos compartidos de archivos. Azure Files facilita la migración de esas aplicaciones que comparten datos a Azure. Si monta el recurso compartido de archivos en la misma letra de unidad que usa la aplicación local, la parte de la aplicación que accede al recurso compartido de archivos debe funcionar con cambios mínimos, si los hay.
- Almacene archivos de configuración en un recurso compartido de archivos y acceda a ellos desde varias máquinas virtuales. Las herramientas y utilidades que usen varios desarrolladores de un grupo pueden almacenarse en un recurso compartido de archivos, lo que garantiza que todos los usuarios puedan encontrarlas y que utilizan la misma versión.
- Escriba datos en un recurso compartido de archivos y procese o analice los datos más adelante. Por ejemplo, puede que desee hacerlo con registros de diagnóstico, métricas y volcados de memoria.

Una cosa que distingue Azure Files de los archivos ubicados en un recurso compartido de archivos corporativo es que puede tener acceso a los archivos desde cualquier lugar del mundo mediante una dirección URL que apunte al archivo. También puede usar tokens de Firma de acceso compartido (SAS) para permitir el acceso a un recurso privado durante un período de tiempo determinado.

# Descripción de los niveles de acceso de blobs

Los datos almacenados en la nube pueden crecer a un ritmo exponencial. Para administrar los costos de las crecientes necesidades de almacenamiento, resulta útil organizar los datos en función de atributos como la frecuencia de acceso y el período de retención planeada. Los datos almacenados en la nube pueden ser diferentes según la forma en que se generan, se procesan y se accede a ellos a lo largo de su vigencia. A algunos datos se accede y se modifican activamente a lo largo de su duración. A algunos datos se accede con frecuencia al principio de su duración, mientras que el acceso cae drásticamente a medida que envejecen los datos. Algunos datos permanecen inactivos en la nube y, después de que se almacenan, no se accede a ellos prácticamente nunca. Para dar cabida a estas diferentes necesidades de acceso, Azure proporciona varios niveles de acceso, que puede usar para equilibrar los costos de almacenamiento con sus necesidades de acceso.


Azure Storage ofrece diferentes niveles de acceso para el almacenamiento de blobs, lo que le ayuda a almacenar datos de objetos de la manera más rentable. Entre los niveles de acceso disponibles se incluyen:

- Nivel de acceso frecuente: optimizado para almacenar datos a los que se accede con frecuencia (por ejemplo, imágenes para el sitio web).
- Nivel de acceso esporádico: optimizado para datos a los que se accede con poca frecuencia y que se almacenan al menos durante 30 días (por ejemplo, las facturas de los clientes).
- Nivel de acceso de archivo: conveniente para datos a los que raramente se accede y que se almacenan durante al menos 180 días con requisitos de latencia flexibles (por ejemplo, copias de seguridad a largo plazo).

# Las siguientes consideraciones se aplican a los distintos niveles de acceso:

- Solo los niveles de acceso frecuente y esporádico se pueden establecer en el nivel de cuenta. El nivel de acceso de archivo no está disponible en el nivel de cuenta.
- Los niveles frecuente, esporádico y de archivo se pueden establecer en el nivel de blob durante la carga o después de esta.
- Los datos del nivel de acceso esporádico pueden tolerar una disponibilidad ligeramente inferior, pero aun así requieren una gran durabilidad, una latencia de recuperación y unas características de rendimiento similares a las de los datos de acceso frecuente. En el caso de los datos de acceso esporádico, un contrato de nivel de servicio (SLA) con una disponibilidad ligeramente inferior y unos costos de acceso mayores, en comparación con los datos de acceso frecuente, es aceptable a cambio de unos costos de almacenamiento menores.
- El almacenamiento de archivo almacena datos sin conexión y ofrece los menores costos de almacenamiento, pero los mayores costos de acceso y rehidratación de datos.


# Exploración de los servicios de análisis y bases de datos de Azure!!!

# Introducción

Debido a un número cada vez mayor de adquisiciones durante la última década, Tailwind Traders usa diversas tecnologías de análisis y bases de datos. A medida que la empresa empiece a migrar las cargas de trabajo de datos existentes y a implementar nuevas cargas de trabajo de datos en Azure, esta debe comprender qué tecnología de Azure será la adecuada para cada carga de trabajo. El director de tecnología de la empresa le ha asignado la tarea de investigar las distintas opciones de bases de datos disponibles. Esta investigación ayudará a la empresa a elegir las opciones adecuadas para cada uno de los escenarios de datos.

# Exploración de Azure Cosmos DB

A lo largo de los años, Tailwind Traders ha adquirido varias empresas más pequeñas. Cada una de estas empresas tenía equipos de desarrolladores que usaban diferentes servicios de bases de datos y varias API para trabajar con sus datos. Un plan a largo plazo podría ser trasladar todos los datos dispares a un servicio de base de datos común. Por el momento, sin embargo, es mejor habilitar cada uno de estos equipos para que trabajen con un entorno en el que puedan usar sus conocimientos existentes. Afortunadamente, Azure Cosmos DB puede ayudarle.

Azure Cosmos DB es un servicio de base de datos de varios modelos distribuido globalmente. Puede escalar de forma elástica e independiente el rendimiento y el almacenamiento en cualquier número de regiones de Azure de todo el mundo. Puede aprovechar un acceso rápido y en milisegundos de un solo dígito a los datos mediante cualquiera de las diversas API populares. Azure Cosmos DB proporciona de forma exclusiva contratos de nivel de servicio completos para garantizar el rendimiento, la latencia, la disponibilidad y la coherencia.

Azure Cosmos DB es compatible con los datos sin esquema, lo que le permite compilar aplicaciones "Always On" con una gran capacidad de respuesta para admitir datos en continuo cambio.

Azure Cosmos DB es flexible. En el nivel más bajo, Azure Cosmos DB almacena los datos en formato de secuencia de registro de átomos (ARS). Después, los datos se abstraen y se proyectan como una API, que se especifica al crear la base de datos. Entre las opciones se incluyen SQL, MongoDB, Cassandra, Tables y Gremlin. Este nivel de flexibilidad implica que, al migrar las bases de datos de la empresa a Azure Cosmos DB, los desarrolladores pueden seguir con la API con la que se encuentren más cómodos.

# Exploración de Azure SQL Database

Azure SQL Database es una base de datos relacional basada en la última versión estable del motor de base de datos de Microsoft SQL Server. SQL Database es una base de datos de alto rendimiento, confiable, totalmente administrada y segura. Puede usarla para compilar aplicaciones y sitios web controlados por datos en el lenguaje de programación que prefiera sin necesidad de administrar infraestructura.

- Características: Azure SQL Database es un motor de base de datos de plataforma como servicio (PaaS). Controla la mayoría de las funciones de administración de bases de datos, como las actualizaciones, las aplicaciones de revisiones, las copias de seguridad y la supervisión, sin intervención del usuario. SQL Database proporciona disponibilidad del 99,99 %.  Puede crear una capa de almacenamiento de datos de gran rendimiento y disponibilidad para las aplicaciones y las soluciones de Azure. SQL Database puede ser la opción adecuada para una variedad de aplicaciones modernas en la nube, porque le permite procesar tanto datos relacionales como estructuras no relacionales, por ejemplo, grafos, JSON, elementos espaciales y XML.
- Migración: En la actualidad, Tailwind Traders usa varios servidores locales que ejecutan SQL Server, que proporcionan almacenamiento de datos para el sitio web de acceso público (por ejemplo, datos de clientes, historial de pedidos y catálogos de productos). Además, los servidores locales que ejecutan SQL Server también proporcionan almacenamiento de datos para el sitio web del portal de aprendizaje solo para uso interno. Tailwind Traders usa el sitio web para los materiales de aprendizaje de los nuevos empleados (como los materiales de estudio, los detalles de certificación y los certificados de aprendizaje). En la ilustración siguiente se muestran los tipos de datos que su empresa puede almacenar en el sitio web del portal de aprendizaje de Azure SQL Database.

Puede migrar las bases de datos existentes de SQL Server con un tiempo de inactividad mínimo mediante Azure Database Migration Service. Microsoft Data Migration Assistant puede generar informes de evaluación que proporcionan recomendaciones para ayudarlo a través de los cambios necesarios anteriores a la ejecución de una migración. Después de evaluar y resolver cualquier corrección necesaria, está listo para comenzar el proceso de migración. Azure Database Migration Service realiza todos los pasos necesarios. 
