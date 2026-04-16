# Prueba Lectiva

Base SvelteKit con arquitectura `feature-first/domain-first` para integrar la API de Rick and Morty.

## Run

```bash
npm install
npm run dev
```

## Check

```bash
npm run check
npm run build
```

## CI/CD y GitHub Pages

- `CI`: valida el proyecto con `npm ci`, `npm run check` y `npm run build`.
- `Deploy`: publica automaticamente en GitHub Pages cuando hay cambios en `main`.
- En GitHub Actions, el `base path` se ajusta automaticamente al nombre del repositorio.

La URL esperada de publicacion es:

```text
https://ingariasf33.github.io/actividad-pipeline-cicd/
```

## Estructura

- `src/lib/core`: cliente HTTP, configuracion y adaptadores.
- `src/lib/entities`: tipos y mapeos de dominio.
- `src/lib/features`: features por caso de uso.
- `src/routes`: composicion de rutas y carga de datos.
