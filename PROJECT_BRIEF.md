# Theravada Buddhist Center Website — Project Brief

## Purpose

Plan a simple, welcoming static website for a Theravada Buddhist center. The site should share the center's community, teachings, schedule, and practical information.

## Principles

- Static website; no user login and no collection of user data.
- Simple, accessible design that works well in desktop and mobile web browsers.
- Traditional visual style, with clear and easy-to-use navigation.
- Use [atamma.org](https://atamma.org/) as a reference for the type of center website, without copying it. Aim for a better-organized, simpler experience.

## Content and features

### About

- Center introduction and background.
- Board members.
- Teachers.

### Events and practice schedule

- Events calendar.
- Meditation and retreat schedules.

### Teachers and teachings

- Teacher profiles.
- Teachings, including YouTube videos and articles.

### Practical information

- Donation links.
- Contact information.
- Center location and directions.

## Language support

- Consider bilingual content in Thai and US English (English as used in the United States).
- Confirm translation and language-switching needs during planning.

## Optional idea

- Consider offering background chanting audio for visitors, with an obvious option to turn it off. This is not a core requirement and should be designed so audio never surprises or disrupts visitors.

## Logistics and maintenance

- The website is not expected to receive frequent updates.
- Trusted developers will make updates; there is no requirement for a public editing interface or CMS.
- Keep content separate from presentation where it makes updates clearer and safer. For a small site, use straightforward Markdown files for longer pages and teachings, and structured data (such as JSON or YAML) for repeatable items like teachers, board members, and events. Avoid adding a CMS or elaborate content pipeline unless maintenance needs change.

## Implementation direction (initial recommendation)

- Chosen direction: Astro, using native Astro components and CSS without React. The site is simple and does not need a client-side application framework.
- Keep the design and page layouts stable after the initial design is approved; future updates are expected to be mostly content changes.
- Store content in files with a consistent format, separate from presentation where practical. Use Markdown for longer pages and teachings, and structured data for repeatable items such as teachers, board members, and events. Add schema validation for repeated content where useful.
- Keep client-side JavaScript minimal and limited to features that need it.
- Keep the calendar simple and manually maintained at first; link to an external calendar only if the center already relies on one.
