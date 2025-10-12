---
icon: triangle-exclamation
---

# Importante

## Errores

Aunque el sistema está terminado, no es perfecto. En ocasiones pueden presentarse errores, algunos causados por la red o por factores humanos.\
A continuación, se describen los tipos de errores más comunes y la manera de afrontarlos:

1. **Error de red:** este es un error <mark style="color:yellow;">`un poco más común`</mark>, pero no afecta el funcionamiento general. Sucede cuando el sistema no logra comunicarse con el servidor encargado de enlazar con la base de datos.
2. **Error de conexión:** este error es <mark style="color:orange;">`algo común`</mark> y también ajeno al sistema. Generalmente se debe a problemas de conexión a internet, lo que impide interactuar correctamente con el sistema.
3. **Ha ocurrido un error / error desconocido / otro:** estos son errores <mark style="color:yellow;">`poco comunes`</mark>. Se presentan cuando una acción no puede completarse correctamente por alguna razón interna.
4. **Errores según la acción realizada:** estos errores aparecen porque el sistema está diseñado para prevenir ciertas acciones y notificar mediante una alerta.

Los `errores` y `advertencias` se muestran mediante notificaciones en la parte superior derecha de la pantalla.

<figure><img src="https://427283098-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2Fc3Xztvbl6hZF1pSc3D5c%2Fuploads%2FLnbhwB22uEMAhcKEfZKL%2FCaptura%20de%20pantalla%202025-10-10%20174233.png?alt=media&#x26;token=a60087e8-95d9-4d70-a3da-17f865f5086e" alt=""><figcaption></figcaption></figure>

Una de las características de este tipo de notificaciones es la posibilidad de interactuar con ellas para leer el mensaje de error con más detalle.

{% hint style="info" %}
Esta acción también aplica para las notificaciones de tipo `Advertencia`.\
No aplica para <mark style="color:blue;">`Aviso`</mark> ni para `Éxito`.
{% endhint %}

<figure><img src="https://427283098-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2Fc3Xztvbl6hZF1pSc3D5c%2Fuploads%2F0ISSlUks4DOWgA5Bav6U%2FCaptura%20de%20pantalla%202025-10-10%20174411.png?alt=media&#x26;token=ad8e871b-1e2f-4ea0-8130-f2a1b59ed561" alt=""><figcaption></figcaption></figure>

Para ver el mensaje completo, se debe dar `clic` sobre la notificación.\
Al hacerlo, esta se ampliará y permanecerá visible el tiempo necesario.

***

## Formato para crear una plantilla

Es importante seguir la nomenclatura establecida y agregar los valores indicados para que el sistema reemplace automáticamente la información correspondiente en el formato final.

### <mark style="color:$success;">Plantilla de horarios</mark>

Para elaborar una nueva plantilla que permita descargar los horarios con el formato adecuado, se debe crear un nuevo archivo ![](../.gitbook/assets/word-24.svg) considerando lo siguiente:

{% code title="formato.docx" overflow="wrap" lineNumbers="true" %}
```
<-- PÁGINA 1 -->
## Cabecera del documento
## Es importante que antes de todo el contenido se agregue lo siguiente:
{#grupos} # Inicio de la iteración

Variables de la tabla 1.

Plantel: {plantel} ...etc
[formato de la tabla] # Se agrega la tabla con el formato esperado

-- SALTO DE PÁGINA --

<-- PÁGINA 2 -->
## Cabecera del documento

{/grupos} # Fin de la iteración
```
{% endcode %}

#### **Tabla 1**

<table><thead><tr><th width="180" align="center">Placeholder</th><th align="center">Descripción</th><th align="center">Ejemplo</th></tr></thead><tbody><tr><td align="center"><kbd>{plantel}</kbd></td><td align="center">Obtiene el nombre del plantel.</td><td align="center"><code>COBAEV 16</code></td></tr><tr><td align="center"><kbd>{carpetaNombre}</kbd></td><td align="center">Obtiene el semestre al cual corresponde el horario.</td><td align="center"><code>2025 AGOSTO-ENERO</code></td></tr><tr><td align="center"><kbd>{grupoNombre}</kbd></td><td align="center">Obtiene el grupo al que pertenece el horario descargado.</td><td align="center"><code>201 Matutino</code></td></tr><tr><td align="center"><kbd>{elaboro}</kbd></td><td align="center">Se reemplaza por el nombre configurado en el sistema.</td><td align="center"><code>LIC. TOMÁS TAXILAGA ACUA</code></td></tr><tr><td align="center"><kbd>{cargoElaboro}</kbd></td><td align="center">Se reemplaza por el cargo configurado en el sistema.</td><td align="center"><code>SUBDIRECTOR ACADÉMICO</code></td></tr><tr><td align="center"><kbd>{vobo}</kbd></td><td align="center">Se reemplaza por el nombre configurado en el sistema para el visto bueno.</td><td align="center"><code>LIC. MARÍA TERESA DE JESÚS MORENO GÓMEZ</code></td></tr><tr><td align="center"><kbd>{cargoVobo}</kbd></td><td align="center">Se reemplaza por el cargo configurado en el sistema para el visto bueno.</td><td align="center"><code>DIRECTORA</code></td></tr></tbody></table>

{% hint style="info" %}
Estos datos pueden colocarse dentro del documento en cualquier orden y su uso es `opcional`.
{% endhint %}

#### **Tabla 2**

La siguiente tabla muestra las variables necesarias para la generación de horarios, ya que se encargan de reemplazar la información de cada grupo.

|                                                                                     Placeholder                                                                                     | Descripción                                                        |
| :---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: | ------------------------------------------------------------------ |
|                                                 <kbd><mark style="color:red;">{#horarios}{/horarios}<mark style="color:red;"></kbd>                                                 | Indica al sistema el inicio y fin de la iteración de los horarios. |
| <kbd><mark style="color:green;">{#esReceso}<mark style="color:green;"></kbd><kbd>{celdaCombinada}</kbd><kbd><mark style="color:green;">{/esReceso}<mark style="color:green;"></kbd> | Coloca la palabra “RECESO” en la tabla.                            |
|                                                      <kbd><mark style="color:purple;">{hora}<mark style="color:purple;"></kbd>                                                      | Muestra las horas correspondientes según el turno.                 |
|                                                <kbd><mark style="color:blue;">{^esReceso}{/esReceso}<mark style="color:blue;"></kbd>                                                | Indica la hora del receso en ambos turnos.                         |
|                                    <kbd><mark style="color:orange;">{lunes}{martes}{miercoles}{jueves}{viernes}<mark style="color:orange;"></kbd>                                   | Coloca los horarios en los días correspondientes.                  |

El diseño de la tabla debe mantener el formato mostrado a continuación, donde se establecen los días de la semana y las celdas donde se reemplazará la información de los grupos.

<figure><img src="../.gitbook/assets/Captura de pantalla 2025-10-11 151816.png" alt=""><figcaption></figcaption></figure>

{% hint style="danger" %}
Estos datos son de carácter obligatorio.
{% endhint %}

#### **Tabla 3**

Esta tabla muestra la información relacionada con las materias y los docentes que las imparten en cada grupo.

<table><thead><tr><th width="305" align="center">Placeholder</th><th>Descripción</th></tr></thead><tbody><tr><td align="center"><kbd><mark style="color:blue;">{#asignaturas}{/asignaturas}</mark></kbd></td><td>Define el inicio de la iteración de las materias asignadas al grupo.</td></tr><tr><td align="center"><kbd><mark style="color:green;">{horas}</mark></kbd></td><td>Muestra las horas semanales asignadas a la materia.</td></tr><tr><td align="center"><kbd><mark style="color:red;">{catedratico}</mark></kbd></td><td>Muestra el nombre del docente asignado a la materia.</td></tr></tbody></table>

<figure><img src="../.gitbook/assets/Captura de pantalla 2025-10-11 153140.png" alt=""><figcaption></figcaption></figure>

{% hint style="success" %}
Es importante organizar estos datos de forma que todo el contenido se mantenga dentro del mismo documento.\
Si es necesario, se recomienda reducir el tamaño de la fuente a un mínimo de `8` puntos para garantizar la legibilidad.
{% endhint %}

El archivo final debe contener dos hojas.\
En la segunda hoja solo debe incluirse la variable <mark style="color:red;">`{/grupos}`</mark>.\
En la siguiente imagen se muestra un ejemplo del formato final.

<figure><img src="../.gitbook/assets/Captura de pantalla 2025-10-11 154400.png" alt=""><figcaption></figcaption></figure>

#### **Descarga la plantilla elaborada**

{% file src="../.gitbook/assets/PLANTILLA_HORARIOS_COBAEV-16.docx" %}

***

### <mark style="color:blue;">Plantilla de docentes</mark>

Para crear una nueva plantilla de docentes, se requiere la siguiente información para garantizar el correcto llenado de los datos provenientes del sistema.

En un nuevo archivo ![](../.gitbook/assets/word-24.svg) se debe considerar lo siguiente:

{% code title="formato.docx" overflow="wrap" lineNumbers="true" %}
```
<-- PÁGINA 1 -->
## Cabecera del documento

{#docentes} # Inicio de la iteración
## Datos importantes de la materia
DOCENTE: {catedratico}
ASIGNATURA (S): {asignaturasCatedratico}
GRUPO (S): {gruposMaterias}
TOTAL HORAS: {totalHoras}
SEMESTRE: {semestre}

[TABLA]

[FIRMAS]

-- SALTO DE PÁGINA --

<-- PÁGINA 2 -->
## Cabecera del documento

{/docentes} # Fin de la iteración
```
{% endcode %}

**Tabla 1**

Las siguientes variables son necesarias para mostrar información detallada sobre el horario final de cada docente.

<table><thead><tr><th width="267" align="center">Placeholder</th><th align="center">Descripción</th></tr></thead><tbody><tr><td align="center"><kbd>{plantel}</kbd></td><td align="center">Muestra el nombre del plantel establecido en la configuración.</td></tr><tr><td align="center"><kbd>{asignaturasCatedratico}</kbd></td><td align="center">Muestra las asignaturas que imparte el docente durante el semestre.</td></tr><tr><td align="center"><kbd>{gruposMaterias}</kbd></td><td align="center">Muestra los grupos en los que el docente imparte clases.</td></tr><tr><td align="center"><kbd>{totalHoras}</kbd></td><td align="center">Muestra el total de horas semanales asignadas al docente.</td></tr><tr><td align="center"><kbd>{semestre}</kbd></td><td align="center">Muestra el semestre en curso.</td></tr><tr><td align="center"><kbd>{elaboro}</kbd></td><td align="center">Indica la persona encargada de la elaboración de los horarios.</td></tr><tr><td align="center"><kbd>{cargoElaboro}</kbd></td><td align="center">Indica el cargo de quien elaboró los horarios.</td></tr></tbody></table>

<figure><img src="../.gitbook/assets/Captura de pantalla 2025-10-11 160749.png" alt=""><figcaption></figcaption></figure>

#### **Tabla 2**

Esta tabla debe contar con un tamaño adecuado, ya que incluye los turnos matutino y vespertino.\
Un tamaño incorrecto puede ocasionar que el horario del docente se extienda a dos páginas debido a la cantidad de información.

<table><thead><tr><th width="374" align="center">Placeholder</th><th align="center">Descripción</th></tr></thead><tbody><tr><td align="center"><kbd><mark style="color:red;">{#horarios}{/horarios}</mark></kbd></td><td align="center">Define el inicio y fin de la iteración de los horarios.</td></tr><tr><td align="center"><kbd><mark style="color:blue;">{#esReceso}</mark>{celdaCombinada}<mark style="color:blue;">{/esReceso}</mark></kbd></td><td align="center">Coloca la palabra “RECESO” en la celda correspondiente.</td></tr><tr><td align="center"><kbd><mark style="color:green;">{hora}</mark></kbd></td><td align="center">Muestra las horas establecidas según el turno.</td></tr><tr><td align="center"><kbd><mark style="color:purple;">{^esReceso}{/esReceso}</mark></kbd></td><td align="center">Indica la hora del receso en ambos turnos.</td></tr><tr><td align="center"><kbd><mark style="color:orange;">{lunes}{martes}{miercoles}{jueves}{viernes}</mark></kbd></td><td align="center">Coloca los horarios en los días correspondientes.</td></tr></tbody></table>

<figure><img src="../.gitbook/assets/Captura de pantalla 2025-10-11 161030.png" alt=""><figcaption></figcaption></figure>

{% hint style="danger" %}
Estos datos son de carácter obligatorio.
{% endhint %}

El archivo debe contener dos hojas en total.\
En la segunda hoja solo debe incluirse la variable <mark style="color:red;">`{/docentes}`</mark>.\
En la siguiente imagen se muestra un ejemplo del formato final.

<figure><img src="../.gitbook/assets/Captura de pantalla 2025-10-11 161648.png" alt=""><figcaption></figcaption></figure>

#### **Descarga la plantilla elaborada**

{% file src="../.gitbook/assets/PLANTILLA_DOCENTES.docx" %}
