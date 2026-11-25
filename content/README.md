# Updating website content

Most routine updates belong in this folder. Each page has a JSON file with its editable copy and, where relevant, a list of published records. Layout, navigation, and styling live under `src/` and normally do not need changes for content updates.

## Files

- `home.json` — home page copy.
- `about.json` — center introduction, teachers, and board information.
- `retreats.json` — confirmed retreat entries and registration links.
- `teachings.json` — published talks and articles.
- `faq.json` — confirmed retreat questions and answers.
- `contact.json` — verified location and contact details.
- `support.json` — support copy and verified donation destination.

## Content PRs

1. Edit only the relevant JSON file for a content-only change.
2. Publish only information confirmed by the center. Leave lists empty and optional URLs blank until details are real and approved.
3. Retreat dates use ISO format (`YYYY-MM-DD`) in `startDate`, with a readable `dateLabel`; include a registration URL only when it is the actual destination.
4. Teaching links must point to the approved article or video. Do not add private or personal information.
5. Keep JSON valid (quoted keys and strings, commas between fields). The site build checks the files before deployment; invalid JSON will stop the build.

An empty list means there are no entries to show yet. The website displays a plain empty state instead of sample or tentative content.
