# Historias de usuario de búsqueda

| Campo | Valor |
| Nombre: | Sabela Moares Torrado |
| Grupo: | A_3 |
| Proyecto | Proyecto Simbiosis |
| Fecha | 27/10/2026 |
| Versión | 1 |
| Estado | Borrador |

## Fuentes comunes

- [Acta de UC-21 Buscar recetas](../captura/acta-acuerdos-uc-21-buscar-recetas.md), v1.1, Vigente.
- [Catálogo de requisitos](catalogo-requisitos.md), UR-08 y FR pertinentes.
- [Modelo de casos de uso](../modelos/modelo-casos-de-uso.md), UC-21.

## Épica de búsqueda

Como persona usiaria registrada, quiero buscar recetas utilizando palabras clave, selección de ingredientes obligatorios e ingredientes a excluir, para localizar de forma eficiente y ajustada a mis necesidades las recetas publicadas que deseo consultar..

**Estado:** descompuesta en US-01, US-02 y US-03. Conserva la necesidad conjunta.

## Justificación de la división

Esta épica reúne las tres necesidades de búsqueda del caso de uso UC-21. Se divide en 3 historias independientes US-01, US-02 y US-03.

## US-01

**Título:** Búsqueda mediante palabra o frase

Como usuario registrado , quiero buscar recetas con tan solo un apalabra o frase, para encontrar recetas con el texto introducido.

**Fuentes:** UR-08; UC-21; FR-085; acta, sección 2.

### Criterios de aceptación

- **CA-01.** Dado existencia de una recete: "Tarta de fresas", cuando la persona busque "Tarta de fresas", entonces la receta aparecerá en los resultados ordenados por fecha de publicación.
- **CA-02.** Dado que ninguna receta cumpla los criterios de la búsqueda y admita una corrección ortográfica, cuando se realiza la consulta, entonces el sistema propone la corrección separada de los resultados.
- **CA-03.** Dado que la persona usuaria está situada en la búsqueda, cuando esta no introduzca nada , entonces el sistema solicita un criterio y la búsqueda no se ejecuta.

## US-02

**Título:** Búsqueda por ingredientes incluidos

Como usuario registrado, quiero buscar recetas por ingredientes incluidos, para encontrar recetas con los ingredientes que quiero usar.

**Fuentes:** UR-08; UC-21; FR-086; acta, sección 2.

### Criterios de aceptación

- **CA-01.** Dado que l apersona seleccione los ingredientes "Huevo" y "Patata", cuando realiza la búsqueda, entonces el sistema muestra todas las recetas que contienen esos ingredientes.
- **CA-02.** Dado que se combine el nombre de una receta y un ingrediente de esta , cuando se realiza la búsqueda, entonces la receta debe cumplir con ambos criterios indicados.
- **CA-03.** Dado usuario selecciona resultados y mira una receta, cuando vuelve a los resultados, entonces se conserva la última búsqueda y su criterio.

## US-03

**Título:** Excluir ingredientes

Como usuario registrado, quiero excluir ingredientes de la búsqueda, para que ninguna receta contenga ingredientes descartados.

**Fuentes:** UR-08; UC-21; FR-085; acta, sección 2.

### Criterios de aceptación

- **CA-01.** Dado que el usuario selecciona un ingrediente para excluirlo, cuando realiza la búsqueda, entonces ninguna receta de los resultados contiene dicho ingrediente.
- **CA-02.** Dado selecciona el mismo ingrediente para incluirlo y para excluirlo, cuando se intente realizar la búsqueda, entonces el sistema señala el conflicto y no ejecuta la búsqueda.
- **CA-03.** Dado que la búsqueda no arroje resultados, cuando  el sistema ofrece alternativas, entonces las sugerencias conservan los ingredientes excluidos.

## Revisión INVEST

La revisión abarca US-01, US-02 y US-03. «Aplicado» indica si se ha realizado la comprobación. «Cumple» indica si todas las historias cumplen el criterio. Si alguna no lo cumple, indicar «No» e identificar la historia y el motivo en la justificación. Si no se ha realizado la comprobación o faltan datos, indicar «Pendiente» en «Cumple».

| Criterio | Pregunta de revisión | Aplicado | Cumple | Justificación |
| --- | --- | --- | --- | --- |
| Independiente | ¿Puede implementarse cada historia y ofrecer un resultado útil sin implementar antes las otras historias del conjunto? Puede compartir infraestructura con ellas. | Sí | Sí | US-01, US-02 y US-03 ya que las capacidades de búsqueda en cada una de ellas es distinta |
| Negociable | ¿Cada historia explica qué necesita la persona y deja margen para discutir los detalles de la solución, respetando los acuerdos confirmados? | Sí | Sí | Describen las necesidades de la usuaria |
| Valiosa | ¿La parte «para…» de cada historia explica el beneficio que obtiene la persona al usar esa capacidad? | Sí | Sí | La historias incluyen el beneficio directo y el valor aportado en la cláusula para |
| Estimable | ¿Están claros el alcance y los datos necesarios para estimar el trabajo de cada historia? | Sí | Sí | Se acota con precisión el detalle técnico de cada historia |
| Pequeña | ¿Se centra cada historia en una única capacidad de alcance manejable? | Sí | Sí | Cada historia tiene una faceta de búsqueda |
| Comprobable | ¿Los criterios de aceptación de cada historia describen acciones y resultados observables que permiten distinguir un comportamiento correcto de uno incorrecto? | Sí | Sí | Todos siguen la misma estructura (Dado, cuando, entonces) |

## Dudas pendientes

«Ninguna»
