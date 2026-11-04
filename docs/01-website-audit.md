# Website audit: MJG Cleaning Services

**Site:** https://www.mjg-cleaning-services.com/
**Audited:** November 4, 2026
**Business:** Home, commercial and deep cleaning in Timmins, Ontario

## Summary

The site looks tidy, but it does little to turn a visitor into a phone call or a quote request. Five problems matter most:

1. **The phone number is hard to use.** It isn't in the header or hero, and the page code has no tap-to-call link.
2. **The contact form doesn't ask for a phone number.** MJG can only reply by email, which is slower than a call.
3. **Parts of the site are dead ends.** All three "More info" service buttons have no link, and the About Us page is blank.
4. **There's nothing to prove the work is good.** The site has no reviews, real job photos, named people or insurance details, and its photos are stock images.
5. **Google has little to rank.** The site has three pages and no service pages, and its homepage title is just "MJG cleaning".

The first three fixes are small and can be made on the current site this week, before the Laravel rebuild starts.

## How this audit was done

| Checked directly | Not checked |
|---|---|
| Page text and raw HTML for all three pages | Google Business Profile, and whether MJG has one |
| Sitemap and robots.txt | Google rankings and search volumes |
| Desktop screenshots of the homepage and About page | Traffic, call and lead numbers |
| Business listings, through web searches | Real-phone testing and a PageSpeed test |

No conversion data was available, so impact ratings below are professional judgment, not measurements.

## What's already working

Keep these in the new site:

- A Timmins-area **705 phone number** and a clear statement that the business is locally owned
- An **FAQ section** (none of the five comparison homepages had one)
- HTTPS, a mobile viewport tag, a sitemap and page canonicals
- A useful selling point: "we bring our own cleaning supplies and equipment"

## 1. Weaknesses that reduce leads

| Priority | Problem | What we found | Fix |
|---|---|---|---|
| High | Phone number is buried | It first appears in the contact section near the bottom of the homepage. No `tel:` link exists in the HTML of any page. | Put a tap-to-call number in the header and hero, plus a fixed call bar on phones. |
| High | Form can't capture a callback number | Fields are Name, Email and Message only. | Ask for name, phone and service first. Make email optional. |
| High | Dead "More info" buttons | All three buttons are `<a>` tags with no `href`. | Link each one to a service page, or to a quote form with that service selected. |
| High | About Us page is blank | The page shows only the navigation and footer, confirmed in the HTML and a screenshot. | Publish the owner's story now. An empty page raises doubts about the business. |
| High | "Book Now" doesn't book | It leads to a general contact form. The FAQ also mentions a "website booking form" that doesn't exist. | Label the button "Get a free quote" until real booking exists, and correct the FAQ. |
| Medium | Hero says little | "Cleanliness is our priority, your satisfaction is our guarantee" doesn't say what MJG cleans or where. The text also runs across the stock photo's spray bottle. | Lead with service and place: "Timmins homes and workplaces, cleaned properly." |
| Medium | Homes and businesses get the same message | Homeowners, offices and commercial buyers all see one short paragraph. | Give each audience its own benefits and its own page. |
| Medium | Common objections go unanswered | The FAQ doesn't cover price, insurance, guarantee terms, or being home during the clean. | Expand the FAQ. See [03-homepage-copy.md](03-homepage-copy.md). |
| Medium | Leads can't be measured | No Google Analytics, Tag Manager or Meta Pixel code appears in the HTML. Webador may offer its own statistics, which wasn't checked. | Track calls and form submissions from launch. |
| Low | Weak button wording | The form button says "Submit form". | Use "Get my free quote". |

## 2. Trust issues

| Priority | Issue | What we found | Fix |
|---|---|---|---|
| High | No social proof | There are no reviews, ratings or testimonials on the site. Web searches didn't surface an MJG review listing, though Google Maps and Facebook weren't checked directly. | Start asking every customer for a Google review, then show real ones on the site. |
| High | Only stock photos | The images are Unsplash stock. The Residential card shows a desk with a calculator and laptops, and Deep Cleaning shows a robot vacuum. | Use real photos of jobs, the team and any vehicles. |
| High | Insurance isn't mentioned | The site has no mention of insurance, WSIB or bonding, while the local competitor below advertises all three. This matters most to commercial buyers. | Publish whichever are true. Offer proof on request. |
| High | No visible people | No owner name, team photo or founding story. "Years of experience" gives no number. | Add a named owner, a photo, a start year and a short reason the business exists. |
| Medium | Guarantee has no terms | "Your satisfaction is our guarantee" is the only statement. | Write it plainly, such as "Tell us within 24 hours and we'll re-clean it free." |
| Medium | Inconsistent name | Variations include "MJG Cleaning Services Inc.", "MJG Cleaning services", "MJG Cleaning" and "MJG cleaning". | Pick one public name and use it everywhere online. |
| Medium | Missing business details | No hours or named communities are listed. A public street address is optional if MJG works only at customer sites. | Publish hours and the actual service area. |
| Low | Signs of a DIY site | Gmail address, "Powered by Webador", and "Phone:-" punctuation. The phone is also formatted differently on two pages. | Use an @mjg-cleaning-services.com email and clean up the formatting. |
| Low | No privacy information | The form has no privacy note and the site has no privacy page. | Add a short note under the form and a privacy page. |

**To check on a real device:** in our screenshot, the Commercial Cleaning card had no image and the map was blank. Either could be a side effect of the automated capture.

## 3. Missing SEO opportunities

| Priority | Opportunity | Now | Recommended |
|---|---|---|---|
| High | Google Business Profile | Not checked | Claim and complete it. Google Maps is likely the biggest source of local leads. |
| High | Service pages | None. The sitemap has only `/`, `/about-us` and `/contact`. | One page each for residential, commercial and deep cleaning, then others MJG actually offers. |
| High | Page titles | Home: "MJG cleaning". Contact: "MJG Cleaning". | "House & Commercial Cleaning in Timmins, ON \| MJG Cleaning Services" |
| High | Meta descriptions | Home: "Cleaning contractors, commercial cleaning." About: empty. Contact: no description found. | Write one per page with the service, the place and a call to action. |
| High | Reviews | None found | Build steady Google reviews. Google lets businesses ask for them, within the rules in the roadmap. |
| Medium | Headings | The homepage has three H1s. About and Contact have none. | One clear H1 on each page. |
| Medium | Structured data | Only a basic `Organization` with a name and URL | `LocalBusiness` with phone, area served and hours. Add review data only when it's real and policy-compliant. |
| Medium | Local content | Timmins is mentioned, but no nearby communities are named. | Name the communities truly served, on one good service area page. |
| Medium | Directory listings | Not audited | Use the same name and phone on Google, Bing, Apple Maps, Facebook, BBB and HomeStars. |
| Medium | Image SEO | Both `<img>` tags have empty alt text. | Use real photos with descriptive filenames and alt text. |
| Low | Internal links | Only the navigation and two "Book Now" buttons link anywhere on the homepage. | Link services, gallery, reviews and the quote form to each other. |
| Later | French pages | English only | Timmins has a large francophone community. Add French pages if MJG can serve customers in French. |

**Search terms to validate.** No search volume data was available, so check these in Google Keyword Planner or Search Console before finalizing pages:

- `cleaning services Timmins`
- `house cleaning Timmins`
- `commercial cleaning Timmins`
- `office cleaning Timmins`
- `deep cleaning Timmins`
- `move out cleaning Timmins`
- `nettoyage Timmins`

## 4. Improvements that should increase quote requests

Listed in recommended order.

**This week, on the current site:**

1. Add the phone number to the top of the homepage and make it tap-to-call.
2. Add a required phone field to the form.
3. Link or remove the "More info" buttons.
4. Fill in the About Us page.
5. Rewrite the homepage title, description and hero headline.

**In the new site:**

6. Put a three-field quote form in the hero and repeat the call to action after each major section.
7. Keep Call and Free Quote buttons fixed on the phone screen.
8. Let each service button open the form with that service already selected.
9. Show the review rating and proof of insurance near each form.
10. Add a real before-and-after gallery.
11. Publish a written guarantee.
12. Show the three steps to getting a quote, and how quickly MJG replies.
13. Text the owner each new lead immediately.
14. Add a commercial page with scope, scheduling, documents and a walkthrough offer.

## 5. Comparison with leading cleaning websites

**Scope limits:** Five sites loaded: one local competitor and four established brands. These are well-known companies, not sites with proven conversion rates. Molly Maid US, Merry Maids, MaidPro, Two Maids, Maid Brigade, Bioclean and Handy failed to load, so they aren't included. Only homepages were reviewed, so "not seen" doesn't mean a site lacks that feature elsewhere.

| | MJG | Northern Star (Timmins) | Molly Maid Canada | Maid Right | The Cleaning Authority | JAN-PRO |
|---|---|---|---|---|---|---|
| **Market** | Home and commercial | Commercial and industrial | Home, light commercial | Home, light commercial | Home | Commercial |
| **Hero** | Slogan | "Professional Cleaning. Northern Reliability." | Professional cleaning you can trust | "House Cleaning Done Right" | "Cleaning Services for Residential Properties" | "The Highest Level of Commercial Cleaning Services – Guaranteed." |
| **Main call to action** | Book Now | Request Free Quote | Submit a Service Inquiry | Free Estimate | Get Pricing | Free Estimate |
| **Phone prominence** | Low | Footer only | High | Not in visible text | High | High |
| **Insurance claim** | Not seen | Insured, bonded, WSIB | Bonded, insured | Insured, bonded | Bonded, insured | Not seen |
| **Guarantee** | Slogan | Listed, no terms | "Not satisfied? We'll make it right." | Report in 24 hrs, fixed in 48 hrs | Next-day re-clean | "Guaranteed" claim, no terms |
| **Social proof** | None | 3 named testimonials | 5 testimonials | Award and rating badges | Not seen | Industry awards |
| **Before and after** | No | Yes | Not seen | Not seen | Not seen | Not seen |
| **Services listed** | 3 | 6 | 8–9 | 4 | 4 | 12 |
| **Service area** | Timmins and surrounding areas | 7 named communities | Postal code finder | Location finder | Not seen | ZIP code finder |
| **Prices on homepage** | No | No | No | No | No, but promotes immediate online quotes | No |

### What this means

**MJG is behind on the basics.** All five comparison sites lead with a clear service message and an estimate or inquiry action. Four of five make a bonded or insured claim, and each states some kind of guarantee.

**The real local benchmark is Northern Star.** Its site has quote buttons, insurance and WSIB claims, testimonials, seven named communities and a before-and-after gallery. A commercial buyer comparing the two sites today would likely see Northern Star as the safer choice. Its testimonial and compliance claims weren't independently verified.

**MJG has real openings:**

- **Homeowners:** Northern Star's homepage presents commercial and industrial services, leaving room to own residential cleaning in Timmins.
- **Phone:** Northern Star's listed number is a (437) number in its footer, while MJG can lead with a local 705 number.
- **Before and after:** Only one of the five sites showed this on its homepage, so a good gallery would stand out, especially to homeowners.
- **Guarantee:** Maid Right's specific time limits are more convincing than a general promise, and MJG can match that clarity.
- **Local service:** The national brands sell systems and scale. MJG can offer a known local team that answers the phone.

## 6. Recommended pages and sections

### Pages

| Page | Suggested URL | Priority | Purpose and main sections |
|---|---|---|---|
| Home | `/` | Launch | See the section list below |
| Residential cleaning | `/residential-cleaning` | Launch | What's included, frequency options, photos, reviews, FAQ, quote form |
| Commercial cleaning | `/commercial-cleaning` | Launch | Types of workplaces, scope, after-hours scheduling, insurance and WSIB, walkthrough request |
| Deep cleaning | `/deep-cleaning` | Launch | When to book, regular versus deep comparison, checklist, before and after, quote form |
| Free quote | `/quote` | Launch | Short form, phone number, what happens next, reassurance |
| Thank you | `/thank-you` | Launch | Confirmation, reply time, phone number. Also used to measure leads. |
| Before and after | `/before-after` | Launch | Real projects by service, each with a short description of the job |
| Reviews | `/reviews` | Launch | Google rating, real reviews, link to leave a review |
| About | `/about` | Launch | Owner, photo, story, team, values and proof of insurance |
| Service area | `/service-area` | Launch | Communities truly served, travel limits, local details |
| FAQ | `/faq` | Launch | Pricing, access, supplies, guarantee, scheduling, cancellations |
| Contact | `/contact` | Launch | Phone, email, hours, form, service area map |
| Privacy policy | `/privacy` | Launch | How form details are used and stored |
| Move-in and move-out | `/move-in-move-out-cleaning` | After launch, if offered | Landlords, tenants, real estate deadlines |
| Post-construction | `/post-construction-cleaning` | After launch, if offered | Builders and renovators, safety, scheduling |
| Careers | `/careers` | Later | Hiring, without crowding out customer pages |
| French pages | `/fr/` | Later, if MJG can serve in French | Translated home, services and quote form |

Avoid near-identical pages for each nearby town. Add a community page only when there's something specific to say, such as local jobs or reviews.

### Homepage sections, in order

1. Header with tap-to-call phone and quote button
2. Hero with service, place and short quote form
3. Trust strip with local ownership, supplies, insurance and guarantee
4. Benefits for homeowners, offices and commercial sites
5. Service cards, each with its own quote button
6. Before-and-after gallery
7. Three steps to a quote
8. Real customer reviews and Google rating
9. FAQ
10. Contact section with full quote form
11. Fixed Call and Free Quote bar on phones

## Sources

**MJG**
- [Homepage](https://www.mjg-cleaning-services.com/)
- [About Us](https://www.mjg-cleaning-services.com/about-us)
- [Contact](https://www.mjg-cleaning-services.com/contact)
- [Sitemap](https://www.mjg-cleaning-services.com/sitemap.xml)

**Comparison sites**
- [Northern Star Janitorial](https://www.northernstarjanitorial.ca/)
- [Molly Maid Canada](https://www.mollymaid.ca/)
- [Maid Right](https://www.maidright.com/)
- [The Cleaning Authority](https://www.thecleaningauthority.com/)
- [JAN-PRO](https://www.jan-pro.com/)
