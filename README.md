# Philoxenia

A redesigned Astro website for Philoxenia by Hustle Hours.

```sh
npm install
npm run dev
```

Astro serves the site at http://localhost:4321. English is at `/`, Greek at `/el/`.

```sh
npm run check
npm run build
npm run preview
```

The production build is static HTML in `dist/`. Deploy this folder to any static host. The canonical domain is configured in `astro.config.mjs` and the layout metadata.

The application buttons link to the existing production application at https://philoxenia.hustlehours.com/apply. Authentication and application handling remain on that service. If replacing the original domain, keep its `/apply` route and backend available, or change the application URL in `src/components/HomePage.astro` and `src/components/Header.astro` to the backend's new location.

Content and all photographs come from the original website; credits are at `/credits/`. Fonts are hosted locally. The expired application countdown was removed; application availability is left to the existing application service.

The design uses the design-taste-frontend system and its motion assets in `public/assets/`. The user's original dark-green, gold and mint identity drives a playful scrapbook direction: candid photos in paper frames, the founders' story as a personal letter, and the original historical-founder collages around “Could this be you?” and “The door is open.” Layouts and content are Astro components; Tailwind provides utility classes. Sections follow their content height, and photographs retain their original aspect ratios. Decorative static rotations and layered photos follow the user's supplied reference. Motion falls back to a static experience when JavaScript is unavailable or reduced motion is enabled.

The current font pair is Geist and Instrument Serif, hosted locally. The invitation ticket is an Astro component. The experimental React Bits stack, chapter badges, mixed-font wordmark and added scroll effects were removed following design feedback; the previously approved scrapbook compositions are retained.
