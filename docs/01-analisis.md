# 01 · Análisis y documentación inicial (RA1)

> **Plantilla.** Se entrega como **H1 el 26-nov-2026**. Cada apartado indica el criterio de evaluación (CE) que evidencia y qué se espera. Borra las notas en cursiva al rellenar.

## 1. Sector y empresas (CE 1a, 1b)
Tenno Helper es una aplicacion web relacionada al videojuego warframe siendo una herramienta complementaria pra dicho videojuego ofreciendo informacion y funcionalidades de gestion y ayuda a los jugadores.

En este paso dentro de warframe existe una comunidad que desarrolla y mantiene diferentes herramientas independientes.

Dentro del sector encontramos diferentes empresas/proyectos como:

|Empresa o Proyecto | Caracteristicas organizativas | Porducto o servicio|
|Digital Extremes| Empresa desarrolladora de videojuegos| Warframe, Warframe companion|
|Overframe|Proyecto comunitario especializado en warframe|Creacion, consulta, y publicaciond e builds|
|Warframe market| Plataforma comunitaria orientada al comercio entre jugadores| Consulta de precios y ofertas de comercio|
|AlecaFrame|Aplicacion independiente integrada en Overwolf| Gestion de inventario, seguimiento de fabricacion, reliquias y estadisticas|

ornanigrama:
flowchart TD
    A["DIRECCIÓN GENERAL<br/>Planificación, coordinación y toma de decisiones"]

    A --> B["DEPARTAMENTO DE DESARROLLO"]
    A --> C["DEPARTAMENTO DE DISEÑO UX/UI"]
    A --> D["DEPARTAMENTO DE SISTEMAS"]
    A --> E["DEPARTAMENTO DE DOCUMENTACIÓN"]
    A --> F["DEPARTAMENTO DE ADMINISTRACIÓN"]

    B --> B1["Desarrollo frontend<br/>HTML, CSS y JavaScript"]
    B --> B2["Desarrollo backend<br/>PHP y lógica del servidor"]
    B --> B3["Bases de datos y APIs<br/>Gestión e integración de datos"]

    C --> C1["Diseño de interfaces<br/>Apariencia visual"]
    C --> C2["Experiencia de usuario<br/>Usabilidad y accesibilidad"]

    D --> D1["Despliegue<br/>Servidores y alojamiento"]
    D --> D2["Mantenimiento y seguridad<br/>Copias de seguridad y actualizaciones"]

    E --> E1["Recopilación de información<br/>Fuentes y documentación"]
    E --> E2["Actualización de datos<br/>Verificación y fiabilidad"]

    F --> F1["Gestión económica<br/>Presupuestos y gastos"]
    F --> F2["Gestión administrativa<br/>Facturas y obligaciones legales"]

    classDef direccion fill:#264653,color:#fff,stroke:#1d3540
    classDef departamento fill:#287271,color:#fff,stroke:#1d5554
    classDef funciones fill:#e9f1f0,color:#222,stroke:#8aaba5

    class A direccion
    class B,C,D,E,F departamento
    class B1,B2,B3,C1,C2,D1,D2,E1,E2,F1,F2 funciones


## 2. Necesidades y oportunidades (CE 1c, 1d)

*Lista **priorizada** de las necesidades más demandadas, con el criterio de priorización y la fuente. Valora las oportunidades de negocio con **al menos un dato cuantitativo** y su fuente.*

| Prioridad | Necesidad | Fuente |
||||
## 3. Tipo de proyecto elegido (CE 1e)

*Qué proyecto das como respuesta y por qué, frente a otras alternativas.*

## 4. Requisitos y restricciones (CE 1f)

*Características que debe cumplir el proyecto, redactadas de forma **verificable** (no «debe ser rápido», sino «responde en menos de 2 s»). Parte de lo que has encontrado en [`01b-sota.md`](01b-sota.md).*

> **Guía.** Numera los requisitos **funcionales** como **RF-01, RF-02…** (qué hace el sistema) y los **no funcionales** como **RNF-01…** (cómo lo hace: rendimiento, seguridad, usabilidad, disponibilidad, accesibilidad). Las **restricciones** (plazo, presupuesto, tecnología obligatoria, normativa) como **REST-01…**. Cada requisito debe tener **una medida o una prueba**. Si aún no sabes cómo lo probarás, escribe «pendiente» y complétalo antes de H3.

| ID | Requisito | Tipo (funcional / no funcional / restricción) | Cómo se verifica |
|---|---|---|---|
| RF-01 | [RELLENAR] | funcional | |
| RNF-01 | [RELLENAR] | no funcional | |
| REST-01 | [RELLENAR] | restricción | |

### Matriz de trazabilidad

*Une cada objetivo con sus requisitos, y estos con lo que los implementa y los comprueba. Se rellena por completo al final del proyecto; en H1 basta con **objetivo y requisito**.*

> **Guía.** Ejemplo ficticio: *OBJ-01 Gestionar citas → RF-02 Crear una cita → CU-03 → `POST /citas` → prueba P-07.* Cada RF y cada RNF de la tabla anterior debe aparecer aquí.

| Objetivo | Requisito | Caso de uso | Pantalla o endpoint | Prueba o indicador |
|---|---|---|---|---|
| OBJ-01 [RELLENAR] | RF-01 | | | pendiente |

## 5. Obligaciones fiscales, laborales y de prevención (CE 1g)

*Las obligaciones que aplican a tu proyecto, **con su norma** y sus condiciones.*

## 6. Ayudas y subvenciones (CE 1h)

*Al menos **una** ayuda real: fuente, requisitos y plazo.*

## 7. Guion de trabajo (CE 1i)

*Fases, hitos y responsables del proyecto. Puede enlazar al tablero de GitHub Projects.*

## 8. Glosario

*Una cosa, un nombre: define los términos del dominio y de tu proyecto, y anota los sinónimos que **no** vas a usar en ningún documento. Con **5 términos** basta; crece con el proyecto.*

| Término | Definición | Sinónimos que NO uso |
|---|---|---|
| [RELLENAR] | | |

---

## Criterios de evaluación de este documento (RA1, texto literal)

- **1a)** Se han clasificado las empresas del sector por sus características organizativas y el tipo de producto o servicio que ofrecen.
- **1b)** Se han caracterizado las empresas tipo indicando la estructura organizativa y las funciones de cada departamento.
- **1c)** Se han identificado las necesidades más demandadas a las empresas.
- **1d)** Se han valorado las oportunidades de negocio previsibles en el sector.
- **1e)** Se ha identificado el tipo de proyecto requerido para dar respuesta a las demandas previstas.
- **1f)** Se han determinado las características específicas requeridas al proyecto.
- **1g)** Se han determinado las obligaciones fiscales, laborales y de prevención de riesgos y sus condiciones de aplicación.
- **1h)** Se han identificado posibles ayudas o subvenciones para la incorporación de nuevas tecnologías de producción o de servicio que se proponen.
- **1i)** Se ha elaborado el guión de trabajo que se va a seguir para la elaboración del proyecto.
