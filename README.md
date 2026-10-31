# Vaibhav Sabale — Interactive Portfolio

A polished, responsive **React + Vite + Framer Motion** portfolio. White/cream visual design, custom project illustrations, interactive filtering, mini-game, keyboard command palette, secret keyboard Easter egg, and resume download.

## Run locally

Install **Node.js 20 LTS or newer**. Open a terminal in this folder:

```bash
npm install
npm run dev
```

Open the localhost URL shown in the terminal (typically http://localhost:5173).

## Build

```bash
npm run build
npm run preview
```

The production files are generated in `dist/`.

## Deploy free with Vercel (recommended)

1. Create a GitHub repository (e.g. `vaibhav-portfolio`).
2. Upload all project files, including `src`, `public`, `package.json`, and `index.html`. **Do not upload `node_modules` or `dist`.**
3. Sign in to Vercel using GitHub, click **Add New → Project**, and import your repository.
4. Framework preset: **Vite**. Build command: `npm run build`. Output directory: `dist`.
5. Click **Deploy**. Vercel provides a public `.vercel.app` URL.
6. Future GitHub pushes automatically trigger deployments.

### Alternative: Netlify

1. Push this folder to GitHub.
2. In Netlify choose **Add new project → Import an existing project** and connect the repository.
3. Build command `npm run build`, publish directory `dist`.
4. Deploy. No environment variables are needed.

### Alternative: GitHub Pages

GitHub Pages needs a base-path adjustment when deployed to a project subpath (`/repo-name/`). Add `base: '/repo-name/'` to a `vite.config.js`, then use an appropriate Pages deployment action. For the easiest deployment without configuration, use Vercel or Netlify.

## Customize

- **Profile photo**: `public/profile.jpeg` (extracted from the uploaded resume PDF).
- **Resume**: `public/Vaibhav_Sabale_Resume.pdf`.
- **Projects, links, skills and text**: `src/main.jsx`.
- **Colors, typography, spacing**: `src/style.css`.
- **SEO title/description**: `index.html`.

## Important details

- The contact button uses `mailto:` (opens a visitor's email app); it is not a server-backed contact form.
- The Smart Timetable project has no repository URL in the supplied resume, so it is intentionally shown without an external project link.
- The 'open to internships' badge is editable text, not a live availability feed.
- The currency example in the project illustration is **decorative sample data**, not a live exchange rate.
- Google Fonts are loaded from the web; the site uses fallback fonts when offline.
- `Ctrl/Cmd + K` opens quick navigation. Try the classic ↑ ↑ ↓ ↓ ← → ← → B A sequence for a surprise.

## Security & accessibility

- External links use `noopener noreferrer`.
- Supports reduced-motion preferences, keyboard navigation, responsive mobile layouts and descriptive image alt text.
- Review whether you want to publish the phone number shown in the downloadable resume before deploying publicly.
