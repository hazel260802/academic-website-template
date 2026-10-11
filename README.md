# LE Huyen-Trang: Personal Academic Website

Source code for my personal academic webpage.

I am a PhD candidate at Cnam and ECE Engineering School (LyRIDS / CEDRIC laboratories), working on certified dynamic reconfiguration of Time-Sensitive Networks (TSN) with network calculus. Before that, I worked on blockchain, zero-knowledge proofs and privacy-preserving systems for healthcare and genomic data at the [IBISC Laboratory](https://www.ibisc.univ-evry.fr/), Université d'Évry Paris-Saclay.

**Live site:** https://hazel260802.github.io/

## What's on the site

- **Home**: short bio, research interests, selected publications and latest news
- **About**: education and awards
- **Publications**: papers and posters, with BibTeX for each entry
- **Talks**: conference talks and poster presentations
- **Research**: overview of my research projects
- **Projects**: software and engineering projects
- **Learning Materials**: my [network calculus notes](https://cnam-ece.github.io/learning-materials/blog/why-deterministic-guarantees) and course materials from my Master's at Paris-Saclay and my engineering degree at HUST

## Editing the content

| What | Where |
|------|-------|
| Name, links, menu | `_config.yml` |
| Publications | `assets/ref.bib` |
| News, awards, talks, projects, education, learning materials | `_data/*.yml` |
| Page text | `_pages/*.md` |
| Photo | `images/` |

Preview locally with Ruby and Bundler installed:

```bash
bundle install
bundle exec jekyll serve   # http://localhost:4000
```

Pushing to the `source` branch builds the site and deploys it with GitHub Actions.

## Credits

This site is built on the [academic-website-template](https://github.com/sbryngelson/academic-website-template) by [Spencer Bryngelson](https://github.com/sbryngelson), released under the [MIT License](LICENSE). Many thanks for the design and the Jekyll setup.

## Contact

- Email: lehuyentrang.workmail@gmail.com
- [LinkedIn](https://www.linkedin.com/in/huyentrang-le) · [GitHub](https://github.com/hazel260802) · [CNAM-ECE GitHub](https://github.com/CNAM-ECE) · [Google Scholar](https://scholar.google.com/citations?user=MD2uJXYAAAAJ)
