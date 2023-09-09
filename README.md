__________________________
# Patrones Arquitectonicos
Una arquitectura adecuada que nos proporcione la funcionalidad deseada y los atributos de calidad. Por lo tanto, debemos entender diferentes arquitecturas, antes de aplicarlas a nuestro diseño.
![image](https://github.com/WinDev-es/PatronesArquitectonicos/assets/62816735/6aae702a-31a2-4f9b-9c89-4c5e15a3c0b2)

## Los 10 patrones comunes de arquitectura de software

## ¿Qué es un patrón arquitectónico?
De acuerdo con Wikipedia,
Un patrón arquitectónico es una solución general y reutilizable a un problema común en la arquitectura de software dentro de un contexto dado. Los patrones arquitectónicos son similares al patrón de diseño de software pero tienen un alcance más amplio.

###En este artículo, explicaré brevemente los siguientes 10 patrones arquitectónicos comunes con su uso, pros y contras.

-[Patrón de capas] (Patrón de capas)
-[Patrón cliente-servidor] (Patrón cliente-servidor)
-[Patrón maestro-esclavo] (Patrón maestro-esclavo)
-[Patrón de filtro de tubería] (Patrón de filtro de tubería)
-[Patrón de intermediario] (Patrón de intermediario)
-[Patrón de igual a igual] (Patrón de igual a igual)
-[Patrón de bus de evento] (Patrón de bus de evento)
-[Modelo-vista-controlador] (Modelo-vista-controlador)
-[Patrón de pizarra] (Patrón de pizarra)
-[Patrón de intérprete] (Patrón de intérprete)

## 1. Patrón de capas
Este patrón se puede utilizar para estructurar programas que se pueden descomponer en grupos de subtareas, cada una de las cuales se encuentra en un nivel particular de abstracción. Cada capa proporciona servicios a la siguiente capa superior.

## Las 4 capas más comúnmente encontradas de un sistema de información general son las siguientes.

Capa de presentación (También conocida como capa UI)
Capa de aplicación (También conocida como capa de servicio)
Capa de lógica de negocios (También conocida como capa de dominio)
Capa de acceso a datos (También conocida como capa de persistencia)

## Uso
Aplicaciones de escritorio generales.
Aplicaciones web de comercio electrónico.

![image](https://github.com/WinDev-es/PatronesArquitectonicos/assets/62816735/3ed57970-cc82-40c5-ba23-055747069a5e)

## 2. Patrón cliente-servidor
Este patrón consiste en dos partes; un servidor y múltiples clientes . El componente del servidor proporcionará servicios a múltiples componentes del cliente. Los clientes solicitan servicios del servidor y el servidor proporciona servicios relevantes a esos clientes. Además, el servidor sigue escuchando las solicitudes de los clientes.

## Uso
Aplicaciones en línea como correo electrónico, uso compartido de documentos y banca.

![image](https://github.com/WinDev-es/PatronesArquitectonicos/assets/62816735/41db8f0b-5e63-49cf-ad86-ba1803805eda)

## 3. Patrón maestro-esclavo
Este patrón consiste en dos partes; maestro y esclavos . El componente maestro distribuye el trabajo entre componentes esclavos idénticos y calcula el resultado final de los resultados que devuelven los esclavos.

## Uso
En la replicación de la base de datos, la base de datos maestra se considera como la fuente autorizada y las bases de datos esclavas se sincronizan con ella.
Periféricos conectados a un bus en un sistema informático (unidades maestra y esclava).

![image](https://github.com/WinDev-es/PatronesArquitectonicos/assets/62816735/365f6127-3400-4529-971f-0d49a29d0c06)

## 4. Patrón de filtro de tubería
Este patrón se puede usar para estructurar sistemas que producen y procesan una secuencia de datos. Cada paso de procesamiento se incluye dentro de un componente de filtro. Los datos que se procesarán se pasan a través de las tuberías . Estas tuberías se pueden utilizar para el almacenamiento en búfer o con fines de sincronización.

## Uso
Compiladores Los filtros consecutivos realizan análisis léxico, análisis sintáctico y generación de código.
Flujos de trabajo en bioinformática.

![image](https://github.com/WinDev-es/PatronesArquitectonicos/assets/62816735/4ef4aa5e-0937-4a47-af02-630edd713556)

## 5. Patrón del agente
Este patrón se usa para estructurar sistemas distribuidos con componentes desacoplados. Estos componentes pueden interactuar entre sí mediante invocaciones de servicios remotos. Un componente de intermediario es responsable de la coordinación de la comunicación entre los componentes .

Los servidores publican sus capacidades (servicios y características) a un intermediario. Los clientes solicitan un servicio del intermediario y el intermediario redirecciona al cliente a un servicio adecuado desde su registro.

## Uso
Software de Message Broker como Apache ActiveMQ , Apache Kafka , RabbitMQ y JBoss Messaging.

![image](https://github.com/WinDev-es/PatronesArquitectonicos/assets/62816735/079f69cb-7755-4daa-acd2-678d8cd1b8b3)

## 6. Patrón de igual a igual
En este patrón, los componentes individuales se conocen como pares . Los pares pueden funcionar tanto como un cliente , solicitando servicios de otros pares, y como un servidor , proporcionando servicios a otros pares. Un par puede actuar como un cliente o como un servidor o como ambos, y puede cambiar su rol dinámicamente con el tiempo.

## Uso
Redes de intercambio de archivos como Gnutella y G2 )
Protocolos multimedia como P2PTV y PDTP.

![image](https://github.com/WinDev-es/PatronesArquitectonicos/assets/62816735/321afb1e-ac12-4e97-87bd-5e13ba9ffb70)

## 7. Patrón de bus de evento
Este patrón trata principalmente con eventos y tiene 4 componentes principales; fuente de evento , escucha de evento , canal y bus de evento . Las fuentes publican mensajes en canales particulares en un bus de eventos. Los oyentes se suscriben a canales particulares. Los oyentes son notificados de los mensajes que se publican en un canal al que se han suscrito anteriormente.

## Uso
Desarrollo de Android
Servicios de notificación.

![image](https://github.com/WinDev-es/PatronesArquitectonicos/assets/62816735/97ae858e-3bf1-4b47-9711-0d97284caa71)

## 8. Patrón de modelo-vista-controlador
Este patrón, también conocido como patrón MVC, divide una aplicación interactiva en 3 partes, como

## modelo — contiene la funcionalidad y los datos básicos
vista : muestra la información al usuario (se puede definir más de una vista)
controlador : maneja la entrada del usuario
Esto se hace para separar las representaciones internas de información de las formas en que se presenta y acepta la información del usuario. Desacopla los componentes y permite la reutilización eficiente del código.

## Uso
Arquitectura para aplicaciones World Wide Web en los principales lenguajes de programación.
Marcos web como Django y Rails.

![image](https://github.com/WinDev-es/PatronesArquitectonicos/assets/62816735/b786862b-3990-4500-9d83-00084b5b246d)

## 9. Patrón de pizarra
Este patrón es útil para problemas para los que no se conocen estrategias de solución deterministas. El patrón de pizarra consta de 3 componentes principales.

## pizarra : una memoria global estructurada que contiene objetos del espacio de solución
fuente de conocimiento : módulos especializados con su propia representación
componente de control : selecciona, configura y ejecuta módulos.
Todos los componentes tienen acceso a la pizarra. Los componentes pueden producir nuevos objetos de datos que se agregan a la pizarra. Los componentes buscan tipos particulares de datos en la pizarra, y pueden encontrarlos por coincidencia de patrones con la fuente de conocimiento existente.

## Uso
Reconocimiento de voz
Identificación y seguimiento del vehículo
Identificación de la estructura proteica
Sonar señala la interpretación.

![image](https://github.com/WinDev-es/PatronesArquitectonicos/assets/62816735/743414f8-a785-4fb8-963b-c805fa5157ed)

## 10. Patrón de intérprete
Este patrón se usa para diseñar un componente que interpreta programas escritos en un lenguaje dedicado. Especifica principalmente cómo evaluar las líneas de programas, conocidas como oraciones o expresiones escritas en un idioma particular. La idea básica es tener una clase para cada símbolo del idioma.

## Uso
Lenguajes de consulta de base de datos como SQL.
Idiomas utilizados para describir los protocolos de comunicación.

![image](https://github.com/WinDev-es/PatronesArquitectonicos/assets/62816735/f54d78ac-98b9-48c3-a429-0737ef1fcace)
