# NextGen Human sample site

Sample website for the NextGen Human longevity, diagnostics and recovery centre in Mansarovar, Jaipur.

This is a static site: one `index.html` and an `img/` folder. There is no build step.

## Pages

All pages live in `index.html` and switch by the link hash.

| Link | Page |
| --- | --- |
| `#home` | Sanctuary (home), with FAQ and Discovery visit form |
| `#memberships` | Credit plans, credit calculator (`#credits`), sessions by how you feel (`#feel`), plan comparison (`#compare`) |
| `#programmes` | 16 programmes across Young & Marriage, Fat Loss, Athlete and C-Suite |
| `#diagnostics` | Diagnostics and technology cards, full session menu with prices and credits |
| `#classes` | Classes and cohorts timetable |
| `#journal` | Journal |
| `#portal` | Member portal sample, with the progress table (`#progress`) |
| `#team` | Care team roles and registrations |

## Run it

Open `index.html` in a browser, or serve the folder:

    npx serve .

## Deploy on Vercel

Import this repository in Vercel. Choose the "Other" framework preset, leave the build command empty and keep the output directory as the repository root.

## Before going live

- Prices, the class timetable, journal articles and member portal figures are illustrative samples.
- Membership plans follow Membership Plan v3 (credit wallets). Update the `TIERS`, `CM` and `MATRIX` data in `index.html` if the plan changes.
- Care team cards show roles only. Add real names and registration numbers once clinicians are appointed.
- The booking form prepares a WhatsApp message to +91 98290 88210. It does not send or store anything.
- Images are stills from the promotional video.
- Remove the "Sample site for review" bar at the top of `index.html`.
