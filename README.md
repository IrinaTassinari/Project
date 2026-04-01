# Meetup Clone

Responsive front-end project inspired by the Meetup website. The project is built with plain HTML, CSS, and JavaScript and includes a landing page plus a separate events page with client-side filtering.

## Live Demo

AWS deployment:

http://63.179.163.24:5000/index.html

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
- Docker
- Nginx
- AWS

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
|-- Dockerfile
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

### Run locally

1. Open the project folder in your editor.
2. Open `index.html` in your browser.

For a better local workflow, you can use VS Code Live Server.

## Run with Docker

The project includes a simple `Dockerfile` based on `nginx:alpine`.

### Build image

```bash
docker build -t meetup-clone .
```

### Run container

```bash
docker run -d -p 5000:80 --name meetup-clone-app meetup-clone
```

Then open:

http://localhost:5000/index.html

## Deployment

The site is deployed on AWS and is available at:

http://63.179.163.24:5000/index.html

Deployment flow:

1. Build the Docker image from the project root.
2. Run the container with port mapping from the server to Nginx inside the container.
3. Serve the static files through Nginx.

## Dockerfile

```dockerfile
FROM nginx:alpine
COPY . /usr/share/nginx/html
EXPOSE 80
```

This configuration copies the project files into the default Nginx web root and serves the static website from port `80` inside the container.

## Notes

- The project uses external CDN resources, so an internet connection is required for fonts and animation libraries.
- Event data for the events page is hardcoded in `scripts/script.js`.
- The design is based on Meetup-inspired practice layout work.


