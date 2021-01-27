# Quick Start

## Local Preview

Previewing your site locally requires serving your files from a web server.

The docsify [Quick Start](//docsify.js.org/#/quickstart) guide recommends [docsify-cli](//github.com/QingWei-Li/docsify-cli) for creating and previewing your site:

```bash
# Install docsify-cli globally
npm install -g docsify-cli

# Serve current directory
docsify serve

# Serve ./docs directory
docsify serve docs
```

A simple [Python](https://www.python.org/) web server can also be used:

```bash
# Change to site directory
cd /path/to/site/files

# Show Python version
python --version

# Launch web server (Python 2.x)
python -m SimpleHTTPServer

# Launch web server (Python 3.x)
python -m http.server
```

## Hosting

Sites powered by [docsify.js](//docsify.js.org/) can be hosted on any web server. The [docsify website](//docsify.js.org/) provides a helpful [deployment guide](//docsify.js.org/#/deploy) with tips for hosting your site on following platforms:

- [GitHub Pages](https://pages.github.com/)
- [GitLab Pages](https://about.gitlab.com/features/pages/)
- [Firebase Hosting](https://firebase.google.com/docs/hosting/)
- [Virtual Private Server (VPS)](https://en.wikipedia.org/wiki/Virtual_private_server)
