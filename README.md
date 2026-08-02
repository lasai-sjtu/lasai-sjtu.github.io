# LaSAI research lab website

This repository contains the source for the LaSAI (Language Science & Artificial Intelligence) research lab website at Shanghai Jiao Tong University.

Website: [https://lasai-sjtu.github.io](https://lasai-sjtu.github.io)

The site is built with [Jekyll](https://jekyllrb.com/) and adapted from the [MaiNLP lab website](https://github.com/mainlp/mainlp.github.io), which is based on the [al-folio](https://github.com/alshedivat/al-folio) theme. The inherited theme code remains available under the MIT License; see [LICENSE](LICENSE).

## Local preview

```bash
bundle install
bundle exec jekyll serve
```

Then open `http://localhost:4000`.

## Main content locations

- `_pages/about.md` — homepage, news, and team
- `_pages/projects.md` — Research page
- `_pages/events.md` — events
- `_pages/publications.md` — publication record
- `_pages/contact.md` — contact information
- `assets/img/` — logo, people, and research graphics
- `_sass/` — LaSAI visual theme
