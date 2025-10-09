---
icon: books
---

# Materias

Página principal donde se muestran todas las materias registradas en el sistema. Si no hay registros, aparecerá un mensaje indicándolo.

<figure><img src="../.gitbook/assets/Captura de pantalla 2025-10-09 092836.png" alt=""><figcaption></figcaption></figure>

Esta vista incluye herramientas para gestionar las materias:

1. **Agregar materia:** permite añadir nuevas materias al sistema.

{% hint style="info" %}
Este botón funciona igual en el diseño final.
{% endhint %}

<figure><img src="../.gitbook/assets/Captura de pantalla 2025-10-09 142302.png" alt="" width="495"><figcaption></figcaption></figure>

### Funciones principales

1. <mark style="color:orange;">**Barra de búsqueda:**</mark> permite buscar materias por nombre o matrícula.
2. <mark style="color:green;">**Vistas:**</mark> cambia entre vista de cuadrícula o lista.
3. <mark style="color:purple;">**Acciones principales:**</mark> botones para registrar y exportar materias.

<figure><img src="../.gitbook/assets/Captura de pantalla 2025-10-09 143609.png" alt=""><figcaption></figcaption></figure>

### Acciones principales

#### Exportar

Exporta <mark style="color:$success;">**TODAS**</mark> las materias registradas en el sistema en los siguientes formatos:

<p align="center"><img src="../.gitbook/assets/pdf-24.svg" alt=""><img src="../.gitbook/assets/word-24.svg" alt=""><img src="../.gitbook/assets/excel-24.svg" alt=""></p>

Los archivos se descargan en formato de tabla con plantillas sencillas y predeterminadas.

#### Importar

Para agilizar la carga de materias, especialmente en el primer uso, puedes importar un archivo ![](../.gitbook/assets/excel-24.svg) con el siguiente formato:

<pre class="language-csv" data-title="formato.xlsx" data-overflow="wrap" data-line-numbers data-full-width="true"><code class="lang-csv"><strong>matricula	materia	horas
</strong></code></pre>

Es importante seguir esta plantilla para que el sistema detecte correctamente todas las materias.

{% hint style="danger" %}
Es importante seguir los requisitos de cada valor. Ir a [#nueva-materia](materias.md#nueva-materia "mention")
{% endhint %}

<figure><img src="../.gitbook/assets/Captura de pantalla 2025-10-09 150849.png" alt=""><figcaption></figcaption></figure>

Cuando tengas el archivo listo, usa el botón <mark style="color:green;">**Importar**</mark> para abrir el selector de archivos. Una vez seleccionado, aparecerá el siguiente diálogo:

1. <mark style="color:red;">**Barra de búsqueda:**</mark> filtra materias por nombre o matrícula cuando el archivo contiene muchos registros.
2. <mark style="color:orange;">**Seleccionar y total:**</mark> selecciona todos los datos extraídos y muestra el total.
3. <mark style="color:green;">**Tabla de datos:**</mark> vista previa de los datos extraídos (matrícula, nombre y horas semanales).
4. <mark style="color:purple;">**Acciones:**</mark> `Cancelar` para abortar la importación o `Importar` para subir los datos seleccionados.

<figure><img src="../.gitbook/assets/Captura de pantalla 2025-10-09 151813.png" alt="" width="347"><figcaption></figcaption></figure>

{% hint style="danger" %}
Esta acción puede fallar por problemas del sistema, datos erróneos o conexión de red. Consulta [#errores](../otros/importante.md#errores "mention") para información sobre notificaciones.
{% endhint %}

#### Nueva materia

Para crear una materia individual, completa los siguientes campos:

1. <mark style="color:green;">**Nombre de la materia:**</mark> entre 5 y 70 caracteres. El sistema no permitirá exceder el límite.
2. <mark style="color:red;">**Matrícula:**</mark> entre 3 y 8 caracteres.
3. <mark style="color:purple;">**Horas por semana:**</mark> entre 1 y 10 horas.

{% hint style="info" %}
Si no se cumplen los requisitos, no se podrá registrar la materia.
{% endhint %}

<figure><img src="../.gitbook/assets/Captura de pantalla 2025-10-09 160150.png" alt="" width="338"><figcaption></figcaption></figure>

{% hint style="danger" %}
Esta acción puede fallar por problemas del sistema, datos erróneos o conexión de red. Consulta [#errores](../otros/importante.md#errores "mention") para información sobre notificaciones.
{% endhint %}

Una vez creada la materia, aparecerán nuevas acciones disponibles:

<figure><img src="../.gitbook/assets/Captura de pantalla 2025-10-09 161933.png" alt="" width="232"><figcaption></figcaption></figure>

#### Editar

Al editar una materia, se aplican las mismas validaciones que al crear. Los campos se rellenan automáticamente con los datos actuales.

<figure><img src="../.gitbook/assets/Captura de pantalla 2025-10-09 161903.png" alt="" width="336"><figcaption></figcaption></figure>

#### Eliminar

Esta acción es irreversible y eliminará completamente la información de la base de datos. Lee cuidadosamente la confirmación antes de proceder.

<figure><img src="../.gitbook/assets/Captura de pantalla 2025-10-09 162306.png" alt="" width="241"><figcaption></figcaption></figure>
