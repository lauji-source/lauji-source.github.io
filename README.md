# Company Website – Jekyll (GitHub Pages)

Multilingual company site built with Jekyll for GitHub Pages.  
**Languages:** English, French, Chinese, Spanish.

## Structure

- **`/`** – English (default)
- **`/fr/`** – Français
- **`/zh/`** – 中文
- **`/es/`** – Español

## Local development

1. Install Ruby and Bundler, then:

   ```bash
   bundle install
   bundle exec jekyll serve
   ```

2. Open **http://127.0.0.1:4000** (or the URL Jekyll prints).

## Deploy on GitHub Pages

1. Push this repo to GitHub.
2. In the repo: **Settings → Pages**.
3. Under **Source**, choose **Deploy from a branch**.
4. Branch: **main** (or **master**), folder: **/ (root)**.
5. Save. The site will be at `https://<username>.github.io/<repo-name>/`.

If the site is in a project repo (e.g. `websiteLaujiFR`), set in `_config.yml`:

```yaml
baseurl: "/websiteLaujiFR"
url: "https://yourusername.github.io"
```

## Customization

- **Company name / meta:** `_config.yml`
- **Texts (all languages):** `_data/translations/`  
  - `en.yml`, `fr.yml`, `zh.yml`, `es.yml`
- **Activity images:** replace placeholders in `assets/images/`:
  - `activity-a.svg` → your image for Activity A (e.g. `activity-a.jpg`)
  - `activity-b.svg` → your image for Activity B (e.g. `activity-b.jpg`)

If you use `.jpg`/`.png`, update the image paths in `_includes/activities.html` to match the new filenames.
