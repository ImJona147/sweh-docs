---
icon: triangle-exclamation
---

# Importante

## Errores

Aunque el sistema está terminado, no es perfecto. En ocasiones pueden aparecer errores, algunos causados por la red o por factores humanos. A continuación se describen los tipos de errores más comunes y cómo afrontarlos:

1. **Error de red**: este es un error <mark style="color:yellow;">`un poco más común`</mark>, pero no afecta el funcionamiento general. Sucede cuando el sistema no logra comunicarse con el servidor encargado de conectar con la base de datos.
2. **Error de conexión**: este error es <mark style="color:orange;">`algo común`</mark> y también ajeno al sistema. Generalmente se debe a problemas con la conexión a internet, lo que impide interactuar correctamente con el sistema.
3. **Ha ocurrido un error / error desconocido / otro**: estos son errores <mark style="color:yellow;">`poco comunes`</mark>. Ocurren cuando una acción no se pudo completar correctamente por alguna razón interna.
4. **Errores según la acción realizada:** estos errores aparecen porque el sistema está diseñado para prevenir ciertas acciones y notificar al usuario mediante una alerta.

Los <mark style="color:$danger;">`errores`</mark> y <mark style="color:$warning;">`advertencias`</mark> se muestran mediante notificaciones en la parte superior derecha de la pantalla.

<figure><img src="https://427283098-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2Fc3Xztvbl6hZF1pSc3D5c%2Fuploads%2FLnbhwB22uEMAhcKEfZKL%2FCaptura%20de%20pantalla%202025-10-10%20174233.png?alt=media&#x26;token=a60087e8-95d9-4d70-a3da-17f865f5086e" alt=""><figcaption></figcaption></figure>

Una de las características de este tipo de notificaciones es que puedes interactuar con ellas para leer el mensaje de error con más detalle.

{% hint style="info" %}
Esta acción también aplica para las notificaciones de tipo `Advertencia`.\
No aplica para <mark style="color:blue;">`Aviso`</mark> ni para `Éxito`.
{% endhint %}

<figure><img src="https://427283098-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2Fc3Xztvbl6hZF1pSc3D5c%2Fuploads%2F0ISSlUks4DOWgA5Bav6U%2FCaptura%20de%20pantalla%202025-10-10%20174411.png?alt=media&#x26;token=ad8e871b-1e2f-4ea0-8130-f2a1b59ed561" alt=""><figcaption></figcaption></figure>

Para ver el mensaje completo, da `clic` sobre la notificación.\
Al hacerlo, esta se ampliará y permanecerá visible el tiempo que necesites.

***

## Formato de plantillas

Es importante seguir la nomenclatura establecida y agregar los valores indicados para que el sistema reemplace automáticamente la información correspondiente en el formato final.

### <mark style="color:$success;">Plantilla de horarios</mark>

Esta plantilla es la más importante, ya que con ella se genera el horario final del semestre.\
Se deben utilizar las siguientes variables exactamente como se muestran para evitar errores durante el proceso.

<table><thead><tr><th width="180" align="center">Placeholder</th><th align="center">Descripción</th><th align="center">Ejemplo</th></tr></thead><tbody><tr><td align="center"><kbd>{plantel}</kbd></td><td align="center">Obtiene el nombre del plantel</td><td align="center"><code>COBAEV 16</code></td></tr><tr><td align="center"><kbd>{carpetaNombre}</kbd></td><td align="center">Obtiene el semestre al cual se elaboro el horario</td><td align="center"><code>2025 AGOSTO-ENERO</code></td></tr><tr><td align="center"><kbd>{grupoNombre}</kbd></td><td align="center">Obtiene el grupo al cual se esta descargando el horario</td><td align="center"><code>201 Matutino</code></td></tr><tr><td align="center"><kbd>{elaboro}</kbd></td><td align="center">Se suplanta por el nombre establecido en configuración</td><td align="center"><sub><code>LIC. TOMAS TAXILAGA ACUA</code></sub></td></tr><tr><td align="center"><kbd>{cargoElaboro}</kbd></td><td align="center">Se suplanta por el nombre establecido en configuración</td><td align="center"><sub><code>SUBDIRECTOR ACÁDEMICO</code></sub></td></tr><tr><td align="center"><kbd>{vobo}</kbd></td><td align="center">Se suplanta por el nombre establecido en configuración</td><td align="center"><sub><code>LIC. MARIA TERESA DE JESUS MORENO GOMEZ</code></sub></td></tr><tr><td align="center"><kbd>{cargoVobo}</kbd></td><td align="center">Se suplanta por el nombre establecido en configuración</td><td align="center"><code>DIRECTORA</code></td></tr></tbody></table>

{% hint style="info" %}
Estos datos son los que pueden ir dentro del documento sin importar el orden y es de carácter opcional.
{% endhint %}

La siguiente tabla muestra las variables que realmente son necesarias para el tema de los horarios, ya que estará haciendo un reemplazo de la información de cada grupo.
