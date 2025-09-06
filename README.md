# To do list


1. Przygotowanie materiałów (jak pisałem wcześniej)

-> logo, kolory, fonty → z brandbooka,
-> zdjęcia (warsztaty, flakony, wnętrza),
-> teksty (tagline, opis oferty, warsztaty, case studies B2B, kontakt),
-> polityka prywatności / cookies,
-> decyzja o rezerwacjach (Calendly embed czy własny flow).

2. Struktura folderów

 /pages
  index.vue         -> Strona główna
  warsztaty.vue
  dla-firm.vue
  o-nas.vue
  kontakt.vue
  blog/[slug].vue
/components
  Navbar.vue
  Hero.vue
  Section.vue
  WorkshopCard.vue
  Footer.vue
/composables
  useSanity.ts       -> klient CMS
/assets
  /fonts /images /brand


3. 

Rezerwacje i kontakt

Warsztaty → embed Calendly iframe albo prosty formularz.

Kontakt → Nuxt server route (/server/api/contact.post.ts) wysyłający email np. przez EmailJS/SendGrid.

MVP → Formspree (zero back-endu)

4. SEO i performance

Nuxt ma useHead do meta tagów:

5. Hosting na Vercel



MVP: Strona główna, warsztaty (statyczne albo CMS), kontakt (formularz/Calendly), deploy.

# Nuxt Minimal Starter

Look at the [Nuxt documentation](https://nuxt.com/docs/getting-started/introduction) to learn more.

## Setup

Make sure to install dependencies:

```bash
# npm
npm install

# pnpm
pnpm install

# yarn
yarn install

# bun
bun install
```

## Development Server

Start the development server on `http://localhost:3000`:

```bash
# npm
npm run dev

# pnpm
pnpm dev

# yarn
yarn dev

# bun
bun run dev
```

## Production

Build the application for production:

```bash
# npm
npm run build

# pnpm
pnpm build

# yarn
yarn build

# bun
bun run build
```

Locally preview production build:

```bash
# npm
npm run preview

# pnpm
pnpm preview

# yarn
yarn preview

# bun
bun run preview
```

Check out the [deployment documentation](https://nuxt.com/docs/getting-started/deployment) for more information.
