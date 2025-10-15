---
icon: calendar-lines-pen
---

# Elaboración de horarios

## Primeros pasos

Hasta este punto para la elaboración de horarios se debió haber realizado los puntos que se mencionan en [#configuracion-del-semestre](../comenzar-interaccion.md#configuracion-del-semestre "mention"). Ya teniendo esa información disponible, nos dirigimos en el apartado de **Semestres y Horarios** en donde se estarán mostrando todos los semestres creados en el sistema. Se puede interactuar con los componentes y se pueda dar clic, lo que hará es dirigirnos a otra vista.

<figure><img src="../.gitbook/assets/Captura de pantalla 2025-10-14 144615.png" alt="" width="231"><figcaption></figcaption></figure>

## Vista dentro del semestre

Dentro de esta vista podremos encontrar lo siguiente:

1. **Barra de búsqueda de grupos:** permite buscar cierto grupo dentro de todos los grupos registrados en el sistema.
2. **Descargar horarios:** permite la descarga de múltiples horarios dentro de este semestre.
3. **Filtrar rango:** permite solo mostrar un cierto rango de los grupos que hay en el sistema.
4. **Grupos:** muestra los grupos correspondientes para el semestre.

<figure><img src="../.gitbook/assets/Captura de pantalla 2025-10-14 144851.png" alt=""><figcaption></figcaption></figure>

### Descargar horarios

El botón de descargar horario nos permite descargar los horarios de grupos específicos o de todos los grupos asignados al semestre.

1. Barra de búsqueda: permite buscar un grupo en especifico para poder seleccionarlo
2. Seleccionar todos: permite al selección de todos los grupos disponibles y asignados al semestre.
3. Grupos: muestra la lista de los grupos, los cuales se podrán seleccionar para su descarga.

<figure><img src="../.gitbook/assets/Captura de pantalla 2025-10-14 154209.png" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
**Nota:** consultar los formatos disponibles en la sección [#formatos-de-descarga](../otros/importante.md#formatos-de-descarga "mention").
{% endhint %}

### Grupos

En los grupos se nos muestra información que podría llegar a ser necesaria e importante para que así no se tenga que estar adentrando dentro de cada grupo para ver información. Para entrar al proceso de elaboración de horarios, debemos dar clic sobre uno de los grupos que se muestra y nos enviará a otra vista.

<figure><img src="../.gitbook/assets/imagen (4).png" alt="" width="563"><figcaption></figcaption></figure>

## Elaboración de horario

Ya estando en esta vista de elaboración de horarios nos encontramos con varias características que se estará explicando con más detalle.



<figure><img src="../.gitbook/assets/imagen (1).png" alt=""><figcaption></figcaption></figure>

Se muestran algunas de las acciones principales o lo que se puede hacer dentro del área de trabajo.

<div data-full-width="true"><figure><img src="../.gitbook/assets/imagen (2).png" alt=""><figcaption></figcaption></figure></div>

### Descargar



### Previsualizar



### Panel de materias

El panel de materia es la parte fundamental para poder trabajar durante la elaboración de horarios, por eso, se explica sus funcionalidades:

1. **Barra de búsqueda:** permite buscar una materia en especifico
2. **Actualizar información:** permite actualizar la información, útil para cuando se olvido hacer los pasos anteriores de [#configuracion-del-semestre](../comenzar-interaccion.md#configuracion-del-semestre "mention") y hay problemas de información.
3. **Materias disponibles:** muestra las materias disponibles y asociadas al grupo, la información que nos brinda es las horas por semana de la materia y su matrícula.
4. **Materias seleccionadas:** componente que se puede arrastrar hacia el área de trabajo (tabla de horario). También nos otorga información relevante como el docente asignado, matrícula y horas por semana.

<figure><img src="../.gitbook/assets/imagen (1) (1).png" alt=""><figcaption></figcaption></figure>

#### Materias seleccionadas

En este apartado se muestran las materias seleccionadas, se colocan dentro del área de **"Arrastra materias aquí"** en donde las materias pueden ser agregadas del mismo panel o de la tabla de horarios.

<figure><img src="../.gitbook/assets/Captura de pantalla 2025-10-14 190335.png" alt=""><figcaption></figcaption></figure>

Las materias dentro de ese contenedor son **arrastrables** lo que nos permite moverlo a la tabla.

{% hint style="danger" %}
**Importante:** a este punto ya se debió haber realizado los pasos necesarios para evitar errores de la materia
{% endhint %}

<figure><img src="../.gitbook/assets/Cobaev 16 - Brave 2025-10-14 19-23-20 - Trim.gif" alt=""><figcaption></figcaption></figure>

También lo que se puede hacer es lo contrario, puede arrastrar una materia agregada a la tabla hacía el panel de materias o directamente puede borrar la materia agregada en la tabla.

### Validaciones

Las validaciones son pruebas que hace el sistema antes de colocar la materia para verificar que todo esta funcionando correctamente y que no haya ningún tipo de problema. Tenemos las siguientes validaciones.

* Docente asignado
* Límite de horas
* Horario base
* Disponibilidad docente
* Conflicto de horario
* Carga del docente

<figure><img src="../.gitbook/assets/Cobaev 16 - Brave 2025-10-14 19-58-17 - Trim.gif" alt=""><figcaption></figcaption></figure>

Esto es cuando la materia cumple con todas las validaciones y se queda colocado correctamente y puede continuar sin ningún tipo de problema.

#### Notificación de errores

Cuando una materia no cumple con las validaciones ya establecidas se hace mención sobre el tipo de error que detecto y lo muestra. Las notificaciones cuentan con ciertas funcionalidades que se explican a continuación.

<figure><img src="../.gitbook/assets/imagen.png" alt=""><figcaption></figcaption></figure>

### **DOCENTE NO ASIGNADO**

Esta validación es la principal y es primordial y consta en verificar si la materia ya tiene asignado un docente, si cuenta con un docente asignado pasa a la siguiente validación, pero de no contar con uno manda el error.

{% include "../.gitbook/includes/no-avanza.md" %}

<figure><img src="../.gitbook/assets/Captura de pantalla 2025-10-14 201826.png" alt=""><figcaption></figcaption></figure>

Las acciones a realizar para este tipo de error son:

1. **Entendido**: permite minimizar la notificación para que no moleste.
2. **Establecer docente**: redirige al apartado correspondiente para poder establecer un docente a la materia.
3. **Limpiar notificación**: limpia directamente la notificación del centro de notificaciones.

### LÍMITE DE HORAS DE LA MATERIA

El límite de horas por materia es algo importante que se debe tomar en cuenta y es la validación que verifica que realmente no se exceda el límite de las horas establecidas de la materia.

{% include "../.gitbook/includes/no-avanza.md" %}

<figure><img src="../.gitbook/assets/Captura de pantalla 2025-10-14 204232.png" alt=""><figcaption></figcaption></figure>

Las acciones a realizar para este tipo de error son:

1. **Entendido:** permite minimizar la notificación para que no moleste
2. **Limpiar notificación:** limpia directamente la notificación del centro de notificaciones.

### DOCENTE SIN PLANIFICACIÓN

Cuando un docente esta asignado a la materia pero este no se le ha asignado aun su horario de trabajo manda ese error, por que es importante y necesario que el docente cuente con su planificación para que así el sistema vaya calculando su horario final.

{% include "../.gitbook/includes/no-avanza.md" %}

<figure><img src="../.gitbook/assets/Captura de pantalla 2025-10-14 205147.png" alt=""><figcaption></figcaption></figure>

Las acciones a realizar para este tipo de error son:

1. **Entendido:** permite minimizar la notificación para que no moleste
2. **Asignar horario de trabajo**: redirige al apartado donde se podrá asignar el horario de trabajo del docente.
3. **Limpiar notificación:** limpia directamente la notificación del centro de notificaciones.

### DISPONIBILIDAD DEL DOCENTE

A la hora de estar colocando la materia en la tabla de horarios se verifica en los diferentes grupos si el docente que esta asignado a la materia que inicialmente se arrastro ya tiene ocupada la hora la que se esta arrastrando, si el docente ya tiene ocupado la misma hora y día se envía la notificación.

{% hint style="warning" %}
**Importante:** permite avanzar siempre y colocar la materia dentro de la tabla siempre y cuando usted se lo indique.
{% endhint %}

<figure><img src="../.gitbook/assets/Captura de pantalla 2025-10-14 210043.png" alt=""><figcaption></figcaption></figure>

Las acciones a realizar para este tipo de error son:

1. **Permitir:** permite avanzar con la colocación de la materia dentro de la tabla aun cuando ya esta ocupada esa hora y día.
2. **Ver disponibilidad:** redirige a la planificación docente para ver las horas disponibles del docente.
3. **Ver horario establecido:** redirige al apartado donde se va mostrando el horario del docente así ver las horas ocupadas.
4. **Limpiar notificación:** limpia directamente la notificación del centro de notificaciones.

### CONFLICTO DE HORARIOS

El conflicto de horario aparecerá en todo momento cuando se intente colocar una materia con un docente que ya tiene conflicto, esto pasa por que si se permitió seguir con la colocación de la materia dentro de la tabla aun así con problemas el sistema estará notificando para que así se tenga en cuenta esos conflictos.

{% hint style="warning" %}
**Importante:** permite avanzar siempre y colocar la materia dentro de la tabla siempre y cuando usted se lo indique.
{% endhint %}

<figure><img src="../.gitbook/assets/Captura de pantalla 2025-10-14 210857.png" alt=""><figcaption></figcaption></figure>

Las acciones a realizar para este tipo de error son:

1. **Continuar igual:** permites seguir continuando aun así con conflictos dentro del horario.
2. **Limpiar notificación:** limpia directamente la notificación del centro de notificaciones.

### SOBRE CARGA DE HORAS DEL DOCENTE

Esta validación es únicamente cuando el sistema detecta que el docente ya esta a un 85% de límite de sus horas de trabajo, y así tener un poco más en cuenta sobre la carga de horas al docente.

{% hint style="info" %}
**Nota:** esto no afecta en nada y permite seguir el flujo normal, solo es una pequeña sugerencia de tener más consideración sobre la carga horaria.
{% endhint %}

<figure><img src="../.gitbook/assets/Captura de pantalla 2025-10-14 213325.png" alt=""><figcaption></figcaption></figure>

Las acciones a realizar para este tipo de error son:

1. **Entendido:** permite minimizar la notificación para que no moleste
2. **Limpiar notificación:** limpia directamente la notificación del centro de notificaciones.
