# DS<sup>2</sup>F

This is the code repository for the pilot implementation of the University of 
Arizona Digital Scholarship & Data Science Fellowship program web page. It has 
been superseded by the site at 
[https://new.library.arizona.edu/ds2f](https://new.library.arizona.edu/ds2f).


### Development notes
These are largely taken from the GitHub help article [Setting up your GitHub Pages site locally with Jekyll](https://help.github.com/en/articles/setting-up-your-github-pages-site-locally-with-jekyll). Instructions below are for Linux, but the GitHub page has information for other operating systems.

1. For local development, will need to have Ruby version 2.1.0 or higher. Check this in a terminal via:
```
ruby --version
```
2. Install Bundler
```
gem install Bundler
```
3. Fork this repo, clone is locally, then navigate to the repo's root directory (i.e. "arizona").
4. _Don't_ install jekyll via `sudo apt-get...`. Instead, install it through the Gemfile. Run this in a Terminal:
```
echo "source 'https://rubygems.org'" >> Gemfile
echo "gem 'github-pages', group: :jekyll_plugins" >> Gemfile
```
5. Install Jekyll using Bundler. Note this should be run in the root directory of the repository, where the Gemfile is located (i.e. "arizona"):
```
bundle Install
```
6. It also wouldn't hurt to add local development Jekyll debris to .gitignore
```
echo "Gemfile" >> .gitignore
echo "Gemfile.lock" >> .gitignore
echo "_site" >> .gitignore
echo ".jekyll-cache" >> .gitignore
```
