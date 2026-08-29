source "https://rubygems.org"

gem "jekyll", "~> 4.4"

# Pinned: 7.1+ requires Ruby ~> 3.1, which excludes the Ruby 4.x used for local
# development. CI runs Ruby 3.3 and would happily install a newer Chirpy, so an
# unpinned bump makes CI and production diverge from what can be previewed
# locally. Revisit when local Ruby moves to a version the newer theme supports.
gem "jekyll-theme-chirpy", "~> 7.0.1"
gem "jekyll-archives"
gem "jekyll-feed"
gem "jekyll-seo-tag"
gem "jekyll-sitemap"
gem "jekyll-paginate"
gem "jekyll-include-cache"

group :development, :test do
  gem "webrick"
  gem "html-proofer", "~> 5.0"
end