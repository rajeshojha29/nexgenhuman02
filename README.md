# NextGen Human sample site

Sample website for the NextGen Human longevity, diagnostics and recovery centre in Mansarovar, Jaipur.

This is a static site: one `index.html`, an `img/` folder and a `video/` folder. There is no build step.

## Structure

The home page is a long scroll: video hero, introduction, six services, the space, programmes with questions, concern tiles, medical leadership, registrations, a video strip, the journal and a closing call to book. The top menu has dropdowns, and every other page sits on a sub-page with a breadcrumb and tabs. Pages switch by the link hash.

| Branch | Pages (link hash) |
| --- | --- |
| The centre | Our approach (`#centre`), Inside the centre (`#inside`), Recovery and skin (`#recovery`), Care team (`#team`) |
| Programmes | By goal (`#programmes`), All programmes (`#plist`) |
| Memberships | Plans and prices (`#memberships`), Plan finder (`#credits`), By how you feel (`#feel`), Compare plans (`#compare`) |
| Diagnostics & Tech | Featured sessions (`#diagnostics`), Full session menu (`#menu`) |
| Classes, journal and portal | `#classes`, `#journal`, Dashboard (`#portal`), Progress table (`#progress`) |
| Visit | Book a visit (`#visit`), Questions (`#faq`) |

To add a page, add a `data-sub` block inside the right `data-view` section and a matching entry in `ROUTES` in the script.

## Run it

Open `index.html` in a browser, or serve the folder:

    npx serve .

## Deploy on Vercel

Import this repository in Vercel. Choose the "Other" framework preset, leave the build command empty and keep the output directory as the repository root.

## Before going live

- Prices, the class timetable, journal articles and member portal figures are illustrative samples.
- Plan data lives in `TIERS`, `CM` and `MATRIX` in `index.html`.
- Care team cards show roles only. Add real names and registration numbers once clinicians are appointed.
- The booking form prepares a WhatsApp message to +1 832 292 7282. It does not send or store anything.
- Images are stills, and `video/` holds short silent loops cut from the promotional video (WebM and MP4 versions of each). Swap in the Higgsfield clips by replacing the files with the same names.
- Remove the "Sample site for review" bar at the top of `index.html`.
