# Portfolio WVazquez

Sitio web de portafolio personal construido con Astro y Tailwind CSS.
Muestra experiencia profesional, proyectos destacados, perfil personal y un formulario de contacto.

## Resumen

Este repositorio contiene un portafolio orientado a presentar el perfil de William Vazquez como Ingeniero de Software.
El sitio esta compuesto por secciones reutilizables y una arquitectura simple para facilitar mantenimiento y escalabilidad.

## Tecnologias principales

- Astro 5
- Tailwind CSS 4 (via `@tailwindcss/vite`)
- TypeScript (configuracion base)
- pnpm como gestor de paquetes

## Caracteristicas

- Landing de presentacion con informacion profesional.
- Seccion de experiencia laboral.
- Seccion de proyectos con stack tecnologico por proyecto.
- Seccion "Sobre mi".
- Formulario de contacto con envio via `fetch` a un servicio externo/local.
- Layout reutilizable con `Header` y `Footer`.

## Estructura del proyecto

```text
Portfolio_wvazquez/
|- public/
|  |- projects/
|  |- william_photo.webp
|  |- favicon.svg
|- src/
|  |- components/
|  |  |- layout/
|  |  |- icons/
|  |  |- ui/
|  |- layouts/
|  |- pages/
|  |- styles/
|- astro.config.mjs
|- package.json
|- pnpm-lock.yaml
```

## Requisitos

- Node.js 20 o superior (recomendado)
- pnpm 10+

## Instalacion y uso local

```bash
pnpm install
pnpm dev
```

El sitio quedara disponible en `http://localhost:4321`.

## Scripts disponibles

- `pnpm dev`: inicia el servidor de desarrollo.
- `pnpm build`: genera la version de produccion en `dist/`.
- `pnpm preview`: sirve localmente la build de produccion.
- `pnpm astro`: ejecuta comandos de Astro CLI.

## Formulario de contacto

El formulario en `src/components/Contact.astro` envia datos a:

- `http://localhost:3000/mail/sendMailWV`

Para que funcione correctamente en local o produccion, debes tener disponible ese servicio o actualizar la URL del endpoint segun tu backend.

## Personalizacion rapida

- Informacion principal: `src/components/Hero.astro`
- Experiencia: `src/components/Experience.astro`
- Proyectos: `src/components/Projects.astro`
- Estilos globales: `src/styles/global.css`
- SEO base (title/description): `src/pages/index.astro`

## Licencia

No se ha definido una licencia en este repositorio.
Si planeas distribuir o abrir este proyecto, agrega un archivo `LICENSE`.
