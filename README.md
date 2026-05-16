# Meetup Clone

Front-end project inspired by the Meetup website. The project is built with plain HTML, CSS, and JavaScript and includes a landing page plus a separate events page with client-side filtering.

## Live Demo

Live on Vercel: https://meetupclone-21kwgnqir-irinas-projects-44afd5ab.vercel.app/

## Overview

This project focuses on static front-end development and basic interactivity:

- desktop layout with a separate mobile adaptation for narrow screens
- two connected pages: home and events
- event search and filter logic in vanilla JavaScript
- dark/light theme toggle with `localStorage`
- animated sections using `animate.css` and `WOW.js`
- embedded Google Map on the events page

## Pages

### `index.html`

Landing page with:

- hero section
- event cards
- online events slider
- category blocks
- popular cities
- informational sections
- footer navigation

### `index2.html`

Events page with:

- search input
- filters by type, distance, and category
- dynamically rendered event cards
- New York map section
- navigation back to the main page

## Tech Stack

- HTML5
- CSS3
- JavaScript
- [Animate.css](https://animate.style/)
- [WOW.js](https://wowjs.uk/)
- Google Fonts
- Google Maps Embed
- Vercel

## Folder Structure

```text
project/
|-- .vscode/
|   `-- settings.json
|-- icons/
|-- images/
|-- scripts/
|   `-- script.js
|-- styles/
|   |-- style.css
|   `-- styleMedia.css
|-- index.html
|-- index2.html
`-- README.md
```

## Features

- desktop version and a separate mobile version for narrow screens
- event search by title or description
- filtering by event type, distance, and category
- persistent theme switching
- horizontal scroll section for online events
- page-to-page navigation buttons

## Getting Started

No build step is required.

### Run locally

1. Open the project folder in your editor.
2. Open `index.html` in your browser.

For a better local workflow, you can use VS Code Live Server.

## Deployment

The site can be deployed on Vercel as a static project.

Recommended deployment flow:

1. Import the GitHub repository into Vercel.
2. Select `Other` as the framework preset.
3. Leave the build command empty.
4. Set the output directory to `.`.
5. Deploy and add the generated URL to this README.

## Notes

- The project uses external CDN resources, so an internet connection is required for fonts and animation libraries.
- Event data for the events page is hardcoded in `scripts/script.js`.
- The mobile styles are written mainly for narrow screens around 370-393px wide, not as a fully fluid layout for every viewport size.
- The design is based on Meetup-inspired practice layout work.
