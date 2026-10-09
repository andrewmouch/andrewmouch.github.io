# website

Personal site for Andrew Mouchantaf. Astro, static output, no runtime dependencies.

## Run it

    npm install
    npm run dev        # http://localhost:4321
    npm run build      # static site to dist/
    npm run preview    # serve the built output

## Layout

    src/pages/index.astro      entry animation, redirects to /home
    src/pages/home.astro       landing
    src/pages/resume.astro     resume, with public/resume.pdf for download
    src/pages/projects.astro   placeholder
    src/pages/contact.astro    email
    src/components/            IsoNameScene (entry), RobotHero (home), Nav, TitleBlock
    src/layouts/Base.astro     page shell: grid surface, nav, drawing legend
    src/styles/global.css      tokens and page surfaces

## Deploy

Pushing to `main` runs `.github/workflows/deploy.yml`, which builds the site and
publishes `dist/` to GitHub Pages at https://andrewmouch.github.io/.
