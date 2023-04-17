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

## Crear Nuevo Recurso

Para crear un nuevo recurso desde cero se deben seguir los siguientes pasos:

1. Dentro de \[Gestión de recursos] se debe seleccionar la opción \[Crear nuevo]
2. Otorgue un \[Nombre corto] al recurso va a cargar, esto permite identificar de manera única el recurso en el entorno del IPT, **y será utilizado en la URL para acceder al recurso a través de Internet.**

> Se recomienda que este nombre contenga al menos tres caracteres, estos podrán ser caracteres alfanuméricos, pero no deberá incluir espacios en blanco o signos de puntuación, excepto guiones o guiones bajos. Ejemplo: (Anfibios de la Reserva Madre de Dios) ANF\_RM

3. Seleccione entre: registros biológicos (Occurrence), lista de chequeo (Checklists), evento de muestreo (Sampling Event data) o metadatos, dependiendo de la naturaleza de los datos a ser compartidos.

> En caso de que usted haya ya completado la publicación en el ITP de prueba y haya descargado su archivo Darwin Core en formato zip debe seleccionar también la opción cargar desde archivo y Pulse en \[Elegir archivo] para seleccionar el archivo (hasta 100MB)

4. Pulse en \[Crear]

## Vista General

En la página de Vista General se encuentra las siguientes secciones.

* [Conjunto de Datos ](compartir-datos-por-el-ipt-integrated-publishing-toolkit.md#conjunto-de-datos)
* [Mapeo Darwin Core ](compartir-datos-por-el-ipt-integrated-publishing-toolkit.md#mapeo-darwin-core)
* Metadatos&#x20;
* Visibilidad&#x20;
* Publicación&#x20;
* Registro&#x20;
* Autopublicación&#x20;
* Redes&#x20;
* Editores de Recursos

Al inicio de la página se visualiza el nombre corto asignado al recurso que se encuentra gestionando. Al pulsar sobre el ícono `Ⓘ`, se despliegan notas explicativas sobre las características de cada sección.

### Conjunto de Datos&#x20;

Permite importar datos primarios al IPT en formato de texto delimitado (csv, tab, y archivos con cualquier otro delimitador) y archivos de Excel, se recomienda subir el archivo en formato de texto (.txt | .tsv) delimitado por tabulaciones.

Para importar datos también es posible hacerlo conectando bases de datos, en la opción “Base de datos” y desde una "URL" pero en esta guía solo se explicará cómo importar datos desde un archivo.&#x20;

Para importar el archivo al IPT, realice las siguientes acciones:&#x20;

![](<.gitbook/assets/image (12).png>)

1. Pulse en \[Agregar], y luego selecciones "Archivo", esto permite ubicar la ruta o acceso del archivo a importar. &#x20;
2. Seleccione el archivo. Seleccionado el archivo, este se visualiza en la página con el nombre y la extensión del mismo (.txt, .csv, entre otros)
3. Pulse en \[Agregar], si el archivo es el correcto, este se carga en el IPT. Si se cometió un error al seleccionar el archivo Pulse en \[Limpiar]. El archivo se quitará de la herramienta.&#x20;
4. Una vez agregado el archivo se abrirá una página que muestra el nombre del recurso y sus características (tamaño, número de filas, etc.), delimitadores, formatos y codificación que realiza el IPT al cargar el archivo. Se recomienda no modificar los elementos a menos que se conozca los efectos sobre la forma de leerlo por el IPT.

![](<.gitbook/assets/image (3).png>)

En la página se visualiza si el archivo es reconocido por el IPT, que se evidencia por el ícono en color verde, ubicado en la parte superior izquierda. Puede observar el número de columnas del archivo que es importante revisarlo para verificar que el archivo esté completo.

En los campos inferiores, es importante indicar la forma como está configurado el archivo indicando:

1. El número de filas de encabezado (nombres de campos).
2. El delimitador de texto, usualmente son comillas dobles \["]
3. La codificación de caracteres del archivo que usualmente es ISO-8859-1.
4. El delimitador de columnas, al ser un archivo .txt separado por tabuladores se deberá ingresar `"\t"`
5. El delimitador de valores múltiples, que, si se aplicó las recomendaciones del estándar definido en el Catálogo Nacional de Objetos Biológicos, este carácter debería ser la línea vertical "|" o pleca.&#x20;
6. El formato de la fecha, que se recomienda sea DD-MM-AAAA o eventualmente podría estar configurado en AAAA-MM-DD

De clic en la opción “Guardar”, una vez se haya revisado la información cargada.

### Mapeo Darwin Core&#x20;

En esta sección se identifica la correspondencia entre los nombres de las columnas del archivo cargado con las columnas del estándar Darwin Core y sus extensiones.

![](<.gitbook/assets/image (1).png>)

El proceso es igual para conjuntos de datos de tipo Occurrence (Datos primarios sobre registros biológicos), Checklist (Listas de chequeo) y Sampling Event (Datos de eventos de muestreo). El mapeo se realiza en los siguientes pasos:

1. Seleccione Agregar,&#x20;
2. Seleccione un paquete del estándar correspondiente para el conjunto de datos y de clic en Agregar.

![](<.gitbook/assets/image (4).png>)

3. Seleccione el Archivo que va a ser mapeado para el paquete correspondiente y de clici en Guardar

![](<.gitbook/assets/image (8).png>)

A continuación, se abrirá la página con la vista general para el mapeo Darwin Core del conjunto de datos.&#x20;

Un mensaje informa sobre los elementos mapeados automáticamente a los elementos del estándar Darwin Core.

![](<.gitbook/assets/image (11).png>)

La página además presenta:&#x20;

* Índice temático de los campos del estándar Darwin Core que cuenta con filtros para mostrar u ocultar campos.&#x20;
* Área de mapeo, donde se muestran los campos del estándar y permite establecer la correspondencia con el campo del conjunto de datos cargado.&#x20;

> Si los datos se cargaron correctamente y los campos del encabezado tienen correspondencia con los del estándar, el mapeo se realizará automáticamente. Caso contrario al final de la página se mostrarán los campos no mapeados. Si esto no sucede se debe asignar los nombres de las columnas del archivo cargado con su equivalente en el DwC de forma manual.

### Metadatos&#x20;





