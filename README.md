# Ontología EDINT de Sensores Medioambientales (EDINT Environmental Sensors Ontology)

Esta ontología tiene como propósito definir y representar estaciones de medición y sensores medioambientales en el contexto de las ciudades inteligentes y la gestión del medio ambiente. Se ha diseñado como una extensión ligera y modular de la ontología SOSA (Sensor, Observation, Sample, and Actuator) y de GeoSPARQL, restringiendo sus mediciones a vocabularios controlados específicos.

# Propósito y alcance de la ontología (Purpose and scope of the ontology)

Actualmente, existen vocabularios consolidados para la representación de sensores y observaciones (SOSA) y geometrías o localizaciones (GeoSPARQL). Sin embargo, existía la necesidad de un modelo específico para representar de forma unificada infraestructuras de medición física (como cabinas de calidad del aire, boyas acuáticas o torres meteorológicas) y vincular de forma estricta los sensores que albergan con el vocabulario controlado SKOS de EDINT para variables medioambientales. Esta ontología cubre dicho propósito.

# Prefijo y espacio de nombres (Prefix and namespace)

El prefijo de la ontología de *Sensores Medioambientales* es: `edintmed` publicado bajo el espacio de nombres:[http://vocab.linkeddata.es/datosabiertos/def/medioambiente/](http://vocab.linkeddata.es/datosabiertos/def/medioambiente/)

# Modelo conceptual (Ontology conceptualization)

![Ontology Conceptualization Diagram](diagrams/diagrama-conceptual.drawio.png)

# Estructura del repositorio (Repository structure)

| Folder | Description |
|--------|--------------|
| **diagrams/** | Stores diagrams and other resources representing the conceptual model of the ontology (e.g., class hierarchies, relationships). |
| **docs/** | Stores the HTML or human oriented documentation of the ontology and related artefacts. |
| **examples/** | Includes examples that demonstrate how to instantiate or apply the ontology in real data scenarios. |
| **kos/** | Stores controlled vocabularies or KOS implementation, usually SKOS implementations in rdf. |
| **ontology/** | Contains the actual ontology implementation files in formats such as `.owl`, `.rdf`, `.ttl`, or `.jsonld`. |
| **requirements/** | Contains all documents used to define the ontology’s requirements: data example, competency questions, functional requirements, use cases, etc. |
| **shapes/** | Contains the SHACL shapes used to define and validate ontology constraints. |

# Mantenimiento y evolución (Maintenance and evolution)

Para manejar las incidencias o mejoras sugeridas con respecto a la ontología, recomendamos seguir las guías proporcionadas en ([Issues Management](./ISSUES.md)) para generar una incidencia.

# Financiación (Funding)

Esta ontología ha sido desarrollada en el contexto del Espacio de Datos para las Infraestructuras Urbanas Inteligentes ([EDINT](https://edint.es)).

![Logos](EDINT_UE_V-Color.png)