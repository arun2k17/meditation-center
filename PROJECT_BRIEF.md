# Theravada Buddhist Center Website — Project Brief

## Purpose

Plan a simple, welcoming static website for a Theravada Buddhist center. The current planning focus is retreats and the practical information visitors need to understand and sign up for them.

- Working name: Northwest Meditation Center.
- Main menu: About, Retreats, Teachings (talks and articles), Contact, Support. Each item has its own page.
- Use the main navigation only for now; add a secondary in-page menu only if a page grows long enough to benefit from section links.

## Principles

- Static website; no user login and no collection of user data.
- Treat the website as copyrighted and proprietary; do not include an open-source license in the repository.
- Simple, accessible design that works well in desktop and mobile web browsers.
- Traditional visual style should be visible in the design: warm paper backgrounds, layered/blended imagery, and restrained floral or lotus details that gently suggest Thai culture and Buddhism while keeping text readable.
- Use decorative flower linework and soft floral backgrounds as accents, not dense wallpaper. Keep the overall layout simple and accessible.
- Use the center’s supplied logo and photographs. Blend photographs into the hero, story sections, and retreat banners rather than adding a separate gallery page for the initial design.
- Center identity details supplied by the user: Bellingham, Washington; nwmeditationcenter@gmail.com; (425) 773-1789; Facebook page `https://www.facebook.com/NWmeditationcenter`. Use the supplied Practical Approach tagline in center copy.
- Use [atamma.org](https://atamma.org/) as a reference for the type of center website, without copying it. Aim for a better-organized, simpler experience.

## Content and features

### Current scope: retreats

- Focus the site on retreats. Do not list chanting, meditation sessions, or other regular activities as current offerings.
- The center is considering holding two retreats per month: one short retreat of about 3 days and one longer retreat of about 5 days.
- Frequency, duration, dates, program, and logistics are all undecided. Present these as tentative planning options, and keep the design flexible so duration does not affect the layout.
- For design review, show a realistic two-month sample schedule: Dec 4–6 and Dec 18–22, 2026; Jan 8–10 and Jan 22–26, 2027. Label every date clearly as sample/tentative until approved.
- Provide a clear sign-up link when the registration destination is chosen.
- Include a retreat FAQ for prospective participants.
- Atamma.org may be used as a source of topic ideas for practical retreat information (for example, registration, meals, lodging, costs/donations, and what to bring). Write original copy and verify all center-specific policies before publishing.

### About

- Center introduction and background.
- Board members.
- Teachers.

### Teachings

- Talks and articles, with links to approved source material such as YouTube videos.

### Practical information

- Contact page with center location and directions.
- Separate Support page with donation links.

## Language support

- Consider bilingual content in Thai and US English (English as used in the United States).
- Confirm translation and language-switching needs during planning.

## Logistics and maintenance

- The website is not expected to receive frequent updates.
- Trusted developers will make updates; there is no requirement for a public editing interface or CMS.
- Keep content separate from presentation where it makes updates clearer and safer. For a small site, use straightforward Markdown files for longer pages and teachings, and structured data (such as JSON or YAML) for repeatable items like teachers, board members, and events. Avoid adding a CMS or elaborate content pipeline unless maintenance needs change.

## Implementation direction (initial recommendation)

- Chosen direction: Astro, using native Astro components and CSS without React. The site is simple and does not need a client-side application framework.
- Hosting direction: GitHub Pages, built and deployed from `main` with GitHub Actions. Keep generated `dist/` output out of source control; set Astro's base path for the repository URL.
- Keep the design and page layouts stable after the initial design is approved; future updates are expected to be mostly content changes.
- Navigation and footer decisions: use uniform styling for all main-menu links, including Support; omit footer navigation and separate footer branding/tagline; keep a centered copyright notice naming the center.
- Store content in files with a consistent format, separate from presentation where practical. Use Markdown for longer pages and teachings, and structured data for repeatable items such as teachers, board members, and events. Add schema validation for repeated content where useful.
- Keep client-side JavaScript minimal and limited to features that need it.
- Keep the calendar simple and manually maintained at first; link to an external calendar only if the center already relies on one.
