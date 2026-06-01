# Dave Pequite Carpentry — Website

Fort Collins, CO independent framing & finish carpentry.  
Built with plain HTML/CSS/JS — no frameworks, no build tools, easy for anyone to maintain.

---

## Quick Start (GitHub Pages)

1. **Create a new repository** on GitHub named `dave-pequite-carpentry` (or `davepequite.com` if using a custom domain)
2. **Upload all files** in this folder to the repository root
3. Go to **Settings → Pages → Source** → select `main` branch → `/ (root)`
4. Your site will be live at `https://yourusername.github.io/dave-pequite-carpentry/`

---

## Custom Domain Setup (davepequite.com)

1. Buy the domain `davepequite.com` from Namecheap, Google Domains, or similar (~$12/year)
2. In your domain registrar, add these DNS records:
   ```
   A     @    185.199.108.153
   A     @    185.199.109.153
   A     @    185.199.110.153
   A     @    185.199.111.153
   CNAME www  yourusername.github.io
   ```
3. In GitHub Pages settings, enter `davepequite.com` under Custom Domain
4. Check "Enforce HTTPS"

---

## Adding Dave's Photos

Add photos to the `images/` folder and update the `src=""` attributes in the HTML files.

### Recommended photos & filenames:
| Filename | Used on | Description |
|---|---|---|
| `dave-hero.jpg` | Homepage hero | Dave with his son at the climbing wall |
| `dave-climbing.jpg` | Story strip | Utah/Colorado climbing |
| `dave-dog-trail.jpg` | Story strip | Big laugh with dog on trail |
| `dave-son-climbing.jpg` | Story strip | Dave & son at the wall |
| `dave-canyon.jpg` | About page | Canyon country with dog |
| `dave-son-shoulders.jpg` | Dad moment | Son on shoulders, climbing wall |
| `dave-climbing-utah.jpg` | About gallery | Utah summit |
| `dave-son-gear.jpg` | About gallery | Gearing up together |
| `dave-dogs-moab.jpg` | About gallery | Moab with dogs |
| `dave-winter-son.jpg` | About gallery | Colorado winter |
| `dave-summit.jpg` | About gallery | Summit shot |

**Image tips:**
- Resize photos to max 1400px wide before uploading (keeps the site fast)
- Save as .jpg at 80% quality
- Free tool: squoosh.app

---

## Setting Up the Contact Form (Formspree)

The contact form sends submissions directly to Dave's email. Setup takes 5 minutes:

1. Go to **[formspree.io](https://formspree.io)** and create a free account
2. Click **"New Form"** and enter Dave's email address
3. Copy the form ID (looks like `xpwzrjkb`)
4. Open `contact.html` and replace `YOUR_FORMSPREE_ID` with your actual ID:
   ```html
   <form action="https://formspree.io/f/xpwzrjkb" ...>
   ```
5. The free plan handles 50 submissions/month. Upgrade anytime for more.

Every form submission will arrive in Dave's inbox with:
- Name, phone, email
- Project type & timeline
- Project description
- How they heard about Dave
- Whether they came from the lawn sign QR code

---

## Lawn Sign QR Code

The QR code on the lawn sign links to:
```
https://davepequite.com/contact.html?ref=sign
```

Forms submitted from the sign are automatically tagged `source: lawn-sign-qr` so Dave knows where the lead came from.

**To generate the QR code for printing:**
1. Go to **[qr.io](https://qr.io)** or **[qrcode-monkey.com](https://qrcode-monkey.com)**
2. Enter the URL: `https://davepequite.com/contact.html`
3. Set foreground color to `#1C1C18` (charcoal) or `#2D4A2A` (forest green)
4. Download as SVG or high-res PNG (minimum 300dpi for print)
5. Send to the sign printer along with the sign artwork

---

## File Structure

```
dave-pequite-carpentry/
├── index.html          # Homepage
├── about.html          # About Dave
├── portfolio.html      # Project gallery
├── accessibility.html  # Aging in place page
├── contact.html        # Contact + intake form
├── css/
│   └── style.css       # All styles
├── js/
│   └── main.js         # Nav, scroll effects
├── images/             # All photos go here
└── README.md           # This file
```

---

## SEO — Already Built In

The site includes:
- **Meta descriptions** on every page targeting Fort Collins carpentry keywords
- **Schema.org LocalBusiness markup** on the homepage (helps Google Maps & AI search)
- **Semantic HTML** (proper heading hierarchy, nav, main, footer)
- **Alt text** on all images
- **Mobile responsive** layout
- **Fast loading** — no JavaScript frameworks

**After launching, also set up:**
- [ ] Google Business Profile (free — critical for local search)
- [ ] Submit sitemap to Google Search Console
- [ ] Create profiles on Houzz and Nextdoor

---

## Updating Content

Everything is plain HTML — open any `.html` file in a text editor and change the text directly. No special tools needed.

**To add a review:** Find the `reviews-grid` div in `index.html` and copy/paste a `review-card` block.

**To add portfolio photos:** Add the image file to `images/`, then add a new `portfolio-item` block in `portfolio.html`.

---

## Contact

Dave Pequite — (970) 749-8800  
Fort Collins, Colorado
