# EOONG Landing Page - Agents Guide

## Development

When starting the dev server, use background mode:

```
astro dev --background
```

Manage the background server with `astro dev stop`, `astro dev status`, and `astro dev logs`.

## Documentation

Full documentation: https://docs.astro.build

Consult these guides before working on related tasks:

- [Adding pages, dynamic routes, or middleware](https://docs.astro.build/en/guides/routing/)
- [Working with Astro components](https://docs.astro.build/en/basics/astro-components/)
- [Using React, Vue, Svelte, or other framework components](https://docs.astro.build/en/guides/framework-components/)
- [Adding or managing content](https://docs.astro.build/en/guides/content-collections/)
- [Adding styles or using Tailwind](https://docs.astro.build/en/guides/styling/)
- [Supporting multiple languages](https://docs.astro.build/en/guides/internationalization/)

---

## EOONG Landing Page Build Instructions

### Project Overview

Build an **award-winning, high-conversion landing page** for EOONG - an IT consulting & development agency solving tech problems for small businesses in Africa. The page should be modern, clean, and professional while showcasing the company's diverse service offerings.

### Design & Branding

**Color Palette:**

- Primary: Extract the dominant color from the EOONG logo (located in `/src/assets/`)
- Secondary: Extract accent colors from the logo
- Neutral Base: White background (#FFFFFF)
- Text: Dark gray/charcoal for readability (#1F2937 or #111827)
- Accents: Use logo colors for CTAs, highlights, and interactive elements

**Logo Usage:**

- Import logo from `/src/assets/`
- Place prominently in navigation header
- Use consistent sizing across all pages
- Ensure logo works well on white background

**Typography & Spacing:**

- Use modern, clean sans-serif (Tailwind defaults or similar)
- Generous whitespace for breathing room
- Clear visual hierarchy (H1 → H2 → H3 → body)
- Readable line lengths (50-75 characters)

### Page Structure & Sections

Build the landing page with these key sections (in order):

#### 1. **Hero Section**

- Compelling headline: "Technology Solutions Built for African Small Businesses"
- Subheading: "Affordable IT. No Complexity. Just Results."
- Background: Clean white with subtle accent color accent (from logo)
- Call-to-action button(s): "Get Started" + "Learn More"
- Optional: Hero image or animated graphic (subtle, not flashy)
- Logo prominently displayed in top navigation

#### 2. **Value Proposition Section**

Display 4 key benefits with icons:

- 💰 **Affordability** - Premium solutions, small business prices
- ⚡ **Speed** - Problems solved in weeks, not months
- ✨ **Quality** - Professional code, not shortcuts
- 🎯 **Simplicity** - Tech explained clearly, no jargon

Use logo colors for icon backgrounds/accents.

#### 3. **Services Overview**

Grid layout (3 columns on desktop, 1 on mobile) showcasing main service categories:

Each card should include:

- Service icon
- Service name
- 1-2 sentence description
- Category examples (bullet points)
- Subtle hover effect (use logo accent colors)

Services to highlight:

1. **Web Development & Apps**
   - Websites, web apps, PWAs, landing pages

2. **Automation & Workflows**
   - Zapier/n8n, process automation, email workflows

3. **Data & Intelligence**
   - Custom dashboards, reporting, analytics

4. **Integrations**
   - CRM setup, accounting software, API connections

5. **E-commerce**
   - Store setup, payment processing, inventory

6. **Mobile Development**
   - iOS, Android, cross-platform apps

#### 4. **Why Choose EOONG**

Comparison or features section highlighting:

- 3-5 person lean team (not bloated)
- Proven expertise (frontend, backend, fullstack, mobile)
- Flexible engagement (projects or retainers)
- African market understanding
- Fast iteration & deployment
- Transparent process

#### 5. **How It Works**

3-4 step process timeline:

1. **Discover** - We understand your problem
2. **Plan** - We design the solution
3. **Build** - We deliver quickly
4. **Support** - We maintain & optimize

Use timeline/step visualization with logo colors.

#### 6. **Pricing Tiers** (Optional)

If included, show:

- Project-based pricing range examples
- Retainer plans (Tier 1, 2, 3)
- Call-to-action for custom quotes

Or just CTA to "Get a Quote"

#### 7. **Industries We Serve**

Quick showcase of diverse industries:

- E-commerce sellers
- Service businesses
- Local retail/restaurants
- Freelancers & solopreneurs
- Non-profits
- "...and many more"

#### 8. **Testimonials/Case Studies** (If available)

- Client quote + name + company
- Use logo colors for accent elements
- Keep it authentic (max 3 testimonials)

#### 9. **Call-to-Action Section**

Large, clear section before footer:

- Headline: "Ready to Solve Your Tech Problem?"
- Subtext: "Let's build something great together"
- Primary CTA button: "Start Your Project"
- Secondary option: "Schedule a Call"
- Contact info or form

#### 10. **Footer**

Clean footer with:

- Logo
- Quick links (Services, About, Contact)
- Social media links
- Contact email
- Copyright

### Technical Requirements

**Structure:**

- Single-page layout with smooth scrolling between sections
- OR multi-page (Home, Services, Contact, About) - your choice

**Responsiveness:**

- Perfect on mobile (< 768px)
- Tablet optimized (768px - 1024px)
- Desktop optimized (> 1024px)
- Test all breakpoints thoroughly

**Performance:**

- Fast load times (images optimized)
- Lighthouse score: 90+
- Mobile-friendly (Google PageSpeed friendly)

**Accessibility:**

- WCAG AA compliant
- Proper heading hierarchy
- Alt text on all images
- Color contrast meets standards
- Keyboard navigable

**Interactions:**

- Smooth scroll anchors between sections
- Hover states on all clickable elements
- Button animations (subtle, professional)
- Form inputs (if contact form included) with validation

### Design Patterns & Best Practices

**Modern Aesthetics:**

- Minimalist, clean design
- Generous whitespace
- Subtle shadows/elevation where appropriate
- Consistent border-radius and spacing
- Use logo accent colors strategically (not overwhelming)

**High-Conversion Elements:**

- Clear, action-oriented copy
- Multiple CTAs throughout (not just at bottom)
- Trust signals (company mission, team expertise)
- Problem-solution-action flow
- Mobile-first approach

**Interactions:**

- Parallax scrolling (optional, subtle)
- Fade-in animations on scroll
- Smooth button transitions
- Loading states visible
- Form success/error states clear

### Content Tone & Voice

- **Professional yet approachable** - Not stuffy corporate speak
- **Problem-focused** - Lead with client pain points
- **Action-oriented** - Clear next steps always visible
- **Local relevance** - Acknowledge African business context
- **Jargon-free** - Explain tech simply
- **Confident but humble** - Show expertise without arrogance

Example:
❌ "Leverage synergistic digital solutions to maximize operational efficiency"
✅ "We automate boring tasks so you can focus on growing"

### Key Messages to Convey

1. **You don't need a huge budget for great tech**
2. **Problems get solved fast here**
3. **This is a real team with real expertise**
4. **We understand small business challenges**
5. **We're easy to work with**
6. **Wide range of services = one stop shop**

### File Organization

```
src/
├── pages/
│   └── index.astro (main landing page)
├── components/
│   ├── Header.astro
│   ├── Hero.astro
│   ├── ValueProp.astro
│   ├── Services.astro
│   ├── WhyChoose.astro
│   ├── HowItWorks.astro
│   ├── CTA.astro
│   ├── Footer.astro
│   └── ... (other components)
├── assets/
│   ├── logo.{png/svg}
│   └── ... (other images)
└── styles/
    └── ... (Tailwind configuration)
```

### Browser Support

- Chrome/Edge: Latest
- Firefox: Latest
- Safari: Latest
- Mobile browsers: Latest versions

### Deployment Ready

- No console errors or warnings
- All links functional
- Forms working (if applicable)
- SEO meta tags included
- Open Graph tags for social sharing
- Favicon set

### Success Criteria

✅ Beautiful, modern design that stands out
✅ All 10 sections present and polished
✅ Logo colors integrated throughout
✅ White background primary
✅ Mobile-responsive and fast
✅ Clear CTAs throughout
✅ Professional copy that converts
✅ User can understand EOONG's value in 30 seconds
✅ Easy to add case studies/testimonials later
✅ Ready to send to potential clients

### Questions to Ask

- Should services be clickable/expandable for more details?
- Do we need a contact form or just email/call buttons?
- Should there be a blog/resources section?
- Do we showcase team members?
- Should pricing be visible or "contact for quote"?

---

**Build Instructions Complete.** Start with the Hero section and work downward. Ensure logo colors are extracted and used tastefully throughout. Keep the design clean, white, and professional—let the content and copy do the selling.
