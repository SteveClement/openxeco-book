


# Compiling and Publishing the Book
## Installing dependencies
### Linux

Tested on: Ubuntu 22.04 LTS & Debian 11.3

```
git clone git@github.com:CybersecurityLuxembourg/openxeco-book.git
cd openxeco-book
sudo apt install -y npm
sudo apt install -y pkg-config libcairo2-dev libgif-dev libjpeg-dev
sudo apt install -y calibre  # for generating PDFs
```

### MacOS
```
# If you have homebrew not installed yet:
## /usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
# For the more adventurous you can install a cask of calibre which gives you access to *ebook-convert*
## brew cask install calibre
brew install pkg-config cairo pango libpng jpeg giflib
```

## npm install honkit

```
npm install honkit gitbook-plugin-github gitbook-plugin-atoc gitbook-plugin-anchors gitbook-plugin-alerts gitbook-plugin-search gitbook-plugin-gist gitbook-plugin-advanced-emoji gitbook-plugin-sitemap gitbook-plugin-codesnippet gitbook-plugin-image-class gitbook-plugin-last-modified gitbook-plugin-fontsettings
```

# Security caveats

[Please see this exerpt](https://github.com/MISP/misp-book/blob/main/USAGE.md#install-notes=)
