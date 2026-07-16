# Jianjun Zhu's Academic Homepage

This repository contains the source code for [Jianjun Zhu's academic homepage](https://jianjunzhu.github.io/).

The website introduces my academic background, research interests, selected publications, research grants, professional service, awards, and teaching activities. My research focuses on medical image computing, computer-assisted intervention, and interventional surgical robotics.

## Website content

- **Profile and CV:** `_pages/about.md`
- **Teaching records:** `_teaching/`
- **Publication records:** `_publications/`
- **Site information and author links:** `_config.yml`
- **Navigation settings:** `_data/navigation.yml`
- **Images and downloadable files:** `images/` and `files/`

The page layout and visual styling are provided by the Academic Pages Jekyll theme. Most routine updates only require editing the Markdown content or `_config.yml`.

## Running locally

The site is built with Jekyll and GitHub Pages.

1. Install Ruby and Bundler.
2. Install the project dependencies:

   ```bash
   bundle install
   ```

3. Start the local development server:

   ```bash
   bundle exec jekyll serve --livereload
   ```

4. Open `http://localhost:4000/` in a browser.

If Bundler cannot write to the system Ruby directories, install dependencies inside the repository:

```bash
bundle config set --local path vendor/bundle
bundle install
```

## Updating the site

Before publishing an update:

1. Review names, dates, affiliations, publication details, and external links.
2. Run the site locally and check the homepage and teaching pages.
3. Commit only the intended content changes.
4. Push the `master` branch to GitHub; GitHub Pages will rebuild the website automatically.

## Credits

This website is based on [Academic Pages](https://academicpages.github.io/), a Jekyll theme derived from [Minimal Mistakes](https://mmistakes.github.io/minimal-mistakes-jekyll-theme/).

The repository is distributed under the terms described in [LICENSE](LICENSE).
