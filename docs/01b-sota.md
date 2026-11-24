# 01b · Estado del arte (SOTA) de mi proyecto

> **Plantilla.** Se entrega con **H1 el 26-nov-2026**, junto al `01-analisis.md`. Es **obligatorio** y breve: **4-6 páginas**. Aquí estudias qué soluciones, **modelos de negocio** y **herramientas** existen ya para el problema que has elegido, y justificas tus decisiones con ello. Cada apartado indica el criterio de evaluación (CE) que alimenta. Borra los bloques «Guía» al rellenar.

> **Guía.** Calendario: **12-nov** preguntas de búsqueda (apartado 1) · **19-nov** tablas de soluciones y herramientas (apartados 2 y 4) · **26-nov** modelos de negocio, hueco, decisiones, fuentes y entrega (apartados 3, 5-8).
>
> **Reglas.**
>
> - Solo cuenta lo que tiene **enlace y fecha de acceso**.
> - Si usas IA para buscar, **abre cada fuente** y comprueba que existe y dice lo que te cuenta la IA. Puede inventar productos, precios o referencias. Decláralo en [`declaracion-uso-ia.md`](declaracion-uso-ia.md).
> - Usa **solo información pública** de las soluciones que estudias. **Nada** de la empresa de prácticas ni de clientes reales.
> - Compara herramientas con **los mismos criterios**, no por opinión. Salvo razón argumentada, prefiere lo que has visto en el ciclo (Java 21, Spring Boot, SQL).
> - Si algo no lo has podido comprobar, dilo en el apartado 8.

## 1. Problema y preguntas de búsqueda (CE 1c)

**Problema:**  Los jugadores de Warframe necesitan utilizar diferentes herramientas y páginas web para consultar información del juego, gestionar su inventario, conocer cómo conseguir objetos y organizar sus configuraciones, ya que estas funcionalidades se encuentran repartidas entre distintas plataformas.

| # | Pregunta | Dónde busqué | Fecha |
|---|---|---|---|
| P1 | ¿Qué aplicaciones y herramientas existen actualmente para ayudar a los jugadores de Warframe?  | Google, páginas oficiales de las herramientas y tiendas de aplicaciones | 19/11/2026 |
| P2 | ¿Qué funcionalidades ofrecen y qué necesidades de los jugadores cubren?  | Warframe Wiki, Overframe, AlecaFrame y Warframe Companion | 19/11/2026 |
| P3 | ¿Qué tecnologías y fuentes de datos pueden utilizarse para desarrollar una aplicación complementaria?  | Documentación oficial de PHP, MySQL y recursos de Warframe | 19/11/2026 |

## 2. Soluciones existentes (CE 1a, 1c, 2a)

| Solución | Para quién | Qué hace | Modelo de precio | Enlace y fecha de acceso |
|---|---|---|---|---|
| Warframe Companion | Jugadores de warframe | Aplicación oficial que permite consultar alertas, invasiones, fisuras, gestionar extractores y fabricar objetos desde la fundición. | Gratuito | https://play.google.com/store/apps/details?id=com.digitalextremes.warframenexus&hl=es 19/11/2026 |
| Overframe | Jugadores interesados en optimizar sus equipamientos. | Permite crear, consultar y compartir builds de Warframes y armas. | Gratuito | https://overframe.gg/ 19/11/2026 |
| Warframe Market | Jugadores que comercian con otros usuarios. | Permite consultar precios y publicar ofertas de compra y venta de objetos. | Gratuito | https://warframe.market/ 19/11/2026 |
| AlecaFrame | Jugadores que quieren controlar su progreso e inventario. | Gestiona el inventario, muestra información de objetos, árboles de fabricación y seguimiento de progreso | Gratuito | https://alecaframe.com/ 19/11/2026 |
| Warframe Wiki | Jugadores que necesitan consultar información detallada. | Recopila información sobre objetos, misiones, personajes, recursos y formas de obtención. | Gartuito | https://wiki.warframe.com/ 19/11/2026 |

*Figura: comparativa de las soluciones (opcional, un cuadrante o un esquema).*

## 3. Modelos de negocio (CE 1d, 1e)

| Patrón | Soluciones que lo usan | Ventaja | Riesgo |
|---|---|---|---|
| Servicio gratuito | Warframe Companion, Warframe Wiki | Permite que cualquier jugador utilice la herramienta sin pagar. | Dependencia de financiación externa y recursos de mantenimiento. |
| Freemium y publicidad | AlecaFrame | Permite ofrecer funcionalidades gratuitas y obtener ingresos mediante publicidad o servicios adicionales. | La publicidad puede perjudicar la experiencia del usuario. |
| Comunidad y aportaciones | Overframe, Warframe Market y proyectos de código abierto | La comunidad participa en el desarrollo y mantenimiento de la plataforma. | Dependencia de los colaboradores y de la actividad de la comunidad. |

Warframe Companion: Es una herramienta oficial gratuita desarrollada por Digital Extremes. Su objetivo es complementar el videojuego y mantener a los jugadores conectados con sus funcionalidades incluso cuando no están jugando. Su mantenimiento depende de la propia empresa desarrolladora.

AlecaFrame: Ofrece gratuitamente funcionalidades de gestión del inventario y seguimiento del progreso. Su distribución mediante Overwolf permite utilizar el ecosistema de aplicaciones de esta plataforma y su modelo incluye publicidad.

WFHelper: Es una aplicación independiente de código abierto que ofrece funcionalidades de inventario, reliquias y precios de mercado. Su financiación se apoya en aportaciones voluntarias mediante Patreon.

**Modelo de negocio para Tenno Helper**

Tenno Helper seguirá un modelo de servicio gratuito y sin publicidad, el objetivo principal es desarrollar una herramienta útil para los jugadores de Warframe, que integre en una sola aplicacion web varias de las caracteristicas dispersas en diferentes aplicaciones web comunitarias y oficiales ya existentes.

## 4. Herramientas y tecnologías (CE 2a, 2b)

*Para cada decisión técnica importante (lenguaje y *framework*, base de datos, despliegue, autenticación…), compara **2-3 opciones con los mismos criterios**. Marca la que eliges.*

| Decisión | Opción | Madurez | Licencia | Coste | Curva de aprendizaje | Encaje con el ciclo | Elegida |
|---|---|---|---|---|---|---|---|


*Cada decisión importante se convierte en una decisión registrada en [`decisiones/`](decisiones/0000-plantilla.md).*

## 5. Hueco y diferenciación (CE 1e)

Las herramientas analizadas ofrecen funcionalidades útiles, pero muchas están especializadas en una única necesidad o presentan sus funciones repartidas entre diferentes apartados y plataformas. Aunque existen soluciones más completas, como AlecaFrame, WFHelper o Cephalon Kronos, algunas requieren instalación de escritorio o dependen de plataformas externas.

Propuesta de valor de Tenno Helper:

Tenno Helper pretende reunir en una única aplicación web las principales funcionalidades de consulta y gestión que necesitan los jugadores de Warframe. Permitirá consultar un catálogo de objetos, conocer sus fuentes y probabilidades de obtención, gestionar un inventario personal, realizar seguimiento de objetos pendientes y guardar builds. Su principal diferenciación será ofrecer estas funciones desde una misma plataforma accesible mediante el navegador, sin necesidad de instalar programas adicionales. No pretende superar a herramientas especializadas como Overframe en la creación avanzada de builds ni sustituir a las soluciones oficiales, sino ofrecer una alternativa integrada y sencilla.

## 6. Decisiones derivadas (CE 1e, 1f, 2b)

*Qué consecuencias tiene este estudio en tu proyecto.*

- **Tipo de proyecto elegido** (enlaza con el apartado 3 de [`01-analisis.md`](01-analisis.md#rf-03))
- **Requisitos que salen del estudio** (con su ID del apartado 4 de [`01-analisis.md`](01-analisis.md#rf-04)) 
- **Decisiones técnicas** (enlace a cada archivo de [`decisiones/`](../decisiones/0000-plantilla.md))

## 7. Fuentes y calidad (CE 2a)

*Al menos **2 fuentes independientes** (no dos páginas de la misma empresa). Datos oficiales o primarios antes que blogs.*

| # | Fuente (enlace) | Tipo | Fecha de acceso | Fiabilidad (alta / media / baja) y por qué |
|---|---|---|---|---|
| F1 | https://overframe.gg/ | Plataforma comunitaria | 19/11/2026 | Media-alta. Permite comprobar las funciones relacionadas con las builds. |
| F2 | https://warframe.market/ | 	Plataforma comunitaria | 19/11/2026 | Media-alta. Fuente directa para conocer sus funciones de comercio. |

## 8. Límites
- No se ha realizado una prueba exhaustiva de todas las herramientas, por lo que la comparación se basa principalmente en sus características documentadas.
- Las funcionalidades de las aplicaciones pueden cambiar con las actualizaciones de Warframe.
- La integración automática del inventario de Warframe no está contemplada debido a las restricciones de permisos de las paginas y aplicaciones web comunitarias estipuladas por Digital Extremes.

---

## Criterios de evaluación que alimenta este documento (texto literal)

- **1a)** Se han clasificado las empresas del sector por sus características organizativas y el tipo de producto o servicio que ofrecen.
- **1c)** Se han identificado las necesidades más demandadas a las empresas.
- **1d)** Se han valorado las oportunidades de negocio previsibles en el sector.
- **1e)** Se ha identificado el tipo de proyecto requerido para dar respuesta a las demandas previstas.
- **1f)** Se han determinado las características específicas requeridas al proyecto.
- **2a)** Se ha recopilado información relativa a los aspectos que van a ser tratados en el proyecto.
- **2b)** Se ha realizado el estudio de viabilidad técnica del mismo.

> El SOTA **no añade criterios de evaluación**: reúne en un solo sitio lo que 1a-1f y 2a-2b ya piden. La evaluación sigue las listas de cotejo de H1 y H2.
