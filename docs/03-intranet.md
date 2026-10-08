# Intranet de Localiza Argentina (nuevo diseño)

**Estado:** Publicada, con mejoras pendientes.

## Resumen

La Intranet es la portada interna de Localiza Argentina: el lugar único donde cualquier empleado
encuentra qué hace cada área, su documentación, a quién contactar, los espacios de cultura de la
compañía y los accesos a los sistemas de uso diario. Vive dentro de la aplicación de gestión
interna de la empresa, así que no hace falta otro usuario ni otra contraseña para entrar.

En 2026 se rediseñó con la identidad de marca de Localiza, se le sumó un buscador real de áreas y
documentos, y la cultura de la empresa pasó a tener página propia.

## Problema que resuelve

Antes, la información de cada área estaba repartida: documentos sueltos en carpetas compartidas,
contactos que había que pedir por chat, links a sistemas guardados en favoritos de cada persona y
materiales de cultura mezclados con la documentación de un área puntual. Encontrar algo dependía
de saber a quién preguntar.

La Intranet ordena todo eso en una sola entrada:

- Un buscador para llegar a un área o a un documento sin saber dónde está guardado.
- Una estructura igual para todas las áreas (inicio, documentación, contacto).
- Un lugar para que cada área publique y mantenga su propio contenido, sin depender de un
  desarrollador para cada cambio.

## Qué incluye

### Portada

- **Franja de marca con saludo y buscador.** Busca áreas y títulos de documentos de todas las
  áreas a la vez. La búsqueda ignora tildes y no repite resultados que apuntan al mismo archivo.
- **Nuestra cultura**, en dos tarjetas:
  - **Nuestros espacios de encuentro**: los rituales de la compañía (RMR, RBD, REX y el Comité de
    Cultura).
  - **Sucursales**: videos para conocer a los equipos de cada sucursal.
- **Áreas**: Administración, Comercial, PYC (Personas y Cultura), IT, Marketing, Operaciones,
  Revenue Management y Multas, en una grilla uniforme. Un área que todavía no tiene contenido
  aparece como **Próximamente** y no se puede abrir.
- **Herramientas**: Hub de Links, Subir Documentos y Permisos de documentos (estas dos últimas
  sólo se muestran a quien tiene el permiso correspondiente).

### Páginas de cada área

Cada área tiene un encabezado de marca y una barra de navegación con las mismas secciones:

| Sección | Para qué sirve |
|---|---|
| **Inicio** | Qué hace el área. |
| **Documentación** | Documentos, manuales y procedimientos, con filtro por título, categoría o sección. |
| **Contacto** | Directorio del área, con búsqueda por nombre, rol o email. |
| **Estructura** | Organigrama (en PYC). |

Algunas áreas suman contenido propio: Administración muestra en su inicio las cotizaciones del
BCRA, Multas lleva a la plataforma de gestión de infracciones y a su página de contacto, e IT
tiene un inventario de equipos de acceso restringido (ver más abajo).

### Nuestra cultura

Página propia con pestañas **Espacios de encuentro**, **RMR**, **RBD** y **Sucursales**:

- **RMR** se agrupa por mes y por jornada (1 a 4).
- **RBD** (Reunión de Buen Día) se agrupa por edición.
- **Sucursales** reproduce los videos dentro de la misma página.

### Hub de Links

Accesos a los sistemas, plataformas y formularios de uso frecuente, filtrables por departamento o
por nombre.

### Inventario IT

Una sección del área de IT para llevar el inventario de equipos y servicios. Los distintos
inventarios usan vocabularios de estado diferentes, así que la herramienta los normaliza a un
estado operativo común (activo, pasivo o baja) para poder compararlos en una vista consolidada.
Los estados que no se reconocen no se pierden: quedan como "sin clasificar" y se ven en pantalla.
La web es la fuente de verdad, y el inventario se replica automáticamente a una planilla de
respaldo.

### Actividad

Los administradores tienen un historial de las subidas y bajas de documentos, para saber quién
cargó o sacó qué y cuándo.

## Cómo se usa

### Si buscás información

1. Entrás a la Intranet desde el menú lateral de la aplicación.
2. Escribís en el buscador de la portada, o entrás directo al área.
3. En **Documentación** filtrás por título, categoría o sección y abrís el documento.
4. Si necesitás hablar con alguien, vas a **Contacto** y buscás por nombre o rol.
5. Para abrir un sistema de uso diario, usás el **Hub de Links**.

### Si mantenés el contenido de un área

1. En **Herramientas**, entrás a **Subir Documentos**.
2. Completás título, área, subcarpeta (si corresponde) y una descripción breve.
3. Cargás el archivo o pegás el link a un archivo que ya está en Drive (útil para videos y
   archivos pesados).
4. El documento queda visible para todos en la **Documentación** del área.
5. Desde la misma Documentación podés editar los datos del documento o borrarlo.

Para RMR y RBD, el formulario pide además el mes y la jornada (o la edición), y se pueden
corregir después.

Los contactos del directorio también se editan desde el propio sitio: quien tiene permiso agrega,
corrige o borra entradas sin pasar por un desarrollo nuevo.

## Permisos

- **Entrar a la Intranet es universal.** Todos los usuarios la ven, sin importar su puesto, y el
  acceso no se puede quitar.
- **Subir documentos** está habilitado por defecto para coordinadores, team leaders, managers,
  usuarios corporativos y administradores.
- **Excepción abierta:** en las secciones RMR y RBD cualquier usuario puede subir su
  presentación. Quien subió ahí sin tener el permiso general no puede mover ese documento a otra
  sección.
- **Editar y borrar:** cada uno puede editar o borrar lo que subió; los documentos de otras
  personas sólo los toca quien tiene ese permiso.
- **Configuración de permisos:** los administradores definen, para cada acción (subir, editar,
  borrar), qué roles la tienen y pueden habilitar o bloquear usuarios puntuales. Un bloqueo
  individual pesa más que una habilitación, y ésta más que el rol.
- **Contactos e Inventario IT** se editan o consultan sólo por una lista reducida de usuarios
  autorizados.

## De dónde sale el contenido

- **Documentos:** se guardan en las carpetas de cada área en Google Drive. La Intranet sube el
  archivo a la carpeta que corresponde y registra sus datos (título, área, sección, descripción,
  quién lo subió). Al abrirlo, se ve en Drive.
- **Documentos por link:** si el archivo ya estaba en Drive, se registra sólo el link. Borrarlo
  de la Intranet no manda el archivo original a la papelera.
- **Borrado seguro:** al borrar un documento queda registro de quién y cuándo lo hizo.
- **Contenido fijo de las áreas** (descripciones, organigrama inicial, links): forma parte de la
  aplicación, con la posibilidad de editar los contactos desde el sitio.

## El rediseño: qué cambió y por qué

El rediseño se hizo en cuatro fases, sobre una propuesta visual "institucional" elegida entre
varias alternativas:

1. **Identidad de marca.** Se incorporaron los colores oficiales (verde y lima) y el logo de
   Localiza en versión vectorial, tomado del manual de marca. En modo oscuro, el texto de marca
   pasa a lima para mantener contraste.
2. **Portada nueva.** Franja verde con logo, saludo y buscador real; tarjeta destacada de cultura;
   áreas y herramientas en una grilla uniforme. Se eliminaron los colores distintos por área y
   el rojo que usaban algunas tarjetas, que se leía como señal de error.
3. **Encabezados de marca en cada área**, para que todas las páginas se vean parte del mismo
   sitio.
4. **Página "Nuestra cultura".** RMR, RBD, REX, Comité de Cultura y los videos de sucursales
   estaban dentro de la documentación de Personas y Cultura. Se mudaron a una página propia
   porque son rituales de toda la compañía, no documentos de un área.

Después se separó la tarjeta de cultura en dos (espacios de encuentro y sucursales), cada una con
accesos directos a su pestaña.

Junto al rediseño se corrigieron detalles operativos: las subidas de cada sección llegan a la
carpeta correcta de Drive, los errores de Drive se muestran en el diálogo de carga con un mensaje
claro en lugar de un error genérico, y el botón de borrar vuelve a pedir confirmación.

## Por qué es mejor

- **Se encuentra más rápido:** un buscador para todo, en lugar de navegar carpetas.
- **Se entiende igual en todas las áreas:** misma estructura, misma navegación.
- **Cada área es dueña de su contenido:** sube, edita y borra sin depender de desarrollo.
- **Control fino de permisos:** por acción, por rol y por persona, configurable desde la propia
  Intranet.
- **Trazabilidad:** queda registro de cada alta y baja de documentos.
- **Cultura visible:** los espacios de encuentro y las sucursales tienen lugar propio en la
  portada.
- **Imagen consistente** con la marca Localiza.

## Pendiente y próximos pasos

- **Agilizar el acceso a la información:** hay cambios pendientes en esa línea, todavía sin
  definir en detalle.
- **RMR y RBD cargadas antes del rediseño** aparecen como "Sin mes asignado" hasta que alguien
  les complete el mes y la jornada.
- **Terminar de alinear la marca:** el directorio de contactos todavía usa la paleta anterior.
- **Áreas en "Próximamente":** se van a habilitar a medida que carguen contenido.
