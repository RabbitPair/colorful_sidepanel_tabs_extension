# Registro de cambios

Todos los cambios notables de este proyecto se documentarán en este archivo.

Este proyecto se adhiere a [Versionado Semántico](https://semver.org/).

----
## [No publicado]

- **Snapshots programados**: Guarda automáticamente snapshots a intervalos especificados. Esta función asegura que tu trabajo se respalde periódicamente, proporcionando una red de seguridad contra la pérdida de datos.

----
## [2.11.0] - 2024-10-07
### Añadido
- **Menú de Pestañas**: Se han añadido nuevos menús:
  - **Renombrar Título de Pestaña**: Permite cambiar el título de la pestaña. Por defecto, la opción para recordar la configuración de la URL está seleccionada, por lo que el título se actualizará automáticamente la próxima vez que abras la URL.
  - **Mover Pestaña a Nueva Ventana**: Permite mover la pestaña a una nueva ventana.
  - **Mover Pestaña a Otra Ventana**: Permite mover la pestaña a otra ventana existente.
  - **Eliminar Pestaña del Grupo**: Permite eliminar la pestaña de su grupo actual.

- **Configuración de Pestañas**: Se han añadido nuevas opciones a la configuración de pestañas:
  - **Máximo de Líneas Mostradas en el Título de la Pestaña**: Establece el número máximo de líneas para mostrar en los títulos de las pestañas. Las líneas adicionales se ocultarán.
  - **Máximo de Líneas Mostradas en el Título del Grupo**: Establece el número máximo de líneas para mostrar en los títulos de los grupos. Las líneas adicionales se ocultarán.
  - **Ancho del Título del Grupo Colapsado**: Cuando el grupo está colapsado, establece el ancho del título del grupo.
  - **Mostrar Conteo de Pestañas del Grupo**: Muestra el número de pestañas en cada grupo junto al nombre del grupo.

- **Configuración del Sitio**: Se han añadido nuevas opciones a la configuración del sitio:
  * **Mantener Página Activa**: Cuando está habilitado, se permitirá que el navegador descarte la pestaña. Si habilitas la configuración de rendimiento y estableces un tiempo para descartar pestañas inactivas, la pestaña se descartará después del tiempo especificado. Si está deshabilitado, la pestaña no se descartará.
  * **Unirse Automáticamente al Grupo**: Cuando está habilitado, el sitio creará o se unirá automáticamente al grupo especificado.
  * **Modo Incógnito**: Cuando está habilitado, puedes elegir borrar automáticamente los datos de navegación al visitar el sitio. Esto incluye varias opciones configurables: Cookies, Historial, CacheStorage, FileSystems, IndexedDB, LocalStorage, ServiceWorkers y WebSQL. Ten en cuenta que no se utiliza el permiso browsingData para evitar solicitar permisos adicionales.
  * **Actualización Automática**: En la configuración de enlaces, puedes especificar URLs para actualizar automáticamente, con soporte para expresiones regulares.

### Cambiado
- **Imagen-en-Imagen Avanzado**: Se añadió soporte universal de subtítulos para el reproductor plyr.
- **Mantener Página Activa**: Funcionalidad mejorada para mantener las pestañas activas.
- **Estilo de Pestañas de Grupo**: Se modificó el estilo de las pestañas dentro de los grupos.
- **Orden del Menú**: Se ajustó el orden de los elementos en el menú de pestañas.

### Corregido
- **Imagen-en-Imagen**: Se solucionó un problema donde el título no cambiaba después de cambiar videos en el reproductor Imagen-en-Imagen.
- **Asignaciones Personalizadas de Grupos**: Se solucionó un problema donde los cambios en las asignaciones personalizadas de grupos para sitios web no surtían efecto inmediatamente cuando la opción "Recordar agrupación del sitio" estaba habilitada en la configuración de Grupos de Pestañas Avanzados. Esto se ha resuelto para aplicar los cambios instantáneamente sin requerir un reinicio.

----


## [2.10.2] - 2024-10-07

- Se solucionó el problema donde los danmaku (comentarios flotantes) se detenían o desaparecían en algunos sitios web después de cambiar de página (evento de ocultación de página)
- Se ocultaron los controles de video HTML5

----
## [2.10.1] - 2024-10-05

### Corregido
- Se solucionó el problema donde los eventos de acceso directo se activaban repetidamente al reproducir múltiples videos consecutivamente
- Se corrigió un problema donde el reproductor fallaba al restaurarse en ciertas situaciones
- Se solucionó el problema donde la barra de progreso de reproducción no funcionaba correctamente al usar el modo Imagen en Imagen
- Se corrigió el problema donde cambiar de pestaña activaba una notificación de detección de Imagen en Imagen después de navegar desde una página con video a una página sin video en la misma pestaña
- Se solucionó el problema donde la ventana de Imagen en Imagen no se cerraba al salir del modo Imagen en Imagen usando jwPlayer
- Se corrigió el problema donde una dirección incorrecta causaba que la página se bloqueara al configurar una imagen de fondo

----
## [2.10.0] - 2024-10-01

### Añadido
- **Documento Imagen-en-Imagen**: Presentamos Imagen-en-Imagen Avanzado, disponible para prueba gratuita antes del lanzamiento oficial de la versión premium de la extensión. Cuando está habilitado, tiene prioridad sobre la Imagen-en-Imagen estándar. Si la página actual no lo admite, se utilizará el modo estándar. Imagen-en-Imagen Avanzado cuenta con un reproductor de video personalizado con funcionalidades como:
  * **Reproducir/Pausar video** (Espacio o K)
  * **Ajustar volumen** (Flecha arriba/abajo)
  * **Silenciar/Activar sonido del video** (M)
  * **Avanzar/Rebobinar video** (Flecha izquierda/derecha o Rueda del ratón)
  * **Avanzar/Rebobinar video 5 segundos** (Flecha izquierda/derecha)
  * **Avanzar/Rebobinar video 10 segundos** (J/L)
  * **Reproducir el siguiente video** (Shift + N)
  * **Reproducir el video anterior** (Shift + P)
  * **Mostrar subtítulos** (compatible en algunos sitios web como youtube.com, vimeo.com, tver.jp, etc.) (C)
  * **Mostrar comentarios** (compatible en algunos sitios web como nicovideo.jp, bilibili.com, etc.) (D)
  * **Salir de Imagen-en-Imagen** (Esc)
  * **Alternar ocultar/mostrar video y reproducir/pausar** (Q)
  * **Alternar pantalla completa** (F)
  * **Ajustar velocidad de reproducción** ( > o <)
  * **Buscar al inicio/fin del video** (Inicio/Fin)
  * **Buscar a un porcentaje del video** (0-9)
  * **Ajustar ventana para que se ajuste al tamaño del video** (W)
  * **Alternar Imagen-en-Imagen desde la página principal** (Alt + P)
  
  > Si los sitios web que visitas frecuentemente admiten subtítulos o comentarios, puedes enviar un [problema: Imagen-en-Imagen Avanzado](https://github.com/RabbitPair/colorful_sidepanel_tabs_extension/issues/new?assignees=&labels=&projects=&template=Advanced-Picture-in-Picture.md&title=), y lo adaptaremos lo antes posible. Ten en cuenta que algunos sitios web pueden tener restricciones regionales, lo que requiere información adicional.
- **Atajo para Imagen-en-Imagen**: Se ha añadido un nuevo atajo de teclado Alt+P para alternar rápidamente el modo Imagen-en-Imagen. Esto permite a los usuarios cambiar fácilmente los videos a la vista Imagen-en-Imagen sin usar el ratón, mejorando la productividad y las capacidades de multitarea.
- **Alternar Imagen-en-Imagen en la Barra de Navegación Inferior**: Ahora puedes agregar una opción de alternar Imagen-en-Imagen a la barra de navegación inferior. Esto se puede configurar en la configuración de apariencia bajo "Mostrar barra de navegación inferior" - "Configurar".
- **Ordenar Pestañas por URL**: Se ha añadido una nueva opción de menú "Ordenar Pestañas por URL" al menú "Más".
- **Comportamiento de Colapso de Grupo de Pestañas**: Se ha añadido una nueva opción "Comportamiento de Colapso de Grupo de Pestañas" al menú "Grupo de Pestañas Avanzado". Puedes modificar el comportamiento del colapso de grupos de pestañas en el navegador. Las opciones incluyen: 'Mostrar grupo actual y colapsar otros grupos', 'Expandir todos los grupos' y 'Usar configuración predeterminada del navegador'.
- **Configuración del Sitio**: Se han añadido tres nuevas opciones a la configuración del sitio:
  * **Acción de Restricción de Imagen-en-Imagen**: Configurar la acción para las restricciones de Imagen-en-Imagen.
  * **Entrar automáticamente en Imagen-en-Imagen**: Entrar automáticamente en el modo Imagen-en-Imagen cuando haya un video presente al ingresar a la página.
  * **Configuración de Subtítulos**: Configurar los selectores CSS para el elemento de subtítulos y su elemento padre en la página.

### Cambiado
- Cuando la pestaña del panel lateral no está abierta, si "Imagen-en-Imagen al Cambiar de Pestaña" está habilitado (habilitado por defecto), entrará automáticamente en el modo Imagen-en-Imagen (Recordatorio importante: Se requiere interacción del usuario, como hacer clic en la página que reproduce el video para activar la interacción del usuario).
- Al cerrar la barra lateral de la página, ahora se elimina en lugar de ocultarse. Volverá a aparecer solo después de actualizar la página.

### Arreglado
- Se ha solucionado el problema donde la lista de Acceso Rápido no manejaba múltiples URLs.

----

## [2.9.0] - 2024-09-15

- Añadido **Borrar Pestañas**: Guarda una instantánea y cierra todas las pestañas excepto la activa. Restaúralas desde las pestañas cerradas recientemente o las instantáneas.
- Añadido **Activar Agrupación de Pestañas Automáticamente**: Crea automáticamente un nuevo grupo al abrir una nueva pestaña. Las pestañas subsecuentes abiertas desde esta pestaña se unirán al grupo.
- Añadido **Espaciado Vertical de la Lista**: Nueva opción en la configuración de Grupo de Pestañas Avanzado para ajustar el espaciado vertical de los elementos de la lista.
- Añadido **Agregar Múltiples URLs a Acceso Rápido**: Permite agregar grupos y seleccionar múltiples pestañas para guardar en Acceso Rápido.
- Añadido **Espaciado de Elementos de Acceso Rápido**: Establece el espaciado vertical/horizontal para los elementos de Acceso Rápido en la página de opciones.

---
## [2.8.0] - 2024-09-12
### Añadido
- Añadido **Historial de Pestañas**: Ahora puedes ver fácilmente qué sitios web se han abierto bajo la misma pestaña. Haz clic izquierdo para abrir el sitio web en la pestaña actual, clic medio o Ctrl+clic izquierdo para abrir el sitio web en una nueva pestaña. Para más detalles, por favor consulta la página de opciones.
- Añadido **Nombres de grupos personalizados**: En la página de opciones - Grupo de Pestañas Avanzado, puedes añadir algunos grupos predefinidos aquí, para que puedas seleccionarlos rápidamente cuando necesites añadir pestañas a un grupo. Ya hemos predefinido algunos nombres de grupos, que puedes modificar o eliminar según tus necesidades.
- Añadido **Usar el nombre de la carpeta de marcadores como nombre de grupo**: En la página de opciones - Grupo de Pestañas Avanzado, se ha añadido una nueva opción. Si el sitio web abierto es un marcador, se añadirá automáticamente al grupo, y el nombre del grupo usará el nombre del directorio de marcadores.
- Añadido **Índice de Pestañas**: En la página de opciones, cuando está habilitado, el índice de pestañas se mostrará junto al título, facilitando la activación de la pestaña usando [Ctrl+número] en Windows o [cmd+número] en Mac. Ejemplo: 1. stackoverflow.com 2. youtube, para que sea fácil hacer Ctrl + 2 en Windows o cmd + 2 en Mac para ir a youtube.
- **Configuraciones del sitio optimizadas**: Mejorada la opción para establecer el color de fondo y el color de la fuente para los sitios.

### Cambiado
- Al comprobar los marcadores, permitir la actualización de las URL redirigidas. Si la URL no es accesible, mostrar códigos de error: Respuestas exitosas (200 – 299), Mensajes de redirección (300 – 399), Respuestas de error del cliente (400 – 499), Respuestas de error del servidor (500 – 599). Para más detalles, por favor consulta: https://developer.mozilla.org/en-US/docs/Web/HTTP/Status

### Arreglado
- Arreglado el problema donde el popup de modificación de marcadores no desaparecía

---

## [2.7.0] - 2024-09-05
### Añadido
- Añadida **gestión de marcadores**: Se añadió funcionalidad completa de gestión de marcadores
- Añadida **barra de navegación de pestañas**: opciones en apariencia, mostrando: pestañas, marcadores, historial, pestañas cerradas recientemente, lista de lectura y acceso rápido en el panel lateral
- Añadido menú **Agregar pestaña al grupo**: agregar pestañas a un nuevo grupo o a un grupo existente
- Añadido resaltado de palabras clave de búsqueda
- Añadida reserva de Edición Premium
### Cambiado
- Ajustados permisos de Cookies, Lista de Lectura y marcadores a permisos opcionales, requiriendo autorización del usuario para su uso
### Obsoleto
- **Página de Opciones - Historial - Mostrar en el panel lateral**: Esta opción ha sido reemplazada por *barra de navegación de pestañas* y pronto será obsoleta

### Arreglado
- Arreglado el problema donde el botón de expandir grupo no aparecía al hacer clic por primera vez en la barra lateral
- Arreglado el problema donde al reabrir el navegador y hacer clic en el icono de la extensión requería volver a seleccionar entre popup o barra lateral
- Arreglado el problema donde el tamaño del icono de pestaña fijada y el icono de acceso rápido eran inconsistentes

---

## [2.6.1] - 2024-08-30

### Cambiado
- Método de visualización del menú optimizado, mejorados los mensajes de error
- Añadida más compatibilidad para navegadores basados en Chromium


---

## [2.6.0] - 2024-08-28
### Añadido
- Añadido **Zoom del Menú de Pestañas**: Se ha añadido una función de zoom al menú de pestañas, permitiendo ajustar libremente el nivel de zoom del 1% al 1000%.

### Cambiado
- El Acceso Rápido se ha movido a un elemento de menú separado.
- Optimizada la clasificación por arrastrar y soltar

### Arreglado
- Arreglado un problema donde algunas áreas no cambiaban después de alterar el color de la fuente.

### Obsoleto
- **Acceso Rápido en el Menú de Pestañas**: El Acceso Rápido se ha movido a un elemento de menú separado. La opción en el menú de pestañas será obsoleta pronto (la funcionalidad sigue siendo la misma).

### Eliminado
- Eliminada la opción de zoom de la configuración del sitio porque ajustar el zoom en el menú no proporcionaba una vista previa intuitiva de los cambios. La función de zoom se ha movido al menú de pestañas para una vista previa en tiempo real.

---

## [2.5.2] - 2024-08-27

### Arreglado

- Arreglado el problema donde las imágenes de fondo guardadas se perdían después de reiniciar la aplicación
- Arreglado el problema donde cerrar todas las pestañas del mismo sitio en todas las ventanas fallaba
- Arreglado el bloqueo al deshabilitar DnD

------

## [2.5.0] - 2024-08-25

### Añadido

- Soporte para la clasificación por arrastrar y soltar de pestañas y grupos en orden de pestañas, y sincronización con Chrome
- Sincronizar el estado de expansión del grupo con Chrome

### Arreglado
- Arreglado el problema donde subir un archivo de imagen de fondo demasiado grande causaba un error de cuota excedida QUOTA_BYTES
- Arreglado el problema donde mostrar todas las pestañas de la ventana causaba un error y agrupar por sitio fallaba


---

## [2.4.0] - 2024-08-20

### Añadido
- añadir **Subir Imagen de Fondo**: Puedes subir una imagen desde tu dispositivo local para usarla como fondo.
- añadir **Color de Fondo Personalizado**: Ahora soporta colores de fondo personalizados, y también puedes elegir un color para generar un hermoso degradado

### Cambiado

- **color de la fuente**: El color de la fuente cambiará automáticamente a negro o blanco basado en el color dominante del fondo o imagen de fondo. Si la imagen es grande, puede tomar algún tiempo aplicar el fondo, lo cual es normal.

### Arreglado
- Arreglado el problema donde algunas áreas no cambiaban después de cambiar el color de la fuente

### Obsoleto
- **Estilo de fondo de lista**: Esta característica establece el estilo de fondo para cada lista, con algunos colores degradados incorporados. Sin embargo, con el lanzamiento de colores de fondo personalizados, su misión ha sido completada y será eliminada pronto.

---

## [2.3.0] - 2024-08-16

### Añadido
- añadir **Barra Lateral en Páginas**: La barra lateral de la página te permite inyectar una barra lateral en las páginas web que estás navegando sin abrir la barra lateral del navegador para gestionar pestañas. Esta es una característica muy útil para usuarios con resoluciones de pantalla más pequeñas que encuentran la barra lateral del navegador demasiado ancha e inajustable. Sin embargo, debido a algunas restricciones, la barra lateral de la página solo ofrece funcionalidad muy limitada. Cuando esta característica está habilitada, puedes usar el ratón para pasar por el borde de la ventana y sacar la barra lateral.

### Eliminado
- eliminar **Bola flotante**

---

## [2.2.0] - 2024-08-14

### Añadido
- Nuevo menú de pestañas **Mantener Pestaña Activa**: Mantén la pestaña activa para que no se descarte automáticamente.

### Cambiado
- Rendimiento optimizado y tamaño del paquete reducido.

---

## [2.1.0] - 2024-08-10

### Añadido
- Guardar automáticamente instantáneas de ventana, grupo y pestaña. Después de reiniciar el navegador, si solo una ventana está abierta y se abren menos de 5 nuevas pestañas, un aviso te pedirá restaurar la última ventana y la información de pestañas guardadas cuando se abra la barra lateral.

### Cambiado
- Optimizados los datos de almacenamiento para acceso rápido para acelerar el tiempo de acceso.

### Arreglado
- Arreglados otros problemas menores.

---

## [2.0.1] - 2024-08-09

### Arreglado
- Arreglado el formato del mensaje para la importación exitosa de instantáneas.
- Arreglado el problema donde las importaciones duplicadas causaban entradas repetidas de acceso rápido.

---

## [2.0.0] - 2024-08-08

### Cambiado
- Renombrada la extensión de "Pestañas de Panel Lateral Colorido" a **"VertiTab - Pestañas Verticales de Panel Lateral"**.

### Añadido
- Instantáneas: Añadida una función de guardar instantáneas de pestañas del navegador con un solo clic. Puedes guardar instantáneas antes de cerrar el navegador y restaurarlas rápidamente la próxima vez que lo abras. Actualmente, se pueden guardar hasta 50 instantáneas.
- Barra de Navegación Inferior Mejorada: Accede a más características desde la barra de navegación inferior, como marcadores, historial, pestañas cerradas recientemente, lista de lectura, acceso rápido, abrir nueva pestaña, crear instantánea, buscar, colapsar grupos, etc.
- Funcionalidad de Importación/Exportación Actualizada: Mejoradas las opciones de importación y exportación para gestionar mejor las pestañas en diferentes dispositivos.

### Arreglado
- Corrección de errores y mejoras de estabilidad.

---

## [1.3.3] - 2022-08-04

### Añadido
- **linkSettings**: La configuración del sitio ahora incluye una nueva opción que te permite agregar reglas para controlar si los enlaces del sitio se abren en la pestaña actual o en una nueva pestaña.

---

## [1.3.2] - 2024-08-02

### Arreglado
- Arreglado el problema donde hacer clic con el botón central del ratón para cerrar la pestaña no funcionaba.

---

## [1.3.1] - 2024-08-01

### Cambiado
- Optimizado el diseño de acceso rápido y añadido soporte para la clasificación por arrastrar y soltar.
- Mejorada la lógica para expandir todos los grupos y recordar su estado.

### Arreglado
- Arreglado el problema donde la importación de datos de acceso rápido fallaba cuando el panel lateral no estaba abierto.
- Arreglado el problema donde los iconos estaban desalineados en la vista de grupo.
- Arreglados otros problemas menores.

---

## [1.3.0] - 2024-07-30

### Añadido
- **Importar/Exportar**: Exportar preferencias de usuario, acceso rápido, configuración del sitio web y datos de pestañas cerradas recientemente, e importarlos en otro navegador para sincronizar los datos de la extensión.
- **Seleccionar acceso rápido desde el historial**: Puedes buscar los sitios web más visitados desde el historial y agregarlos al acceso rápido.
- **Más opciones en la barra de herramientas**: Añadir más opciones a la barra de herramientas. Puedes ocultar la etiqueta en la barra de herramientas y controlar qué iconos se muestran en la barra de herramientas.

### Cambiado
- **Cuadro de búsqueda**: El cuadro de búsqueda ahora soporta la tecla Enter para buscar palabras clave en una nueva pestaña. Si no hay pestañas o historial coincidentes después de ingresar la palabra clave, puedes presionar Enter para buscar usando el motor de búsqueda predeterminado.
- **Inicialización de datos**: Ajustar el tiempo de inicialización de datos y optimizar el renderizado repetido causado por modificaciones de datos.
- **URL del registro de cambios**: Actualizar la URL del registro de cambios a la URL de lanzamiento en GitHub.
- **Optimización del diseño**: Optimizar los cambios de diseño cuando cambia el tamaño de la ventana.
- **Registro de errores**: Usar Sentry para recopilar registros de errores. Ten la seguridad de que esta función no recopilará tus datos privados.

### Arreglado
- **Error de posición de la información sobre herramientas**: Arreglar el problema donde la información sobre herramientas parpadea al cambiar temas y vistas en la barra de herramientas.
- **Navegación inferior**: Arreglar el problema donde la navegación inferior bloquea la lista cuando hay muchas pestañas abiertas.

---
## [1.2.3] - 2024-07-23

### Arreglado
- Arreglada la altura de desplazamiento de la lista incorrecta cuando las pestañas fijadas y los iconos de acceso rápido exceden 1 fila.

### Cambiado
- Cambiado descartar pestañas inactivas para excluir pestañas fijadas.
- Cambiado cerrar todas las pestañas descartadas para excluir pestañas fijadas.
- Ajustar el tamaño de los iconos de pestañas fijadas y de acceso rápido.

---

## [1.2.2] - 2024-07-19

### Añadido
- Añadir acceso rápido: Puedes configurar una pestaña para que aparezca en Acceso rápido y sea fácil de encontrar. Simplemente haz clic derecho (o mantén presionado) y selecciona Fijar en Acceso rápido. Desfíjala cuando ya no la necesites allí haciendo clic derecho (o manteniendo presionado) y seleccionando Eliminar de Acceso rápido. La diferencia con las pestañas fijadas es que Acceso rápido guarda la URL y abre una nueva pestaña cada vez que se hace clic.

### Cambiado
- Las pestañas fijadas solo muestran iconos para evitar que se hagan clic accidentalmente y se desfijen.
- Modificar el tamaño de los iconos de pestañas fijadas.

---

## [1.2.1] - 2022-07-17

### Añadido
- Añadir nuevo menú a la navegación inferior: descartar pestañas inactivas.
- Añadir nuevo menú a la navegación inferior: cerrar todas las pestañas descartadas.

### Cambiado
- Los cambios en el menú de navegación inferior "Agrupar por sitio" solo afectan a la ventana actual.

### Arreglado
- Arreglado el problema donde la interfaz de usuario saltaba debido a la inconsistencia de altura al cambiar pestañas activas en la lista.

---

## [1.2.0] - 2024-07-16

### Añadido
- Añadir Configuraciones del Sitio: Personaliza configuraciones específicas del sitio, como deshabilitar el modo de Imagen en Imagen, deshabilitar el modo de descarte automático, y más.

### Arreglado
- Arreglar Crear o Unirse Automáticamente al Mismo Grupo de Dominio: Resuelto un problema donde la creación o unión automática a los mismos grupos de dominio no funcionaba cuando se actualizaba una pestaña.
- Arreglar Página No Recibiendo Mensajes de Actualización de Configuración: Asegurado que las páginas reciban correctamente los mensajes de actualización de configuración.
- Arreglar Otros Errores: Abordados varios otros errores para mejorar la estabilidad y el rendimiento.

### Cambiado
- Añadir Opción para Mostrar el Botón de Cerrar al Pasar el Ratón: Añadida una opción para mostrar el botón de cerrar solo al pasar el ratón sobre una pestaña.

---

## [1.1.0] - 2024-07-13

### Añadido
- Añadir Opciones de Rendimiento: Introducir nuevas configuraciones de rendimiento para personalizar y mejorar tu experiencia de navegación.
- Añadir Icono de Desplazamiento a la Pestaña Activa: Navega fácilmente a la pestaña activa con un nuevo icono de desplazamiento a la pestaña activa.
- Añadir Ordenar Pestañas por Dominio: Organiza tus pestañas por dominio con una nueva función de ordenación.
- Silenciar Todas las Pestañas que Hacen Sonido: Silencia rápidamente todas las pestañas que están reproduciendo sonidos para una experiencia de navegación más tranquila.

### Cambiado
- Eliminar Icono de Restaurar: El icono de restaurar ha sido eliminado y reemplazado con la opacidad del texto de la lista establecida en 0.5 para una apariencia más limpia.

### Deprecado
- Eliminar Ordenación por Arrastrar y Soltar: La solución actual para la ordenación por arrastrar y soltar tiene problemas de rendimiento y ha sido eliminada temporalmente.

---

## [1.0.4] - 2024-07-09

### Añadido
- Ordenación por Arrastrar y Soltar para Pestañas: Reorganiza fácilmente tus pestañas con la funcionalidad de arrastrar y soltar.

### Cambiado
- Optimizar la Velocidad de Carga de la Página: Mejorada aún más la velocidad de carga de la página para una experiencia de navegación aún más fluida.

---

## [1.0.3] - 2024-07-05

### Arreglado
- Arreglar Error del Menú de Vista Mixta: Resuelto un problema donde el menú de vista mixta mostraba errores.

### Cambiado
- Optimizar el Menú de Dominio del Grupo de Pestañas: Mejorado el menú de dominio del grupo de pestañas para una mejor organización y usabilidad.
- Optimizar el Relleno de Pestañas: Ajustado el relleno de pestañas para un diseño más estilizado y visualmente atractivo.

---

## [1.0.2] - 2024-07-04

### Añadido
- Indicador de Pestaña Activa Actual: Identifica fácilmente la pestaña activa con un nuevo indicador visual.
- Color de Fuente Personalizado: Personaliza tu interfaz configurando un color de fuente personalizado.

### Cambiado
- Optimizar la Velocidad de Carga: Mejorada la velocidad de carga para una experiencia de usuario más rápida y fluida.

### Configuraciones Predeterminadas
- Configurar por Defecto No Usar el Modo de Color: La configuración predeterminada ahora usa el modo de un solo color para una apariencia simplificada.

---

## [1.0.1] - 2024-07-02

### Añadido
- Registro Completo del Historial por Rango de Tiempo: Accede y gestiona tu historial de navegación con registros detallados ordenados por rango de tiempo.
- Modo de Color Único para la Lista: Introducir un modo de color único para una apariencia de lista simplificada y consistente.

### Cambiado
- Tiempo de Actualización Completa de la Barra de Progreso de Audio: Mejorada la precisión de las actualizaciones de la barra de progreso de audio para una experiencia multimedia más fluida.
- Método Optimizado de Adquisición de Iconos de Lista: Mejorado el método para adquirir iconos de lista, resultando en una carga de iconos más rápida y confiable.

### Arreglado
- Arreglar Problema de Visualización Incorrecta del Estado de Activación en Múltiples Ventanas: Resuelto un problema donde el estado de activación se mostraba incorrectamente cuando había múltiples ventanas abiertas.

---

## [1.0.0] - 2024-06-29

### Añadido
- Alternar Modo Claro/Oscuro: Elige entre modos de visualización claro y oscuro para que coincidan con tus preferencias.
- Tamaño de Fuente Personalizable: Ajusta el tamaño de la fuente para una experiencia de lectura más cómoda.
- Diseño de Interfaz Personalizable: Personaliza el diseño de la interfaz según tus hábitos de uso.
- Opciones de Personalización: Añade fondos coloridos e imágenes de fondo para hacer único tu panel lateral.
- Gestión Avanzada de Pestañas: Vistas previas en miniatura, opciones de ordenación y visualización ricas, y un menú de acciones completo para una gestión eficiente de pestañas.
- Funcionalidad de Búsqueda: Busca rápidamente pestañas cerradas recientemente o navega por tu historial para encontrar lo que necesitas.
- Modo Imagen en Imagen: Cambia sin problemas al modo Imagen en Imagen al cambiar de pestañas o desplazarte por páginas.
- Agrupación Automática: Crea o únete automáticamente a grupos basados en el mismo dominio para una mejor organización.
- Barra de Progreso de Lectura: Rastrea tu progreso de lectura en tiempo real para saber cuánto has leído.
- Barra de Progreso de Reproducción: Controla la reproducción multimedia con opciones para avanzar rápidamente, retroceder, controlar el volumen y ajustar la velocidad de reproducción.
