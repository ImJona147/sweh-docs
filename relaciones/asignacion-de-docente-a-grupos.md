---
icon: users-rectangle
---

# Asignación de docente a grupos

## Primeros pasos

Este tipo de asociación es fundamental para el sistema, ya que permite indicar con precisión qué docente impartirá clases en determinados grupos. Esto resulta esencial en las materias que son impartidas por varios docentes, pues el sistema necesita identificar cuál de ellos está asignado a cada grupo.

<figure><img src="../.gitbook/assets/Captura de pantalla 2025-10-12 133755.png" alt=""><figcaption></figcaption></figure>

{% include "../.gitbook/includes/relations.md" %}

## Funciones principales

1. <mark style="color:orange;">**Barra de búsqueda:**</mark> permite buscar las relaciones registradas en todo el sistema.
2. <mark style="color:green;">**Seleccionar semestre:**</mark> muestra las materias que cuentan con más de un docente, permitiendo realizar las asociaciones correspondientes.
3. <mark style="color:blue;">**Nueva relación:**</mark> con base en el semestre seleccionado, el sistema identifica y muestra las materias que tienen más de un docente.

<figure><img src="../.gitbook/assets/imagen (3).png" alt=""><figcaption></figcaption></figure>

### <mark style="color:green;">Asignación por semestre</mark>

Primero debe seleccionarse el semestre en el que se buscarán las materias con más de un docente, de modo que se muestren todas las materias correspondientes a ese periodo.

<figure><img src="../.gitbook/assets/Captura de pantalla 2025-10-12 134332.png" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
Se recomienda seleccionar el **último semestre creado**, ya que es el que estará activo en ese momento.
{% endhint %}

### <mark style="color:blue;">Nueva relación</mark>

Antes de comenzar con las asociaciones, deben haberse realizado previamente los siguientes pasos:

* [#nuevo-semestre](../recursos-academica/semestres.md#nuevo-semestre "mention")
* [#nueva-relacion-entre-materia-y-grupo](materias-con-grupos.md#nueva-relacion-entre-materia-y-grupo "mention")
* [#nueva-relacion-entre-materia-y-docente](docentes-con-materias.md#nueva-relacion-entre-materia-y-docente "mention")

Si el semestre seleccionado **no cuenta con materias que tengan más de un docente**, se mostrará el siguiente mensaje.\
Esto **no afecta el funcionamiento del sistema**, incluso si no se agrega dicha información.\
Este proceso tiene un propósito **preventivo**, ayudando a reducir posibles errores del sistema.

<figure><img src="../.gitbook/assets/Captura de pantalla 2025-10-12 142838.png" alt=""><figcaption></figcaption></figure>

Si el semestre cuenta con **materias impartidas por más de un docente**, se mostrará un modal como el siguiente, donde se visualizan inicialmente las materias que cumplen con esta condición.

<figure><img src="../.gitbook/assets/imagen1 (1).png" alt=""><figcaption></figcaption></figure>

Una vez seleccionada la materia, el sistema mostrará **todos los docentes** que la imparten.\
Esta parte resulta más interactiva, ya que permite **seleccionar un docente y asociarlo con los distintos grupos disponibles**.

<figure><img src="../.gitbook/assets/Captura de pantalla 2025-10-12 143824.png" alt="" width="563"><figcaption></figcaption></figure>

Al seleccionar un docente, se desplegarán **los grupos con los que está relacionada la materia**.\
Por este motivo, es importante [docentes-con-materias.md](docentes-con-materias.md "mention") y [materias-con-grupos.md](materias-con-grupos.md "mention"), ya que define las opciones disponibles para la asignación.

<figure><img src="../.gitbook/assets/Captura de pantalla 2025-10-12 144145.png" alt="" width="563"><figcaption></figcaption></figure>

Una ventaja de esta interfaz es que **permite visualizar en todo momento los docentes que ya están asignados a ciertos grupos**, lo cual se representa mediante **diferentes colores**.\
Después de seleccionar los grupos donde el docente impartirá clases, se debe presionar el botón **Crear asignación** para guardar los cambios.

{% hint style="info" %}
Este proceso debe repetirse para **cada uno de los docentes** que aparezcan en la lista.
{% endhint %}

<figure><img src="../.gitbook/assets/Captura de pantalla 2025-10-12 144425.png" alt="" width="560"><figcaption></figcaption></figure>

{% include "../.gitbook/includes/actionerror.md" %}

## Información obtenida

Al crear las asociaciones se estará mostrando de la siguiente manera, en donde solo se podrá eliminar las asociaciones, no se podrá modificar, si hay una equivocación, se deberá borrar la relación y repetir los paso nuevamente.

<figure><img src="../.gitbook/assets/Captura de pantalla 2025-10-12 144802.png" alt=""><figcaption></figcaption></figure>

### <mark style="color:red;">Eliminar</mark>

Esta acción es irreversible y eliminará completamente la información de la base de datos. Lee cuidadosamente la confirmación antes de proceder.

<figure><img src="../.gitbook/assets/Captura de pantalla 2025-10-12 145629.png" alt="" width="238"><figcaption></figcaption></figure>
