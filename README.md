# Bobby Hendricks ??? Personal Portfolio Website

**Live site:** https://bobbyhendricks.netlify.app

Personal portfolio website for data science and data engineering roles, built with the Hugo static site generator. The site serves as a full replacement for my resume and LinkedIn profile.

## Built With

- [Hugo](https://gohugo.io/) v0.166.0 (extended), the Go static site generator
- [Hugo Profile](https://github.com/gurusabarish/hugo-profile) theme, added as a git submodule
- Markdown content with Go templating provided by the theme
- [Netlify](https://www.netlify.com/) for free hosting with continuous deployment from GitHub

## Site Structure

| Path | Purpose |
|---|---|
| `config/_default/hugo.yaml` | Site settings, navigation menu, homepage profile, social links |
| `content/experience.md` | Professional experience |
| `content/projects.md` | Projects with links to code repositories |
| `content/skills.md` | Technical skills and tools |
| `content/resume.md` | Education, certifications, contact, and resume download |
| `static/Bobby-Hendricks-Resume.pdf` | Downloadable PDF resume |
| `netlify.toml` | Netlify build settings |

## Run Locally

    git clone --recurse-submodules https://github.com/CHbobray/my-portfolio.git
    cd my-portfolio
    hugo server -D

Then open http://localhost:1313. Hugo watches for changes and reloads the browser automatically.

## Deployment

Every push to the `main` branch triggers a Netlify build (`hugo --gc --minify`), which publishes the updated site automatically.

