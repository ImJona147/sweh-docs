---
icon: books
---

# Materias

Página inicial donde se muestran todas las materias dadas de alta al sistema. Inicialmente esta todo vacío y se logra apreciar por el mensaje que nos indica si hay o no materia registrada.

<figure><img src="../.gitbook/assets/Captura de pantalla 2025-10-09 092836.png" alt=""><figcaption></figcaption></figure>

En esta vista tenemos algunas opciones que podría servir de ayuda y también para poder hacer que funcione el sistema, a continuación el funcionamiento:

1. **Agregar materia:** el funcionamiento de este es cuando no hay ninguna materia registrada en el sistema, con ese botón se podrá agregar una nueva materia.

{% hint style="info" %}
Este botón su funcionamiento es igual al que se verá en el diseño final.
{% endhint %}

<figure><img src="../.gitbook/assets/Captura de pantalla 2025-10-09 142302.png" alt="" width="495"><figcaption></figcaption></figure>

### Funciones principales

1. <mark style="color:orange;">**Barra de búsqueda:**</mark> aquí podrás ingresar el nombre/matrícula de una materia en especifico, siempre y cuando este registrado en el sistema.
2. <mark style="color:green;">**Vistas:**</mark> este botón es algo sencillo y solo sirve por pura comodidad de cambiar el tipo de vista ya sea a cuadrilla o lista.
3. <mark style="color:purple;">**Acciones principales:**</mark> estos botones son las acciones que directamente interactúa con el sistema para poder registrar/exportar las materias.

<figure><img src="../.gitbook/assets/Captura de pantalla 2025-10-09 143609.png" alt=""><figcaption></figcaption></figure>

### Acciones principales

#### Exportar

Este botón sirve para exportar <mark style="color:$success;">**TODAS**</mark> las materias registradas en el sistema en los siguientes formatos.

<p align="center"><img src="../.gitbook/assets/pdf-24.svg" alt=""><img src="../.gitbook/assets/word-24.svg" alt=""><img src="../.gitbook/assets/excel-24.svg" alt=""></p>

Se descargará en formato de tabla, en el caso de ![](../.gitbook/assets/word-24.svg) se descargará con una plantilla predeterminada y sencilla. y para el caso de ![](../.gitbook/assets/pdf-24.svg) será de igual manera un formato sencillo.

#### Importar

Esto es importante para poder agilizar la carga de materias y más cuando es la primera vez que se sube las materias. Para importar las materias solo y únicamente se puede hacer mediante un archivo ![](../.gitbook/assets/excel-24.svg) la cual debe tener el siguiente formato.

<pre class="language-csv" data-title="formato.xlsx" data-overflow="wrap" data-line-numbers data-full-width="true"><code class="lang-csv"><strong>matricula	materia	horas
</strong></code></pre>

Es importante seguir esta plantilla para que el sistema pueda detectar todas las materias del archivo ![](../.gitbook/assets/excel-24.svg) y pueda mostrar el contenido.

{% hint style="danger" %}
Es importante seguir los requisitos de cada valor. Ir a [#nueva-materia](materias.md#nueva-materia "mention")
{% endhint %}

<figure><img src="../.gitbook/assets/Captura de pantalla 2025-10-09 150849.png" alt=""><figcaption></figcaption></figure>

Cuando se tenga el formato listo con todas las materias con la información correspondiente. Nos dirigimos al botón de <mark style="color:green;">**Importar**</mark> el cual nos abrirá el selector de archivos donde debemos elegir el archivo con las materias, una vez seleccionado se verá el siguiente dialogo.

1. <mark style="color:red;">**Barra de búsqueda:**</mark> este buscador es únicamente por si queremos importar al sistema algunas materias y en dado caso que el archivo contenga un gran número de materias será más complicado su búsqueda, para eso esta este buscador, para buscar por nombre y/o matrícula.
2. <mark style="color:orange;">**Seleccionar y total:**</mark> en este es algo sencillo, si los datos a importar son varios, con dar clic se seleccionarán todos los datos extraídos del archivo ![](../.gitbook/assets/excel-24.svg) y a la vez se mostrará los datos seleccionados y el total que extrajo del archivo.
3. <mark style="color:green;">**Tabla de datos:**</mark> solo se muestra todos los datos extraídos del archivo, mostrando su matrícula, nombre y las horas que se impartirá por semana.
4. <mark style="color:purple;">**Acciones:**</mark> estas son acciones a realizar, tenemos `Cancelar` que lo único que hará es cancelar la operación de importación y la de `Importar` es para subir al sistema los `n` datos seleccionados.

<figure><img src="../.gitbook/assets/Captura de pantalla 2025-10-09 151813.png" alt="" width="347"><figcaption></figcaption></figure>

{% hint style="danger" %}
Esta acción es propensa a dar algún error, ya sea por parte del sistema, error humano (datos erróneos o estructura mal) o de red. Consulta la sección [#errores](../otros/importante.md#errores "mention")para saber el funcionamiento de la notificación.
{% endhint %}

#### Nueva materia

Aquí es lo importante para poder crear una única materia, para ello se tiene los siguientes datos.

1. <mark style="color:green;">**Nombre de la materia:**</mark> la cual debe seguir unos requisitos para cumplir, la cual esta en tener al menos `5` caracteres y máximo `70`. Por lo que si sobre pasa el sistema no lo no permitirá, ya que no se seguirá escribiendo.
2. <mark style="color:red;">**Matrícula:**</mark> La matrícula de igual manera es importante seguir lo que pide, en este caso un mínimo de `3` caracteres y máximo `8` para continuar.
3. <mark style="color:purple;">**Horas por semana:**</mark> este es más sencillo, solo es aumentar o disminuir y el mínimo de horas es de `1` y el máximo es `10`.

{% hint style="info" %}
Si no se cumple con los requisitos no se podrá registrar la materia en el sistema.
{% endhint %}

<figure><img src="../.gitbook/assets/Captura de pantalla 2025-10-09 160150.png" alt="" width="338"><figcaption></figcaption></figure>

{% hint style="danger" %}
Esta acción es propensa a dar algún error, ya sea por parte del sistema, error humano (datos erróneos o estructura mal) o de red. Consulta la sección [#errores](../otros/importante.md#errores "mention")para saber el funcionamiento de la notificación.
{% endhint %}

Una vez se haya creado la materia se estaría viendo de esta manera, en la cual se muestran dos nuevas acciones que se podrá realizar.

<figure><img src="../.gitbook/assets/Captura de pantalla 2025-10-09 161933.png" alt="" width="232"><figcaption></figcaption></figure>

#### Editar

A la hora de editar, se deberá seguir de igual manera la misma lógica que en [#nueva-materia](materias.md#nueva-materia "mention")sobre los datos que se ingresa. En automático se rellenan los datos de la materia que se esta realizando la acción de edición.

<figure><img src="../.gitbook/assets/Captura de pantalla 2025-10-09 161903.png" alt="" width="336"><figcaption></figcaption></figure>

#### Eliminar

Para esta acción hay que tener algo de cuidado, si bien se muestra una alerta para confirmar la acción, hay que leer y tener en cuenta que esta acción no se puede revertir y eliminará completamente la información de la base de datos.

<figure><img src="../.gitbook/assets/Captura de pantalla 2025-10-09 162306.png" alt="" width="241"><figcaption></figcaption></figure>
