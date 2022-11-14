![Classification:PUBLIC](https://img.shields.io/badge/🔖_Classification-PUBLIC-blue)
[![license](https://img.shields.io/badge/©️_License-CC_BY_4.0-yellow?style=flat)](/LICENSE.md)

# 👋 Welcome to the nBold URL Shortener repo

## ABSTRACT

This repository contains assets for making an URL Shortener with Jekyll and GitHub Pages.

View the URL Shortener in action: https://fa-st.co

> [URL shortening](https://en.wikipedia.org/wiki/URL_shortening) is a technique on the World Wide Web in which a Uniform Resource Locator (URL) may be made substantially shorter and still direct to the required page.

To learn more about SalesTim templates capabilities, including how to create templates visually from our UI, please refer to our ***[Docs Center](https://docs.nbold.co)***.

If you want to integrate your contents or applications with the nBold Platform API, for instance create template-based teams from Microsoft PowerAutomate, please refer to our ***[API Reference](https://docs.nbold.co/api)***.

## A. CONFIGURATION

Edit the `_config.yml` file:

```yaml
title: nBold URL Shortener
description: ✂️🔗 This repo hosts nBold URL Shortener (built with with Jekyll and GitHub Pages).
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

## B. USAGE

***How to create a new link?***

Create a new file in the root, such as `<your-keyword>.md`.  
Include this content in the file:

```markdown
---
title: <title>
redirect_to: <redirect-to>
redirect_from:
  - <alias>
---
```

- The `<title>` could be used to describe the target page. Consider to take the *exact* title of the target page.
- The `<redirect_to>` is the URL to the target page. This is the only [front matter](https://jekyllrb.com/docs/front-matter/) that is mandatory to make the short link work.
- The `<redirect_from>` is a list of aliases to the keyword, preceded by a "`/`" character, for instance `/TechHub`. This [front matter](https://jekyllrb.com/docs/front-matter/) is optional but recommended.

Best Practices:
- Keywords by default are **case-sensitives**, but you can include aliases to accept multiple variations for the same keyword, such as `/TechHub`, `/tech-hub`, `/Tech-Hub`...
- Don't forget, your file MUST start AND end with the `"---"` lines.
- Use only alphanumeric and lower-case characters for keywords.
- Separate keywords by using the `"-"` character.
- The file can have a `.md` (Markdown) or `.html` extension, but please use `.md` for consistency.

## C. TECHNOLOGIES

- Jekyll: https://jekyllrb.com
- jekyll-theme-minimal: https://github.com/pages-themes/minimal
- jekyll-redirect-from: https://github.com/jekyll/jekyll-redirect-from
- GitHub Pages: https://pages.github.com

## 📡 Communicating with the team
The easiest way to communicate with the team is via [GitHub Issues](https://github.com/nboldhq/url-shortener/issues/).

Please [file new issues](https://github.com/nbolhq/url-shortener/issues/new/choose), feature requests and suggestions, but **DO search for similar open/closed pre-existing issues before creating a new issue.**

## 🛂 Code of Conduct
See [CODE OF CONDUCT](./CODE_OF_CONDUCT.md).

## 🔐 Security Policy
See [SECURITY](./SECURITY.md).

## © License
See [LICENSE](./LICENSE.md).
