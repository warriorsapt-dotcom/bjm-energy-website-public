# BJM Energy Website

A static business website for BJM Energy Solution LTD. It presents solar services for homes and businesses and helps visitors turn their requirements into a structured enquiry.

Built with HTML, CSS and vanilla JavaScript, with no package installation or build step.

## Features

- Service, solution, founder and FAQ sections.
- A project brief form covering property type, service, location and project details.
- Service links that preselect the relevant enquiry option.
- Gmail and WhatsApp draft links populated from the brief.
- Downloadable plain-text project briefs.
- CSS solar illustration and a local brand asset.

## Run locally

```sh
git clone https://github.com/warriorsapt-dotcom/bjm-energy-website-public.git
cd bjm-energy-website-public
```

Open `index.html` in a browser, or use Python 3 to serve the files locally:

```sh
python -m http.server 8000
```

Open http://localhost:8000.

## Enquiry flow

1. Choose a property type and service.
2. Enter a location and project details.
3. Open the prepared enquiry in Gmail or WhatsApp, or download it as a text file.
4. Review the draft and send it in the selected service.

The website does not send messages automatically and has no form-processing backend. Gmail requires the visitor to sign in. Downloading a brief saves it locally without submitting it.

## Project structure

| File | Purpose |
| --- | --- |
| `index.html` | Page content, navigation and enquiry form |
| `app.js` | Service selection, draft links and brief download |
| `style.css` | Core page styling |
| `brand-colors.css` | Brand color styling |
| Other `.css` files | Section, illustration, logo and layout styling |
| `assets/bjm-logo.png` | Company logo |

## Customize and deploy

Update page copy and contact links in `index.html`. If the destination email address or WhatsApp number changes, update the corresponding values in `app.js` as well.

Upload the HTML, JavaScript, CSS and `assets/` directory to a static host. Preserve relative paths; no build command or server runtime is required.

## Manual verification

- Select a service link and confirm the form selection updates.
- Confirm required fields prevent empty enquiries.
- Check that Gmail and WhatsApp drafts contain the entered brief; sending is a separate user action.
- Download the brief and verify its text.
- Review navigation and layout at desktop and mobile widths.
