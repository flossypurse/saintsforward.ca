# Saints Forward Website

**Building the future of Spruce Grove soccer.**

A community initiative to secure dedicated indoor space and professional coaching for the Spruce Grove Saints Soccer Association (SGSA).

## Project Overview

This is a single-page static website designed to:
- Present the vision for SGSA's future with dedicated facilities and professional coaching
- Educate members, parents, and stakeholders with research-backed data
- Build community support for facility development and coaching investment
- Provide a respectful bridge for dialogue with the SGSA board

## File Structure

```
/
├── index.html                      # Main website (single-page)
├── assets/
│   ├── images/
│   │   ├── saints-forward-logo.svg
│   │   ├── saints-forward-logo-dark-bg.svg
│   │   ├── saints-forward-logo-compact.svg
│   │   ├── saints-forward-favicon.svg
│   │   └── saints-forward-og-image.svg
│   └── reports/                    # (optional) PDF reports for download
├── robots.txt                      # SEO configuration
├── .gitignore                      # Git ignore patterns
└── README.md                       # This file
```

## Technology Stack

- **HTML5** - Semantic markup
- **Tailwind CSS** - Utility-first CSS via CDN
- **Google Fonts** - Inter font family
- **Vanilla JavaScript** - Smooth scrolling and fade-in animations
- **No build process** - Simple, portable, and easy to deploy

## Design System

### Colors
- **Primary (Forest Green):** `#1B4332`
- **Secondary (Gold):** `#D4A843`
- **Background (Warm White):** `#F8F6F0`
- **Dark (Charcoal):** `#1A1A2E`

### Typography
- **Font Family:** Inter (Regular, Semibold, Bold, Black)
- **Body Text:** 16px minimum, line-height 1.6
- **Headings:** Bold to Black weight

### Layout
- **Max Content Width:** 1200px (7xl container)
- **Mobile-First:** Fully responsive design
- **Generous Whitespace:** Clean, breathable layout

## Content Sections

1. **Hero** - Full-width landing with project name and tagline
2. **Vision** - Aspirational description of SGSA's potential future
3. **Problem (Why Now?)** - Six fact cards with data-driven evidence
4. **Plan** - Two goals with detailed implementation plans:
   - Goal 1: Dedicated Indoor Facility (dome, costs, funding, precedents)
   - Goal 2: Professional Coaching Staff (positions, costs, examples)
5. **Get Involved** - Action items for community members and board outreach
6. **Footer** - Links, contact, disclaimer

## Deployment Options

### Option 1: Netlify (Recommended)
1. Create a free account at [netlify.com](https://www.netlify.com/)
2. Connect your GitHub repository
3. Deploy automatically on every push to main branch
4. Configure custom domain `saintsforward.ca`
5. SSL certificate automatically provisioned

### Option 2: Vercel
1. Create a free account at [vercel.com](https://vercel.com/)
2. Import your GitHub repository
3. Deploy with zero configuration
4. Add custom domain in project settings

### Option 3: GitHub Pages
1. Go to repository Settings → Pages
2. Select branch `main` and root folder
3. Save and wait for deployment
4. Configure custom domain in DNS settings

## Custom Domain Setup

Once deployed, configure your domain `saintsforward.ca`:

1. **Purchase domain** from Namecheap, Cloudflare Registrar, or similar (~$15/year for .ca)
2. **Add DNS records** (provided by your hosting service):
   - For Netlify/Vercel: Add CNAME record pointing to their nameservers
   - For GitHub Pages: Add A records + CNAME
3. **Enable SSL** (automatic on Netlify/Vercel/GitHub Pages)
4. **Test** - Visit `https://saintsforward.ca` to verify

## Content Updates

### To Update Text Content
1. Open `index.html` in any text editor
2. Find the section you want to update
3. Edit the text within the HTML tags
4. Save and commit changes
5. Push to GitHub (will auto-deploy if connected)

### To Replace Images
1. Replace the SVG files in `assets/images/` with your updated logos
2. Keep the same filenames for seamless replacement
3. Ensure images are optimized for web (SVG is ideal for logos)

### To Add a Hero Background Image
1. Add your hero image (e.g., `hero.jpg`) to `assets/images/`
2. Open `index.html` and find the Hero Section (line ~111)
3. Uncomment the background image `<img>` tag
4. Update the `src` attribute to point to your image
5. Optimize image for web (compress to < 200KB for fast loading)

## Performance Optimization

- **Image Compression:** Use tools like TinyPNG or ImageOptim
- **SVG Optimization:** Use SVGO for smaller vector files
- **Lazy Loading:** Images below the fold load only when scrolled into view
- **CDN Resources:** Tailwind CSS and Google Fonts load from CDN (cached globally)
- **Target:** Lighthouse score 95+ once real images are added

## Accessibility

The website follows WCAG AA standards:
- ✅ Semantic HTML5 structure
- ✅ Color contrast meets AA requirements
- ✅ Keyboard navigation supported
- ✅ Screen reader friendly
- ✅ Responsive typography (16px minimum)
- ✅ Alt text for all images (add to hero image when replaced)

## Browser Support

Tested and working on:
- Chrome/Edge (latest)
- Firefox (latest)
- Safari (latest)
- Mobile browsers (iOS Safari, Chrome Mobile)

## Contact

**Saints Forward Initiative**
Email: [hello@saintsforward.ca](mailto:hello@saintsforward.ca)

---

## For Developers

### Local Development
Simply open `index.html` in any browser. No build process or local server required.

### Git Workflow
```bash
# Make changes to index.html or assets
git add .
git commit -m "Update content"
git push origin main
```

### Repository
GitHub: [github.com/flossypurse/saintsforward.ca](https://github.com/flossypurse/saintsforward.ca)

---

## Post-Launch Checklist

After deploying, complete these tasks:

- [ ] Verify all links work on live site
- [ ] Test responsive layout on mobile devices
- [ ] Check that all sections render correctly
- [ ] Verify smooth scrolling and animations
- [ ] Test social media sharing (Facebook, Twitter)
- [ ] Confirm contact email is correct
- [ ] Share with 5-10 trusted SGSA parents for feedback
- [ ] Make any final adjustments based on feedback
- [ ] Announce to broader SGSA community

---

**Built with care for the Spruce Grove soccer community. ⚽**
