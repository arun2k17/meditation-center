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
2. Keep the public copy natural and complete. Do not add editorial labels such as “sample,” “tentative,” or “placeholder.”
3. Retreat dates use ISO format (`YYYY-MM-DD`) in `startDate` and a readable date label. Keep event descriptions and durations in the same retreat record.
4. Use working links for registration, donation, teaching, and contact actions. Until the center supplies a destination, link to a relevant page on this site.
5. Keep JSON valid (quoted keys and strings, commas between fields). The site build checks the files before deployment; invalid JSON will stop the build.

The current copy and retreat entries are working content for shaping the site. Replace them through content PRs as the center’s final details are settled.
