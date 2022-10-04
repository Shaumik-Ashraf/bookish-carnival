# Bookish Carnival

Trying Jekyll &amp; GitHub Pages (again)

## Devlog
 - create repo from GitHub
 - clone with ssh url
 - `jekyll new bookish-carnival --force`
 - `bundle add webrick` (for Ruby 3)

**Failure**

GitHub actions for deploying Jekyll fails!! (Both the jekyll.yml 3rd party one and pages.yml GitHub 1st party one). Switching from actions to traditional pages causes page deployment as a whole to fail.
