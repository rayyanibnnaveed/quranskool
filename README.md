# QuranSkool website

A complete, responsive website built from the course content at https://quranskool.carrd.co/.

## Deploy on Vercel

1. Extract this ZIP.
2. Create a GitHub repository and upload the **contents** of the `quranskool-vercel` folder. `index.html`, `styles.css`, `script.js`, `vercel.json`, and `assets/` should be at the root of that repository.
3. In Vercel, select **Add New → Project**, then import the repository.
4. Select **Other** as the framework preset. Leave the build command empty and use the repository root as the output directory. No install command or environment variables are needed.
5. Deploy. You can add your domain from the project's domain settings.

Alternatively, with the Vercel CLI installed, run `vercel` from this folder and follow the prompts, then `vercel --prod` when ready.

## Preview locally

Run `python -m http.server 3000` in this folder, then open http://localhost:3000. The page can also be opened directly from `index.html`.

## Included

- Responsive desktop and mobile layouts
- Existing QuranSkool logo and Faraz's real photograph
- Custom Quran hero image
- Accessible mobile navigation, keyboard controls, native expandable FAQs
- Reduced-motion support and progressive enhancement
- Course details, teacher profile, founding offer, and Skool signup links
- Page metadata, social sharing image, and favicon
- No dependencies, subscriptions, API keys, tracking scripts, or build step

## Content and links

All signup buttons link to https://www.skool.com/the-quran-skool-1322/.

Edit the course wording, offer, and FAQ answers in `index.html`. The £20 price is explicitly for the first month; ongoing pricing was not specified in the Carrd source. Confirm the live offer and teacher biography before launching. No class day or time was included because the source does not specify one.

Change the palette and typography at the top of `styles.css`. Fonts are served by Google Fonts, with local system fallbacks if unavailable. Images are included locally in `assets/`.

The social preview uses `/assets/social-preview.jpg`. Once you choose the production domain, set `og:image` to its full HTTPS URL (for example `https://your-domain.com/assets/social-preview.jpg`) for the broadest social crawler compatibility. Add your canonical URL and `og:url` at that point.

## Asset provenance

- Logo: supplied QuranSkool brand asset.
- Teacher photo and course facts: https://quranskool.carrd.co/.
- Hero image: custom generated using the built-in image generation tool. Full generation prompt is in `ASSETS.md`.

This package is ready for your own Vercel deployment. It has not been deployed to Vercel automatically.

Vercel deployment documentation: https://vercel.com/docs/builds/configure-a-build
