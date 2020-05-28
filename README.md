[![license](https://img.shields.io/badge/License-MIT-yellow?style=flat)](/LICENSE.md)
![GitHub repo size](https://img.shields.io/github/repo-size/salestim/template-manifests)
![GitHub last commit](https://img.shields.io/github/last-commit/salestim/template-manifests)
[![linkedin](https://img.shields.io/badge/follow-@salestim-blue?logo=linkedin&logoColor=white)](https://www.linkedin.com/company/salestim/)
[![twitter](https://img.shields.io/badge/follow-@salestim-blue?logo=twitter&logoColor=white)](https://twitter.com/intent/follow?screen_name=salestimcrm)
[![store](https://img.shields.io/badge/visit-SalesTim%20Template%20Store-black?logo=microsoft-teams&logoColor=white)](https://store.salestim.com)

*"SalesTim URL Shortener" is licensed under a [MIT License](/LICENSE.md).*

# Welcome to the SalesTim URL Shortener repo

## ABSTRACT

This repository contains assets for making an URL Shortener with Jekyll and GitHub Pages.

View the URL Shortener in action: https://fa-st.co

> [URL shortening](https://en.wikipedia.org/wiki/URL_shortening) is a technique on the World Wide Web in which a Uniform Resource Locator (URL) may be made substantially shorter and still direct to the required page.

To learn more about SalesTim templates capabilities, including how to create templates visually from our UI, please refer to our ***[Help Center](https://help.salestim.com/)***.

If you want to integrate your contents or applications with the SalesTim Platform API, for instance create template-based teams from Microsoft PowerAutomate, please refer to our ***[Tech Hub](https://developers.salestim.com/)***.

## CONFIGURATION

Edit the `_config.yml` file:

```yaml
title: SalesTim URL Shortener
description: ✂️🔗 This repo hosts SalesTim URL Shortener (built with with Jekyll and GitHub Pages).
logo: /assets/img/color.png
show_downloads: false
google_analytics: UA-XXXXXXX-YY
theme: jekyll-theme-minimal
permalink: /:slug/
plugins:
  - jekyll-redirect-from
```

Usage:
- Change the `title` and `description` to something you like. Consider to make your own `logo` by replacing the `/assets/img/logo.png` image.
- The `show_downloads` flag indicates whether to provide downloads links for the code in the repository on the site.
- Set the `google_analytics` tracking code if you are interested in the website traffic.
- Read more about the `theme` at https://github.com/pages-themes/minimal
- The global `permalink` for pages is set to `/:slug/`.
  - Permalinks are the output path for your pages, posts, or collections. They allow you to structure the directories of your source code different from the directories in your output.
  - Slugified title from the document’s filename (any character except numbers and letters is replaced as hyphen). May be overridden via the document’s `slug` front matter.

Read more about permalinks at https://jekyllrb.com/docs/permalinks/

It is the `jekyll-redirect-from` plugin that does the redirecting from the *short link* to the *target page*.
Read more about the plugin at https://github.com/jekyll/jekyll-redirect-from

## USAGE

Create a new file in the root of the repository.

This repository has one example, [`techhub.md`](techhub.md):

```md
---
title: SalesTim Tech Hub
redirect_to: https://developers.salestim.com
---
```

This results in:
- "Short" link: https://fa-st.co/techhub
- Target page:  https://developers.salestim.com

The `title` could be used to describe the target page. Consider to take the *exact* title of the target page.
The `redirect_to` is the URL to the target page. This is the only [front matter](https://jekyllrb.com/docs/front-matter/) that is mandatory to make the short link work.

The file can have a `.md` (Markdown) or `.html` extension, but please use `.md` for consistency.

## TECHNOLOGIES

- Jekyll: https://jekyllrb.com
- jekyll-theme-minimal: https://github.com/pages-themes/minimal
- jekyll-redirect-from: https://github.com/jekyll/jekyll-redirect-from
- GitHub Pages: https://pages.github.com

## X. APPENDICES

### COMMUNICATING WITH THE TEAM

The easiest way to communicate with the team is via [GitHub Issues](/issues).

Please [file new issues](/issues/new/choose), feature requests and suggestions, but **DO search for similar open/closed pre-existing issues before creating a new issue.**

### SECURITY POLICY

This project has adopted the [SalesTim Security Policy](https://developers.salestim.com/platform/securitypolicy.html).

### CODE OF CONDUCT

This project has adopted the [SalesTim Open Source Code of Conduct](https://codeofconduct.salestim.com).

Additional resources:
- [SalesTim Code of Conduct FAQ](https://codeofconduct.salestim.com/faq/)
- Contact [codeofconduct@salestim.com](mailto:codeofconduct@salestim.com) with questions or concerns