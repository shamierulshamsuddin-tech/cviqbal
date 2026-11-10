# Muhammad Shamierul Iqbal – Digital CV

A single-page digital CV for an AI developer and AI engineer, built with React. It shows work experience at MIMOS Solution, university projects, skills and education.

Live site: `https://YOUR-USERNAME.github.io`

## Features

- Animated hero with a computer-vision style detection overlay on the profile photo
- Sticky navigation that highlights the current section, plus a scroll progress bar
- Experience at MIMOS Solution split into tracks (RAG, OCR, sentiment analysis, LLM chatbot, audio AI, OSINT knowledge)
- University projects with a technology filter
- Light and dark mode (follows the visitor's system setting, with a manual switch)
- "Save as PDF" button that opens a clean print layout
- Works on phones, tablets and desktops

## Files

| File | What it is |
| --- | --- |
| `index.html` | The whole site: HTML, CSS and React code in one file |
| `README.md` | This file |

There is no build step. React and the fonts load from a CDN, and the profile photo is embedded inside `index.html`.

## Deploy on GitHub Pages (free)

1. Create a public repository named `YOUR-USERNAME.github.io`.
2. Upload `index.html` and `README.md` (Add file, then Upload files, then Commit changes).
3. Go to Settings, then Pages.
4. Set Source to "Deploy from a branch", choose the `main` branch and `/ (root)`, then click Save.
5. Wait about a minute, then open `https://YOUR-USERNAME.github.io`.

To update the site, edit `index.html` on GitHub (pencil icon) and commit. Pages redeploys automatically.

## Edit the content

Open `index.html` and find the `CV` object near the top of the `<script>` section. Change the text there:

- `name`, `role`, `summary`, `email`, `place`: the hero and contact details
- `job.tracks`: the experience tracks and their bullet points
- `projects`: the university projects (each has a name, meta line, description and `tech` tags)
- `skills`, `education`, `extra`: skills, education, certification and languages

## Change the photo

The photo is embedded in the `<img class="photo">` area of the hero (the `src` starts with `data:image/jpeg;base64,`). To use a file instead:

1. Upload `photo.jpg` to the same folder as `index.html`.
2. Replace the long `src="data:image/jpeg;base64,..."` value with `src="photo.jpg"`.

Use a sharp photo at least 600 pixels wide. The detection boxes in the CSS (`.d1` and `.d2`) are positioned for a photo of one person standing, so adjust their `left`, `top`, `width` and `height` values if your new photo is framed differently.

## Built with

- [React 18](https://react.dev/) (loaded from cdnjs)
- [htm](https://github.com/developit/htm) for JSX-style templates without a build step
- Google Fonts: Bricolage Grotesque and IBM Plex Sans

## Contact

shamierul.shamsuddin@gmail.com
