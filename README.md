# Hamdoon Ijaz

Academic personal site for Hamdoon Ijaz, a Ph.D. student at The Hong Kong University of Science and Technology. The layout is [Academic Pages](https://github.com/academicpages/academicpages.github.io) (a Minimal Mistakes Jekyll theme): a left sidebar with name, role, location, and institution, and a main column for the biography and publications.

The site is intended for GitHub Pages at <https://hamdoon-ust.github.io/>, from the repository `Hamdoon-UST.github.io`.

Adding a photo, paper, project, video, or talk is described in [HOW_TO_ADD_CONTENT.md](HOW_TO_ADD_CONTENT.md).

## Preview locally

Install Ruby, Bundler, Node.js, and a C compiler. On Debian or Ubuntu:

```bash
sudo apt install ruby-dev ruby-bundler nodejs build-essential
```

From this directory:

```bash
bundle config set --local path 'vendor/bundle'
bundle install
npm run build:js
bundle exec jekyll build
```

`bundle exec jekyll build` writes the site into `_site/`. That command is the check that the site builds.

To read it in a browser, with styles loaded from this machine:

```bash
bundle exec jekyll serve --host 127.0.0.1 --port 8642 --config _config.yml,_config_dev.yml
```

Then open <http://127.0.0.1:8642/>. `_config_dev.yml` is only for that local server. The GitHub Action uses `_config.yml` alone. The theme needs Jekyll 4, which is newer than GitHub’s classic Pages builder, so publishing uses the GitHub Actions workflow in `.github/workflows/jekyll.yml`. In the repository settings, set Pages to deploy from GitHub Actions. Pushing to `main` runs that workflow.

The sidebar photograph is `images/profile.jpg`.
