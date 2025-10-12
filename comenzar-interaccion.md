---
icon: right-to-bracket
layout:
  width: default
  title:
    visible: true
  description:
    visible: true
  tableOfContents:
    visible: true
  outline:
    visible: true
  pagination:
    visible: true
  metadata:
    visible: true
---

# Primeros pasos

## Inicio de sesión

Para acceder al sistema, es necesario contar con las credenciales correctas. Estas garantizan que el usuario pueda ingresar y continuar con las operaciones dentro del sistema.

1. <mark style="color:blue;">**Usuario:**</mark> ingresa el nombre de usuario.
2. <mark style="color:green;">**Contraseña:**</mark> ingresa la contraseña.
3. <mark style="color:orange;">**Ingresar:**</mark> botón para validar las credenciales e ingresar al sistema.

<figure><img src=".gitbook/assets/pm_login.avif" alt="" width="375"><figcaption></figcaption></figure>

Si las credenciales son correctas, el sistema redirigirá automáticamente al [#dashboard](comenzar-interaccion.md#dashboard "mention").\
En caso contrario, se mostrarán algunos errores.

{% include ".gitbook/includes/actionerror.md" %}

***

## Dashboard

El **panel de control (dashboard)** muestra información general sobre el estado del sistema y confirma si todo está correctamente configurado cuando se habilita un [#nuevo-semestre](recursos-academica/semestres.md#nuevo-semestre "mention").

<figure><img src=".gitbook/assets/pm_dashboard.avif" alt=""><figcaption></figcaption></figure>

#### Semestre actual

En esta sección se muestra el **último semestre creado** en el sistema, lo que permite verificar en todo momento si los datos que se visualizan corresponden al periodo activo.

También se muestra el **estado del semestre**, el cual indica si el proceso de elaboración de horarios ha concluido o sigue en curso.

{% hint style="warning" %}
Este apartado solo aparece cuando se ha creado un nuevo semestre.
{% endhint %}

<figure><img src=".gitbook/assets/pm_dashboard_sm.avif" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
Para más detalles sobre los semestres y sus funcionalidades, consulta la sección [semestres.md](recursos-academica/semestres.md "mention").
{% endhint %}

### Configuración inicial

Estas configuraciones se realizan una sola vez, ya que contienen información base que no cambia con frecuencia.

1. **Agregar materias**: muestra el total de materias registradas.
2. **Agregar docentes**: muestra el total de docentes registrados.
3. **Agregar grupos**: muestra el total de grupos registrados.
4. **Crear semestre**: muestra el total de semestres creados.
5. **Configuración general**: indica si se ha establecido correctamente la información académica general.

Además, se muestra una **barra de progreso** que refleja el avance a medida que se completa cada paso.

{% hint style="info" %}
La siguiente imagen muestra una configuración inicial completamente vacía.
{% endhint %}

<figure><img src=".gitbook/assets/pm_dashboard_ci.avif" alt=""><figcaption></figcaption></figure>

A continuación, se muestra la configuración inicial completa, con todos los pasos correctamente realizados.

<figure><img src=".gitbook/assets/pm_dashboard_ci_finish.avif" alt=""><figcaption></figcaption></figure>

Una vez completada la configuración sin errores, esta será la base de datos que el sistema utilizará de manera global.

### Configuración del semestre

Si todos los pasos anteriores se realizaron correctamente, esta sección no debería mostrarse. Sin embargo, si aún no existe un [semestres.md](recursos-academica/semestres.md "mention"), es necesario crearlo.

<figure><img src=".gitbook/assets/pm_dashboard_empty.avif" alt=""><figcaption></figcaption></figure>

Los siguientes pasos son <mark style="color:red;">**IMPORTANTES**</mark> y deben realizarse cada vez que se crea un nuevo semestre académico, ya que contienen información fundamental para la elaboración de los horarios.

6. **Asignar materias a los grupos**: Permite definir qué materias se imparten en cada grupo, optimizando la creación de horarios al mostrar solo las materias relevantes.
7. **Asignar docentes a materias**: Asocia las materias a los docentes responsables, lo cual es esencial para reflejar correctamente los horarios finales de cada docente.
8. **Asignar docentes a grupos**: Este paso permite vincular docentes con los grupos asignados. Es posible que una misma materia tenga `uno o más` docentes.

{% hint style="warning" %}
Recuerda: esta configuración debe realizarse **cada vez que se crea un nuevo semestre escolar**.
{% endhint %}

<figure><img src=".gitbook/assets/pm_dashboard_cs_null.avif" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
Cada paso muestra información relevante, incluyendo la cantidad de datos esperados y el porcentaje de avance correspondiente.
{% endhint %}

<figure><img src=".gitbook/assets/pm_dashboard_cs_finish.avif" alt=""><figcaption></figcaption></figure>

{% hint style="success" %}
Una vez completados todos los pasos y alcanzado el porcentaje requerido, el sistema mostrará el estado como **completo y listo para trabajar**.
{% endhint %}
