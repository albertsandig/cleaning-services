# MJG Cleaning Services: project docs

Planning documents for the MJG Cleaning Services redesign. Read these before starting the Laravel build.

## Documents

| Document | What it's for | Audience |
|---|---|---|
| [01-website-audit.md](01-website-audit.md) | What's wrong with the current site, how it compares, and which pages to build | Project team |
| [02-90-day-roadmap.md](02-90-day-roadmap.md) | The plan for leads, trust, SEO, booking, reviews and photos | Business owner |
| [03-homepage-copy.md](03-homepage-copy.md) | Homepage wording, including form and error messages | Owner and project team |
| [04-homepage-prototype.html](04-homepage-prototype.html) | Working homepage design in Tailwind. Open it in a browser. | Owner and project team |
| [05-owner-top-10.md](05-owner-top-10.md) | How to pitch the redesign, and the top 10 revenue improvements | Whoever presents the proposal |
| [prompts.md](prompts.md) | The original briefs, word for word | Project team |

## What we know about the business

From the live website on November 4, 2026. The owner should still confirm these.

| Item | Current information |
|---|---|
| Name | MJG Cleaning Services Inc. (the site also uses other versions) |
| Phone | 705-465-1721 |
| Email | cleaningmjg@gmail.com |
| Location | Timmins, Ontario |
| Service area | "Timmins, Ontario and the surrounding areas" |
| Services | Residential, commercial and deep cleaning |
| Stated claims | Locally owned and operated, brings own supplies and equipment, "years of experience" |

## Questions for the owner

The copy and prototype can't be finalized until these are answered. Each answer replaces a marked placeholder.

**Business**

1. What is the legal name, and what public name should be used everywhere?
2. What year did the business start, and who should the About page name?
3. What are the business hours?
4. Which communities are served, and how far will the team travel?
5. Can the team serve customers in French?

**Trust**

6. What liability insurance is in place, and for how much? Is WSIB coverage in place? Is the business bonded?
7. What guarantee is the owner willing to put in writing?
8. Are there existing Google reviews? Does a Google Business Profile exist?
9. Are there real job photos, and permission to use them?

**Services and pricing**

10. What exactly is included in each service?
11. Are move-in and move-out or post-construction cleans offered?
12. Which schedules are offered, including evenings and weekends?
13. Are quotes free? Should a starting price be published?
14. Do customers need to be home during the clean?

**Operations**

15. Who responds to leads, how quickly, and on which phone?
16. Is an email at the business's own domain wanted?
17. Who controls the domain and the current Webador account?

## Notes for the Laravel build

Starting points, not final technical decisions:

- **Pages:** Build from the page list in [section 6 of the audit](01-website-audit.md#6-recommended-pages-and-sections).
- **Tailwind:** The prototype uses the CDN for convenience. Compile Tailwind through Vite in production.
- **Quote requests:** Save each one in the database as well as sending a notification, so no lead depends on email alone. Include spam protection and record the lead source.
- **Owner-managed content:** The owner will need a simple way to manage gallery items and selected reviews from a phone. Include a permission record for each gallery item.
- **SEO:** Set a unique title and description per page, `LocalBusiness` structured data and a sitemap. Redirect `/about-us` to any new About URL.
- **Measurement:** Track tap-to-call clicks and quote form submissions from launch.

**Remove from the prototype before launch:**

- The prototype notice bar
- All highlighted `confirm` marks
- The `noindex` tag
- The placeholder illustrations and review slots
- The form's "does not send" behaviour
