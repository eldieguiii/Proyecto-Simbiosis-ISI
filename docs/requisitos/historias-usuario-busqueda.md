# Historias de usuario de búsqueda

| Campo | Valor |
| --- | --- |
| Proyecto | Proyecto Simbiosis |
| Fecha | 29/10/2026 |
| Versión | 2 |
| Estado | Borrador |

## Fuentes comunes

- [Acta de UC-21 Buscar recetas](../captura/acta-acuerdos-uc-21-buscar-recetas.md), v1.1, Vigente.
- [Catálogo de requisitos](catalogo-requisitos.md), UR-08 y FR pertinentes.
- [Modelo de casos de uso](../modelos/modelo-casos-de-uso.md), UC-21.

## Épica de búsqueda

Como cliente, quiero poder realizar una búsqueda avanzada, para encontrar las recetas que cumplan ciertos criterios.

**Estado:** descompuesta en US-01, US-02 y US-03. Conserva la necesidad conjunta.

## Justificación de la división

# ---

## US-01

**Título:** Buscar mediante una palabra o frase.

Como cliente, quiero buscar una receta mediante palabra o frase, para poder encontrar recetas fácilmente.

**Fuentes:** UR-08; UC-21; [FR principal]; acta, [apartado pertinente].

### Criterios de aceptación

- **CA-01.** Dada una palabra o frase específica, cuando realice la búsqueda, entonces se mostrarán las recetas que contengan la palabra o frase en su título o descripción.
- **CA-02.** Dada una palabra o frase no presentes en ninguna receta, cuando se realice la búsqueda, entonces se indica que no hay resultados para esa búsqueda.
- **CA-03.** Dada una palabra o frase en la que faltan tildes o mayúsculas necesarias, cuando se realice la búsqueda, entonces se buscarán las recetas correspondientes sin tener en cuenta la falta de tilde o mayúscula.

## US-02

**Título:** Buscar por ingredientes incluídos.

Como cliente, quiero buscar una receta por sus ingredientes incluidos, para poder encontrar recetas con mayor precisión.

**Fuentes:** UR-08; UC-21; [FR principal]; acta, [apartado pertinente].

### Criterios de aceptación

- **CA-01.** Dada una selección de ingredientes, cuando se realice la búsqueda, entonces se mostrarán aquellas recetas que incluyan todos los ingredientes concretados.
- **CA-02.** Dada una combinación de ingredientes que ninguna receta contiene, cuando se realice la búsqueda, entonces se indica que no hay resultados para esa búsqueda.
- **CA-03.** Dado que se seleccione un mismo ingrediente como incluido y excluido, cuando se realice la búsqueda, entonces no se ejecuta la búsqueda hasta que se arregle el error.

## US-03

**Título:** Excluír ingredientes.

Como cliente, quiero buscar una receta por sus ingredientes excluidos, para poder encontrar recetas con mayor precisión.

**Fuentes:** UR-08; UC-21; [FR principal]; acta, [apartado pertinente].

### Criterios de aceptación

- **CA-01.** Dada una combinación de ingredientes excluidos válida, cuando se realice la búsqueda, entonces se mostrarán aquellas recetas que no incluyan ningún ingrediente excluido.
- **CA-02.** Dada una combinación de ingredientes excluidos que no se corresponda a ninguna receta, cuando se realice la búsqueda, entonces se indica que no hay resultados para esa búsqueda.
- **CA-03.** Dado que se seleccioneun mismo ingrediente como incluido y excluido, cuando se realice la búsqueda, entonces no se ejecuta la búsqueda hasta que se arregle el error.

## Revisión INVEST

La revisión abarca US-01, US-02 y US-03. «Aplicado» indica si se ha realizado la comprobación. «Cumple» indica si todas las historias cumplen el criterio. Si alguna no lo cumple, indicar «No» e identificar la historia y el motivo en la justificación. Si no se ha realizado la comprobación o faltan datos, indicar «Pendiente» en «Cumple».

| Criterio | Pregunta de revisión | Aplicado | Cumple | Justificación |
| --- | --- | --- | --- | --- |
| Independiente | ¿Puede implementarse cada historia y ofrecer un resultado útil sin implementar antes las otras historias del conjunto? Puede compartir infraestructura con ellas. | Sí | Sí | [Historias y motivo] |
| Negociable | ¿Cada historia explica qué necesita la persona y deja margen para discutir los detalles de la solución, respetando los acuerdos confirmados? | Sí | Sí | [Historias y motivo] |
| Valiosa | ¿La parte «para…» de cada historia explica el beneficio que obtiene la persona al usar esa capacidad? | Sí | Sí | [Historias y motivo] |
| Estimable | ¿Están claros el alcance y los datos necesarios para estimar el trabajo de cada historia? | Sí | Sí | [Historias y motivo] |
| Pequeña | ¿Se centra cada historia en una única capacidad de alcance manejable? | Sí | Sí | [Historias y motivo] |
| Comprobable | ¿Los criterios de aceptación de cada historia describen acciones y resultados observables que permiten distinguir un comportamiento correcto de uno incorrecto? | Sí | Sí | [Historias y motivo] |

## Dudas pendientes

Ninguna
