# Bookish Carnival

[![Jekyll site CI](https://github.com/Shaumik-Ashraf/bookish-carnival/actions/workflows/jekyll-docker.yml/badge.svg)](https://github.com/Shaumik-Ashraf/bookish-carnival/actions/workflows/jekyll-docker.yml)
[![pages-build-deployment](https://github.com/Shaumik-Ashraf/bookish-carnival/actions/workflows/pages/pages-build-deployment/badge.svg?branch=main)](https://github.com/Shaumik-Ashraf/bookish-carnival/actions/workflows/pages/pages-build-deployment)

Trying Jekyll &amp; GitHub Pages (again). See <https://shaumik-ashraf.github.io/bookish-carnival>

## Devlog
 - create repo from GitHub
 - clone with ssh url
 - `jekyll new bookish-carnival --force`
 - `bundle add webrick` (for Ruby 3)
 - apply GitHub actions for [GitHub Pages](https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site)
 
**Failure**

GitHub actions for deploying Jekyll fails!! (Both the jekyll.yml 3rd party one and pages.yml GitHub 1st party one). Switching from actions to traditional pages causes page deployment as a whole to fail.

You cannot disable the pages action.

Salvaged
=======

## Devlog cont'd
 - remove actions, try traditional github pages deployment
   + keep jekyll-docker CI action (just compiles jekyll on docker container)
 - Re-config repository to render pages from main-branch docs/ folder
 - Re-configure Jekyll to take source from src/, compile to docs/ and run on url base https://shaumik-ashraf.github.io/bookish-carnival
 - restructure repository
