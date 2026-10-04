# DrvSniff wiki

MkDocs Material wiki. Every push to `main` deploys to https://drvsniff.github.io/wiki/

## Adding pages (any device)

Use the page maker, or add a `.md` file under `docs/<section>/`. New pages appear in the nav on their own. Section names come from each folder's `.nav.yml`. To add a section, make a folder with `index.md` and `.nav.yml`, then list it in `docs/.nav.yml`.

## Notes

- Assumes repo `drvsniff/wiki`, branch `main`. If you rename it, change `repo_url` and `edit_uri` in `mkdocs.yml` and the Repository box in the page maker.
- Material for MkDocs is in maintenance mode (bug and security fixes only). Zensical, from the same team, reads `mkdocs.yml`, so you can switch later.
- Preview locally: `pip install -r requirements.txt && mkdocs serve`
