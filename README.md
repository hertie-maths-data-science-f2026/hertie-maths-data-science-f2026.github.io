<!-- SYSTEM-OWNED - do not edit. Generated and redeployed by the DSL course sync. -->

# hertie-maths-data-science-f2026 - auto-deployed course website

**Do not edit this repository.** It is machine-written: every sync rewrites the generated files below and pushing redeploys the site, so an edit here is overwritten and lost.

Its content comes from the cohort's `classroom-config/` files (`schedule.yml`, `people.yml`) and what the course org actually releases.

## What the sync owns

| Path | Holds |
| --- | --- |
| `_lectures/` | one page per session and lab |
| `_assignments/` | one page per handed-out assignment |
| `_events/` | exams, term dates, display-only rows |
| `_data/people.yml` | the staff cards |
| `_data/nav.yml` | the nav bar |
| `_data/materials.yml` | the All Materials index |
| the tab pages - `lectures.md`, `labs.md`, `readings.md`, `assignments.md`, `materials.md` | the wrappers the tabs point at |
| `_layouts/`, `_includes/`, `_sass/_course.scss` | how every page renders |
| `.github/workflows/deploy.yml` | the Pages build |
| `_config.yml` | the course identity keys, the pinned theme, and the `collections:`/`defaults:` the layouts need |

Each collection is CLEARED and rewritten on every sync, so a file you add to one disappears on the next run. The tab pages are rewritten too - they are generated wrappers, so put your own words in `index.md`, or in a page of your own linked from there.

## Everything else is yours

`index.md`, `schedule.md`, any page you add yourself, `_announcements/`, `_images/`, `Gemfile`, `.gitignore`, `_data/late_policy.yml`, `_data/previous_offering.yml`, further `_data/*.yml` - seeded once when the site is created, then never rewritten. Change them freely.

The rendering is not yours to change here: `_layouts/`, `_includes/` and `_sass/_course.scss` are shipped from `templates/site/` in the DSL teaching toolkit, and the rest of the styling from the shared `dsl-jekyll-theme`. An edit in this repo is overwritten on the next sync; open a PR against the toolkit instead, and every course site gets it.

If you edit a generated file anyway, the sync opens an issue naming the commit it overwrote, so the change can be copied back out of it.
