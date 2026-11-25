# artemborisov.com

Source for [Artem Borisov’s personal website](https://artemborisov.com/).

A minimal, bilingual static site with dark and light themes, a short introduction, and downloadable CVs. Built with plain HTML and CSS, with no build step, JavaScript, or backend in the current site.

## Pages

| | English | Русский |
|---|---|---|
| Dark | [/](https://artemborisov.com/) | [/ru/](https://artemborisov.com/ru/) |
| Light | [/light/](https://artemborisov.com/light/) | [/light/ru/](https://artemborisov.com/light/ru/) |

## Structure

```text
index.html       English, dark theme
ru/              Russian, dark theme
light/           Light theme in English and Russian
site/            Shared stylesheets
cv/              Public CV PDFs in English and Russian
CNAME            Custom domain for GitHub Pages
```

The English pages link to the English CV; the Russian pages link to the Russian CV.

## Local preview

From the repository root:

```sh
python3 -m http.server 8000 --bind 127.0.0.1
```

Open <http://localhost:8000/>. Serve the repository root so that absolute stylesheet and CV paths resolve correctly.

## Deployment

GitHub Pages serves the repository root from `master` at **artemborisov.com**. Merging into `master` publishes the changes.

Make changes on a separate branch and open a pull request. Before merging, check all four page variants, language and theme navigation, stylesheet paths, and both CV downloads. Keep the copy consistent across languages and themes.

## Historical versions and licensing

Earlier versions used HTML5 UP templates, including [Aerial](https://html5up.net/aerial). The original Creative Commons Attribution 3.0 license text is retained in [LICENSE.txt](LICENSE.txt). This historical attribution does not assign a new license to the current site or CV documents.

Deleting a page from the current site does not erase it from Git history or other branches.
