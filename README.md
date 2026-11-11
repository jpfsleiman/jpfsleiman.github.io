# jpfsleiman.github.io

Personal site for JohnPaul Sleiman. Built with Jekyll, which GitHub Pages runs for you: change a file in this repository and the live site rebuilds in about a minute.

## Where things live

| To change | Edit |
|---|---|
| Menu | `_data/nav.yml` |
| Home page text | `index.html` |
| About page text | `about.html` |
| Career column on the About page | `_data/career.yml` |
| Résumé page (experience, volunteering, education) | `_data/resume.yml` |
| Home page photo | replace `assets/img/portrait.jpg` (keep the same file name) |
| Papers and the policy memo | `_data/publications.yml` |
| Research project write-ups | `research.html` |
| Photos on Field notes | `_data/photos.yml` and `assets/img/` |
| Résumé PDF | replace `assets/files/JohnPaul_Sleiman_Resume.pdf` (keep the same file name) |
| Email, LinkedIn, GitHub, ORCID links | `_config.yml` |
| Colors and fonts | the top of `assets/css/site.css` |

## Add a post from the Hill

1. In the `_posts` folder, choose **Add file → Create new file**.
2. Name it `YEAR-MONTH-DAY-short-title.md`, for example `2026-12-03-what-a-markup-looks-like.md`.
3. Paste this at the top, change it, then write the post underneath:

```
---
title: "What a markup looks like from the staff bench"
date: 2026-12-03
summary: One sentence that appears in lists.
topics: [energy, oversight]
---

Your post starts here.
```

4. Commit. The post appears on the home page, on the On the Hill page, and under each of its topics on the Topics page.

## Add an op-ed

1. In the `_opeds` folder, create a file named `short-title.md`.
2. Paste this at the top and change it:

```
---
title: "The op-ed's headline"
date: 2025-10-14
publication: Campus Times
summary: One sentence saying what it argues.
topics: [science funding]
external_url: https://link-to-the-original
---
```

3. Either stop there (the Writing page will link straight to the original) or paste the full text underneath to host it here.

## Add a photo

1. Upload the image to `assets/img/`. Use a `.jpg` under about 500 KB. iPhone photos are often HEIC files even when named `.jpg`, and most browsers cannot show those, so export as JPEG first.
2. Add a block to `_data/photos.yml`:

```
- image: file-name.jpg
  alt: One sentence describing the picture.
  caption: What the visitor reads.
  where: Place, year
```

## Add a paper

Copy a block in `_data/publications.yml` and change the details. Add `url:` for the DOI link and, where the journal allows it, `pdf:` for a file you uploaded to `assets/files/`.

## Placeholders

Anything with `placeholder: true` shows a yellow "Placeholder" badge. To hide every placeholder at once, set `show_placeholders: false` in `_config.yml`. Delete the placeholder files once real ones replace them.

## Preview on your own computer (optional)

```
bundle install
bundle exec jekyll serve
```

Then open http://localhost:4000.
