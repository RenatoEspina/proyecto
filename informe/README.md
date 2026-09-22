# Informe 2 — UML · Caso BeeTracer (ICI-3242)

Documento principal: **[`INFORME-2-UML.md`](INFORME-2-UML.md)**

## Estructura

```
informe/
├── INFORME-2-UML.md          ← el informe completo
├── README.md                 ← este archivo
└── diagramas/
    ├── *.png                 ← imágenes referenciadas por el informe
    ├── svg/*.svg             ← versiones vectoriales (lectura en detalle)
    └── fuente/*.puml         ← código fuente PlantUML de cada diagrama
```

## Cobertura respecto de la pauta

| Sección de la pauta | Puntaje | Estado |
|---|---|---|
| 1. Introducción | — | ✅ Completa |
| 2. Definición del problema | — | ✅ Completa |
| 3. Descripción general | — | ✅ Completa |
| 4. Clientes y usuarios | — | ✅ Completa |
| 5. Funciones del sistema (alto nivel) | **1,25** | ✅ Completa (8 grupos, 55 funciones + atributos del sistema) |
| 6. Diagrama de Casos de Uso | **1,25** | ✅ 2 diagramas gráficos + 22 narrativos de alto nivel + **6 expandidos**. Quedan plantillas para los restantes |
| 7. Diagrama de Secuencia y Colaboración | **1,25** | ✅ 4 de secuencia + 2 de colaboración. Quedan 6 casos de uso por modelar (listados en 7.3) |
| 8. Diagrama de Clases (de Diseño) | **1,25** | ✅ Completo (29 clases en 5 paquetes) |
| 9. Diccionario de Clases | — | ✅ Completo |
| 10. Conclusiones | — | ⚠️ Borrador redactado; **personalizar con la experiencia del equipo** |
| 11. Referencias bibliográficas | **1,0** | ⚠️ Bibliografía metodológica completa; faltan URL y fechas exactas de las fuentes del caso |

## Pendientes

Todos los puntos por completar están marcados dentro del informe con **🔲 [POR COMPLETAR]**
(12 marcas). Los principales:

1. **Datos de portada** — integrantes, profesor, sección, fecha de entrega.
2. **Conclusiones personales** — dificultades del modelado y aprendizaje del equipo (sección 10).
3. **Referencias del caso** — URL del sitio de BeeTracer, fecha y expositor de la charla,
   y al menos una fuente formal del dominio logístico (sección 11).
4. *(Opcional)* Expandir CU-11 y CU-14, y modelar las interacciones faltantes (secciones 6.5 y 7.3).

## Regenerar los diagramas

```bash
sudo apt-get install -y plantuml graphviz
cd informe/diagramas
plantuml -charset UTF-8 -tpng -o .. fuente/*.puml
plantuml -charset UTF-8 -tsvg -o ../svg fuente/*.puml
```

## Fuentes utilizadas

Todo el contenido se construyó a partir de los documentos de `material de apoyo/`:

- `Resumen Charla - Beetracer.pdf` — fuente principal del flujo operativo y los desafíos técnicos
- `Bases Charla Beetracer.pdf` — actores, arquitectura y fases del proceso
- `BeeTracer_ el negocio detrás del sistema.pdf` — contexto logístico de importación
- `CONTROL-2-IngenieriaInversa-TrabajoDeTitulo-PUCV.pdf` — sitio web público de BeeTracer
- `BeeTracer_Pitch.pdf` — módulos del sistema y encuadre del trabajo
- `PAUTA INFORME 2 - UML.pdf` — estructura y puntajes del informe
