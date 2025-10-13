---
icon: person-chalkboard
---

# Docentes

## Primeros pasos

Página principal donde se muestran todos los `docentes` registradas en el sistema. Si no hay registros, aparecerá un mensaje indicándolo.

<figure><img src="../.gitbook/assets/Captura de pantalla 2025-10-09 184325.png" alt=""><figcaption></figcaption></figure>

## Funciones principales

1. <mark style="color:orange;">**Barra de búsqueda:**</mark> permite buscar un docente por su nombre.
2. <mark style="color:green;">**Vistas:**</mark> cambia entre vista de cuadrícula o lista.
3. <mark style="color:purple;">**Acciones principales:**</mark> botones para registrar y exportar docentes.

<figure><img src="../.gitbook/assets/Captura de pantalla 2025-10-09 184506.png" alt=""><figcaption></figcaption></figure>

### <mark style="color:$success;">Exportar</mark>

Descarga **TODOS** los docentes registradas en el sistema en los siguientes formatos:

<div align="center"><img src="../.gitbook/assets/pdf-24.svg" alt=""> <img src="../.gitbook/assets/word-24.svg" alt=""> <img src="../.gitbook/assets/excel-24.svg" alt=""></div>

{% hint style="info" %}
**Nota:** consultar los formatos disponibles en la sección[#formatos-de-descarga](../otros/importante.md#formatos-de-descarga "mention")
{% endhint %}

### <mark style="color:blue;">Importar</mark>

Para agilizar la carga de docentes, especialmente en el primer uso, se puede importar un archivo ![](../.gitbook/assets/excel-24.svg) con el siguiente formato:

{% hint style="success" %}
Copiar y pegar el siguiente código en un archivo ![](../.gitbook/assets/excel-24.svg)
{% endhint %}

{% code title="formato.xlsx" overflow="wrap" lineNumbers="true" fullWidth="true" %}
```csv
nombre
```
{% endcode %}

{% hint style="warning" %}
Es importante seguir esta plantilla para que el sistema detecte correctamente todos los docentes.
{% endhint %}

{% hint style="danger" %}
Debes seguir los requisitos del nombre. Ir a [#nuevo-docente](docentes.md#nuevo-docente "mention") para obtener más información.
{% endhint %}

<figure><img src="../.gitbook/assets/Captura de pantalla 2025-10-09 185030.png" alt=""><figcaption></figcaption></figure>

Cuando el archivo esté listo, usa el botón <mark style="color:green;">**Importar**</mark> para abrir el selector de archivos. Una vez seleccionado, aparecerá el siguiente diálogo:

1. <mark style="color:red;">**Barra de búsqueda:**</mark> filtra docentes por nombre cuando el archivo contiene muchos registros.
2. <mark style="color:orange;">**Seleccionar y total:**</mark> selecciona todos los datos extraídos y muestra el total.
3. <mark style="color:green;">**Tabla de datos:**</mark> vista previa de los datos extraídos.
4. <mark style="color:purple;">**Acciones:**</mark> `Cancelar` para abortar la importación o `Importar` para subir los datos seleccionados.

<figure><img src="../.gitbook/assets/Captura de pantalla 2025-10-09 185144.png" alt=""><figcaption></figcaption></figure>

{% include "../.gitbook/includes/actionerror.md" %}

### <mark style="color:$primary;">Nuevo docente</mark>

Para crear un docente individual, completa los siguientes campos:

1. <mark style="color:green;">**Nombre del docente:**</mark> entre 10 y 50 caracteres. El sistema no permitirá exceder el límite.

<figure><img src="../.gitbook/assets/Captura de pantalla 2025-10-09 185423.png" alt="" width="377"><figcaption></figcaption></figure>

{% include "../.gitbook/includes/actionerror.md" %}

## Información obtenida

Una vez creado el docente, aparecerán nuevas acciones disponibles:

1. <mark style="color:green;">**Horario:**</mark> se muestra si el docente cuenta con horario establecido para el último semestre registrado. Para más información en [planificacion-docente.md](../gestion-de-horarios/planificacion-docente.md "mention").
2. <mark style="color:red;">**Materias:**</mark> esto nos indica si ya se han asignado materias al docente en el último semestre registrado. Para más información en [docentes-con-materias.md](../relaciones/docentes-con-materias.md "mention").

<figure><img src="../.gitbook/assets/Captura de pantalla 2025-10-09 185837.png" alt="" width="227"><figcaption></figcaption></figure>

### <mark style="color:blue;">Editar</mark>

Al editar a un docente, se aplican las mismas validaciones que al crear. Los campos se rellenan automáticamente con los datos actuales.

<figure><img src="../.gitbook/assets/Captura de pantalla 2025-10-09 190652.png" alt="" width="381"><figcaption></figcaption></figure>

### <mark style="color:red;">Eliminar</mark>

Esta acción es irreversible y eliminará completamente la información de la base de datos. Lee cuidadosamente la confirmación antes de proceder.

<figure><img src="../.gitbook/assets/Captura de pantalla 2025-10-09 190746.png" alt="" width="239"><figcaption></figcaption></figure>
