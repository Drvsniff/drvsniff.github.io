# DrvSniff wiki

MkDocs Material wiki. Every push to `main` deploys to https://drvsniff.github.io/wiki/

## One-time setup (needs a computer)

1. Create an empty repo named `wiki` under `drvsniff`.
2. In this folder run:
   `git init && git add -A && git commit -m "wiki" && git branch -M main && git remote add origin https://github.com/drvsniff/wiki.git && git push -u origin main`
3. Repo Settings, Pages, Source: **GitHub Actions**. Then re-run the failed or pending workflow in the Actions tab.
4. Open https://drvsniff.github.io/wiki/maker/ on your phone and add it to your home screen.

Use git for step 2 rather than the web uploader: the `.github` folder and the `.nav.yml` files are hidden files and are easy to miss.

## Adding pages (any device)

Use the page maker, or add a `.md` file under `docs/<section>/`. New pages appear in the nav on their own. Section names come from each folder's `.nav.yml`. To add a section, make a folder with `index.md` and `.nav.yml`, then list it in `docs/.nav.yml`.

## Notes

- Assumes repo `drvsniff/wiki`, branch `main`. If you rename it, change `repo_url` and `edit_uri` in `mkdocs.yml` and the Repository box in the page maker.
- Material for MkDocs is in maintenance mode (bug and security fixes only). Zensical, from the same team, reads `mkdocs.yml`, so you can switch later.
- Preview locally: `pip install -r requirements.txt && mkdocs serve`
