---
icon: person-chalkboard
---

# Docentes

Página inicial donde se muestran todos los docentes dados de alta en el sistema. Si no hay registros, se mostrará un mensaje indicándolo.

En esta vista encontrarás opciones y herramientas para gestionar docentes:

1. Agregar docente.
2. Importar docentes desde Excel para cargas masivas.
3. Exportar todos los docentes (PDF, Word, Excel).
4. Buscar, cambiar vista y realizar acciones sobre cada registro.

<figure><img src="../.gitbook/assets/Captura de pantalla 2025-10-09 092836.png" alt=""></figure>

En la parte superior hay controles útiles:

- Barra de búsqueda: busca por nombre o matrícula.
- Vistas: alterna entre cuadrícula y lista.
- Acciones principales: botones para registrar, importar y exportar.

Funciones principales

1. Exportar

   Permite descargar TODAS las entradas de docentes en formatos comunes. Los formatos disponibles suelen ser:

   - PDF: descarga en formato sencillo y legible.
   - Word: plantilla básica con la información en formato documento.
   - Excel: tabla con los datos para edición o importación posterior.

   <p align="center"><img src="../.gitbook/assets/pdf-24.svg" alt=""><img src="../.gitbook/assets/word-24.svg" alt=""><img src="../.gitbook/assets/excel-24.svg" alt=""></p>

2. Importar

   Para facilitar la entrada masiva de docentes, el sistema acepta un archivo Excel (.xlsx). El archivo debe respetar una plantilla mínima para que el sistema pueda leerlo correctamente.

   Plantilla mínima (columnas):

   matricula	docente	especialidad

   - matricula: identificador del docente (ID o matrícula).
   - docente: nombre completo del docente.
   - especialidad: área, departamento o especialidad (opcional pero recomendable).

   Al elegir el archivo se abrirá un diálogo donde se muestran los datos extraídos:

   1. Barra de búsqueda: útil para filtrar filas cuando el archivo contiene muchos registros.
   2. Seleccionar y total: permite marcar todos los registros extraídos y ver el total seleccionado.
   3. Tabla de datos: vista previa de las filas con matrícula, nombre y especialidad.
   4. Acciones: `Cancelar` para abortar la importación, o `Importar` para subir los registros seleccionados.

   <figure><img src="../.gitbook/assets/Captura de pantalla 2025-10-09 151813.png" alt="" width="347"></figure>

   Nota: la importación puede fallar por formato incorrecto, datos inválidos o problemas de red. Revisa la sección `../otros/importante.md#errores` para más información sobre notificaciones y manejo de errores.

3. Nuevo docente

   Para crear un docente individualmente, el formulario solicita los datos principales con validaciones:

   - Nombre de docente: mínimo 5 y máximo 70 caracteres.
   - Matrícula (ID): mínimo 3 y máximo 8 caracteres.
   - Especialidad / Departamento: campo de texto (opcional).

   Si los valores no cumplen las restricciones, el sistema no permitirá guardar el registro.

   <figure><img src="../.gitbook/assets/Captura de pantalla 2025-10-09 160150.png" alt="" width="338"></figure>

   Ten en cuenta que esta acción puede fallar por datos erróneos o problemas del sistema; consulta `../otros/importante.md#errores` si aparece una notificación.

Una vez creado el docente, en la lista aparecerán nuevas acciones para cada registro:

<figure><img src="../.gitbook/assets/Captura de pantalla 2025-10-09 161933.png" alt="" width="232"></figure>

4. Editar

   Al editar, los campos se rellenan con los datos actuales del docente. Aplica las mismas validaciones que al crear.

<figure><img src="../.gitbook/assets/Captura de pantalla 2025-10-09 161903.png" alt="" width="336"></figure>

5. Eliminar

   Esta acción es irreversible: al confirmar se eliminará completamente el registro del docente de la base de datos. Lee la advertencia antes de confirmar.

<figure><img src="../.gitbook/assets/Captura de pantalla 2025-10-09 162306.png" alt="" width="241"></figure>

Errores y validaciones

- Asegúrate de que el archivo de importación tenga las columnas en el orden y formato correctos.
- Los campos obligatorios deben respetar las longitudes mínimas y máximas indicadas.
- Si ocurre un fallo, revisa la conexión y los datos fuente; las notificaciones del sistema indicarán el tipo de error.

Si quieres, puedo adaptar la plantilla de importación para incluir más columnas (correo, teléfono, asignaturas asignadas) o generar un ejemplo descargable en CSV/Excel.

