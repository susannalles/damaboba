# Criterios para la creación de los metadatos

## `ID` DEL OBJETO

Para la nomenclatura de cada uno de los objetos se ha optado por asignar un código alfanumérico único para cada caso, este está formado por el prefijo "dbitem" seguido por diez números que responden al siguiente esquema:

* Los cuatro primeros números indican la colección digital o institución a la que pertenece el objeto referido (0000: sin procedencia digital; 0100: colección propia; 1000: Bibilioteca Digital Hispánica; 2000: Museo del Prado; 3000: Memoria de Madrid; 4000: Plataformas de internet; 5000: Biblioteca Institut del Teatre; 6000: Biblioteca Menéndez Pelayo; 7000: Biblioteca de Catalunya; 8000: Hemeroteca de Sevilla; 9000: Biblioteca Digital de la Comunidad de Madrid; 1100: Internet Archives; 1200: Hathi Trust Digital Library)
* Los dos siguientes indican el siglo de pertenencia.
* Los dos siguientes indican la pertenencia a una de las cinco categorías establecidas (01: libros; 02: represantaciones teatrales; 03: imágenes fotográficas y pinturas; 04: representaciones no teatrales; 05: miscelánea)
* Los dos últimos responden a un número asignado a cada objeto dentro de la categoría

Ejemplo: dbitem1000170101 (dbitem+1000[BDH]+17[s.XVII]+01[libro]+01[ID])

## ELEMENTOS EN DUBLIN CORE

Se exponen aquí los elementos descritos por DC que se han utilizado para crear los diferentes registros:

- Título: `dc:title`
Nombre del objeto.

- Creador: `dc:creator`
Autor/es o creador/es del mismo.

- Descripción: `dc:description`
Breve descripción sobre el objeto referido.

- Publisher: `dc:publisher`
  1: Persona o institución que publica o edita el objeto analógico.
  2: Persona o institución encargada de disponer el recurso digital.

- Contribuyente: `dc:contributor`
Persona o institución que colabora en la elaboración del objeto (impresor, editor, productor...)

- Fecha: `dcterms:created`
Fecha de creación del objeto referido. Se aconseja que se siga la estructura YYYY-MM-DD.

- Tipología: `dc:type`
Señala la tipología material del objeto.

- Identificador: `dc:identifier`

- Fuente: `dc:source`
Indica la procedencia del objeto digital, enlace desde el origen, si lo hubiere.

- Idioma: `dc:language`
Idioma en el que está producido el objeto.

- Relación: `dc:relation`
Propiedad que señala la relación entre dos objetos, este campo es descriptivo, pero adicionalmente se debe incluir una propiedad (Ej: dcterms:isVersionOf/isPartOf) que indique el tipo de vínculo y el ID del objeto con que el que se relaciona.
  - `dcterms:isVersionOf`
  Se usa para señalar que el elemento presente versiona a pero sin cambiar la materialidad. (Ej: una reedición)
  - `dcterms:isPartOf`
  Indica la pertenecia del objeto a fotógrafo
  - `dcterms:conformsTo`
  Indica una reproducción aproximada de un objeto anterior pero que no puede ser filiado directamente.
  - `dcterms:isBasedOn`
  Indica si el objeto descrito se basa o inspira en otro precedente para su creación. (Ej: Un testimonio que deriva de otro)
  - `dcterms:isCopyOf`
Se usa siempre y cuando el objeto se haya creado con la intención de copiar el referido.

- Cobertura: `dcterms:temporal/spatial`
 Cobertura espacial o temporal del recurso. Es decir, lugares y periodos en los que estuvo vigente. Generalmente usado para representaciones de la obra.

- Derechos: `dc:rights`
Indica el tipo de derechos que protegen al objeto digital, si lo hubiere.

- Procedencia: `dcterms:provenance`
Utilizado para indicar si el objeto analógico al que hace referencia ha cambiado de custodia o propiedad si tiene relevancia para su estudio.

- Derechos de propiedad: `dcterms:rightsholder`
Indica quién tiene la propiedad actual del objeto analógico.
