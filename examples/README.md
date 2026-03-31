# Pruebas de la ontología

Esta carpeta contiene todas las **pruebas diseñadas para verificar que la ontología cumple con sus requisitos definidos**.  
Estas pruebas aseguran que la ontología representa correctamente el conocimiento previsto, satisface las preguntas de competencia y se alinea con las necesidades del dominio y los interesados.

# Propósito
El objetivo de este directorio es almacenar **artefactos de validación y verificación** que confirmen que la ontología se comporta como se espera.  
Las pruebas ayudan a garantizar la **calidad, consistencia y completitud** de la ontología con respecto a sus requisitos.

# Contenido
Incluye aquí cualquier archivo o script utilizado para probar la ontología, como:

- **Pruebas Themis** — Pruebas automatizadas escritas en [Themis](https://themis.linkeddata.es/).
- **Consultas SPARQL** — Para comprobar que las preguntas de competencia pueden ser respondidas utilizando la ontología.  
- **Informes de validación SHACL** — Para verificar que los datos se ajustan a las restricciones de la ontología.  
- **Scripts de prueba automatizados** — Implementados en Python, Java u otros lenguajes para ejecutar comprobaciones de ontología.  
- **Conjuntos de datos de prueba** — Archivos RDF o Turtle utilizados como entrada para validación.  
- **Informes de prueba** — Documentos que resumen los resultados de las pruebas de ontología.

# Formatos aceptados
Puedes utilizar formatos como:
- `.rq` — Archivos de consulta SPARQL  
- `.py`, `.sh`, `.ipynb` — Scripts de prueba automatizados  
- `.ttl`, `.rdf`, `.jsonld` — Datos de ejemplo para pruebas  
- `.md`, `.pdf` — Informes o documentación de resultados de pruebas  

# Mejores prácticas
- Alinea cada prueba con un **requisito específico o pregunta de competencia**.  
- Mantén los archivos de prueba **versionados** junto con las actualizaciones de la ontología.  
- Automatiza las pruebas cuando sea posible (por ejemplo, GitHub Actions o flujos de trabajo CI).  
- Documenta los resultados esperados de cada prueba para garantizar la reproducibilidad.  
- Almacena los datos de prueba por separado de los datos de producción o ejemplo.

# Notas
- Esta carpeta es solo para **validación de requisitos y pruebas de ontología** — no para archivos de implementación o formas SHACL en sí mismas.  
- Considera organizar subcarpetas, por ejemplo:
  - `/preguntas-competencia/`  
  - `/pruebas-automatizadas/`  
  - `/informes/`
