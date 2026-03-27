# Meetup Clone

Responsive front-end project inspired by the Meetup website. The project is built with plain HTML, CSS, and JavaScript and includes a landing page plus a separate events page with client-side filtering.

## Overview

This project focuses on static front-end development and basic interactivity:

- responsive layout for desktop and mobile
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

- responsive desktop and mobile versions
- event search by title or description
- filtering by event type, distance, and category
- persistent theme switching
- horizontal scroll section for online events
- page-to-page navigation buttons

## Getting Started

No build step is required.

1. Open the `project` folder in your editor.
2. Start `index.html` in a browser.

For a better local workflow, run the project with VS Code Live Server.

## Notes

- The project uses external CDN resources, so an internet connection is required for fonts and animation libraries.
- Event data for the events page is hardcoded in `scripts/script.js`.
- The design is based on Meetup-inspired practice layout work.

## Future Improvements

- move event data into a separate JSON file
- add validation for the modal form
- improve accessibility and keyboard support
- reduce duplicated markup between desktop and mobile sections
- optimize images and normalize file naming
