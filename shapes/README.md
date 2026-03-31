# Formas SHACL

Esta carpeta contiene las **formas SHACL (Shapes Constraint Language)** asociadas a la ontología.  
Estas formas se utilizan para **validar datos RDF** y asegurar que los datos de instancias se ajusten a la estructura, restricciones y semántica de la ontología.

# Propósito
El objetivo de este directorio es almacenar las **reglas de validación y restricciones** definidas para la ontología.  
Las formas SHACL ayudan a verificar que los datos que utilizan la ontología sigan el modelo previsto comprobando la pertenencia a clases, rangos de propiedades, cardinalidades y otras condiciones estructurales.

# Contenido
Incluye aquí cualquier archivo que defina formas SHACL, como:

- `.ttl` — Formas SHACL escritas en sintaxis Turtle  
- `.rdf` — Formas SHACL en formato RDF/XML  
- `.jsonld` — Formas SHACL en formato JSON-LD  

También puedes incluir documentación de apoyo que explique la lógica de validación o las instrucciones de uso.

# Mejores prácticas
- Mantén las formas SHACL **consistentes** con la última versión de la ontología.  
- Valida regularmente todos los conjuntos de datos de ejemplo (almacenados en `/examples/`) contra estas formas.  
- Documenta el propósito y alcance de cada forma (por ejemplo, a nivel de clase, de propiedad, de conjunto de datos).  
- Utiliza un diseño modular si tu ontología incluye múltiples dominios o módulos (por ejemplo, `/shapes/core/`, `/shapes/extensions/`).

# Notas
- Esta carpeta es solo para **definiciones de validación y restricciones** — no para la implementación de la ontología o datos de ejemplo.  
- Considera mantener un registro de cambios para rastrear las actualizaciones de las reglas SHACL.
