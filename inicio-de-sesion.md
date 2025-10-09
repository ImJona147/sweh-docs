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

# Inicio de sesión

### Credenciales

Para acceder al sistema, es necesario contar con las credenciales correctas. Estas garantizan que el usuario pueda ingresar y continuar con las operaciones dentro del sistema.

1. **Usuario**
2. **Contraseña**
3. **Ingresar**

<figure><img src="https://427283098-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2Fc3Xztvbl6hZF1pSc3D5c%2Fuploads%2FVgiEHe42xtqY2W9NeWkm%2F1.png?alt=media&#x26;token=04326a8b-6a7a-4c26-881e-11e4acc0888a" alt=""><figcaption></figcaption></figure>

Si las credenciales son correctas, el sistema redirigirá automáticamente al #dashboard.\
En caso contrario, se mostrarán algunos de los siguientes errores comunes:

{% hint style="warning" %}
Los mensajes de error por notificación cuentan con funcionalidades adicionales. Consulta la sección [#errores](otros/importante.md#errores "mention") para obtener más información sobre su funcionamiento.
{% endhint %}

1. **Usuario no encontrado:** Ocurre cuando el nombre de usuario no existe o fue ingresado incorrectamente.
2. **Contraseña incorrecta:** Sucede cuando la contraseña ingresada es incorrecta o no cumple con los requisitos establecidos.

{% hint style="info" %}
Existen otros errores que pueden presentarse por causas externas al sistema y que no dependen directamente de las acciones del usuario.
{% endhint %}

***

### Dashboard

El **panel de control (dashboard)** muestra información general sobre el estado del sistema y confirma si todo está correctamente configurado cuando se habilita un nuevo **semestre**.

<figure><img src="https://427283098-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2Fc3Xztvbl6hZF1pSc3D5c%2Fuploads%2F0qTJynHhhwifqFy7yCi3%2FCaptura%20de%20pantalla%202025-10-08%20213928.png?alt=media&#x26;token=a8d10867-5487-44b3-bdbb-147ef93888d4" alt=""><figcaption></figcaption></figure>

### Semestre actual

En esta sección se muestra el **último semestre creado** en el sistema, lo que permite verificar en todo momento si los datos que se visualizan corresponden al periodo activo.

También se muestra el **estado del semestre**, el cual indica si el proceso de elaboración de horarios ha concluido o sigue en curso.

{% hint style="warning" %}
Este apartado solo aparece cuando se ha creado un nuevo semestre.
{% endhint %}

<figure><img src="https://427283098-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2Fc3Xztvbl6hZF1pSc3D5c%2Fuploads%2FpPhiOa7HOmshxJ0xk2Gm%2FCaptura%20de%20pantalla%202025-10-08%20215421.png?alt=media&#x26;token=cba30a73-3e8a-46c4-b9c5-24fd39a89a96" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
Para más detalles sobre los semestres y sus funcionalidades, consulta la sección [semestres.md](recursos-academica/semestres.md "mention").
{% endhint %}

### Configuración inicial

Estas configuraciones se realizan una sola vez, ya que contienen información base que no cambia con frecuencia.

1. [<mark style="color:orange;">**Agregar materias**</mark>](https://docs.sistemahorarios.me/tDaJOooJQpDbSTEIS4kV/recursos-academica/materias): muestra el total de materias registradas.
2. [<mark style="color:blue;">**Agregar docentes**</mark>](https://docs.sistemahorarios.me/tDaJOooJQpDbSTEIS4kV/recursos-academica/docentes): muestra el total de docentes registrados.
3. [<mark style="color:red;">**Agregar grupos**</mark>](https://docs.sistemahorarios.me/tDaJOooJQpDbSTEIS4kV/recursos-academica/grupos): muestra el total de grupos registrados.
4. [<mark style="color:green;">**Crear semestre**</mark>](https://docs.sistemahorarios.me/tDaJOooJQpDbSTEIS4kV/recursos-academica/semestres): muestra el total de semestres creados.
5. [**Configuración general**](https://docs.sistemahorarios.me/tDaJOooJQpDbSTEIS4kV/otros/configuracion): indica si se ha establecido correctamente la información académica general.

Además, se muestra una **barra de progreso** que refleja el avance a medida que se completa cada paso.

{% hint style="info" %}
La siguiente imagen muestra una configuración inicial completamente vacía.
{% endhint %}

<figure><img src="https://427283098-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2Fc3Xztvbl6hZF1pSc3D5c%2Fuploads%2F0AkGvafOjc04eKqSOuQC%2FCaptura%20de%20pantalla%202025-10-08%20220636.png?alt=media&#x26;token=8836a952-8b68-4c3f-9fee-337ca9965dd8" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
A continuación, se muestra la configuración inicial completa, con todos los pasos correctamente realizados.
{% endhint %}

<figure><img src="https://427283098-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2Fc3Xztvbl6hZF1pSc3D5c%2Fuploads%2FQDz8hC2F7NSEKUPfhgBj%2FCaptura%20de%20pantalla%202025-10-08%20220022.png?alt=media&#x26;token=545950a1-c883-4cfc-98a7-b3bfe27da335" alt=""><figcaption></figcaption></figure>

Una vez completada la configuración sin errores, esta será la base de datos que el sistema utilizará de manera global.

#### Configuración del semestre

Si todos los pasos anteriores se realizaron correctamente, esta sección no debería mostrarse. Sin embargo, si aún no existe un [semestres.md](recursos-academica/semestres.md "mention"), es necesario crearlo.

<figure><img src="https://427283098-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2Fc3Xztvbl6hZF1pSc3D5c%2Fuploads%2Fb64LA3bYlbLWUeFsfPzH%2FCaptura%20de%20pantalla%202025-10-09%20091838.png?alt=media&#x26;token=6b7a8ea7-4ab6-459a-aac6-ed0540ae60b0" alt=""><figcaption></figcaption></figure>

Los siguientes pasos son <mark style="color:red;">**IMPORTANTES**</mark> y deben realizarse cada vez que se crea un nuevo semestre académico, ya que contienen información fundamental para la elaboración de los horarios.

6. [**Asignar materias a los grupos**](https://docs.sistemahorarios.me/tDaJOooJQpDbSTEIS4kV/relaciones/materias-con-grupos): Permite definir qué materias se imparten en cada grupo, optimizando la creación de horarios al mostrar solo las materias relevantes.
7. [**Asignar docentes a materias**](https://docs.sistemahorarios.me/tDaJOooJQpDbSTEIS4kV/relaciones/docentes-con-materias): Asocia las materias a los docentes responsables, lo cual es esencial para reflejar correctamente los horarios finales de cada docente.
8. [**Asignar docentes a grupos**](https://docs.sistemahorarios.me/tDaJOooJQpDbSTEIS4kV/relaciones/asignacion-de-docente-a-grupos): Este paso permite vincular docentes con los grupos asignados. Es posible que una misma materia tenga `uno o más` docentes.

{% hint style="warning" %}
Recuerda: esta configuración debe realizarse **cada vez que se crea un nuevo semestre escolar**.
{% endhint %}

<figure><img src="https://427283098-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2Fc3Xztvbl6hZF1pSc3D5c%2Fuploads%2FYtjjZGFzsm5jNUYCdI9h%2FCaptura%20de%20pantalla%202025-10-09%20092230.png?alt=media&#x26;token=bd45ee5c-daa8-4ad9-b487-60b8069bdbce" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
Cada paso muestra información relevante, incluyendo la cantidad de datos esperados y el porcentaje de avance correspondiente.
{% endhint %}

<figure><img src="https://427283098-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2Fc3Xztvbl6hZF1pSc3D5c%2Fuploads%2F1vEBEhTHU5o1HJQb5nez%2FCaptura%20de%20pantalla%202025-10-09%20093958.png?alt=media&#x26;token=e2260645-a32c-4808-8351-757b4a3b2191" alt=""><figcaption></figcaption></figure>

{% hint style="success" %}
Una vez completados todos los pasos y alcanzado el porcentaje requerido, el sistema mostrará el estado como **completo y listo para trabajar**.
{% endhint %}
