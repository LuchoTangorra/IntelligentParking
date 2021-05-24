# Intelligent parking (final degree project)
Tesis presentada y aprobada para la finalización de la carrera Ingeniería de Sistemas, brindada en la Universidad del Centro de la Provincia de Buenos Aires. 

El informe presentado se podrá encontrar en el archivo **Informe Tesis Luciano Tangorra.pdf**

### Motivación
Una porción significativa de las ciudades está destinada a espacio de estacionamiento, por ejemplo, en 18% de espacio en la ciudad de Nueva York está destinado al estacionamiento, en Londres el 16%, aunque puede llegar a cerca del 80% en ciudades como Los Ángeles o Melbourne. Las soluciones de estacionamiento inteligente, o Smart Parking, proponen integrar diversas tecnologías para mejorar la administración de dichos espacios. Sin embargo, el estacionamiento inteligente es un área multidisciplinaria, ya que integra diversos actores con diferentes objetivos. Por un lado, se encuentra el ciudadano/conductor, que espera poder conseguir un lugar de estacionamiento lo más cercano posible a su destino. Además, puede tener intereses económicos, como estacionar en zonas sin estacionamiento medido. Por otro lado, el municipio que puede estar interesado en reducir el tiempo que los ciudadanos estacionan en zonas de alto tráfico para que más ciudadanos puedan acceder a esos puntos de estacionamiento, reducir el tráfico y la contaminación generada por conductores buscando lugar para estacionar, detectar patrones anómalos de estacionamiento (por ejemplo, más autos estacionados que espacios disponibles) que pueden indicar conductas ilegales como estacionamiento en doble fila y/o lugares prohibidos para una mejor asignación de los inspectores de tránsito. También, puede haber intereses privados, como estacionamientos privados o concesiones de estacionamiento medido que podrían brindar sus servicios o detectar lugares donde los conductores no fichan sus autos en los parquímetros.

Muchas de las soluciones actuales se basan en la instalación de sensores especializados. Algunos de estos sensores incluyen sensores infrarrojos, de ultrasonido, y magnéticos. Sin embargo, según Evenepoel et. al. el costo de instalar y operar estas redes de sensores puede ser prohibitivo. En particular, a medida que se incrementa el número de sensores a instalar, el costo de los sensores baja linealmente de 150 euros a unos 50 euros, pero el costo de operar los mismos crece de forma exponencial. Esto presenta una limitante a la hora de implementar estas soluciones en ciudades medianas o pequeñas, con presupuestos limitados. Para solucionar esta y otras limitantes de las infraestructuras de sensores, diversos trabajos han analizado la posibilidad de utilizar los dispositivos móviles de los conductores para la recolección de datos de sus sensores. Esta metodología de recolección de datos de sensores se conoce como CrowdSensing. Por ejemplo, en se analiza la posibilidad de utilizar los magnetómetros, sensores de campos magnéticos, de los dispositivos móviles de los conductores para mapear qué lugares de estacionamiento se encuentran libres. PhonePark propone utilizar el GPS y acelerómetro de los teléfonos móviles para detectar el comportamiento de los conductores, en particular dónde estacionan y cuándo liberan el espacio, de manera de generar en tiempo real informes de disponibilidad de estacionamiento. Otros ejemplos son, en estos casos es el usuario el encargado de informar manualmente el estado de un lugar de estacionamiento. En estos casos, las aplicaciones están pensadas para playas de estacionamiento y a los usuarios se le asigna un nivel de confianza. En este sentido, el incentivo para los usuarios para participar es que la aplicación facilita encontrar lugar para estacionar.

### Objetivos
La hipótesis principal del trabajo es que se puede extraer información sobre las acciones de los conductores a través de los parquímetros de la ciudad de Tandil para detectar cuándo estacionan o liberan un lugar de estacionamiento. Se buscarán patrones de estacionamiento de los conductores para mejorar las predicciones realizadas, además de realizar un análisis de los datos obtenidos para obtener valores que serán útiles a la hora de entrenar modelos de machine learning.

Se utilizarán los parquímetros la ciudad ya que, además de poseer un gran volúmen de información de todos los usuarios que ingresan en el día a día, son sistemas que se encuentran actualmente instalados, por lo que el costo de implementación es nulo. Además, a comparación de utilizar sensores de dispositivos móviles, no se necesita ningún usuario en el sistema para poder realizar las predicciones, por lo que el volumen de conductores ingresados a nuestro sistema no será un problema. 

El objetivo final de este trabajo es utilizar la información ofrecida por los parquímetros en tiempo real para generar predicciones de qué lugares de estacionamiento se encontrarán libres en un momento determinado. En particular el proyecto tiene dos objetivos específicos: 
- Recolectar y analizar datos de parquímetros de la ciudad de Tandil para determinar las acciones de los conductores y los hábitos de estacionamiento.
- Desarrollar modelos de machine learning capaz de predecir lugares libres para estacionar.

### Conclusiones
La hipótesis en la que se afirmaba que es posible extraer información sobre las acciones de los conductores a través de los parquímetros de la ciudad de Tandil fue validada. Se pudo observar que los conductores tienden a seguir el mismo patrón de estacionamiento. A las 10 de la mañana se visualiza una gran cantidad de entradas al sistema, disminuyendo gradualmente hacia el mediodía y volviendo a aumentar el valor a la tarde. Además se advirtieron diferencias en la ocupación de cada calle según el día y el mes en el que ocurrieron.
