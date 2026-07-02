# Pravin Kumar Singh — Academic Website

A personal academic website for **Dr. Pravin Kumar Singh, Ph.D.**, Assistant Professor,
Department of Physics, Manipal University Jaipur. Built with the same underlying
theme (Minimal Mistakes + Academicons) used by many academic personal sites.

Structure and markup (masthead greedy-nav, sticky sidebar with author avatar/bio/social icons,
`page__inner-wrap` > `page__title` > `page__content`, and footer) are modeled directly on the
academicpages/Minimal Mistakes reference page you shared (Khac-Hoang Ngo's site).

## Structure

```
index.html           Home — bio, contact, news
cv.html               Curriculum vitae — education, positions, awards, skills, patents, books, membership
research.html         Research areas, major projects, conferences organized, editorial roles
publications.html     Journal articles + conference presentations
teaching.html         Teaching experience, courses, student supervision
talks.html            Invited talks
Pravin_Kumar_Singh_CV.pdf   Downloadable CV
images/profile.jpg    Profile photo
assets/css/main.css        Theme stylesheet (yours, provided)
assets/css/academicons.css Academic icon font styles (yours, provided)
assets/js/main.min.js      Theme JS (yours, provided) — powers the collapsing "greedy-nav" menu
```

Icons (Font Awesome + Academicons webfonts) are loaded from CDN in the `<head>`
of each page so they render correctly even though the local `academicons.css`
doesn't include its font files. You can remove the CDN links later if you add
the `fonts/` folder alongside `assets/css/academicons.css`.

## How to publish this on GitHub Pages

1. Create a new GitHub repository, e.g. `pravinsingh.github.io`
   (using exactly `<your-username>.github.io` gives you a root-domain site;
   any other repo name works too, served at `<username>.github.io/<repo>`).
2. Upload/push all the files in this folder to the repository (keep the same
   folder structure).
3. In the repo, go to **Settings → Pages**, set:
   - Source: `Deploy from a branch`
   - Branch: `main` (or `master`), folder `/ (root)`
4. Save. GitHub will publish the site at `https://<your-username>.github.io/`
   (or `/<repo-name>/` if not a root-named repo) within a minute or two.
5. Edit `index.html`, `cv.html`, `publications.html`, `talks.html` directly
   any time your CV changes — no build step required, it's plain HTML/CSS/JS.

## Editing content

Every page is a self-contained HTML file, so you can edit text directly.
Your contact details, bio, awards, and publication list were populated from
`Pravin_Kumar_Singh_CV.pdf`. Update Google Scholar/ORCID links, add a
personal photo update, or update publications by editing the relevant
`<div class="archive__item">` blocks in `publications.html`.
