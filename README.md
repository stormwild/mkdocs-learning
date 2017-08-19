# mkdocs-learning

Learning MkDocs

## Setup

### Pre-requisites

> MkDocs supports Python versions 2.6, 2.7, 3.3, 3.4, 3.5 and pypy.

### Setup on Cloud 9

Check python and pip version

```
$ python --version
Python 2.7.2
$ pip --version
pip 1.5.2
```

Install MkDocs

```
sudo pip install mkdocs
```

Setup project in current directory, use `.`, otherwise specify a directory `myproject`


```
mkdocs new .
```

The following directory structure was generated:

```
.
├── LICENSE
├── README.md
├── docs
│   └── index.md
├── mkdocs.yml
└── site
    ├── css
    │   ├── highlight.css
    │   ├── theme.css
    │   └── theme_extra.css
    ├── fonts
    │   ├── fontawesome-webfont.eot
    │   ├── fontawesome-webfont.svg
    │   ├── fontawesome-webfont.ttf
    │   └── fontawesome-webfont.woff
    ├── img
    │   └── favicon.ico
    ├── index.html
    ├── js
    │   ├── highlight.pack.js
    │   ├── jquery-2.1.1.min.js
    │   ├── modernizr-2.8.3.min.js
    │   └── theme.js
    ├── mkdocs
    │   ├── js
    │   │   ├── lunr.min.js
    │   │   ├── mustache.min.js
    │   │   ├── require.js
    │   │   ├── search-results-template.mustache
    │   │   ├── search.js
    │   │   └── text.js
    │   └── search_index.json
    ├── search.html
    └── sitemap.xml

8 directories, 26 files
```

Use `mkdocs serve` to run locally

```
mkdocs serve -a $IP:$PORT
```

To deploy the docs to github pages, while in master branch, run the following:

```
mkdocs gh-deploy --clean
```

This creates a new branch gh-pages and pushes it to the remote repository

## Github Page

Sample MkDocs deployed to github pages

[MkDocs Learning](https://stormwild.github.io/mkdocs-learning/)

## References

- [Building Product Documentation with MkDocs](https://www.sitepoint.com/building-product-documentation-mkdocs/)
- [MkDocs](http://www.mkdocs.org/)
