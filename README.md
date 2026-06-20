# warandco.com

Brand design portfolio — hosted on GitHub Pages.

## Structure

```
/
├── index.html          # Home / portfolio grid
├── venom-vodka.html    # Project page (duplicate pattern for each project)
├── about.html          # About page
├── contact.html        # Contact page
├── WandCo.svg          # Logo
├── css/
│   └── style.css
├── js/
│   └── main.js
└── images/
    └── (project images go here)
```

## Adding a new project

1. Duplicate `venom-vodka.html`, rename it.
2. Update the title, description, sidebar meta, and image paths.
3. Add a new `.card` block in `index.html` pointing to the new page via `data-href`.

## Replacing placeholder images

The colored `<div>` placeholders in cards and project pages are sized with `aspect-ratio`. 
Replace each with:

```html
<img src="images/your-image.jpg" alt="Description" loading="lazy" />
```

inside the existing `.card__img-wrap` or `.project__img` containers.

## Deploying to GitHub Pages

1. Create a repo named `warandco.com` (or your username's `<username>.github.io`).
2. Push all files to the `main` branch.
3. In repo Settings → Pages → set source to `main` branch, `/ (root)`.
4. Add a custom domain if using your own.
