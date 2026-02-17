# GDG Speaker — Presentation & Materials

A simple React app for your Google Developer Group speaker session: presentation PDF and social links (LinkedIn, Facebook, GitHub). Ready to deploy on **Netlify** (free tier).

## Quick start

```bash
npm install
npm run dev
```

Open [http://localhost:5173](http://localhost:5173).

## Add your content

1. **PDF**  
   Put your presentation PDF in the `public` folder and name it `presentation.pdf`.  
   To use another path or filename, edit `PDF_URL` and `PDF_LABEL` in `src/SpeakerPage.jsx`.

2. **Social links**  
   In `src/SpeakerPage.jsx`, update the `SOCIAL_LINKS` object with your real URLs:
   - `linkedin`: your LinkedIn profile URL  
   - `facebook`: your Facebook profile URL  
   - `github`: your GitHub profile URL  

3. **Title & copy**  
   Adjust the hero text and section titles in `src/SpeakerPage.jsx` to match your talk (e.g. session title, description).

## Deploy on Netlify (free tier)

1. Push this repo to GitHub (or GitLab/Bitbucket).
2. Log in to [Netlify](https://www.netlify.com) and click **Add new site** → **Import an existing project**.
3. Connect your repo. Netlify will use the built-in settings from `netlify.toml`:
   - **Build command:** `npm run build`  
   - **Publish directory:** `dist`
4. Click **Deploy site**.  
   Your site will be live at a `*.netlify.app` URL. You can add a custom domain in Site settings.

## Tech

- [React](https://react.dev/) + [Vite](https://vitejs.dev/)
- Styled with CSS (no UI framework)
- Single-page layout, Netlify redirects configured for SPA
