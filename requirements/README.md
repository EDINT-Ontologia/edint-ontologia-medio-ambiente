# Requisitos de la ontología

Esta carpeta contiene todos los **requisitos y materiales de apoyo** utilizados durante el desarrollo de la ontología.

# Propósito
El objetivo de este directorio es almacenar y organizar la **información fundamental** que guía el diseño y la implementación de la ontología.  
Estos requisitos definen **qué debe representar la ontología**, **por qué se está desarrollando** y **cómo debe soportar los casos de uso previstos**.

# Contenido
Incluye aquí cualquier documento o recurso que describa o justifique los requisitos de la ontología, como:

- **Preguntas de competencia** — Preguntas que la ontología debe ser capaz de responder.  
- **Casos de uso y escenarios** — Descripciones de contextos del mundo real donde se aplicará la ontología.  
- **Requisitos de dominio** — Listas de conceptos clave, relaciones o restricciones recopiladas de expertos.  
- **Requisitos de los interesados** — Necesidades funcionales y no funcionales de usuarios u organizaciones.  

# Formatos aceptados
Puedes utilizar los siguientes formatos:
- `.md` — Documentos Markdown  
- `.docx` / `.pdf` — Documentos formales de requisitos  
- `.csv` / `.xlsx` — Listas de requisitos o matrices de trazabilidad  
- `.txt` — Notas o borradores preliminares de requisitos  

# Mejores prácticas
- Mantén los requisitos **trazables** — vincula cada uno con elementos de la ontología (clases, propiedades, etc. Véase la plantilla).  
- Mantén el historial de versiones a medida que evolucionan los requisitos.  
- Asegura la consistencia entre los requisitos, los diagramas de conceptualización y la implementación.  
- Revisa y valida los requisitos con expertos de dominio antes de que comience el desarrollo de la ontología. La [metodología LOT](https://doi.org/10.1016/j.engappai.2022.104755) propone algunas pautas:
  - Un conjunto de requisitos es correcto si cada requisito se refiere a algunas características de la ontología a desarrollar.
  - Un conjunto de requisitos es completo si los usuarios y expertos de dominio revisan los requisitos y confirman que no son conscientes de requisitos adicionales.
  - Un conjunto de requisitos es internamente consistente si no existen conflictos entre ellos.
  - Un conjunto de requisitos es verificable si existe un proceso finito con un costo razonable que comprueba si la ontología final satisface cada requisito.
  - Un conjunto de requisitos es comprensible si cada uno de los requisitos es comprensible para usuarios y expertos de dominio.
  - Un conjunto de requisitos es no ambiguo si cada uno de los requisitos tiene solo una interpretación posible; es decir, si no admite ninguna duda o malentendido.
  - Un conjunto de requisitos es conciso si cada uno de los requisitos es relevante, y no existen requisitos duplicados o irrelevantes.


# Notas
- Esta carpeta está destinada solo para **documentación de requisitos** — no para diagramas de ontología o archivos de implementación.  
- Utiliza subcarpetas si es necesario (por ejemplo, `/preguntas-competencia/`, `/casos-uso/`, `/trazabilidad/`).
