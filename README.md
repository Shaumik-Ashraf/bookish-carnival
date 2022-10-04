# Bookish Carnival

[![Jekyll site CI](https://github.com/Shaumik-Ashraf/bookish-carnival/actions/workflows/jekyll-docker.yml/badge.svg)](https://github.com/Shaumik-Ashraf/bookish-carnival/actions/workflows/jekyll-docker.yml)
[![pages-build-deployment](https://github.com/Shaumik-Ashraf/bookish-carnival/actions/workflows/pages/pages-build-deployment/badge.svg?branch=main)](https://github.com/Shaumik-Ashraf/bookish-carnival/actions/workflows/pages/pages-build-deployment)

Trying Jekyll &amp; GitHub Pages (again). See <https://shaumik-ashraf.github.io/bookish-carnival>

## Devlog
 - create repo from GitHub
 - clone with ssh url
 - `jekyll new bookish-carnival --force`
 - `bundle add webrick` (for Ruby 3)

**Failure**

GitHub actions for deploying Jekyll fails!! (Both the jekyll.yml 3rd party one and pages.yml GitHub 1st party one). Switching from actions to traditional pages causes page deployment as a whole to fail.

You cannot disable the pages action.
