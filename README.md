# You Will Do Better in Toledo

An aggressively open-source, public-domain rebuild of a classic symbol for a modern Toledo.

[betterintoledo.com](https://betterintoledo.com) is a public brand resource built around Toledo’s enduring civic message. It preserves the character of the original “You Will Do Better in Toledo” sign while making the mark and its supporting system useful across contemporary formats.

Use it. Change it. Print it. Sell it. Build on it. No permission or attribution required for original project assets released under CC0.

## What is here

- Rebuilt logo artwork in multiple configurations
- Brand colors, typography guidance, and structural graphics
- Downloadable public-domain archival photography
- Historical context for the original Toledo sign
- Contribution and licensing guidance
- The source for the public website

The project does not claim trademark rights to “You Will Do Better in Toledo.” The goal is straightforward public use, not control.

## Design direction

The system is rooted in historic optimism rebuilt for modern Toledo: industrial, gritty, optimistic, local, durable, and slightly weird. It favors real places, real history, disciplined supporting typography, and short declarative language over generic civic branding.

The original mark remains the expressive element. Supporting design uses Barlow Condensed, IBM Plex Sans, IBM Plex Mono, a primarily black-and-white palette, Toledo-derived accent colors, heavy frames, and structural geometry inspired by the original sign.

## Technology

- [Astro](https://astro.build) for statically generated HTML
- [Tailwind CSS](https://tailwindcss.com) for utility styling and brand tokens
- Astro’s asset pipeline for responsive and optimized imagery
- [GitHub Pages](https://pages.github.com) for hosting and deployment

The site intentionally avoids a client-side application framework. JavaScript is added only where an interaction requires it, and the primary content remains useful as rendered HTML.

## Local development

Node.js 22.12 or newer is required.

```sh
git clone https://github.com/toledowebprofessionals/better-in-toledo.git
cd better-in-toledo
npm install
npm run dev
```

Open [http://localhost:4321](http://localhost:4321).

## Commands

| Command | Purpose |
| --- | --- |
| `npm run dev` | Start the local Astro development server |
| `npm run build` | Generate the production site in `dist/` |
| `npm run preview` | Preview the production build locally |
| `npm run format` | Format Astro files with Prettier |

## Deployment

Pushes to `main` are built and deployed to GitHub Pages by
`.github/workflows/deploy.yml`. The workflow installs the locked dependencies, builds the static
site into `dist/`, and publishes that artifact through GitHub Pages.

In the repository settings, set **Pages → Build and deployment → Source** to **GitHub Actions**.
The production custom domain is `betterintoledo.com` and is also configured as Astro’s canonical
site URL.

## Project structure

```text
src/
├── assets/images/             Source images and downloadable brand assets
├── components/
│   ├── article/               Shared editorial-page components
│   ├── brand-system/          Brand standards components
│   └── page-components/       Homepage and photography sections
├── layouts/                   Shared site and brand-system layouts
├── pages/                     File-based routes
└── styles/                    Global styles and brand tokens
public/                        Fixed-URL public files
```

Displayed raster images are processed through Astro and generally served as appropriately sized WebP files. Full-resolution downloadable originals remain available through imported asset URLs with readable download filenames.

## Contributing

This is a public resource and should improve through public participation. Code, design refinements, logo applications, documentation, historical corrections, and original Toledo photography are welcome.

Read [CONTRIBUTING.md](CONTRIBUTING.md) before submitting work. If you do not use Git, email ideas or original contributions to [contribute@betterintoledo.com](mailto:contribute@betterintoledo.com).

## License and rights

Except where otherwise credited, the website, brand system, and original project assets are released into the public domain under [CC0 1.0 Universal](https://creativecommons.org/publicdomain/zero/1.0/), to the extent legally possible.

Third-party material is not automatically covered by that dedication. Fonts, photography, archival records, and other credited material retain their stated terms. Review the source and license information attached to each asset before reuse.

The project’s [plain-language license overview](https://betterintoledo.com/license/) explains the intended use and important limitations. The official CC0 legal code controls.

## Contact

Created and maintained by [Dan Paquette](https://danpaquette.net). Questions and contributions can be sent to [contribute@betterintoledo.com](mailto:contribute@betterintoledo.com).
