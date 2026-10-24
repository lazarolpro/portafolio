# Portafolio — 9 capacidades con evidencia online

> Mantenimiento electromecánico y soporte técnico. Convierto datos de campo en
> decisiones: diagnostico fallas por causa raíz, integro equipos y sistemas,
> automatizo procesos, prototipo firmware, valido con metrología, cuantifico
> eficiencia energética, controlo clima con IoT, diseño enlaces de radio y asisto
> con IA local — todo con demos reproducibles.

> © 2026 Ronny L. Díaz López. **Todos los derechos reservados.** El código fuente,
> los datos de detalle y los informes completos son propiedad del autor y no se
> publican. Prohibida su venta o uso comercial sin autorización escrita. Ver
> [`LICENSE`](LICENSE).

Este repositorio es el índice. Cada capacidad vive en su propio repo y se
ejecuta sin instalar nada más que Python 3.

## Las nueve capacidades

| # | Capacidad | Repo | Qué demuestra |
| --- | --- | --- | --- |
| 1 | Diagnóstico y soporte técnico | [rca-telemetria](https://github.com/lazarolpro/rca-telemetria) | Causa raíz sobre telemetría |
| 2 | Ingeniería de aplicación | [gateway-industrial](https://github.com/lazarolpro/gateway-industrial) | Integración equipo → API REST |
| 3 | Automatización de datos | [etl-produccion](https://github.com/lazarolpro/etl-produccion) | Limpieza + KPIs + informe |
| 4 | I+D y prototipado | [nodo-sensor-esp32](https://github.com/lazarolpro/nodo-sensor-esp32) | Firmware + simulación online |
| 5 | Validación y metrología | [banco-validacion-metrologia](https://github.com/lazarolpro/banco-validacion-metrologia) | Conformidad + incertidumbre |
| 6 | Eficiencia energética | [auditoria-energetica](https://github.com/lazarolpro/auditoria-energetica) | KPIs + ahorro estimado |
| 7 | Control climático e IoT | [invernadero-ecosmart](https://github.com/lazarolpro/invernadero-ecosmart) | Gemelo digital + control difuso |
| 8 | Radiocomunicaciones | [radioenlace-backtoback](https://github.com/lazarolpro/radioenlace-backtoback) | Presupuesto de enlace de radio |
| 9 | Asistente IA local | [proyectia-asistente](https://github.com/lazarolpro/proyectia-asistente) | Recuperación aumentada (RAG) local |

## Cómo ejecutar todo

Cada proyecto es independiente y usa solo la biblioteca estándar de Python 3.

```bash
git clone https://github.com/lazarolpro/rca-telemetria && cd rca-telemetria && python rca.py --demo && python -m pytest -q
git clone https://github.com/lazarolpro/gateway-industrial && cd gateway-industrial && python gateway.py --demo && python -m pytest -q
git clone https://github.com/lazarolpro/etl-produccion && cd etl-produccion && python etl_report.py --demo && python -m pytest -q
git clone https://github.com/lazarolpro/nodo-sensor-esp32 && cd nodo-sensor-esp32 && python sim/sensor_sim.py --sweep
git clone https://github.com/lazarolpro/banco-validacion-metrologia && cd banco-validacion-metrologia && python validate.py --demo && python -m pytest -q
git clone https://github.com/lazarolpro/auditoria-energetica && cd auditoria-energetica && python energy_audit.py --demo && python -m pytest -q
git clone https://github.com/lazarolpro/invernadero-ecosmart && cd invernadero-ecosmart && python demo.py --demo && python -m pytest -q
git clone https://github.com/lazarolpro/radioenlace-backtoback && cd radioenlace-backtoback && python radioenlace.py --demo && python -m pytest -q
git clone https://github.com/lazarolpro/proyectia-asistente && cd proyectia-asistente && python asistente.py --demo && python -m pytest -q
```

## Criterio de cada repo

- El comando del README corre sin instalar dependencias.
- Hay al menos una salida de evidencia versionada (`report.md`, SVG, JSON).
- Los tests pasan (`python -m pytest -q`).
- CI en verde con GitHub Actions.

## Licencia

© Ronny L. Díaz López, 2026. Todos los derechos reservados. Prohibida la venta o
el uso comercial sin autorización escrita del autor. Contacto:
ronnynations21@gmail.com
