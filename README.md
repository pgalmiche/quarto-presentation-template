# Quarto Presentation Template

This repository provides a ready-to-use template for creating presentation slides using the [Quarto](https://quarto.org/) framework with [Reveal.js](https://revealjs.com/).

It supports modern slide features and is suitable for both local development and GitLab Pages deployment.

---

## ✨ Features

- Built with [Reveal.js](https://revealjs.com/): a powerful framework for HTML presentations.
- Easily embed:
  - GIFs
  - Iframes and websites
  - External links
- Fully customizable design: layout, themes, color schemes, and more.
- Online deployment via GitLab Pages.

---

## 🚧 TODO

- [ ] Create a polished title slide
- [ ] Improve slide and link color themes
- [ ] Add documentation for advanced features (e.g., Excalidraw integration)

---

## 🛠 Local Development

You can run the project locally using Docker Compose:

### 1. Start the project

```bash
docker compose up
```

This will build the presentation in the `/quarto/_output/` directory.

### 2. Preview your slides

Open `index.html` inside the `_output` folder in your browser.

### 3. Modify and Rebuild

To customize your slides:

- Edit `index.qmd` and the files inside `/chapters/`
- Then re-run:

```bash
docker compose up
```

- Refresh your browser to see the updates.

---

## 🚀 Optional: Install Quarto Locally

If you prefer to run Quarto outside Docker, follow the official [installation guide](https://quarto.org/docs/get-started/) and render slides manually:

```bash
quarto render index.qmd --to revealjs
```

---

## 🔁 CI/CD with GitLab/GitHub

This project supports automated deployment for both GitLab and GitHub:

- For GitLab, the included .gitlab-ci.yml file builds and deploys your slides to GitLab Pages when changes are pushed to the repository.

- For GitHub, the .github/workflows/deploy.yml workflow handles the build and publishes the slides to GitHub Pages automatically.
