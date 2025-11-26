# VAT EPR EXPERT FRANCE - Marketing Website

A professional, Webflow-compatible marketing website for **VAT EPR EXPERT FRANCE**, a French firm specialising in VAT fiscal representation and EPR authorised representation for cross-border e-commerce sellers and their partners.

## Overview

This website is built using HTFlow, a framework for creating Webflow-compatible static sites. The site presents VAT EPR EXPERT FRANCE's services to:

- **Partners**: Tax firms, marketplaces, platforms, and logistics providers
- **E-commerce sellers**: EU and non-EU sellers needing French VAT and/or EPR compliance
- **Regulators**: French authorities and eco-organisations

## Project Structure

```
vat-epr-expert-france-site/
├── src/
│   ├── index.html                    # Home page
│   ├── vat-representation.html       # VAT fiscal representation service
│   ├── epr-representation.html       # EPR authorised representation service
│   ├── faq.html                      # Frequently asked questions
│   ├── contact.html                  # Contact form and information
│   └── blog/
│       ├── index.html                # Blog listing page
│       └── post-template.html        # Single blog post template
├── .htflowrc.json                    # HTFlow configuration
├── package.json                      # Node.js dependencies and scripts
└── README.md                         # This file
```

## Installation

1. Navigate to the project directory:
   ```bash
   cd vat-epr-expert-france-site
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

## Development

Start the development server:

```bash
npm run dev
```

This will start the HTFlow development server, typically at `http://localhost:3000`.

## Production

Start the production server (required for HTFlow → Webflow integration):

```bash
npm run serve
```

This starts the production server that the HTFlow Chrome extension connects to for copying pages into Webflow.

## HTFlow → Webflow Workflow

### Copying Pages to Webflow

1. Start the production server: `npm run serve`
2. Open the HTFlow Chrome extension
3. Connect to your Webflow project
4. Select a page from this site
5. Copy to Webflow as native components

### Blog CMS Mapping

When setting up the blog in Webflow CMS, create a Collection with these fields:

| Field Name | Type | Description |
|------------|------|-------------|
| `title` | Plain Text | Article title |
| `slug` | Plain Text | URL slug |
| `category` | Reference / Option | VAT, EPR, or Partners |
| `excerpt` | Plain Text | Short summary for listings |
| `body` | Rich Text | Full article content |
| `author` | Reference | Author reference |
| `published_date` | Date | Publication date |
| `featured_image` | Image | Optional featured image |

## Design System

### Colors

| Token | Value | Usage |
|-------|-------|-------|
| Primary | `#1E3A8A` | Trust/main brand color |
| Secondary | `#10B981` | Compliance/success |
| Accent | `#F59E0B` | Highlights (non-price) |
| Background | `#F9FAFB` | Light sections |
| Text | `#111827` | Primary text |

### Typography

- **Font**: Inter (loaded from Google Fonts)
- **H1**: 2.25–3rem, 700 weight
- **H2**: 1.75–2.25rem, 700 weight
- **H3**: 1.25–1.5rem, 600–700 weight
- **Body**: 1–1.0625rem, 400 weight

### Breakpoints

HTFlow uses these responsive breakpoints:

- Desktop: default
- Tablet: `max-width: 991px`
- Mobile Landscape: `max-width: 767px`
- Mobile Portrait: `max-width: 479px`

### Component Classes

All classes use the `veef-` prefix (VAT EPR EXPERT FRANCE):

- `.veef-container` - Content container
- `.veef-button` / `.veef-button--primary` / `.veef-button--secondary` - Buttons
- `.veef-section` / `.veef-section--gray` - Page sections
- `.veef-header` / `.veef-footer` - Navigation
- `.veef-faq-item` - FAQ accordions
- `.veef-blog-card` - Blog article cards

## Pages

### Home (`index.html`)
- Hero with value proposition and CTAs
- Services overview (VAT & EPR)
- Audience sections (Partners & Sellers)
- Why choose us
- How it works (3-step process)
- Founder section
- Blog preview
- Final CTA

### VAT Representation (`vat-representation.html`)
- Service explanation
- Who it's for
- What we do (before/during)
- Partner section
- Mini FAQ

### EPR Representation (`epr-representation.html`)
- EPR explanation
- Product categories
- Who needs representation
- What we do
- VAT + EPR combined benefits
- Mini FAQ

### FAQ (`faq.html`)
- Accordion-style FAQ
- Organised by category (VAT, EPR, Firm)

### Contact (`contact.html`)
- Contact form
- Direct contact information
- Practical details
- Map placeholder

### Blog (`blog/`)
- Index with article grid and sidebar
- Post template for articles

## Placeholders

The following items are marked as placeholders for Tristan to fill in:

- Company legal name
- Legal form (SARL, SAS, etc.)
- Share capital
- RCS registration
- SIREN number
- VAT number
- Professional liability insurance
- Contact email
- Contact phone
- Office address/city
- Response time
- Office hours

All placeholders are styled in gold (`#F59E0B`) and italic for easy identification.

## Important Notes

- **No pricing**: The site intentionally contains no pricing information
- **No regulatory claims**: No claims about official approvals or certifications
- **Partner focus**: The messaging emphasises partner relationships throughout
- **HTFlow compliance**: All code follows HTFlow conventions for Webflow compatibility
  - Internal `<style data-ht-styles>` tags
  - Internal `<script data-ht-main-script>` tags
  - `data-ht-*` attributes for JavaScript DOM selection
  - `.htflow-wrapper` container

## License

UNLICENSED - Proprietary

---

Built with HTFlow for VAT EPR EXPERT FRANCE by Tristan Perot.

