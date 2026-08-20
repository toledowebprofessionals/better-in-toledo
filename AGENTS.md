# You Will Do Better in Toledo

This repository contains the public brand resource website for “You Will Do Better in Toledo.” The project rebuilds Toledo’s historic civic message as a practical, open-source brand system intended for public use.

## Project principles

- Preserve the character of the original mark while making the surrounding system durable and contemporary.
- Keep the voice confident, plainspoken, specific, optimistic, and slightly unconventional.
- Favor real Toledo history and texture over generic tourism or economic-development language.
- Keep original project artwork available under CC0 1.0 whenever legally possible.
- Do not imply that third-party photography, fonts, or source material is covered by the project’s CC0 dedication. Preserve asset-level credits and license notices.
- Do not claim trademark rights to “You Will Do Better in Toledo.”

## Stack

- Astro, rendered as static HTML for GitHub Pages
- Tailwind CSS
- Astro assets for image optimization
- No client framework unless an interaction genuinely requires one
- Client-side JavaScript should remain small, progressive, and optional where possible

## Commands

```sh
npm run dev
npm run build
npm run preview
npm run format
```

Run `npm run build` after substantive changes. Run `npm run format` after editing Astro files.

## Structure

- `src/layouts/BaseLayout.astro` owns the shared document head, site header, and site footer.
- `src/layouts/BrandSystemLayout.astro` owns the brand-system sidebar and content layout.
- `src/components/page-components/` contains homepage and photography-page sections.
- `src/components/brand-system/` contains reusable brand-standard components.
- `src/components/article/` contains reusable components for editorial pages such as Contribute and License.
- `src/assets/images/` is the single source for site imagery, logos, graphic elements, and downloadable image assets.
- `public/` is reserved for files that must retain a fixed public URL, such as `humans.txt` and the favicon.

## Components and pages

- Put shared site chrome in layouts or shared components rather than duplicating it in pages.
- Keep page frontmatter readable and use page-level data objects to supply component content.
- Prefer reusable components when markup, spacing, or behavior occurs across multiple pages.
- Keep truly page-specific styling with its page or component.
- Preserve semantic HTML, sensible heading order, keyboard access, visible focus states, and descriptive alternative text.

## Styling

- Follow the existing container widths and spacing system before introducing new values.
- Use the established CSS custom properties and Tailwind brand tokens.
- Supporting typography uses Barlow Condensed, IBM Plex Sans, and IBM Plex Mono.
- The master logo is artwork; do not recreate or replace its lettering with live type.
- Keep black, white, and neutral fields dominant. Use Glass Blue and Foundry Orange deliberately.
- Avoid unnecessary animation. Respect reduced-motion preferences when adding motion.
- Formatting follows `.prettierrc.json` and `.editorconfig`.

## Images and downloads

- Import images from `src/assets/images/` instead of referencing hard-coded `/images/` paths.
- Use Astro’s image pipeline for displayed raster previews, generally serving WebP at an appropriate display size.
- Keep downloadable originals at full resolution and use imported `?url` values for their links.
- Set an explicit `download` filename so Astro’s hashed output URL does not become the saved filename.
- Store attribution or provenance documentation beside the relevant asset when practical.

## Licensing and attribution

- Original website and brand-system contributions must be ready for release under CC0 1.0 to the extent legally possible.
- Verify that contributors own or may dedicate submitted work before describing it as CC0 or public domain.
- Preserve per-asset source, contributor, license, and copyright-status fields for archival photography.
- Do not remove required attribution from third-party assets. The skyline photograph, for example, is licensed separately under CC BY 2.0.
- Treat the license pages as plain-language explanations, not legal advice, and link to the controlling license text.

## Change discipline

- Keep changes scoped to the request and preserve unrelated work.
- Do not add React or another client framework for interactions that native HTML, CSS, or small scripts can handle.
- Check desktop and mobile behavior when changing layouts.
- Before handing off substantive work, format the Astro files and confirm that the production build succeeds.
