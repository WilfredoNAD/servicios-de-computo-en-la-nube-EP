**1. Máquinas Virtuales: ¿Qué tipo de aplicaciones podrías ejecutar en una máquina virtual (AWS EC2, Azure Virtual Machines, Google Compute Engine)? Da al menos 3 ejemplos concretos y explica por qué una máquina virtual sería adecuada para cada caso.**

Empezando por **¿Que es una maquina virtual?** es un entorno informático aislado que simula un ordenador físico completo, ejecutando un sistema operativo y aplicaciones, dentro de otro sistema operativo.

   Los tipos de aplicaciones que se pueden ejecutar en una maquina virtual son mucho y se dividen dependiendo de la necesidad o el fin:

  **Desarrollo de software:**
   
       Entornos de desarrollo integrados (IDEs)
       Servidores de desarrollo
       Bases de datos
  
  **Pruebas de software:**
        
        Entornos de prueba: Para ejecutar pruebas unitarias, de integración y de sistema en un entorno controlado.
        Entornos de staging: Para probar aplicaciones antes de desplegarlas en producción.

  **Producción:**
  
    Servidores web: Para hospedar sitios web, aplicaciones web y servicios web.
    Bases de datos: Para almacenar grandes volúmenes de datos.
    Servidores de correo electrónico: Para gestionar el correo electrónico de una organización.
    Servidores de archivos: Para almacenar y compartir archivos.
    Aplicaciones empresariales: Como ERP, CRM, software de contabilidad, etc.
    Aplicaciones de virtualización: Para crear máquinas virtuales dentro de otras máquinas virtuales (nested virtualization).
       
**Otros usos:**

    Juegos: Para ejecutar juegos antiguos o que requieren configuraciones específicas.
    Sistemas operativos antiguos: Para ejecutar aplicaciones que solo funcionan en versiones antiguas de Windows o Linux.
    Análisis de datos: Para ejecutar herramientas de análisis de datos como Hadoop o Spark.
    Machine learning: Para entrenar y desplegar modelos de machine learning.

**   Ejemplos:**

  **Numero 1:**

Un equipo de desarrolladores planea realizar una distribucion linux propia, la cual esta distinada para un grupo de tareas especificas, entonces luego de los pasos previos a la creacion de la misma. lo mas sensato es utilizar un entorno virtual con la finalidad de ver el rendimiento de dicha  nueva distribucion y poder observar los errores o defectos que tengan la misma, mientras se va realizando todos estos pasos ya luego en un piloto se utiliza una maquina real para observar dicha nueva Distro.


  **Numero 2:**

Un grupo de amigos con conocimientos medios en informatica y computacion quieren pasar tiempo libre compartiendo jugando un juego online el cual es minecraft, pero quieren lograr usar un servidor propio, con sus reglas debido a que los serves publicos son muy complicados con la experiencia de juego. Entonces a travez de una maquina virtual investigan y configuran un servidor propio con la ayuda de contenedores docker y asi pueden lograr jugar en su propio servidor

   **Numero 3:**

Los estudiantes de desarrollo web, ambientado al lado full stack para seguir en sus practicas de despliegue, pues empiezan a aprender sobre la maquinas virtuales para alojar sus propias paginas web o aplicaciones web utilizan maquinas virtuales para varias funciones, puede usarlas para alojar la propia pagina o app, alojar la parte del servidor de su app web o hasta para manejar sus servicios de correos propios.
   

2. Funciones Serverless: ¿Qué es una función serverless (AWS Lambda, Azure Functions, Google Cloud Functions)? Explica su funcionamiento y da al menos 2 ejemplos de casos de uso.

    Serverless significa sin servidor, es una solución que permite crear y ejecutar aplicaciones con rapidez y menor costo total de propiedad, ya que no es necesario aprovisionar y administrar infraestructura.

   ¿Cómo funcionan las funciones serverless?

**Eventos:** El código se activa en respuesta a eventos específicos. Estos eventos pueden ser muy variados, desde una solicitud HTTP (por ejemplo, cuando alguien visita tu sitio web) hasta cambios en una base de datos, cargas de archivos, mensajes en colas, o incluso eventos programados (como ejecutar una tarea cada día a las 3 de la mañana).
   
**Ejecución bajo demanda:** Cuando se produce el evento, la plataforma serverless detecta el evento y ejecuta tu código automáticamente.
   
**Escalado automático:** La plataforma se encarga de escalar los recursos de manera automática para hacer frente a la demanda. Si tienes un pico de tráfico, se provisionarán más recursos para ejecutar tus funciones; si el tráfico disminuye, se reducirán los recursos. Esto significa que puedes manejar picos de carga sin preocuparte por quedarte sin capacidad.
   
**Pago por uso:** Solo pagas por la cantidad de tiempo que se ejecuta tu código. Esto significa que si tu función se ejecuta durante un segundo, solo pagarás por ese segundo. No hay costos fijos por mantener servidores inactivos.

Ejemplo:

  **Numero 1:**


Automatización de tareas

Caso de uso: Una empresa quiere automatizar tareas repetitivas, como enviar correos electrónicos programados o generar informes diarios.
Solución serverless: Se crean funciones serverless que se ejecutan en momentos específicos o en respuesta a eventos programados. Por ejemplo:
-Una función que envía un correo electrónico de bienvenida a los nuevos usuarios cada mañana.
-Otra función que genera un informe de ventas diario y lo envía a los responsables.

   **Numero 2:**

   Chatbots y asistentes virtuales

Caso de uso: Una empresa quiere crear un chatbot para atender a sus clientes.
Solución serverless: Cada vez que un usuario envía un mensaje al chatbot, se activa una función serverless que:
-Analiza el mensaje del usuario para entender su intención.
-Busca la respuesta adecuada en una base de conocimiento.
-Genera una respuesta personalizada y la envía al usuario.

3. Comparación: ¿Qué diferencias hay entre usar una máquina virtual y una función serverless? ¿En qué situaciones usarías cada una?  Considera factores como control, escalabilidad, costo y facilidad de uso.

    La elección entre una máquina virtual (VM) y una función serverless depende en gran medida de las necesidades específicas de tu proyecto. Ambas tecnologías ofrecen formas de ejecutar código en la nube, pero tienen características y usos distintos.

   en cuanto a las carecteristica son muy distintas:

   en cuanto a:

   **Control:** En este ambito el se alza con la victoria el Serverless ya que requiere de un control minimo en comparacion a una MV

  **Escalabilidad:** La podemos dejar en un empate tecnico ya que a pesar de que por el lado de serverless es automatica, po
   el lado de la MV es manual y puede ser ajustado a lo que requiera el producto.

   **Costo:** En este apartado el gana definitivamente el Serverless debido a que en las MV tienen precio y cuotas fijas se usen
   o no!
   en cambio en serverles se cobra dependiendo del uso se utilizó por 1 segundo pues simplemente se cobrara ese segundo

  **Facilidad:** en este ambito es mucho mas facil utilizar funciones severless debido a que las MV tiene una mucho mayor curva de
   aprendizaje

   Ya con estos puntos podemos decir que todo va a depender de la finalidad que se le va a dar a l servicio elegido:

   **Máquinas virtuales:** Son ideales para aplicaciones que requieren un alto nivel de control, personalización y estabilidad.
   Son adecuadas para cargas de trabajo estables y predecibles.
   
   **Funciones serverless:** Son ideales para aplicaciones que necesitan escalar rápidamente, tienen picos de tráfico impredecibles y
   requieren un desarrollo rápido. Son perfectas para microservicios y procesamiento de eventos.

4. Sitio Web Sencillo: Si tuvieras que construir un sitio web sencillo, ¿qué servicio de cómputo usarías (máquina virtual o función serverless) y por qué?  Justifica tu elección.

    Si es una pagina sencilla que en su mayoria va a estar compuesta por el trio del front (HTML, CSS y JS) y tambien
   metiendo una que otra API sensilla, seria mejor decantarse por un Serverless. ya que existe ya herramientas como vercel o
   hostinger para la facil configuracion de la misma.

5. Tipos de Instancias (AWS EC2): Investiga al menos 3 tipos de instancias de Amazon EC2 (ej. t2.micro, m5.large, etc.) y explica para qué se utiliza cada una. Considera factores como capacidad de procesamiento, memoria RAM y costo.

**t2.micro:** Instancia de uso general, de bajo costo, ideal para cargas de trabajo pequeñas y medianas. Ofrece un rendimiento de CPU base con capacidad de burst para manejar picos de carga.
Es una excelente opción para comenzar y para aplicaciones que no requieren un rendimiento de CPU demasiado altos y aun asi son
excelentes opciones para bases de datos pequeñas y medianas, servicios web de trafico mediano a alto y procesamiento de datos.

**m5.large:** Instancia de uso general de última generación, que ofrece un equilibrio de CPU, memoria y E/S. Ideal para cargas de trabajo variadas, como servidores web, bases de datos y aplicaciones empresariales.
Esta es una mucha mejor opcion que la t2.micro, ya que maneja la ultima generacion de intel y el rendimiento de la misma aumenta
asi que puede usarse de en una escala mucho mayor que la anterior y con una buena relacion precio/rendimiento

**c5.large:** están optimizadas para cargas de trabajo con uso intensivo de computación y ofrecen un alto rendimiento de manera rentable con una buena relación entre capacidad de computación y precio. ya este es un nivel mayor de instancia la cual soporta grandes cantidades de carga de trabajo.


6. Activación de Funciones Serverless: ¿Cómo se activa una función serverless? Explica los diferentes tipos de triggers o eventos que pueden iniciar la ejecución de una función.

Activar una función serverless significa iniciar la ejecución de un fragmento de código en respuesta a un evento específico.

Para que se ejecuten estos fragmentos de codigo es necesario una accion o evento y esa son los triggers. Los triggers son el corazón de las funciones serverless, permitiendo que estas se ejecuten de manera reactiva en respuesta a eventos específicos. Al comprender los diferentes tipos de triggers y cómo configurarlos, podrás construir aplicaciones serverless altamente escalables y eficientes.

La configuración de los triggers varía según la plataforma serverless que estés utilizando (AWS Lambda, Google Cloud Functions, Azure Functions, etc.). Generalmente, se realiza a través de una consola de administración o mediante la definición de recursos en un archivo de configuración (como un archivo YAML o JSON)

En cuanto a los tipo de triggers o eventos mencionaremos algunos:

-Peticiones HTTP: La función se activa cuando recibe una solicitud HTTP, ya sea un GET, POST, PUT, DELETE o cualquier otro método HTTP.

-Eventos de base de datos: Al realizar operaciones en una base de datos (inserción, actualización, eliminación), se pueden generar eventos que activan funciones.

-Eventos de mensajería: Servicios de mensajería como SNS (Simple Notification Service) o SQS (Simple Queue Service) permiten enviar mensajes que desencadenan funciones.

-Eventos de programación: Puedes programar una función para que se ejecute en intervalos regulares (cron jobs) o en momentos específicos.


9. Herramientas de Despliegue: Investiga al menos 2 herramientas que se utilizan para desplegar aplicaciones en la nube (ej. AWS Elastic Beanstalk, Azure DevOps, Google Cloud Build). Describe brevemente sus funciones.

**AWS Elastic Beanstalk:**
 es un servicio que se usa para implementar y escalar aplicaciones y servicios web. Cargue el código y Elastic Beanstalk administrará de manera automática la implementación, desde el aprovisionamiento de la capacidad, el equilibrio de carga y el escalado automático hasta la supervisión del estado de la aplicación.

entre sus funciones destacamos:

-Automatizacion del despliegue: Subes tu código y Elastic Beanstalk se encarga de todo el proceso de despliegue en la nube de AWS.
-Provisiona los recursos necesarios: Crea y configura automáticamente los recursos necesarios para ejecutar tu aplicación, como instancias EC2, balanceadores de carga y grupos de autoescalado.
-Gestiona la escalabilidad: Ajusta automáticamente la capacidad de tu aplicación para hacer frente a las variaciones de carga.
-Supervisa el estado de la aplicación: Te proporciona herramientas para monitorear el rendimiento y la salud de tu aplicación.
-Soporta múltiples lenguajes: Es compatible con una amplia variedad de lenguajes de programación, como Java, .NET, Python, Ruby, Node.js, PHP, Go y más.

**Google Cloud Build:**

Google Cloud Build es una plataforma de CI/CD (Integración Continua y Entrega Continua) que te permite automatizar el proceso de construcción de software en Google Cloud.

Entre sus funciones estan:

-Automatiza la compilación: Define una configuración de compilación (build config) que especifica los pasos necesarios para construir tu aplicación, como descargar dependencias, compilar el código y crear contenedores Docker.
-Integración continua: Se integra con sistemas de control de versiones como GitHub, GitLab o Bitbucket para automatizar las compilaciones cada vez que se produce un cambio en el código.
-Pruebas: Puedes ejecutar pruebas unitarias, de integración y otras pruebas automatizadas como parte del proceso de compilación.
-Creación de imágenes de contenedor: Genera imágenes de contenedor Docker que pueden ser desplegadas en diferentes entornos.
-Despliegue: Puede desplegar directamente a diferentes entornos como Cloud Run, Kubernetes Engine, App Engine, etc.
-Escalabilidad: Puede manejar múltiples compilaciones en paralelo y escalar automáticamente para adaptarse a las necesidades de tu proyecto.


