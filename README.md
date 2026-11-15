# Rocket Elevators – Web Development 1

## Description
A multi-page static marketing website for **Rocket Elevators**, an elevator company operating since 1976. The site promotes the brand, showcases residential and commercial services, displays a portfolio, testimonials, industry news and partner logos, and gives visitors a way to contact the company or request a quote.

It was built for the CodeBoxx Web Development 1 module by adapting and fully rebranding the SmartyTemplates HTML template. Copy was generated with AI and edited by hand (see `PROMPTS.md`).

## Pages
| File | Purpose |
|------|---------|
| `index.html` | Homepage: hero slider, services, portfolio (filterable), testimonials, news, clients, contact form, map, footer |
| `residential.html` | Landing page for homeowners |
| `commercial.html` | Landing page for business clients |
| `quote.html` | Quote request page |

## Technology Stack
- HTML5
- CSS3 with Bootstrap (included in the template)
- JavaScript / jQuery (included in the template)
- Plugins already shipped with the template: Revolution Slider, MixItUp (portfolio filter), Owl Carousel, Magnific Popup
- Google Maps embed (iframe)

No server-side framework and no additional libraries were added.

## Project Structure
```
.
├── index.html            Homepage
├── residential.html      Residential landing page
├── commercial.html       Commercial landing page
├── quote.html            Quote request page
├── PROMPTS.md            First five AI prompts, with reflections
├── README.md             This file
└── assets/
    ├── css/              Template styles + rocket-custom.css (Rocket Elevators branding)
    ├── js/               Template scripts
    ├── plugins/          Bootstrap, jQuery, sliders, carousel, filters
    ├── fonts/
    └── images/
        └── rocketElevators/   Logo, favicon, hero, portfolio, client and news images
```
Rocket Elevators brand overrides (colors, hero backgrounds, buttons, footer) live in `assets/css/rocket-custom.css`, which loads last so it overrides the template styles.

## Installation and Setup
No build step or dependencies are needed.

1. Clone the repository:
   ```bash
   git clone git@github.com:regsmith90-creator/RocketElevators-WebDevelopment1.git
   cd RocketElevators-WebDevelopment1
   ```
2. Open `index.html` directly in a browser, **or** serve it locally (recommended):
   ```bash
   python3 -m http.server 8000
   ```
   then visit <http://localhost:8000>.

## Environment Variables
None. The project is fully static and uses no credentials or secrets.

## APIs
The project does not consume any API. The only external embed is Google Maps (iframe) in the Contact section. The contact form is front-end only in this module and is not wired to a back end.

## Known Issues
No known console errors were identified in a static check; all linked local files resolve. Browser console behavior should be confirmed when reviewing.

## Branching
Work was done on the `dev` branch and merged into `main` for submission.

## Author
Gee Smith
