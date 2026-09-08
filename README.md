# Minirreto 1: integración, entrega y despliegue continuos

En este minirreto observarás cómo una misma *pipeline* va automatizando cada vez más pasos del camino entre un cambio y una web publicada.

## Forma de trabajo

Todo el trabajo relacionado con GitHub se realiza desde la interfaz web de tu **fork** y directamente sobre la rama `main`. No necesitas clonar el repositorio ni conocer todavía los comandos de Git.

La progresión será:

1. **Integración continua:** validar el catálogo y ejecutar las pruebas.
2. **Entrega continua:** construir además el sitio y conservarlo como artefacto.
3. **Despliegue continuo:** desplegar automáticamente el sitio en Netlify.

Las tres versiones del workflow están en `workflow-templates/`. En cada tarea copiarás la plantilla indicada a `.github/workflows/pipeline.yml` usando el editor web de GitHub.

## Archivos principales

- `catalog.csv`: metadatos de los modelos publicados.
- `models/`: modelos UVL pequeños.
- `validate.py`: valida el catálogo.
- `build.py`: genera la web en `site/`.
- `workflow-templates/`: versiones progresivas de la pipeline.

## Requisito para el despliegue manual

En las dos primeras tareas necesitarás una cuenta gratuita de Netlify. Para la primera tarea también necesitarás Python 3.10 o posterior para generar la web manualmente a partir del ZIP descargado.

Sigue la guía proporcionada por el profesorado. No copies las tres plantillas a la vez: el objetivo es observar cómo evoluciona una única pipeline.
