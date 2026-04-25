# pye-landing

Landing page de la comunidad **Programadores y Estudiantes** (PyE).
Construido con [Astro](https://astro.build) y [Tailwind CSS](https://tailwindcss.com).

## Desarrollo

```sh
pnpm install
pnpm dev          # http://localhost:4321
pnpm build
pnpm preview
```

> El lockfile es `pnpm-lock.yaml`. Si preferís otro package manager, regenerá el lock correspondiente.

## Deploy con Docker

```sh
./run.sh          # build + run, expone http://localhost:4321
```

O manualmente:

```sh
docker build -t somospye-landing .
docker run -d -p 4321:80 somospye-landing
```

## Estructura

```
src/
  components/    # Cover, Welcome, Carousel, Goals, Contact, CTA
  layouts/       # Layout base
  pages/         # index.astro
  styles/
public/          # assets estáticos
```

## Stack

- Astro 5
- Tailwind CSS 4
- TypeScript
- Nginx (runtime, vía Docker)

## Contribuir

Issues y PRs bienvenidos. Para cambios grandes, abrí primero un issue para alinear scope.
