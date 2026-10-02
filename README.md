# www.atabertay.com

Source for Ata Can Bertay's academic website, built with [Quarto](https://quarto.org) and published by GitHub Pages. Every push to `main` rebuilds and publishes the site in about two minutes.

## Common updates

| To do this | Edit this |
| --- | --- |
| Add or update a published paper | `data/publications.yml` (newest first; copy an existing entry) |
| Add a working paper | `data/working-papers.yml` |
| Add a policy paper or technical note | `data/policy.yml` |
| Change which papers are featured | set `featured: true` and `featured_order` on 3 entries |
| Replace the CV | upload the new PDF as `files/cv.pdf` (keep the name so links never break) |
| Add a news item | the News list in `index.qmd` |
| Change the bio or contact details | `index.qmd`; email lives in `_variables.yml` |
| Teaching | `teaching.qmd` |
| Columns, press, policy work | `media.qmd` |

Paper PDFs go in `files/` and are linked as `files/name.pdf`.

## Editing without installing anything

Open a file on github.com, click the pencil icon, edit, then "Commit changes". The Actions tab shows the rebuild; the site updates when it turns green.

## Previewing locally (optional)

Install Quarto, then run `quarto preview` in this folder.

## Automatic checks

`.github/workflows/link-check.yml` checks every link on the 1st of each month and opens an issue listing any that are broken.
