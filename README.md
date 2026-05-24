# AUA Technologies — Official Website

**Bridging Technology, Research and Innovation for Sustainable Impact.**

This repository contains the official website of AUA Technologies Pvt. Ltd., the parent company of [GIRA Global](https://giraglobal.org) and [PhonDekho](https://www.phondekho.com).

---

## 🗂️ Project Structure

```
aua-technologies/
├── index.html          ← Main website (single page)
├── css/
│   └── style.css       ← All styles
├── js/
│   └── main.js         ← Interactions & animations
└── README.md
```

## 🚀 Deploying to GitHub Pages

1. Push this repository to GitHub
2. Go to **Settings → Pages**
3. Under **Source**, select `main` branch, root folder `/`
4. Click **Save** — your site will be live at `https://<your-username>.github.io/<repo-name>/`

## 🌐 Linking to a Custom Domain

1. In **Settings → Pages → Custom Domain**, enter your domain (e.g. `auatechnologies.com`)
2. With your domain registrar, add these DNS records:

   | Type  | Name | Value                          |
   |-------|------|-------------------------------|
   | A     | @    | 185.199.108.153               |
   | A     | @    | 185.199.109.153               |
   | A     | @    | 185.199.110.153               |
   | A     | @    | 185.199.111.153               |
   | CNAME | www  | `<your-username>.github.io`   |

3. Check **Enforce HTTPS** once DNS propagates (may take up to 48 hours)

## ✏️ Updating Content

All content is in `index.html`. Key sections:

- **Hero tagline** — `#hero .hero-title`
- **Contact details** — `#contact .contact-info-list`
- **Office address** — Replace `India Office — Address on Enquiry`
- **Phone number** — Add to contact info section
- **Form handling** — In `js/main.js`, replace the mock `setTimeout` with your preferred service (Formspree, EmailJS, or a backend endpoint)

## 📬 Contact Form Setup (Formspree — free)

1. Sign up at [formspree.io](https://formspree.io)
2. Create a new form and get your endpoint URL
3. In `index.html`, change `<form id="contact-form">` to:
   ```html
   <form id="contact-form" action="https://formspree.io/f/YOUR_ID" method="POST">
   ```
4. Remove the mock handler in `main.js` and let the form post natively

---

© 2025 AUA Technologies Pvt. Ltd.
