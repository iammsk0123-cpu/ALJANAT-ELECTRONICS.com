# ALJANAT ELECTRONICS Store

A lightweight, responsive electronics storefront built as a single-page static web app. The project includes a product catalog, category filters, live search, shopping cart, WhatsApp ordering flow, and an admin panel for managing store content.

## Overview

This repository contains a storefront website for ALJANNAT ELECTRONICS with:

- Product browsing by category
- Search and sorting options
- Cart and total calculation
- WhatsApp checkout integration
- Admin panel for editing products and store settings
- Firebase Hosting configuration for quick deployment

## Project files

- `index.html` — main storefront page, styles, and JavaScript logic
- `firebase.json` — Firebase Hosting configuration
- `README.md` — project documentation

## Features

- Responsive design for desktop and mobile screens
- Product cards with pricing, sale badges, and category labels
- WhatsApp-based ordering for quick customer conversions
- Local browser storage for cart and store edits
- In-browser admin editing for products and visible storefront content

## Local preview

Because this is a static website, you can preview it in two simple ways:

1. Open `index.html` directly in a browser.
2. Or run a small local web server:

```bash
python -m http.server 8000
```

Then open:

```text
http://localhost:8000
```

## Deployment

This project is configured for Firebase Hosting.

### Prerequisites

- Node.js and npm
- Firebase CLI

### Deploy steps

```bash
npm install -g firebase-tools
firebase login
firebase deploy
```

The repository already includes a Firebase configuration in `firebase.json`, and it is set to serve the project root as the public directory.

## Customization

You can customize the store by updating the embedded store data in `index.html` or using the admin panel on the website. The admin panel allows editing:

- Store name and announcement
- Contact details and hours
- Product list and categories
- Product images, pricing, and descriptions

## Notes

- This is a static storefront and does not require a backend server.
- Orders are sent through WhatsApp using the configured phone number in the store settings.
- Store edits made in the admin panel are saved in the browser and can be downloaded as an updated HTML file for publishing.

## License

This project is provided as-is for personal or business use. If you plan to publish it publicly, confirm the branding, contact information, and product data are correct before deployment.
