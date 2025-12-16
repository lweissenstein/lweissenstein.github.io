# Portfolio Website

**Developer:** Lennart Weissenstein
**Project:** Personal Portfolio & Resume (Jekyll/GitHub Pages)

---

## Overview

This repository hosts my personal portfolio website, designed to showcase my projects from university and private development, as well as my professional CV. The site is built as a static web page using **Jekyll** and hosted via **GitHub Pages**, providing a fast, responsive, and easily maintainable platform for my internship applications.

It is based on the [al-folio](https://github.com/alshedivat/al-folio) theme but has been significantly customized to focus on a portfolio-first approach rather than an academic blog.

---

## Screenshots

To be completed...

---

## View the Portfolio

You can visit the live website here:
[lweissenstein.github.io](https://lweissenstein.github.io)

---

## Key Features & Tech Stack

* **Static Site Generation** using Jekyll and Liquid templating.
* **Responsive Design** utilizing Bootstrap for grid layouts and mobile compatibility.
* **Data-Driven Resume** generated dynamically from a `resume.json` file.
* **Automated Deployment** via GitHub Actions (CI/CD).
* **Dark/Light Mode** support with custom color variable overrides.

---

## Customization & Implementation

While based on the al-folio template, the following modifications were made to tailor the site for a Game Design/Tech Art portfolio:

* **Streamlined Architecture:** Removed academic-focused sections (Blog, News, Bookshelf) by commenting out references and excluding them from the build to keep the navigation clean.
* **Custom Styling:** Created a `custom.scss` to overwrite theme defaults, specifically adjusting button styles and color variables (`$blue-color`) to match personal branding.
* **Enhanced "About" Page:** Engineered a "Selected Projects" section using **Bootstrap grid** logic directly on the landing page. This allows recruiters to see featured work immediately upon arrival without navigating away.
* **Project Structure:** Implemented a markdown-based workflow for projects, where each project (e.g., *Astro Dungeon*, *BioTopia*) exists as a standalone `.md` file with dedicated metadata.

---

## The JSON Resume System

To ensure a "Single Source of Truth" for my professional history, the CV section is powered by a standardized JSON schema.

* **File:** `assets/json/resume.json`
* **Function:** Stores all data regarding Work Experience, Education, and Skills.
* **Rendering:** Liquid templates parse this JSON to generate the HTML Resume, making updates simple and error-proof.

---

## CI/CD Workflow

The project utilizes **GitHub Actions** for continuous integration and deployment.

1.  **Push to Main:** Triggers the workflow.
2.  **Build:** Sets up Ruby, installs dependencies via Bundler, and builds the Jekyll site.
3.  **Deploy:** Automatically pushes the static build to the `gh-pages` branch, making the changes live instantly.

---

## Purpose

This portfolio serves as the central hub for my application to **Technical Artist** and **Game Design** internships. It demonstrates not only my creative work (3D modeling, Game Dev) but also my technical literacy in web development, version control, and pipeline automation.

---

## Credits & Licenses

* **Theme:** Based on [al-folio](https://github.com/alshedivat/al-folio) by Al Shedivat.
* **Content:** All project text, code, and images are &copy; Lennart Weissenstein unless otherwise stated.

---