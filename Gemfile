source "https://rubygems.org"

# GitHub Pages: the meta-gem that pins all supported plugins
# https://pages.github.com/versions/
gem "github-pages", group: :jekyll_plugins

group :jekyll_plugins do
  gem "jekyll-feed"
  gem "jekyll-seo-tag"
  gem "jekyll-sitemap"
end

# Windows-specific
platforms :mingw, :x64_mingw, :mswin, :jruby do
  gem "tzinfo"
  gem "tzinfo-data"
end

gem "wdm", "~> 0.1.1", :platforms => [:mingw, :x64_mingw, :mswin]
