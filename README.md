# Leire Mineria Twitter 2006-2019

Informe estatico e interactivo de actividad publica en X/Twitter relacionada con `@leirediezpas`, entre el 21 de marzo de 2006 y el 31 de diciembre de 2019.

El repositorio contiene un visor HTML y los ficheros de datos descargables.

## Que hace el HTML

`index.html` abre un visor navegable del grafo generado a partir de tweets publicos recuperados en la mineria.

Funciones principales:

- Grafo interactivo de cuentas y relaciones observables.
- Buscador global por cuenta, nombre, ID y texto de tweet.
- Filtros por año y tipo de relacion.
- Panel lateral al seleccionar una cuenta.
- Actividad global de la cuenta dentro de la mineria.
- Actividad recibida por esa cuenta dentro de la mineria.
- Actividad directa hacia `@leirediezpas` cuando exista.
- Listado de tweets vinculados a la seleccion.
- Descarga de todos los datos en formatos reutilizables.

Una relacion en el grafo significa que aparece una mencion, respuesta, cita, retuit o co-mencion en los datos recuperados. No implica afinidad, coordinacion ni relacion personal fuera de lo publicado.

## Descargas incluidas

Los datos estan disponibles en varios formatos:

- `tweets.csv`: tweets recuperados, fechas, autores, texto, metricas, enlaces y origen.
- `users.csv`: cuentas detectadas durante la mineria.
- `edges.csv`: relaciones completas tweet a tweet.
- `edges-aggregated.csv`: relaciones agregadas por origen, destino y tipo.
- `sources.csv`: trazabilidad de consulta, ventana temporal y capa de recuperacion.
- `graph.json`: datos usados por el visor HTML.
- `graph-gephi.gexf`: grafo listo para abrir en Gephi.
- `gephi-nodes.csv`: nodos para Gephi.
- `gephi-edges.csv`: aristas para Gephi.
- `raw-pages.ndjson`: paginas crudas recuperadas, para auditoria tecnica.
- `manifest.json`: parametros, periodo, conteos y metadatos de la exportacion.
