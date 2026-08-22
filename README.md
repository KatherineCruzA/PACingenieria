# Resumen Ejecutivo PAC — Proyecto 375 PTAP-MAN

**🔗 Ver el dashboard en vivo:** https://katherinecruza.github.io/PACingenieria/

Tablero de control para el seguimiento semanal de ingeniería del proyecto **375 PTAP-MAN**
(planta de tratamiento de agua potable), ejecutado por **Schrader Camargo S.A.S.** en
consorcio con **Consorcio Manantiales**, para **EPM**.

![Vista del dashboard](dashboard-interactivo/screenshots/preview-actual.png)

## ¿Qué es esto?

Un tablero ejecutivo que traduce el seguimiento semanal del **Last Planner System (LPS)**
—la metodología con la que el equipo de ingeniería planea y revisa su propio avance cada
semana— en indicadores claros para dirección de proyecto:

- **PAC (Porcentaje de Actividades Cumplidas / PPC):** de todo lo que cada disciplina se
  comprometió a hacer en una semana, ¿cuánto realmente se cumplió a tiempo?
- **CNC (Causas de No Cumplimiento):** cuando algo no se cumple, ¿por qué? (falta de
  prioridad, de recursos, de definiciones, cambios de alcance, etc.)
- **Tendencia semana a semana** por especialidad — Civil, Eléctrica, Hidráulica,
  Mecánica, Instrumentación (ICO) y Procesos — comparada contra la meta del 80%.
- **Plan semanal**: qué se hizo la semana pasada, qué se está haciendo esta semana, y qué
  viene programado la próxima, actividad por actividad, con responsable y estado.

La idea es que cualquier persona del equipo o del cliente pueda abrir un link y entender
en 30 segundos cómo va la ingeniería del proyecto, sin tener que abrir el Excel del LPS.

## Qué se puede hacer en el tablero

- Cambiar la ventana de análisis (1, 2, 3 o 6 meses) para ver más o menos historial.
- Filtrar por una sola especialidad haciendo clic en su nombre.
- Ver, para cada semana (pasada / en curso / próxima), el detalle de cada actividad
  planeada: descripción, responsable y si se cumplió — con secciones que se pueden
  contraer o expandir.
- Exportar la vista actual a PDF para un comité o informe.

## De dónde salen los datos

Los números se calculan directamente de las hojas semanales de programación
(**`PCP {Disciplina}`**) del archivo Excel del Last Planner System del proyecto, tarea por
tarea — no de hojas resumen previamente calculadas, que en este archivo se encontraron
desactualizadas o con fórmulas rotas. Esa metodología de extracción (y los problemas ya
identificados y corregidos en el camino) queda documentada en [`docs/SKILL.md`](docs/SKILL.md)
para quien continúe actualizando este tablero.

## Estructura del repositorio

```
index.html                       ← el dashboard (esto es lo que ves en el link de arriba)
dashboard-interactivo/           ← misma copia del dashboard + los datos y Excel fuente
docs/SKILL.md                    ← metodología de extracción y notas técnicas
```

## Aviso

Este repositorio se publicó con autorización de Schrader Camargo S.A.S. e incluye datos
reales del proyecto (nombres de responsables y avances de obra).

---
*Construido con [Claude](https://claude.ai) (Anthropic), como Claude Design Component.*
