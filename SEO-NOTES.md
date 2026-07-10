# ACS Jammu — SEO Notes & Off-Site Checklist

This documents the on-site SEO already implemented in the code, plus the off-site steps **you** need to do (they can't be done in code). Together these are what get you ranking top for "best school in Jammu".

## ✅ Done in code
- One `<h1>` per page, `<html lang>`, full meta (robots, geo, theme-color, author).
- Open Graph + Twitter Card on both pages; local `og-image.jpg` (1200×630).
- Structured data (JSON-LD): School with both campuses (address + GPS), WebSite, VideoObject, FAQPage, BreadcrumbList — all validated.
- Favicon set (`favicon.ico`, `apple-touch-icon.png`, `icon-192/512.png`) + `site.webmanifest`.
- Images converted to WebP, compressed, sized, lazy-loaded; hero preloaded; 20 MB video → 7.6 MB.
- GA4 (`G-WR2L5K1P2H`) on both pages.
- Sitemap with image entries; robots.txt allows all + points to sitemap.
- NAP (Name/Address/Phone) consistent: Bantalab +91 72981 07471 / 181123; Rajpura +91 84920 12304 / 180001.
- **Content pages added (Jul 2026)** — real, standalone, keyword-targeted pages, all reusing the
  existing design (`style.css`), shared header/navbar/footer, and per-page SEO + JSON-LD:
  - `about.html` — About / history / vision & mission / director (AboutPage + Breadcrumb schema)
  - `academics.html` — Streams + curriculum by stage (Breadcrumb schema)
  - `admissions.html` — Admission process, classes, docs, enquiry form (FAQPage + Breadcrumb)
  - `results.html` — Board results & achievers (Breadcrumb; figures match site claims)
  - `facilities.html` — Facilities & infrastructure (Breadcrumb)
  - `gallery.html` — Campus photo gallery (ImageGallery + Breadcrumb)
  - `contact.html` — Both campuses, maps, directions, contact form (School + Breadcrumb)
  - `best-school-in-jammu.html` — re-skinned to the shared design (was a standalone CSS look)
  - Every page: unique title/description, canonical, OG + Twitter, geo meta, GA4, one H1,
    visible breadcrumb, and cross-links between pages. All 8 URLs added to `sitemap.xml`.
  - Nav + footer across the whole site now link these pages (true multi-page internal linking).
  - Note: `best-school-in-jammu.css` is now unused/orphaned — safe to delete.

## ⬜ Off-site — do these (highest impact for local ranking)
1. **Google Business Profile** — claim/verify a listing for BOTH campuses. Use the EXACT same name, address, phone as on the site. Add photos, hours, category "School". This is the single biggest lever for "school in Jammu" local results.
2. **Google Search Console** — the site already has a verification token. Log in at search.google.com/search-console, confirm ownership, and **re-submit `https://acsjammu.com/sitemap.xml`** (it now lists all 8 pages). Use "Request indexing" for each new page so they get crawled quickly.
3. **Bing Webmaster Tools** — import from Search Console and submit the sitemap.
4. **Local citations / directories** — list the school on JustDial, Sulekha, IndiaMART education, Schools.org.in, etc. Keep NAP identical everywhere (inconsistent addresses hurt ranking).
5. **Reviews** — ask parents to leave Google reviews. Volume + recency of reviews strongly affects local ranking. (Once you have real ratings, we can add `AggregateRating` schema.)
6. **Social** — Instagram is linked (`a.c.s_jammu`). If you create Facebook/YouTube pages, send me the URLs and I'll add them to `sameAs` schema + the footer.
7. **Backlinks** — get listed on JKBOSE affiliated-school lists, local news, education blogs.

## Notes / follow-ups
- No Facebook or YouTube URL provided yet — only Instagram is wired in.
- If you get a professional 1200×630 banner photo, replace `og-image.jpg` for a nicer social-share preview.
- ✅ Content pages (Admissions, Academics, Results, About, Facilities, Gallery, Contact) are now
  live and interlinked — done. A blog is still a good next step for long-tail keywords.
- **Reality check on "rank #1 for best school in Jammu":** the code now maxes out *on-page* SEO
  (content, keywords, structured data, internal links, sitemap). The remaining — and decisive —
  levers for the top spot are the **off-site** items above, especially Google Business Profile
  for both campuses and genuine Google reviews. Those cannot be done in code.
