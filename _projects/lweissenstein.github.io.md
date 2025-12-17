---
layout: page
title: Portfolio Website
description: Jekyll-based static site development and CI/CD implementation.
img: /assets/img/screenshot_landing.png
importance: 4
category: private
---

This project displays the development, deployment, and ongoing maintenance of this portfolio website. Looking to develop my technical expertise in static site generation, front-end customization, and continuous integration/continuous deployment (CI/CD) workflows using GitHub Actions.

The primary goal was to create a fast, portfolio-first web presence that efficiently showcases my Projects in 3D Art, Game Development, and Technical Art projects while providing a comprehensive, data-driven CV.

---

## Screenshot

The following image shows the responsive design of the landing page, highlighting the custom "Selected Projects" integration.

<div class="row justify-content-sm-center">
    <div class="col-sm-12 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/screenshot_landing.png" title="Screenshot of the live portfolio website" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    custom main landing page featuring grid layout for selected projects
</div>

---

## Key Features & Tech Stack

- **Static Site Generation** using Jekyll and Liquid templating.
- **Responsive Design** utilizing Bootstrap for grid layouts and mobile compatibility.
- **Data-Driven Resume** generated dynamically from a `resume.json` file.
- **Automated Deployment** via GitHub Actions (CI/CD).
- **Dark/Light Mode** support with custom color variable overrides.

---

## Customization & Implementation

While based on the al-folio template, the following modifications were made by me to tailor the site for a Game Design/Tech Art portfolio:

- **Streamlined Webpage:** Removed academic-focused sections (Blog, News, Bookshelf) by commenting out references and excluding them from the build to keep the navigation clean.
- **Custom Overwriting:** Created a `custom.scss` to overwrite theme defaults, adjusting button styles, changing specific fonts and more.
- **Improved About Page:** Added a "Selected Projects" section using **Bootstrap grid** logic directly on the landing page. This allows recruiters to see featured work immediately upon arrival without navigating away.

---

## CI/CD Workflow

The project utilizes **GitHub Actions** for continuous integration and deployment.

1.  **Push to Main:** Triggers the workflow.
2.  **Build:** Sets up Ruby, installs dependencies via Bundler, and builds the Jekyll site.
3.  **Deploy:** Automatically pushes the static build to the `gh-pages` branch, making the changes live instantly.

---

## Repository and Live Site

- **View the Live Portfolio:** [lweissenstein.github.io](https://lweissenstein.github.io)
- **GitHub Repository:** [github.com/lweissenstein](https://github.com/lweissenstein)

---
