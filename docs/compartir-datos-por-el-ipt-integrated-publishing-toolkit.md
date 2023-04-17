# Compartir datos por el IPT (Integrated Publishing Toolkit)

Integrated Publishing Toolkit (IPT) es una aplicación web disponible de forma gratuita que ayuda en el proceso de publicación de datos sobre biodiversidad en GBIF. La Autoridad Nacional Ambiental, como Nodo Nacional de GBIF, la utiliza para gestionar conjuntos de datos de biodiversidad. Existe la posibilidad de compartir información por cuatro categorías:

1. Metadatos (Resources metadata)
2. Datos primarios sobre registros biológicos (Occurrence)
3. Listas de chequeo (Checklists)
4. Datos de eventos de muestreo (Sampling Event data)

Para poder acceder al IPT, Ingrese al enlace [http://patrimonio.ambiente.gob.ec/iptmae/](http://patrimonio.ambiente.gob.ec/iptmae/) y digite las credenciales otorgadas por el Nodo Nacional de Gbif.

<figure><img src=".gitbook/assets/image.png" alt=""><figcaption></figcaption></figure>

Adicionalmente, el nodo nacional de GBIF cuenta con un IPT en ambiente de prueba donde podrá realizar ejercicios para familiarizarse con el entorno de la herramienta, con la posibilidad que desde el ambiente de pruebas una vez revisada y verificada la información pueda realizar la carga del conjunto de datos en forma directa en el IPT de producción.

Se accede a través del siguiente enlace: [https://patrimonio.ambiente.gob.ec/iptmae\_test](https://patrimonio.ambiente.gob.ec/iptmae\_test)

## Página de inicio

Al acceder a la herramienta se presenta una página donde puede visualizar las opciones:

![](<.gitbook/assets/image (10).png>)

**Inicio.-** Permite visualizar los recursos compartidos en el IPT, se muestra la siguiente información: el logo de la Organización, nombre del recurso, organización publicadora, tipo de recurso, número de registros y las fechas de publicación.

**Gestión de Recursos.-** La página permite crear y gestionar los recursos de datos compartidos por la Organización. Esta sección solo está disponible al acceder con las credenciales otorgadas por el Administrador del Nodo.&#x20;

**Acerca de.-** Expone las características del Nodo Nacional correspondiente al Ministerio de Ambiente, Agua y Transición Ecológica.

### Gestión de recursos

&#x20;Muestra todos los recursos a los cuales el usuario tiene autorización para modificar, al pulsar sobre ellos se habilita las opciones de edición de datos y metadatos. Además, en esta página **`es posible crear un nuevo recurso`** para su carga en el IPT.&#x20;

Si cuenta con un archivo Darwin Core Archive (A-DwC) en formato .zip puede realizar la publicación en forma directa, subiendo el archivo en la opción correspondiente.&#x20;

## Crear Nuevo Recurso

Para crear un nuevo recurso desde cero se deben seguir los siguientes pasos:

1. Dentro de \[Gestión de recursos] se debe seleccionar la opción \[Crear nuevo]
2. Otorgue un \[Nombre corto] al recurso va a cargar, esto permite identificar de manera única el recurso en el entorno del IPT, **y será utilizado en la URL para acceder al recurso a través de Internet.**

> Se recomienda que este nombre contenga al menos tres caracteres, estos podrán ser caracteres alfanuméricos, pero no deberá incluir espacios en blanco o signos de puntuación, excepto guiones o guiones bajos. Ejemplo: (Anfibios de la Reserva Madre de Dios) ANF\_RM

3. Seleccione entre: registros biológicos (Occurrence), lista de chequeo (Checklists), evento de muestreo (Sampling Event data) o metadatos, dependiendo de la naturaleza de los datos a ser compartidos.

> En caso de que usted haya ya completado la publicación en el ITP de prueba y haya descargado su archivo Darwin Core en formato zip debe seleccionar también la opción cargar desde archivo y Pulse en \[Elegir archivo] para seleccionar el archivo (hasta 100MB)

4. Pulse en \[Crear]
