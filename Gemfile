source "https://rubygems.org"

# This site uses plain Jekyll (no plugins), so it builds the same locally and
# on GitHub Pages via the Actions workflow in .github/workflows/jekyll.yml.
gem "jekyll", "~> 4.2"

# ffi / public_suffix are pinned only for the legacy system Ruby 2.6 used for
# local preview on this Mac. CI (Ruby 3.2) and any modern Ruby skip these.
if RUBY_VERSION < "3.0"
  gem "ffi", "1.15.5"
  gem "public_suffix", "5.1.1"
end
