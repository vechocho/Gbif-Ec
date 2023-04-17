# Página de inicio

## Página de inicio

Al acceder a la herramienta se presenta una página donde puede visualizar las opciones:

![](<../.gitbook/assets/image (10) (1).png>)

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

* [Conjunto de Datos ](pagina-de-inicio.md#conjunto-de-datos)
* [Mapeo Darwin Core ](pagina-de-inicio.md#mapeo-darwin-core)
* [Metadatos ](pagina-de-inicio.md#metadatos)
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

![](<../.gitbook/assets/image (12).png>)

1. Pulse en \[Agregar], y luego selecciones "Archivo", esto permite ubicar la ruta o acceso del archivo a importar. &#x20;
2. Seleccione el archivo. Seleccionado el archivo, este se visualiza en la página con el nombre y la extensión del mismo (.txt, .csv, entre otros)
3. Pulse en \[Agregar], si el archivo es el correcto, este se carga en el IPT. Si se cometió un error al seleccionar el archivo Pulse en \[Limpiar]. El archivo se quitará de la herramienta.&#x20;
4. Una vez agregado el archivo se abrirá una página que muestra el nombre del recurso y sus características (tamaño, número de filas, etc.), delimitadores, formatos y codificación que realiza el IPT al cargar el archivo. Se recomienda no modificar los elementos a menos que se conozca los efectos sobre la forma de leerlo por el IPT.

![](<../.gitbook/assets/image (3) (2).png>)

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

![](<../.gitbook/assets/image (1).png>)

El proceso es igual para conjuntos de datos de tipo Occurrence (Datos primarios sobre registros biológicos), Checklist (Listas de chequeo) y Sampling Event (Datos de eventos de muestreo). El mapeo se realiza en los siguientes pasos:

1. Seleccione Agregar,&#x20;
2. Seleccione un paquete del estándar correspondiente para el conjunto de datos y de clic en Agregar.

![](<../.gitbook/assets/image (4).png>)

3. Seleccione el Archivo que va a ser mapeado para el paquete correspondiente y de clici en Guardar

![](<../.gitbook/assets/image (8).png>)

A continuación, se abrirá la página con la vista general para el mapeo Darwin Core del conjunto de datos.&#x20;

Un mensaje informa sobre los elementos mapeados automáticamente a los elementos del estándar Darwin Core.

![](<../.gitbook/assets/image (11).png>)

La página además presenta:&#x20;

* Índice temático de los campos del estándar Darwin Core que cuenta con filtros para mostrar u ocultar campos.&#x20;
* Área de mapeo, donde se muestran los campos del estándar y permite establecer la correspondencia con el campo del conjunto de datos cargado.&#x20;

> Si los datos se cargaron correctamente y los campos del encabezado tienen correspondencia con los del estándar, el mapeo se realizará automáticamente. Caso contrario al final de la página se mostrarán los campos no mapeados. Si esto no sucede se debe asignar los nombres de las columnas del archivo cargado con su equivalente en el DwC de forma manual.

### Metadatos&#x20;

Los metadatos responden a las preguntas ¿Quién?, ¿Qué?, ¿Dónde?, ¿Cuándo? y ¿Cómo? de un conjunto de datos, que permite al usuario conocer su contexto y el uso concreto de los mismos.&#x20;

![](<../.gitbook/assets/image (10).png>)

Para completar los metadatos del Recurso haga clic en \[Editar] Se abre la página “Metadatos Básicos”, la cual está organizada por temática (geografía, taxonomía, etc.).&#x20;

La columna a la izquierda lista los apartados para cada set de información que se constituirán en los metadatos relacionados con el archivo a compartirse. Haga clic en cada título para acceder a un apartado particular.

#### Metadatos básicos

En esta página la página complete la información requerida:&#x20;

![](../.gitbook/assets/image.png)

Título. - Nombre largo. Describa el contenido del recurso. Responde a las preguntas ¿Qué?, ¿Dónde?, ¿Cuándo? y ¿Cómo?&#x20;

Organización Publicadora. - La organización responsable de la publicación del recurso. Una vez seleccionada la Organización, ésta no puede ser cambiada.&#x20;

> En el IPT de producción aparecerá listada su organización. En caso de no estar disponible, deberá contactarse con el Administrador del Nodo para que se registre la organización. En el IPT de pruebas esta opción no está disponible.&#x20;

**Tipo. -** El valor de este campo depende del mapeo del recurso y no es posible editarlo si el mapeo Darwin Core ya se ha hecho. Si el tipo de recurso deseado no se encuentra en la lista, se puede elegir el campo “otro”.&#x20;

**Subtipo. -** Las opciones dependen del elemento Tipo. Si el subtipo no se encuentra en la lista, deje el campo con la selección por defecto. Para los especimenes de Herbarios y museos se debe seleccionar "Ejemplar"

**Idioma de los Metadatos. -** El idioma en que está escrita la información de los metadatos.&#x20;

**Idioma de los Datos. -** El idioma principal de los datos.&#x20;

**Licencia de los datos. -** La licencia que se aplica a un conjunto de datos proporciona una forma estandarizada de definir el uso apropiado de su trabajo.&#x20;

* CC0 1.0 Dominio público, la renuncia a todos los derechos sobre la obra. Se puede copiar, modificar, distribuir y reproducir el trabajo, incluso para fines comerciales, sin previa autorización.&#x20;
* CC BY 4.0 Permite distribuir, mezclar, ajustar y construir a partir de su obra, incluso con fines comerciales, siempre que sea reconocida la autoría.&#x20;
* CC BY-NC 4.0 Permite distribuir, mezclar, ajustar y construir a partir de su obra, siempre que sea reconocida la autoría de la creación original y no tenga fines comerciales.&#x20;

> La licencia seleccionada aquí deberá ser la misma que se indique en el conjunto de datos en el campo si este fue incluido en el archivo.

**Descripción. -** Una breve descripción del recurso que está siendo documentado, pueden ser varios párrafos. Debe proveer información que permita entender el contexto del conjunto de datos. Para añadir saltos de línea haga clic en \[Añadir Párrafo]

> Los apartados con el símbolo “\*” son obligatorios. Frecuencia de actualización. - Frecuencia con la que se planifica realizar cambios al recurso.&#x20;

**Contactos del Recurso. -** Personas y organizaciones que custodian o deben ser contactadas para obtener más información o puedan resolver los posibles problemas con el recurso o los datos compartidos.&#x20;

* Haga clic en \[Añadir contacto del recurso]&#x20;
* Complete el formulario&#x20;

**Creadores del recurso. -** Lista de creadores, corresponde a las personas y organizaciones que han creado el recurso, en orden de prioridad. La lista será utilizada para generar la referencia del recurso (si la generación automática está activada).&#x20;

* Haga clic en \[Añadir creador del recurso]&#x20;
* Complete el formulario&#x20;

**Proveedores de los Metadatos. -** Personas y organizaciones responsables de generar los metadatos del recurso.&#x20;

* Haga clic en \[Añadir proveedor de los metadatos]&#x20;
* Complete el formulario

Complete toda la información solicitada, recuerde que los ítems con “\*” son obligatorios.&#x20;

Una vez completada la sección, de clic en guardar.

#### Cobertura geográfica

![](<../.gitbook/assets/image (2).png>)

Expone el área geográfica cubierta por el recurso, por defecto se encuentra activada la opción \[Establecer cobertura global], si la cobertura no es global desmarque la opción y se libera el uso de la aplicación.&#x20;

**Mapa de cobertura. -** El mapa muestra un recuadro. Las esquinas corresponden a los valores de Latitud y Longitud.&#x20;

* Desplace las esquinas para establecer los límites geográficos del recuadro.&#x20;
* Establecer cobertura global. - Haga clic en la casilla, y la cobertura geográfica cambia a una cobertura global.&#x20;

**Longitud Mínima/Longitud Máxima/Latitud Mínima/Latitud Máxima. -** Estos valores se cargan automáticamente una vez fijado el recuadro; o puede ingresar manualmente la información del cuadrante geográfico de cobertura de los datos.&#x20;

**Descripción. -** Redacte un párrafo que explique la selección del recuadro, sea porque el recurso cubre la superficie del país o corresponde a una localidad en particular.&#x20;

Una vez completada la información, haga clic en \[Guardar]