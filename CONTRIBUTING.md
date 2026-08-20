# Contributing

“You Will Do Better in Toledo” is being rebuilt as a public resource and a public good. Contributions that make the brand system more useful, accurate, accessible, and representative of Toledo are welcome.

## Ways to contribute

You can help by:

- Improving the website’s design, accessibility, performance, or documentation
- Creating useful logo arrangements, templates, or graphic tools
- Correcting historical information and supplying reliable sources
- Contributing original photography of Toledo
- Reviewing copy for clarity, accuracy, and local specificity
- Reporting bugs, broken links, accessibility problems, or unclear guidance
- Showing how you have used or adapted the system

Before starting substantial work, open a [GitHub issue](https://github.com/toledowebprofessionals/better-in-toledo/issues) so the idea and its scope can be discussed.

## Public-domain contribution requirement

Original work contributed to this project must be ready for release under [CC0 1.0 Universal](https://creativecommons.org/publicdomain/zero/1.0/), to the extent legally possible. By contributing original work, you agree that it may be released with the project under CC0.

Only contribute work you created or have the legal authority to dedicate. Do not submit copyrighted logos, photographs, illustrations, writing, or other assets copied from elsewhere simply because they are available online.

When a contribution relies on third-party material:

- Identify the creator and original source.
- Provide the exact license or public-domain status.
- Preserve any required attribution.
- Explain whether you modified the material.
- Do not describe it as part of the project’s CC0 dedication unless it is legally eligible.

CC0 addresses copyright and related rights. It does not grant rights that a contributor does not own, and it does not resolve privacy, publicity, patent, or other restrictions that may apply to a particular use.

## Photography

Original Toledo photography is especially welcome. Contributions should show the city as it exists: neighborhoods, people, storefronts, porches, signs, bridges, industry, architecture, ordinary moments, and useful details.

For each photograph, include:

- Photographer’s name
- A concise title and description
- Approximate date and location, when known
- Confirmation that the photographer owns the image
- Confirmation that the image may be dedicated under CC0
- Any relevant information about identifiable people, private property, artwork, or trademarks

Historical or third-party photography must include its source institution, source-record URL, contributor or creator, stated rights information, and any uncertainty about copyright outside the United States.

## Development workflow

1. Fork the repository and create a focused branch.
2. Install dependencies with `npm install`.
3. Start the site with `npm run dev`.
4. Make a focused change and check it at desktop and mobile widths.
5. Run `npm run format` after editing Astro files.
6. Run `npm run build` before submitting your work.
7. Open a pull request explaining what changed and why.

This project requires Node.js 22.12 or newer.

## Technical expectations

- Keep the site statically rendered with Astro and suitable for GitHub Pages.
- Prefer semantic HTML and CSS over client-side abstractions.
- Do not add React or another framework unless an interaction genuinely requires it.
- Keep client-side JavaScript small and progressively enhanced.
- Reuse existing layouts and components before duplicating markup or styling.
- Preserve keyboard access, visible focus states, heading order, and descriptive alternative text.
- Follow `.editorconfig`, `.prettierrc.json`, and the repository conventions in `AGENTS.md`.

## Images and downloadable assets

- Store source assets in `src/assets/images/`.
- Use Astro’s image pipeline for displayed raster previews.
- Serve appropriately sized WebP previews where practical.
- Keep full-resolution originals available for explicit downloads.
- Import downloadable files with `?url` and set a readable `download` filename.
- Store provenance and attribution information alongside the asset or in its page data.

Do not commit generated files from `dist/`, Astro’s `.astro/` directory, dependency folders, editor settings, or operating-system metadata.

## Pull requests

Keep pull requests narrow enough to understand and review. A useful description includes:

- The problem or opportunity
- The proposed change
- Screenshots for visible changes
- Desktop and mobile behavior checked
- Accessibility considerations
- Asset sources and licenses, when applicable
- Confirmation that `npm run build` succeeds

Review may request changes for accessibility, technical consistency, historical accuracy, licensing clarity, or alignment with the project’s public-purpose goals.

## Don’t know Git?

Git is not a requirement for having a useful idea. Email alterations, concepts, corrections, source material, or original photography to [contribute@betterintoledo.com](mailto:contribute@betterintoledo.com).

Include enough context to understand the contribution and, for any asset, its creator, source, and proposed license. Large files may be shared through a download link.

## Conduct

Be direct, constructive, and generous with other contributors. Critique the work rather than the person. Respect Toledo’s communities, history, and the people represented in submitted material. Contributions that are discriminatory, harassing, deceptive, or intentionally destructive are not welcome.
